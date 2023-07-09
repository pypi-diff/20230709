# Comparing `tmp/nescs-0.3.2.tar.gz` & `tmp/nescs-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nescs-0.3.2.tar", last modified: Sat Jul  8 18:21:05 2023, max compression
+gzip compressed data, was "nescs-0.3.3.tar", last modified: Sun Jul  9 07:03:19 2023, max compression
```

## Comparing `nescs-0.3.2.tar` & `nescs-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-08 18:21:05.614515 nescs-0.3.2/
--rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-08 05:36:40.000000 nescs-0.3.2/MANIFEST.in
--rw-r--r--   0 twoics    (1000) twoics    (1000)     5094 2023-07-08 18:21:05.614515 nescs-0.3.2/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)     4882 2023-07-08 18:18:34.000000 nescs-0.3.2/README.rst
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-08 18:21:05.613515 nescs-0.3.2/nesc/
--rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-08 05:36:40.000000 nescs-0.3.2/nesc/__init__.py
--rw-r--r--   0 twoics    (1000) twoics    (1000)     5189 2023-07-08 18:11:53.000000 nescs-0.3.2/nesc/service.py
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-08 18:21:05.614515 nescs-0.3.2/nescs.egg-info/
--rw-r--r--   0 twoics    (1000) twoics    (1000)     5094 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)      233 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/SOURCES.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/dependency_links.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)       42 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/requires.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-08 18:21:05.000000 nescs-0.3.2/nescs.egg-info/top_level.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-08 05:36:40.000000 nescs-0.3.2/pyproject.toml
--rw-r--r--   0 twoics    (1000) twoics    (1000)      408 2023-07-08 18:21:05.614515 nescs-0.3.2/setup.cfg
--rw-r--r--   0 twoics    (1000) twoics    (1000)      131 2023-07-08 05:36:40.000000 nescs-0.3.2/setup.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:03:19.927134 nescs-0.3.3/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-08 05:36:40.000000 nescs-0.3.3/MANIFEST.in
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5049 2023-07-09 07:03:19.927134 nescs-0.3.3/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     4837 2023-07-09 03:13:48.000000 nescs-0.3.3/README.rst
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:03:19.926134 nescs-0.3.3/nesc/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-08 05:36:40.000000 nescs-0.3.3/nesc/__init__.py
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     6964 2023-07-09 03:13:48.000000 nescs-0.3.3/nesc/service.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-09 07:03:19.927134 nescs-0.3.3/nescs.egg-info/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5049 2023-07-09 07:03:19.000000 nescs-0.3.3/nescs.egg-info/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      233 2023-07-09 07:03:19.000000 nescs-0.3.3/nescs.egg-info/SOURCES.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-09 07:03:19.000000 nescs-0.3.3/nescs.egg-info/dependency_links.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       42 2023-07-09 07:03:19.000000 nescs-0.3.3/nescs.egg-info/requires.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-09 07:03:19.000000 nescs-0.3.3/nescs.egg-info/top_level.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-09 06:58:46.000000 nescs-0.3.3/pyproject.toml
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      408 2023-07-09 07:03:19.927134 nescs-0.3.3/setup.cfg
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      131 2023-07-09 06:58:46.000000 nescs-0.3.3/setup.py
```

### Comparing `nescs-0.3.2/PKG-INFO` & `nescs-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nescs
-Version: 0.3.2
+Version: 0.3.3
 Summary: Библиотека создания моделей вложенных сериализаторов
 Author: cifra-k
 License: MIT
 Requires-Python: >=3.8
 
 =====
 NESCS
@@ -64,15 +64,14 @@
             )
 
         def create(self, validated_data):
             service = SerializerCreateService(self, validated_data, m2m_fields=['publications'])
             current_instance = super().create(validated_data)
 
             service.create_m2m_instances(
-                related_name='publications',
                 parent_instance=current_instance
             )
             return current_instance
 
 One to one case
 ~~~~~~~~~~~~~~~~~
 Для создание объектов с отношением **o2o** используется метод ``create_child_instances``
```

### Comparing `nescs-0.3.2/README.rst` & `nescs-0.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
             )
 
         def create(self, validated_data):
             service = SerializerCreateService(self, validated_data, m2m_fields=['publications'])
             current_instance = super().create(validated_data)
 
             service.create_m2m_instances(
-                related_name='publications',
                 parent_instance=current_instance
             )
             return current_instance
 
 One to one case
 ~~~~~~~~~~~~~~~~~
 Для создание объектов с отношением **o2o** используется метод ``create_child_instances``
```

### Comparing `nescs-0.3.2/nescs.egg-info/PKG-INFO` & `nescs-0.3.3/nescs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nescs
-Version: 0.3.2
+Version: 0.3.3
 Summary: Библиотека создания моделей вложенных сериализаторов
 Author: cifra-k
 License: MIT
 Requires-Python: >=3.8
 
 =====
 NESCS
@@ -64,15 +64,14 @@
             )
 
         def create(self, validated_data):
             service = SerializerCreateService(self, validated_data, m2m_fields=['publications'])
             current_instance = super().create(validated_data)
 
             service.create_m2m_instances(
-                related_name='publications',
                 parent_instance=current_instance
             )
             return current_instance
 
 One to one case
 ~~~~~~~~~~~~~~~~~
 Для создание объектов с отношением **o2o** используется метод ``create_child_instances``
```

