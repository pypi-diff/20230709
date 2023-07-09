# Comparing `tmp/mlflow_registry_mongostore-0.1.4-py3-none-any.whl.zip` & `tmp/mlflow_registry_mongostore-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 20248 bytes, number of entries: 10
+Zip file size: 20536 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 09:59 mlflow_registry_mongostore/__init__.py
 -rw-r--r--  2.0 unx    18488 b- defN 23-Jun-29 10:01 mlflow_registry_mongostore/_version.py
--rw-r--r--  2.0 unx     5214 b- defN 23-Jul-06 13:06 mlflow_registry_mongostore/models.py
+-rw-r--r--  2.0 unx     6391 b- defN 23-Jul-09 09:57 mlflow_registry_mongostore/models.py
 -rw-r--r--  2.0 unx    40867 b- defN 23-Jun-30 11:20 mlflow_registry_mongostore/mongo_store.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1388 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx      155 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      977 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/RECORD
-10 files, 78565 bytes uncompressed, 18534 bytes compressed:  76.4%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-09 15:44 mlflow_registry_mongostore-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1388 b- defN 23-Jul-09 15:44 mlflow_registry_mongostore-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 15:44 mlflow_registry_mongostore-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      155 b- defN 23-Jul-09 15:44 mlflow_registry_mongostore-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Jul-09 15:44 mlflow_registry_mongostore-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      977 b- defN 23-Jul-09 15:44 mlflow_registry_mongostore-0.1.5.dist-info/RECORD
+10 files, 79742 bytes uncompressed, 18822 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: mlflow_registry_mongostore/models.py
 Comment: 
 
 Filename: mlflow_registry_mongostore/mongo_store.py
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.4.dist-info/LICENSE
+Filename: mlflow_registry_mongostore-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.4.dist-info/METADATA
+Filename: mlflow_registry_mongostore-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.4.dist-info/WHEEL
+Filename: mlflow_registry_mongostore-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.4.dist-info/entry_points.txt
+Filename: mlflow_registry_mongostore-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.4.dist-info/top_level.txt
+Filename: mlflow_registry_mongostore-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.4.dist-info/RECORD
+Filename: mlflow_registry_mongostore-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_registry_mongostore/models.py

```diff
@@ -1,8 +1,9 @@
 import numbers
+from flask import request
 from mlflow.entities.model_registry import (
     RegisteredModel,
     ModelVersion,
     RegisteredModelTag,
     ModelVersionTag,
 )
 from mlflow.entities.model_registry.model_version_stages import STAGE_NONE
@@ -14,19 +15,43 @@
     ListField,
     EmbeddedDocument,
     EmbeddedDocumentField,
     IntField,
     LongField,
     ReferenceField,
     CASCADE,
+    QuerySet,
+    Q,
 )
 
 
-REGISTERED_MODEL_COLLECTION_NAME = "registered_model"
-MODEL_VERSION_COLLECTION_NAME = "model_version"
+REGISTERED_MODEL_COLLECTION_NAME = "mlflow_registered_model"
+MODEL_VERSION_COLLECTION_NAME = "mlflow_model_version"
+
+
+def get_workspace_id():
+    if request:
+        if request.headers:
+            if request.headers:
+                return request.headers.get("Workspace-Id", None)
+    return None
+
+
+class CustomQuerySet(QuerySet):
+    def __call__(self, q_obj=None, **query):
+
+        q_obj = q_obj if q_obj else Q()
+
+        # Combine the existing query with the new filter
+        workspace_id = get_workspace_id()
+        if workspace_id:
+            q_obj &= Q(mlflow_workspace_id=workspace_id)
+
+        # call the super class's __call__ with the updated query.
+        return super().__call__(q_obj, **query)
 
 
 def compare_attr(val1, comp, val2):
     """
     Compares two values based on a comparator and returns the result.
 
     :param val1: The first value to be compared.
@@ -86,56 +111,67 @@
 class MongoRegisteredModel(Document):
     name = StringField(primary_key=True)
     registed_model_id = StringField(max_length=32, db_field="id")
     creation_timestamp = LongField(default=get_current_time_millis)
     last_updated_timestamp = LongField()
     description = StringField(max_length=256)
     tags = ListField(EmbeddedDocumentField(MongoRegisteredModelTag))
+    mlflow_workspace_id = StringField(max_length=32)
 
-    meta = {"collection": REGISTERED_MODEL_COLLECTION_NAME}
+    meta = {
+        "collection": REGISTERED_MODEL_COLLECTION_NAME,
+        "queryset_class": CustomQuerySet,
+    }
 
     def to_mlflow_entity(self) -> RegisteredModel:
         return RegisteredModel(
             name=self.name,
             creation_timestamp=self.creation_timestamp,
             last_updated_timestamp=self.last_updated_timestamp,
             description=self.description,
             tags=[t.to_mlflow_entity() for t in self.tags],
         )
 
     def get_tags_by_key(self, key):
         return list(filter(lambda param: param.key == key, self.tags))
 
     def save(self, *args, **kwargs):
+        self.mlflow_workspace_id = get_workspace_id()
         self.registed_model_id = self.name
         return super(MongoRegisteredModel, self).save(*args, **kwargs)
 
 
 class MongoModelVersion(Document):
     # name = StringField(primary_key=True)
     registered_model_id = ReferenceField(
-        "MongoRegisteredModel", reverse_delete_rule=CASCADE
+        "MongoRegisteredModel",
+        reverse_delete_rule=CASCADE,
+        db_field="mlflow_registered_model_id",
     )
     version = IntField(required=True)
     creation_timestamp = LongField(default=get_current_time_millis)
     last_updated_timestamp = LongField()
     description = StringField(max_length=5000)
     user_id = StringField(max_length=256)
     current_stage = StringField(max_length=20, default=STAGE_NONE)
     source = StringField(max_length=200)
-    run_id = StringField(max_length=32)
+    run_id = StringField(max_length=32, db_field="mlflow_run_id")
     run_link = StringField(max_length=500)
     status = StringField(
         max_length=20, default=ModelVersionStatus.to_string(ModelVersionStatus.READY)
     )
     status_message = StringField(max_length=500)
+    mlflow_workspace_id = StringField(max_length=32)
 
     tags = ListField(EmbeddedDocumentField(MongoModelVersionTag))
 
-    meta = {"collection": MODEL_VERSION_COLLECTION_NAME}
+    meta = {
+        "collection": MODEL_VERSION_COLLECTION_NAME,
+        "queryset_class": CustomQuerySet,
+    }
 
     def to_mlflow_entity(self) -> ModelVersion:
         return ModelVersion(
             name=str(self.registered_model_id.id),
             version=self.version,
             creation_timestamp=self.creation_timestamp,
             last_updated_timestamp=self.last_updated_timestamp,
@@ -154,7 +190,11 @@
         return list(filter(lambda param: param.key == key, self.tags))
 
     @staticmethod
     def get_attribute_name(mlflow_attribute_name):
         return {"name": "registered_model_id"}.get(
             mlflow_attribute_name, mlflow_attribute_name
         )
+
+    def save(self, *args, **kwargs):
+        self.mlflow_workspace_id = get_workspace_id()
+        return super(MongoModelVersion, self).save(*args, **kwargs)
```

