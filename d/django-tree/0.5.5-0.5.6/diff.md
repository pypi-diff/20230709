# Comparing `tmp/django-tree-0.5.5.tar.gz` & `tmp/django-tree-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tree-0.5.5.tar", last modified: Thu Jul  6 18:43:02 2023, max compression
+gzip compressed data, was "dist/django-tree-0.5.6.tar", last modified: Sun Jul  9 14:08:37 2023, max compression
```

## Comparing `django-tree-0.5.5.tar` & `django-tree-0.5.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9498 2023-07-06 13:11:50.000000 django-tree-0.5.5/README.rst
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/benchmark/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/benchmark/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3945 2023-07-06 18:27:12.000000 django-tree-0.5.5/benchmark/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.5/benchmark/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/router.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30521 2023-07-06 00:41:03.000000 django-tree-0.5.5/benchmark/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.5/benchmark/utils.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.5/requirements.txt
--rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.5/setup.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/django_tree.egg-info/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/requires.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/top_level.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.5/django_tree.egg-info/not-zip-safe
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-06 18:43:01.000000 django-tree-0.5.5/django_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.5/MANIFEST.in
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tests/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tests/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.5/tests/migrations/0003_test_migrations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.5/tests/migrations/0002_add_tmp_model.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3010 2023-07-06 18:27:12.000000 django-tree-0.5.5/tests/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tests/migrations/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      910 2023-07-06 10:40:54.000000 django-tree-0.5.5/tests/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.5/tests/settings.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    48189 2023-07-06 14:12:28.000000 django-tree-0.5.5/tests/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tests/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12444 2023-07-06 18:43:02.000000 django-tree-0.5.5/PKG-INFO
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1985 2023-07-06 18:42:44.000000 django-tree-0.5.5/CHANGELOG.rst
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.5/LICENSE
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-06 18:43:02.000000 django-tree-0.5.5/setup.cfg
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tree/
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tree/migrations/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/migrations/0002_remove_old_functions.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/migrations/0001_initial.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tree/migrations/__init__.py
-drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-06 18:43:02.000000 django-tree-0.5.5/tree/sql/
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9408 2023-07-06 14:52:11.000000 django-tree-0.5.5/tree/sql/postgresql.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/sql/base.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.5/tree/sql/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/transforms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1764 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/query.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/signals.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.5/tree/forms.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/apps.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4961 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/models.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1815 2023-07-06 18:25:02.000000 django-tree-0.5.5/tree/lookups.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/operations.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.5/tree/types.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-06 18:42:44.000000 django-tree-0.5.5/tree/__init__.py
--rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4966 2023-07-06 18:27:12.000000 django-tree-0.5.5/tree/fields.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9509 2023-07-09 11:25:49.000000 django-tree-0.5.6/README.rst
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/benchmark/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/benchmark/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3945 2023-07-06 18:27:12.000000 django-tree-0.5.6/benchmark/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.6/benchmark/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1660 2023-07-06 00:41:03.000000 django-tree-0.5.6/benchmark/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      317 2018-02-09 14:18:58.000000 django-tree-0.5.6/benchmark/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      434 2018-02-09 14:18:58.000000 django-tree-0.5.6/benchmark/router.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    30532 2023-07-09 11:27:28.000000 django-tree-0.5.6/benchmark/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.6/benchmark/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      903 2018-02-09 14:18:58.000000 django-tree-0.5.6/benchmark/utils.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-06 00:41:03.000000 django-tree-0.5.6/requirements.txt
+-rwxrwxr-x   0 bertrand  (1000) bertrand  (1000)     1315 2023-07-06 00:45:16.000000 django-tree-0.5.6/setup.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/django_tree.egg-info/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1015 2023-07-09 14:08:37.000000 django-tree-0.5.6/django_tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       17 2023-07-09 14:08:37.000000 django-tree-0.5.6/django_tree.egg-info/requires.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       21 2023-07-09 14:08:37.000000 django-tree-0.5.6/django_tree.egg-info/top_level.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12455 2023-07-09 14:08:37.000000 django-tree-0.5.6/django_tree.egg-info/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2018-03-23 16:20:04.000000 django-tree-0.5.6/django_tree.egg-info/not-zip-safe
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        1 2023-07-09 14:08:37.000000 django-tree-0.5.6/django_tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      100 2018-02-09 14:18:58.000000 django-tree-0.5.6/MANIFEST.in
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/tests/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/tests/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      612 2023-07-06 00:41:03.000000 django-tree-0.5.6/tests/migrations/0003_test_migrations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1071 2018-02-09 15:32:30.000000 django-tree-0.5.6/tests/migrations/0002_add_tmp_model.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     3010 2023-07-06 18:27:12.000000 django-tree-0.5.6/tests/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.6/tests/migrations/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      959 2023-07-09 11:01:34.000000 django-tree-0.5.6/tests/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      230 2018-02-09 14:18:58.000000 django-tree-0.5.6/tests/settings.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    49267 2023-07-09 11:47:55.000000 django-tree-0.5.6/tests/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.6/tests/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)    12455 2023-07-09 14:08:37.000000 django-tree-0.5.6/PKG-INFO
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2346 2023-07-09 12:48:26.000000 django-tree-0.5.6/CHANGELOG.rst
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1485 2018-02-09 14:18:58.000000 django-tree-0.5.6/LICENSE
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)       59 2023-07-09 14:08:37.000000 django-tree-0.5.6/setup.cfg
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/tree/
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/tree/migrations/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      556 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/migrations/0002_remove_old_functions.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      275 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/migrations/0001_initial.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.6/tree/migrations/__init__.py
+drwxrwxr-x   0 bertrand  (1000) bertrand  (1000)        0 2023-07-09 14:08:37.000000 django-tree-0.5.6/tree/sql/
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     9281 2023-07-09 11:04:34.000000 django-tree-0.5.6/tree/sql/postgresql.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     5152 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/sql/base.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)        0 2018-02-09 14:18:58.000000 django-tree-0.5.6/tree/sql/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      228 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/transforms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     2011 2023-07-09 11:25:48.000000 django-tree-0.5.6/tree/query.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      963 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/signals.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      242 2018-03-23 19:35:02.000000 django-tree-0.5.6/tree/forms.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      540 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/apps.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6099 2023-07-09 11:41:25.000000 django-tree-0.5.6/tree/models.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     1815 2023-07-06 18:25:02.000000 django-tree-0.5.6/tree/lookups.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4395 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/operations.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     6320 2023-07-06 00:41:03.000000 django-tree-0.5.6/tree/types.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)      110 2023-07-09 12:48:26.000000 django-tree-0.5.6/tree/__init__.py
+-rw-rw-r--   0 bertrand  (1000) bertrand  (1000)     4784 2023-07-09 11:16:20.000000 django-tree-0.5.6/tree/fields.py
```

### Comparing `django-tree-0.5.5/README.rst` & `django-tree-0.5.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     obj.get_prev_sibling()  # Fetches the previous sibling.
     obj.get_next_sibling()
     # Same as `get_prev_sibling`, except that we get the first public one.
     obj.get_prev_siblings().filter(public=True).first()
     other = YourModel.objects.all()[1]
     obj.is_ancestor_of(other)
     obj.is_descendant_of(other, include_self=True)
