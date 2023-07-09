# Comparing `tmp/mlflow_tracking_mongostore-0.1.4-py3-none-any.whl.zip` & `tmp/mlflow_tracking_mongostore-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17943 bytes, number of entries: 9
+Zip file size: 18222 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 09:59 mlflow_tracking_mongostore/__init__.py
--rw-r--r--  2.0 unx     8249 b- defN 23-Jul-06 13:05 mlflow_tracking_mongostore/models.py
--rw-r--r--  2.0 unx    43830 b- defN 23-Jun-30 11:53 mlflow_tracking_mongostore/mongo_store.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1389 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      881 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/RECORD
-9 files, 65974 bytes uncompressed, 16381 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx     9301 b- defN 23-Jul-09 10:10 mlflow_tracking_mongostore/models.py
+-rw-r--r--  2.0 unx    43818 b- defN 23-Jul-08 17:57 mlflow_tracking_mongostore/mongo_store.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1389 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      881 b- defN 23-Jul-09 15:45 mlflow_tracking_mongostore-0.1.5.dist-info/RECORD
+9 files, 67014 bytes uncompressed, 16660 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mlflow_tracking_mongostore/models.py
 Comment: 
 
 Filename: mlflow_tracking_mongostore/mongo_store.py
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE
+Filename: mlflow_tracking_mongostore-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.4.dist-info/METADATA
+Filename: mlflow_tracking_mongostore-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.4.dist-info/WHEEL
+Filename: mlflow_tracking_mongostore-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.4.dist-info/entry_points.txt
+Filename: mlflow_tracking_mongostore-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.4.dist-info/top_level.txt
+Filename: mlflow_tracking_mongostore-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.4.dist-info/RECORD
+Filename: mlflow_tracking_mongostore-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_tracking_mongostore/models.py

```diff
@@ -1,8 +1,9 @@
 import numbers
+from flask import request
 from mlflow.entities import (
     Experiment,
     ExperimentTag,
     RunTag,
     RunInfo,
     RunData,
     Run,
@@ -10,34 +11,57 @@
     Param,
     SourceType,
     RunStatus,
 )
 from mlflow.entities import LifecycleStage
 from mlflow.utils.mlflow_tags import _get_run_name_from_tags
 from mlflow.utils.time_utils import get_current_time_millis
-
 from mongoengine import (
     Document,
     StringField,
     ListField,
     EmbeddedDocument,
     EmbeddedDocumentField,
     FloatField,
     IntField,
     BooleanField,
     LongField,
     ReferenceField,
     CASCADE,
     EmbeddedDocumentListField,
+    QuerySet,
+    Q,
 )
 
 
-EXPERIMENT_COLLECTION_NAME = "experiment"
-RUN_COLLECTION_NAME = "run"
-METRIC_COLLECTION_NAME = "metrics"
+EXPERIMENT_COLLECTION_NAME = "mlflow_experiment"
+RUN_COLLECTION_NAME = "mlflow_run"
+METRIC_COLLECTION_NAME = "mlflow_metric"
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
@@ -111,29 +135,35 @@
     exp_id = StringField(max_length=32, db_field="id")
     name = StringField(required=True, max_length=200)
     artifact_location = StringField(max_length=256)
     lifecycle_stage = StringField(max_length=50, default=LifecycleStage.ACTIVE)
     tags = ListField(EmbeddedDocumentField(MongoExperimentTag))
     creation_time = LongField()
     last_update_time = LongField()
+    mlflow_workspace_id = StringField(max_length=32)
 
-    meta = {"collection": EXPERIMENT_COLLECTION_NAME, "strict": False}
+    meta = {
+        "collection": EXPERIMENT_COLLECTION_NAME,
+        "strict": False,
+        "queryset_class": CustomQuerySet,
+    }
 
     def to_mlflow_entity(self) -> Experiment:
         return Experiment(
             experiment_id=str(self.id),
             name=self.name,
             artifact_location=self.artifact_location,
             lifecycle_stage=self.lifecycle_stage,
             tags=[t.to_mlflow_entity() for t in self.tags],
             creation_time=self.creation_time,
             last_update_time=self.last_update_time,
         )
 
     def save(self, *args, **kwargs):
+        self.mlflow_workspace_id = get_workspace_id()
         self.exp_id = self.experiment_id
         return super(MongoExperiment, self).save(*args, **kwargs)
 
 
 class MongoTag(EmbeddedDocument):
     key = StringField(required=True)
     value = StringField(required=True)
@@ -151,15 +181,15 @@
 
 
 class MongoMetric(Document):
     key = StringField(required=True)
     timestamp = LongField(default=get_current_time_millis)
     step = LongField(required=True, default=0)
     is_nan = BooleanField(required=True, default=False)
-    run_id = StringField(required=True)
+    run_id = StringField(required=True, db_field="mlflow_run_id")
     value = FloatField(
         unique_with=["key", "timestamp", "step", "run_id"], required=True
     )
 
     meta = {"collection": METRIC_COLLECTION_NAME}
 
     def to_mlflow_entity(self) -> Metric:
@@ -203,22 +233,25 @@
     start_time = LongField(default=get_current_time_millis)
     end_time = LongField()
     deleted_time = LongField()
     source_version = StringField(max_length=50)
     lifecycle_stage = StringField(max_length=20, default=LifecycleStage.ACTIVE)
     artifact_uri = StringField(max_length=200)
 
-    experiment_id = ReferenceField("MongoExperiment", reverse_delete_rule=CASCADE)
+    experiment_id = ReferenceField(
+        "MongoExperiment", reverse_delete_rule=CASCADE, db_field="mlflow_experiment_id"
+    )
+    mlflow_workspace_id = StringField(max_length=32)
 
     latest_metrics = ListField(EmbeddedDocumentField(MongoLatestMetric))
     params = ListField(EmbeddedDocumentField(MongoParam))
     # tags = ListField(EmbeddedDocumentField(MongoTag))
     tags = EmbeddedDocumentListField(MongoTag)
 
-    meta = {"collection": RUN_COLLECTION_NAME}
+    meta = {"collection": RUN_COLLECTION_NAME, "queryset_class": CustomQuerySet}
 
     def to_mlflow_entity(self) -> Run:
         run_info = RunInfo(
             run_uuid=self.run_uuid,
             run_id=self.run_uuid,
             run_name=self.run_name,
             experiment_id=str(self.experiment_id.id),
@@ -256,9 +289,10 @@
         params = list(filter(lambda param: param.key == key, self.params))
         return params[0] if params else None
 
     def get_tags_by_key(self, key):
         return list(filter(lambda param: param.key == key, self.tags))
 
     def save(self, *args, **kwargs):
+        self.mlflow_workspace_id = get_workspace_id()
         self.run_id = self.run_uuid
         return super(MongoRun, self).save(*args, **kwargs)
```

