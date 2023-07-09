# Comparing `tmp/tsc-es-0.2.tar.gz` & `tmp/tsc-es-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-es-0.2.tar", last modified: Sun Jul  9 14:48:16 2023, max compression
+gzip compressed data, was "tsc-es-0.3.tar", last modified: Sun Jul  9 14:51:32 2023, max compression
```

## Comparing `tsc-es-0.2.tar` & `tsc-es-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:48:16.468776 tsc-es-0.2/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-09 14:48:16.468776 tsc-es-0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 14:48:16.468776 tsc-es-0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-09 14:47:33.000000 tsc-es-0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:48:16.464775 tsc-es-0.2/tsc_es/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.2/tsc_es/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16571 2023-07-09 14:47:24.000000 tsc-es-0.2/tsc_es/mongo_es.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:48:16.468776 tsc-es-0.2/tsc_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-09 14:48:16.000000 tsc-es-0.2/tsc_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-09 14:48:16.000000 tsc-es-0.2/tsc_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 14:48:16.000000 tsc-es-0.2/tsc_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-09 14:48:16.000000 tsc-es-0.2/tsc_es.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-09 14:48:16.000000 tsc-es-0.2/tsc_es.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:51:32.550081 tsc-es-0.3/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-09 14:51:32.550081 tsc-es-0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 14:51:32.550081 tsc-es-0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-09 14:51:30.000000 tsc-es-0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:51:32.550081 tsc-es-0.3/tsc_es/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.3/tsc_es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16553 2023-07-09 14:51:26.000000 tsc-es-0.3/tsc_es/mongo_es.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 14:51:32.550081 tsc-es-0.3/tsc_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-09 14:51:32.000000 tsc-es-0.3/tsc_es.egg-info/top_level.txt
```

### Comparing `tsc-es-0.2/LICENSE` & `tsc-es-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-es-0.2/setup.py` & `tsc-es-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = ''
 
 setup(
     name='tsc-es',
-    version='0.2',
+    version='0.3',
     description="mongo to es",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tsc',
     license='GPLv3',
     url='',
     keywords='tools',
```

### Comparing `tsc-es-0.2/tsc_es/mongo_es.py` & `tsc-es-0.3/tsc_es/mongo_es.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,16 @@
                 "properties": properties,
             },
         },
     }
     if is_stream:
         index_template_body['data_stream'] = {}
     # pprint(index_template_body)
-    ret = client.indices.put_index_template(name=template_name, **index_template_body)
-    logging.warning(f"Template '{template_name}' is created: {ret}")
+    ret = client.indices.put_index_template(name=name, **index_template_body)
+    logging.warning(f"Template '{name}' is created: {ret}")
     return True
 
 
 def create_index(client: Elasticsearch, name: str, is_stream=False):
     """
     创建索引
     :param client: es 客户端
```