-    YourModel.get_roots()
+    YourModel.objects.filter_roots()
 
     #
     # Advanced usage
     # Use the following methods only if you understand exactly what they mean.
     #
 
     YourModel.rebuild_paths()  # Rebuilds all paths of this field, useful only
```

### Comparing `django-tree-0.5.5/benchmark/migrations/0001_initial.py` & `django-tree-0.5.6/benchmark/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/benchmark/models.py` & `django-tree-0.5.6/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/benchmark/base.py` & `django-tree-0.5.6/benchmark/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,15 +711,15 @@
     def run(self):
         list(self.model._default_manager.root_nodes())
 
 
 @Benchmark.register_test('Get roots', TreePlace)
 class TestGetRoots(BenchmarkTest):
     def run(self):
-        list(self.model.get_roots())
+        list(self.model.objects.filter_roots())
 
 
 @Benchmark.register_test(
     'Get roots', (TreebeardALPlace, TreebeardMPPlace, TreebeardNSPlace))
 class TestGetRoots(BenchmarkTest):
     def run(self):
         list(self.model.get_root_nodes())
```

### Comparing `django-tree-0.5.5/benchmark/utils.py` & `django-tree-0.5.6/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/setup.py` & `django-tree-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/django_tree.egg-info/SOURCES.txt` & `django-tree-0.5.6/django_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/django_tree.egg-info/PKG-INFO` & `django-tree-0.5.6/django_tree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.5
+Version: 0.5.6
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
@@ -218,15 +218,15 @@
             obj.get_prev_sibling()  # Fetches the previous sibling.
             obj.get_next_sibling()
             # Same as `get_prev_sibling`, except that we get the first public one.
             obj.get_prev_siblings().filter(public=True).first()
             other = YourModel.objects.all()[1]
             obj.is_ancestor_of(other)
             obj.is_descendant_of(other, include_self=True)
