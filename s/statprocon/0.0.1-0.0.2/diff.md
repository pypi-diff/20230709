# Comparing `tmp/statprocon-0.0.1.tar.gz` & `tmp/statprocon-0.0.2.tar.gz`

## Comparing `statprocon-0.0.1.tar` & `statprocon-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 statprocon-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 statprocon-0.0.1/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/xmr.iml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.1/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.1/statprocon/charts/__init__.py
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 statprocon-0.0.1/statprocon/charts/xmr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 statprocon-0.0.1/tests/test_xmr.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 statprocon-0.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.1/LICENSE
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 statprocon-0.0.1/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 statprocon-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 statprocon-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 statprocon-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/xmr.iml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 statprocon-0.0.2/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.2/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 statprocon-0.0.2/statprocon/charts/xmr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 statprocon-0.0.2/tests/test_xmr.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 statprocon-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 statprocon-0.0.2/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 statprocon-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 statprocon-0.0.2/PKG-INFO
```

### Comparing `statprocon-0.0.1/.idea/workspace.xml` & `statprocon-0.0.2/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `statprocon-0.0.1/.idea/workspace.xml` & `statprocon-0.0.2/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment="">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -62,15 +62,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment=""/>
       <created>1688827023388</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
-      <workItem from="1688848868641" duration="11581000"/>
+      <workItem from="1688848868641" duration="14801000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `statprocon-0.0.1/statprocon/charts/xmr.py` & `statprocon-0.0.2/statprocon/charts/xmr.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,34 @@
 from typing import cast, Union, Optional
 
 TYPE_COUNTS = list[Decimal | int]
 TYPE_MOVING_RANGES = list[Decimal | int | None]
 
 
 class XmR:
-    def __init__(self, counts: TYPE_COUNTS):
+    def __init__(
+            self,
+            counts: TYPE_COUNTS,
+            subset_start_index: int = 0,
+            subset_end_index: Optional[int] = None,
+    ):
+        """
+
+        :param counts: TYPE_COUNTS list of data to be used by the X chart
+        :param subset_start_index: Optional starting index of counts to calculate limits from
+        :param subset_end_index: Optional ending index of counts to calculate limits to
+        """
         self.counts = counts
         self._mr: TYPE_MOVING_RANGES = []
+        self.i = max(0, subset_start_index)
+        self.j = len(counts)
+        if subset_end_index:
+            self.j = min(self.j, subset_end_index)
+
+        assert self.i <= self.j
 
     def moving_ranges(self) -> TYPE_MOVING_RANGES:
         """
         Moving ranges are the absolute differences between successive count values.
         The first element will always be None
         """
         if self._mr:
@@ -25,19 +42,19 @@
             else:
                 value = cast(Union[Decimal | int], abs(c - self.counts[i - 1]))
                 result.append(value)
         self._mr = result
         return self._mr
 
     def x_average(self) -> Decimal:
-        return self.mean(self.counts)
+        return self.mean(self.counts[self.i:self.j])
 
     def mr_average(self) -> Decimal:
         assert self.moving_ranges()[0] is None
-        valid_values = cast(TYPE_COUNTS, self.moving_ranges()[1:])
+        valid_values = cast(TYPE_COUNTS, self.moving_ranges()[self.i+1:self.j])
         return self.mean(valid_values)
 
     def upper_range_limit(self) -> Decimal:
         limit = Decimal('3.268') * self.mr_average()
         return round(limit, 3)
 
     def upper_natural_process_limit(self) -> Decimal:
```

### Comparing `statprocon-0.0.1/tests/test_xmr.py` & `statprocon-0.0.2/tests/test_xmr.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,29 @@
 
     def test_lower_natural_process_limit(self):
         counts = [1, 10, 100, 50]
         xmr = XmR(counts)
         limit = xmr.lower_natural_process_limit()
         self.assertEqual(limit, Decimal('-91.863'))
 
+    def test_limits_with_subsets(self):
+        counts = [1] * 25
+        counts[1] = 10
+        counts[2] = 100
+        counts[3] = 50
+
+        xmr = XmR(counts, subset_end_index=24)
+        self.assertEqual(xmr.upper_natural_process_limit(), Decimal('30.441'))
+        self.assertEqual(xmr.upper_range_limit(), Decimal('28.133'))
+
+        # Adjust manually so that all subset values should be 1
+        xmr.i = 4
+        self.assertEqual(xmr.x_average(), 1)
+        self.assertEqual(xmr.lower_natural_process_limit(), xmr.upper_natural_process_limit())
+
     def test_rule_1_points_beyond_upper_limits(self):
         """
         This test dataset comes from Table 9.1: Accident Rates in Making Sense of Data
         """
 
         group_a = [43, 40, 37, 33, 30, 33, 34, 35, 29, 33, 31, 39]
         group_b_upper = Decimal('39.3')
```

### Comparing `statprocon-0.0.1/LICENSE` & `statprocon-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.0.1/README.md` & `statprocon-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -53,14 +53,26 @@
 
 Activate virtualenv
 
 ```shell
 source venv/bin/activate
 ```
 
+[Build](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archiveshttps://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives)
+
+```shell
+python -m build
+```
+
+[Upload](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives)
+
+```shell
+python -m twine upload dist/*
+```
+
 ### Testing
 
 [Install package from source](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#installing-from-source)
 ```shell
 python3 -m pip install .
 ```
```

### Comparing `statprocon-0.0.1/pyproject.toml` & `statprocon-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.0.1/PKG-INFO` & `statprocon-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
@@ -69,14 +69,26 @@
 
 Activate virtualenv
 
 ```shell
 source venv/bin/activate
 ```
 
+[Build](https://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archiveshttps://packaging.python.org/en/latest/tutorials/packaging-projects/#generating-distribution-archives)
+
+```shell
+python -m build
+```
+
+[Upload](https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-the-distribution-archives)
+
+```shell
+python -m twine upload dist/*
+```
+
 ### Testing
 
 [Install package from source](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#installing-from-source)
 ```shell
 python3 -m pip install .
 ```
```