## Comparing `mlflow_registry_mongostore-0.1.4.dist-info/LICENSE` & `mlflow_registry_mongostore-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlflow_registry_mongostore-0.1.4.dist-info/METADATA` & `mlflow_registry_mongostore-0.1.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-registry-mongostore
-Version: 0.1.4
+Version: 0.1.5
 Summary: Mlflow plugin to use MongoDB as backend for MLflow Model Registry service
 Home-page: UNKNOWN
 Author: Rachid Belmeskine
 Maintainer-email: rachid.belmeskine@gmail.com
 License: UNKNOWN
 Keywords: mlflow
 Platform: UNKNOWN
```

## Comparing `mlflow_registry_mongostore-0.1.4.dist-info/RECORD` & `mlflow_registry_mongostore-0.1.5.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mlflow_registry_mongostore/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_registry_mongostore/_version.py,sha256=nTDwWbHLCXMqdi1bkEkchAiz_JAzkXcmH3bKG0jf6fg,18488
-mlflow_registry_mongostore/models.py,sha256=GtrxUR_y0t9QoWf3JmiVNR4zlnmCw4TOJryUb_IT4Dg,5214
+mlflow_registry_mongostore/models.py,sha256=G0SE4PHLoDTJZzqCBgX5qbqJFtyduKT2jaZwsYPH3zY,6391
 mlflow_registry_mongostore/mongo_store.py,sha256=5lxamQ_HlvoRbcZt3wD7NTz3toIk6JfG68bNePWyNzY,40867
-mlflow_registry_mongostore-0.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mlflow_registry_mongostore-0.1.4.dist-info/METADATA,sha256=tC2MAzmWXDVc8YuotCGi0mIzYDjBinycSi8QxbPJhoo,1388
-mlflow_registry_mongostore-0.1.4.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-mlflow_registry_mongostore-0.1.4.dist-info/entry_points.txt,sha256=tfl_ffj0PkSrXY4rvesmyyvPXDS-j5egPU_XNXoVKm4,155
-mlflow_registry_mongostore-0.1.4.dist-info/top_level.txt,sha256=6DHvL6p3UTy_bC25io6QqOIFVHNwvfFY0Nj_664suUE,27
-mlflow_registry_mongostore-0.1.4.dist-info/RECORD,,
+mlflow_registry_mongostore-0.1.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mlflow_registry_mongostore-0.1.5.dist-info/METADATA,sha256=foz8QXo1BV51l8Y4R6xvqE4dBZn7_pP0FI4MXNsY_nc,1388
+mlflow_registry_mongostore-0.1.5.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+mlflow_registry_mongostore-0.1.5.dist-info/entry_points.txt,sha256=tfl_ffj0PkSrXY4rvesmyyvPXDS-j5egPU_XNXoVKm4,155
+mlflow_registry_mongostore-0.1.5.dist-info/top_level.txt,sha256=6DHvL6p3UTy_bC25io6QqOIFVHNwvfFY0Nj_664suUE,27
+mlflow_registry_mongostore-0.1.5.dist-info/RECORD,,
```