-            YourModel.get_roots()
+            YourModel.objects.filter_roots()
         
             #
             # Advanced usage
             # Use the following methods only if you understand exactly what they mean.
             #
         
             YourModel.rebuild_paths()  # Rebuilds all paths of this field, useful only
```

### Comparing `django-tree-0.5.5/tests/migrations/0003_test_migrations.py` & `django-tree-0.5.6/tests/migrations/0003_test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tests/migrations/0002_add_tmp_model.py` & `django-tree-0.5.6/tests/migrations/0002_add_tmp_model.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tests/migrations/0001_initial.py` & `django-tree-0.5.6/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tests/models.py` & `django-tree-0.5.6/tests/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
     class Meta:
         ordering = ['path', 'name']
         indexes = [
             *PathField.get_indexes('place', 'path'),
         ]
 
+    def __str__(self):
+        return self.name
+
 
 class Person(TreeModel):
     century = SmallIntegerField(null=True, blank=True)
     first_name = CharField(max_length=20, blank=True)
     last_name = CharField(max_length=50)
     parent = ForeignKey('self', null=True, blank=True, on_delete=CASCADE)
     path = PathField(order_by=['century', 'last_name', 'first_name'])
```

### Comparing `django-tree-0.5.5/tests/base.py` & `django-tree-0.5.6/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 from __future__ import unicode_literals
 
 import decimal
-from unittest import expectedFailure
 
+from django.core.exceptions import ValidationError
 from django.db import transaction, InternalError, connection
 from django.test import TransactionTestCase
 
 from .models import Place, Person
 
 
 # TODO: Test same order_by values.
@@ -34,17 +34,19 @@
 def path(*path_components):
     return [decimal.Decimal(f'{value:.10f}') for value in path_components]
 
 
 class CommonTest(TransactionTestCase):
     maxDiff = 1000
 
-    def create_place(self, name, parent=None, n_queries=1):
-        with self.assertNumQueries(n_queries):
+    def create_place(self, name, parent=None):
+        with self.assertNumQueries(1):
             p = Place.objects.create(name=name, parent=parent)