## mlflow_tracking_mongostore/mongo_store.py

```diff
@@ -373,15 +373,15 @@
             )
 
         if artifact_location:
             artifact_location = resolve_uri_if_local(artifact_location)
 
         creation_time = get_current_time_millis()
 
-        tags_dict = tags_dict = {tag.key: tag.value for tag in tags} if tags else {}
+        tags_dict = {tag.key: tag.value for tag in tags} if tags else {}
         exp_tags = [
             MongoExperimentTag(key=key, value=value) for key, value in tags_dict.items()
         ]
 
         try:
             with self.__db.client.start_session() as session:
                 with session.start_transaction():
```

## Comparing `mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE` & `mlflow_tracking_mongostore-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlflow_tracking_mongostore-0.1.4.dist-info/METADATA` & `mlflow_tracking_mongostore-0.1.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-tracking-mongostore
-Version: 0.1.4
+Version: 0.1.5
 Summary: Mlflow plugin to use MongoDB as backend for MLflow tracking service
 Home-page: UNKNOWN
 Author: Rachid Belmeskine
 Maintainer-email: rachid.belmeskine@gmail.com
 License: UNKNOWN
 Keywords: mlflow
 Platform: UNKNOWN
```

## Comparing `mlflow_tracking_mongostore-0.1.4.dist-info/RECORD` & `mlflow_tracking_mongostore-0.1.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlflow_tracking_mongostore/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mlflow_tracking_mongostore/models.py,sha256=6HsTzJDkLzIjZl0vLa_xZNYKtSkhpIO470yfFum756A,8249
-mlflow_tracking_mongostore/mongo_store.py,sha256=O8A07-rNkeuJG6saX6KUok_DNZV36QsDpWAuZqqWT0Q,43830
-mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mlflow_tracking_mongostore-0.1.4.dist-info/METADATA,sha256=yZQUhf1rFv4m4D8layQ6GKit6BFocBZ_E6RZb0By_p8,1389
-mlflow_tracking_mongostore-0.1.4.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-mlflow_tracking_mongostore-0.1.4.dist-info/entry_points.txt,sha256=1DhRgG-R9Qmgl1i-WxNc8x5JtKenuAkyVNYfAmZQOBo,149
-mlflow_tracking_mongostore-0.1.4.dist-info/top_level.txt,sha256=OWuYjvOHTC4KzmrdfxF9HUBd_TMuvjKoihXmytBaCKM,27
-mlflow_tracking_mongostore-0.1.4.dist-info/RECORD,,
+mlflow_tracking_mongostore/models.py,sha256=xU86qrI_ox1HL0yiB94UlbEZAYAr3NwTaCrP23F2AHM,9301
+mlflow_tracking_mongostore/mongo_store.py,sha256=PQ58RDY9AtodaKhml7aLQFH-pa7AlkR58QlcdlIh5RE,43818
+mlflow_tracking_mongostore-0.1.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mlflow_tracking_mongostore-0.1.5.dist-info/METADATA,sha256=7SurnQJOEyzbePy52xX3j89CeVLaROrg3Y-UASbL2aw,1389
+mlflow_tracking_mongostore-0.1.5.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+mlflow_tracking_mongostore-0.1.5.dist-info/entry_points.txt,sha256=1DhRgG-R9Qmgl1i-WxNc8x5JtKenuAkyVNYfAmZQOBo,149
+mlflow_tracking_mongostore-0.1.5.dist-info/top_level.txt,sha256=OWuYjvOHTC4KzmrdfxF9HUBd_TMuvjKoihXmytBaCKM,27
+mlflow_tracking_mongostore-0.1.5.dist-info/RECORD,,
```