+        with self.assertNumQueries(1):
+            p.clean()
         # We fetch the object again to populate the path.
         return Place.objects.get(pk=p.pk)
 
     def create_test_places(self):
         self.correct_raw_places_data = [
             (path(0), 'France'),
             (path(0, 0), 'Normandie'),
@@ -78,14 +80,15 @@
         yield osterreich
         vienne = self.create_place('Vienne', osterreich)
         yield vienne
         poitou_charentes = self.create_place('Poitou-Charentes', france)
         yield poitou_charentes
         yield self.create_place('Poitiers', vienne)
         vienne.parent = poitou_charentes
+        vienne.clean()
         vienne.save()
         yield vienne
 
     def create_all_test_places(self):
         list(self.create_test_places())
 
     def assertPlaces(self, values, queryset=None, n_queries=1):
@@ -109,14 +112,15 @@
             self.assertEqual(place1.path.value, path(0))
         with self.assertNumQueries(1):
             place2 = Place.objects.create(name='place2', parent=place1)
         with self.assertNumQueries(1):
             self.assertEqual(place2.path.value, path(0, 0))
         with self.assertNumQueries(1):
             place2.parent = None
+            place2.clean()
             place2.save()
         with self.assertNumQueries(1):
             self.assertEqual(place2.path.value, path(1))
 
     def test_insert(self):
         it = self.create_test_places()
         next(it)
@@ -238,14 +242,15 @@
 
     def test_move_root_to_prev_root(self):
         self.create_all_test_places()
 
         osterreich = Place.objects.get(name='Österreich')
         osterreich.name = 'Autriche'
         with self.assertNumQueries(1):
+            osterreich.clean()
             osterreich.save()
         self.assertPlaces([
             (path(-1), 'Autriche'),
             (path(0), 'France'),
             (path(0, 0), 'Normandie'),
             (path(0, 0, -1), 'Eure'),
             (path(0, 0, -0.5), 'Manche'),
@@ -270,14 +275,15 @@
 
     def test_move_root_to_next_root(self):
         self.create_all_test_places()
 
         france = Place.objects.get(name='France')
         france.name = 'République française'
         with self.assertNumQueries(1):
+            france.clean()
             france.save()
         self.assertPlaces([
             (path(1), 'Österreich'),
             (path(2), 'République française'),
             (path(2, 0), 'Normandie'),
             (path(2, 0, -1), 'Eure'),
             (path(2, 0, -0.5), 'Manche'),
@@ -315,14 +321,16 @@
             (path(0, 1, 0, 0), 'Poitiers'),
             (path(0.5), 'Île-de-France'),
             (path(1), 'Österreich'),
         ])
 
         little_france.parent = Place.objects.get(name='France')
         with self.assertNumQueries(1):
+            little_france.clean()
+        with self.assertNumQueries(1):
             little_france.save()
         self.assertPlaces([
             (path(0), 'France'),
             (path(0, -1), 'Île-de-France'),
             (path(0, 0), 'Normandie'),
             (path(0, 0, -1), 'Eure'),
             (path(0, 0, -0.5), 'Manche'),
@@ -362,14 +370,16 @@
             (path(0, 1, 0), 'Vienne'),
             (path(0, 1, 0, 0), 'Poitiers'),
             (path(1), 'Österreich'),
         ])
 
         bretagne.parent = Place.objects.get(name='France')
         with self.assertNumQueries(1):
+            bretagne.clean()
+        with self.assertNumQueries(1):
             bretagne.save()
         self.assertPlaces([
             (path(0), 'France'),
             (path(0, -1), 'Bretagne'),
             (path(0, 0), 'Normandie'),
             (path(0, 0, -1), 'Eure'),
             (path(0, 0, -0.5), 'Manche'),
@@ -409,14 +419,16 @@
             (path(0, 1, 0, 0), 'Poitiers'),
             (path(0.5), 'Grattenoix'),
             (path(1), 'Österreich'),
         ])
 
         grattenoix.parent = Place.objects.get(name='Seine-Maritime')
         with self.assertNumQueries(1):
+            grattenoix.clean()
+        with self.assertNumQueries(1):
             grattenoix.save()
         self.assertPlaces([
             (path(0), 'France'),
             (path(0, 0), 'Normandie'),
             (path(0, 0, -1), 'Eure'),
             (path(0, 0, -0.5), 'Manche'),
             (path(0, 0, 0), 'Seine-Maritime'),
@@ -456,14 +468,16 @@
             (path(0, 1, 0), 'Vienne'),
             (path(0, 1, 0, 0), 'Poitiers'),
             (path(1), 'Österreich'),
         ])
 
         evreux.parent = Place.objects.get(name='Eure')
         with self.assertNumQueries(1):
+            evreux.clean()
+        with self.assertNumQueries(1):
             evreux.save()
         self.assertPlaces([
             (path(0), 'France'),
             (path(0, 0), 'Normandie'),
             (path(0, 0, -1), 'Eure'),
             (path(0, 0, -1, 0), 'Évreux'),
             (path(0, 0, -0.5), 'Manche'),
@@ -1040,21 +1054,21 @@
         for place in Place.objects.all():
             self.assertFalse(place.is_descendant_of(place))
             self.assertTrue(place.is_descendant_of(place,
                                                    include_self=True))
             for descendant in place.get_descendants():
                 self.assertTrue(descendant.is_descendant_of(place))
 
-    def test_get_roots(self):
+    def test_filter_roots(self):
         self.create_all_test_places()
 
         self.assertPlaces([
             (path(0), 'France'),
             (path(1), 'Österreich'),
-        ], queryset=Place.get_roots())
+        ], queryset=Place.objects.filter_roots())
 
     def test_rebuild(self):
         self.create_all_test_places()
 
         with Place.disabled_tree_trigger():
             updated_places = []
             for i, place in enumerate(Place.objects.order_by('name')):
@@ -1108,25 +1122,44 @@
             Place.rebuild_paths()
         self.assertPlaces(self.correct_places_data)
 
     def test_cycle(self):
         # Simple cycle
         a = Place.objects.create(name='a')
         a.parent = a
+
         with self.assertRaisesMessage(
-                InternalError, 'Cannot set itself or a descendant as parent.'):
+            ValidationError,
+            "{'parent': [\"Value 'a' is not a valid choice.\"]}",
+        ):
+            with transaction.atomic():
+                with self.assertNumQueries(1):
+                    a.clean()
+
+        with self.assertRaisesMessage(
+            InternalError, 'Cannot set itself or a descendant as parent.',
+        ):
             with transaction.atomic():
                 with self.assertNumQueries(1):
                     a.save()
 
         # Complex cycle
         b = Place.objects.create(name='b', parent=a)
         c = Place.objects.create(name='c', parent=b)
         d = Place.objects.create(name='d', parent=c)
         a.parent = d
+
+        with self.assertRaisesMessage(
+            ValidationError,
+            "{'parent': [\"Value 'd' is not a valid choice.\"]}",
+        ):
+            with transaction.atomic():
+                with self.assertNumQueries(1):
+                    a.clean()
+
         with self.assertRaisesMessage(
                 InternalError, 'Cannot set itself or a descendant as parent.'):
             with transaction.atomic():
                 with self.assertNumQueries(1):
                     a.save()
 
     def test_path_in_cursor(self):
@@ -1173,14 +1206,15 @@
         self.wolfgang_mozart = Person.objects.create(
             century=18, first_name='Wolfgang Amadeus', last_name='Mozart',
         )
         self.leopold_mozart = Person.objects.create(
             century=18, first_name='Leopold', last_name='Mozart',
         )
         self.wolfgang_mozart.parent = self.leopold_mozart
+        self.wolfgang_mozart.clean()
         self.wolfgang_mozart.save()
         self.maria_anna_mozart = Person.objects.create(
             parent=self.leopold_mozart,
             century=18, first_name='Maria Anna', last_name='Mozart',
         )
         self.tchaikovski = Person.objects.create(
             century=19, first_name='Piotr Ilyich', last_name='Tchaikovski',
@@ -1214,14 +1248,15 @@
         with Person.disabled_tree_trigger():
             for i, person in enumerate(
                 Person.objects.order_by('-last_name', '-first_name')
             ):
                 # We add 10 to make sure
                 # we do not clash with the existing paths.
                 person.path = [10 + i]
+                person.clean()
                 person.save()
         self.assertPersons([
             (path(10), 18, 'Antonio Lucio', 'Vivaldi'),
             (path(11), 19, 'Piotr Ilyich', 'Tchaikovski'),
             (path(12), 19, 'Johann (son)', 'Strauss'),
             (path(13), 19, 'Johann (father)', 'Strauss'),
             (path(14), 20, '', 'Strauss'),
@@ -1265,14 +1300,15 @@
         self.assertLess(vivaldi2.path, self.vivaldi.path)
         self.assertPersons([
             (path(-4), 18, 'Some', 'Guy'),
             (path(-1), 18, 'Antonio Lucio', 'Vivaldi'),
         ], queryset=Person.objects.filter(last_name__in=['Vivaldi', 'Guy']))
         vivaldi2.first_name = 'Antonio Lucio'
         vivaldi2.last_name = 'Vivaldi'
+        vivaldi2.clean()
         vivaldi2.save()
         self.assertPersons([
             (path(-1), 18, 'Antonio Lucio', 'Vivaldi'),
             (path(-0.875), 18, 'Antonio Lucio', 'Vivaldi'),
         ], queryset=Person.objects.filter(last_name='Vivaldi'))
         Person.rebuild_paths()
         self.assertPersons([
```

### Comparing `django-tree-0.5.5/PKG-INFO` & `django-tree-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tree
-Version: 0.5.5
+Version: 0.5.6
 Summary: Fast and easy tree structures.
 Home-page: https://github.com/BertrandBordage/django-tree
 Author: Bertrand Bordage
 Author-email: bordage.bertrand@gmail.com
 License: BSD
 Description: Django-tree
         ===========
@@ -218,15 +218,15 @@
             obj.get_prev_sibling()  # Fetches the previous sibling.
             obj.get_next_sibling()
             # Same as `get_prev_sibling`, except that we get the first public one.
             obj.get_prev_siblings().filter(public=True).first()
             other = YourModel.objects.all()[1]
             obj.is_ancestor_of(other)
             obj.is_descendant_of(other, include_self=True)
-            YourModel.get_roots()
+            YourModel.objects.filter_roots()
         
             #
             # Advanced usage
             # Use the following methods only if you understand exactly what they mean.
             #
         
             YourModel.rebuild_paths()  # Rebuilds all paths of this field, useful only
```

### Comparing `django-tree-0.5.5/CHANGELOG.rst` & `django-tree-0.5.6/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+0.5.6 (2023-07-09)
+==================
+
+- Adds a model validation in addition to the existing database error,
+  when users try to make a cycle (mark a node as its own parent or ancestor)
+- Moves ``PathField.get_roots()`` to ``TreeQuerySetMixin.filter_roots()``.
+- Fixes a ``TypeError`` when using ``TreeQuerySetMixin.get_descendants()``
+  on an empty queryset.
+
 0.5.5 (2023-07-06)
 ==================
 
 Fixes another PostgreSQL 12 compatibility issue.
 
 0.5.4 (2023-07-06)
 ==================
```

### Comparing `django-tree-0.5.5/LICENSE` & `django-tree-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/migrations/0002_remove_old_functions.py` & `django-tree-0.5.6/tree/migrations/0002_remove_old_functions.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/sql/postgresql.py` & `django-tree-0.5.6/tree/sql/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             UPDATE {table} AS t2 SET {path} = t1.path
             FROM generate_paths AS t1
             WHERE t2.{pk} = t1.pk AND t2.{pk} != $1.{pk}
                 AND (t2.{path} IS NULL OR t2.{path} != t1.path)
         )
         SELECT path FROM generate_paths
         WHERE pk = $1.{pk}
+        LIMIT 1
     """, using=['OLD'], into=[f'NEW.{path}'])
 
     get_new_parent_path = execute_format(f"""
         SELECT {path} FROM {table} WHERE {pk} = $1.{parent}
     """, using=['NEW'], into=['new_parent_path'])
 
     get_prev_sibling_decimal = execute_format(f"""
@@ -133,15 +134,14 @@
     """, using=['NEW', 'OLD'])
 
     row_unchanged = join_and([
         compare_columns(f'OLD.{where_column}', f'NEW.{where_column}')
         for where_column in [parent, *where_columns]
     ])
 
-    # TODO: Add `LIMIT 1` where appropriate to see if it optimises a bit.
     return f"""
         CREATE OR REPLACE FUNCTION update_{table}_{path}_paths() RETURNS trigger AS $$
         DECLARE
             prev_sibling_decimal decimal := NULL;
             next_sibling_decimal decimal := NULL;
             new_parent_path decimal[];
         BEGIN
@@ -185,15 +185,14 @@
                     BETWEEN prev_sibling_decimal AND next_sibling_decimal
             THEN
                 RETURN NEW;
             END IF;
             
             {get_new_parent_path}
             IF TG_OP = 'UPDATE' THEN
-                -- TODO: Add this behaviour to the model validation.
                 IF new_parent_path[:array_length(OLD.{path}, 1)] = OLD.{path} THEN
                     RAISE 'Cannot set itself or a descendant as parent.';
                 END IF;
             END IF;
             
             NEW.{path} = new_parent_path || (
                 prev_sibling_decimal + next_sibling_decimal
```

### Comparing `django-tree-0.5.5/tree/sql/base.py` & `django-tree-0.5.6/tree/sql/base.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/query.py` & `django-tree-0.5.6/tree/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,33 @@
     raise ValueError(
         'You need to specify which `PathField` to use for this query '
         'among these values: %s' % [f.name for f in path_fields])
 
 
 # TODO: Implement a faster `QuerySet.delete` and add it to the benchmark.
 class TreeQuerySetMixin:
-    def _get_path_field_name(self, name):
-        return _get_path_field(self.model, name).name
+    def _get_path_field_attname(self, name):
+        return _get_path_field(self.model, name).attname
+
+    def filter_roots(self, path_field=None):
+        attname = self._get_path_field_attname(path_field)
+        return self.filter(**{f'{attname}__level': 1})
 
     def get_descendants(self, include_self=False, path_field=None):
-        name = self._get_path_field_name(path_field)
+        attname = self._get_path_field_attname(path_field)
         # TODO: Avoid doing an extra query.
-        ancestor_paths = list(self.values_list(name, flat=True))
+        ancestor_paths = list(self.values_list(attname, flat=True))
         queryset = self.model.objects.all()
+        if not ancestor_paths:
+            return queryset.none()
         if not include_self:
-            queryset = queryset.exclude(**{name + '__in': ancestor_paths})
+            queryset = queryset.exclude(**{attname + '__in': ancestor_paths})
         return queryset.filter(
             reduce(operator.or_, [
-                Q(**{name + '__descendant_of': ancestor_path})
+                Q(**{attname + '__descendant_of': ancestor_path})
                 for ancestor_path in ancestor_paths
             ])
         )
 
 
 class TreeQuerySet(TreeQuerySetMixin, QuerySet):
     pass
```

### Comparing `django-tree-0.5.5/tree/signals.py` & `django-tree-0.5.6/tree/signals.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/apps.py` & `django-tree-0.5.6/tree/apps.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/models.py` & `django-tree-0.5.6/tree/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from contextlib import contextmanager
 from typing import Optional
 
+from django.core.exceptions import ValidationError
 from django.db import DEFAULT_DB_ALIAS, transaction
 from django.db.models import Model
 
 from .query import _get_path_fields, _get_path_field, TreeManager
 
 
 class TreeModelMixin:
@@ -69,18 +70,43 @@
                                 include_self=include_self))
 
     def is_descendant_of(self, other, include_self=False, path_field=None):
         return (self._get_path_value(path_field)
                 .is_descendant_of(other._get_path_value(path_field),
                                   include_self=include_self))
 
-    # TODO: Remove this method.
-    @classmethod
-    def get_roots(cls, path_field=None):
-        return cls._get_path_field(path_field).get_roots()
+    def clean(self):
+        super().clean()
+        if not self._state.adding:
+            for path_field in self._get_path_fields():
+                old_path = getattr(self, path_field.attname)
+                parent_field = path_field.parent_field
+                new_parent = getattr(self, parent_field.name)
+                if not new_parent:
+                    continue
+
+                if not isinstance(new_parent, Model):
+                    try:
+                        new_parent = self.__class__._default_manager.get(
+                            pk=new_parent,
+                        )
+                    except self.__class__.DoesNotExist:
+                        new_parent = self
+
+                new_parent_path = getattr(new_parent, path_field.attname)
+                if new_parent_path.is_descendant_of(
+                    old_path, include_self=True,
+                ):
+                    raise ValidationError({
+                        parent_field.name: ValidationError(
+                            parent_field.error_messages['invalid_choice'],
+                            code='invalid_choice',
+                            params={'value': str(new_parent)},
+                        )
+                    })
 
     def delete(self, using=None, **kwargs):
         assert self.pk is not None, (
             "%s object can't be deleted because "
             "its %s attribute is set to None." %
             (self._meta.object_name, self._meta.pk.attname)
         )
```

### Comparing `django-tree-0.5.5/tree/lookups.py` & `django-tree-0.5.6/tree/lookups.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/operations.py` & `django-tree-0.5.6/tree/operations.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/types.py` & `django-tree-0.5.6/tree/types.py`

 * *Files identical despite different names*

### Comparing `django-tree-0.5.5/tree/fields.py` & `django-tree-0.5.6/tree/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         name, path, args, kwargs = super(PathField, self).deconstruct()
         del kwargs['base_field']
         if not kwargs['editable']:
             del kwargs['editable']
         del kwargs['default']
         del kwargs['null']
         del kwargs['size']
-        if self.order_by != []:
+        if self.order_by:
             kwargs['order_by'] = self.order_by
         if self.parent_field_name != 'parent':
             kwargs['parent_field_name'] = self.parent_field_name
         return name, path, args, kwargs
 
     def from_db_value(self, value, expression, connection):
         if isinstance(value, Path):
@@ -100,20 +100,14 @@
         return Path(self, value)
 
     def get_prep_value(self, value):
         if isinstance(value, Path):
             return value.value
         return value
 
-    # TODO: Move this method to a queryset.
-    def get_roots(self):
-        return self.model._default_manager.filter(**{
-            f'{self.attname}__level': 1,
-        })
-
     def _check_database_backend(self, db_alias):
         if connections[db_alias].vendor != 'postgresql':
             raise NotImplementedError(
                 'django-tree is only for PostgreSQL for now.')
 
     def rebuild(self, db_alias=DEFAULT_DB_ALIAS):
         self._check_database_backend(db_alias)
```

