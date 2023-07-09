# Comparing `tmp/crown-0.3.0.tar.gz` & `tmp/crown-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crown-0.3.0.tar", last modified: Tue Jun 27 03:34:55 2023, max compression
+gzip compressed data, was "crown-0.3.1.tar", last modified: Sun Jul  9 03:29:04 2023, max compression
```

## Comparing `crown-0.3.0.tar` & `crown-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-06-27 03:34:55.979344 crown-0.3.0/
--rw-r--r--   0 machine    (501) staff       (20)     1064 2023-06-27 00:25:34.000000 crown-0.3.0/LICENSE
--rw-r--r--   0 machine    (501) staff       (20)    22502 2023-06-27 03:34:55.979198 crown-0.3.0/PKG-INFO
--rw-r--r--   0 machine    (501) staff       (20)    22062 2023-06-27 03:15:14.000000 crown-0.3.0/README.rst
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-06-27 03:34:55.978256 crown-0.3.0/crown/
--rw-r--r--   0 machine    (501) staff       (20)      395 2023-06-27 03:15:23.000000 crown-0.3.0/crown/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)     1718 2023-06-27 01:43:26.000000 crown-0.3.0/crown/common.py
--rw-r--r--   0 machine    (501) staff       (20)    18278 2023-06-27 02:28:59.000000 crown-0.3.0/crown/crown.py
--rw-r--r--   0 machine    (501) staff       (20)     7227 2023-06-27 02:39:01.000000 crown-0.3.0/crown/database.py
--rw-r--r--   0 machine    (501) staff       (20)     3333 2023-06-27 01:44:38.000000 crown-0.3.0/crown/eng_taosrestful.py
--rw-r--r--   0 machine    (501) staff       (20)     3469 2023-06-27 01:44:45.000000 crown-0.3.0/crown/eng_taosrestful3.py
--rw-r--r--   0 machine    (501) staff       (20)     7895 2023-06-27 02:27:17.000000 crown-0.3.0/crown/field.py
--rw-r--r--   0 machine    (501) staff       (20)    27152 2023-06-27 02:58:52.000000 crown-0.3.0/crown/query.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-06-27 03:34:55.978992 crown-0.3.0/crown.egg-info/
--rw-r--r--   0 machine    (501) staff       (20)    22502 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/PKG-INFO
--rw-r--r--   0 machine    (501) staff       (20)      319 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/SOURCES.txt
--rw-r--r--   0 machine    (501) staff       (20)        1 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/dependency_links.txt
--rw-r--r--   0 machine    (501) staff       (20)       17 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/requires.txt
--rw-r--r--   0 machine    (501) staff       (20)        6 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/top_level.txt
--rw-r--r--   0 machine    (501) staff       (20)       38 2023-06-27 03:34:55.979385 crown-0.3.0/setup.cfg
--rw-r--r--   0 machine    (501) staff       (20)     1099 2023-06-27 03:23:04.000000 crown-0.3.0/setup.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-07-09 03:29:04.430983 crown-0.3.1/
+-rw-r--r--   0 machine    (501) staff       (20)     1064 2023-06-27 00:25:34.000000 crown-0.3.1/LICENSE
+-rw-r--r--   0 machine    (501) staff       (20)    22502 2023-07-09 03:29:04.430802 crown-0.3.1/PKG-INFO
+-rw-r--r--   0 machine    (501) staff       (20)    22062 2023-06-27 03:15:14.000000 crown-0.3.1/README.rst
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-07-09 03:29:04.429866 crown-0.3.1/crown/
+-rw-r--r--   0 machine    (501) staff       (20)      395 2023-06-27 03:15:23.000000 crown-0.3.1/crown/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)     1718 2023-06-27 01:43:26.000000 crown-0.3.1/crown/common.py
+-rw-r--r--   0 machine    (501) staff       (20)    18278 2023-06-27 02:28:59.000000 crown-0.3.1/crown/crown.py
+-rw-r--r--   0 machine    (501) staff       (20)     7227 2023-06-27 02:39:01.000000 crown-0.3.1/crown/database.py
+-rw-r--r--   0 machine    (501) staff       (20)     3333 2023-06-27 01:44:38.000000 crown-0.3.1/crown/eng_taosrestful.py
+-rw-r--r--   0 machine    (501) staff       (20)     3521 2023-07-09 03:02:01.000000 crown-0.3.1/crown/eng_taosrestful3.py
+-rw-r--r--   0 machine    (501) staff       (20)     7992 2023-07-09 03:23:56.000000 crown-0.3.1/crown/field.py
+-rw-r--r--   0 machine    (501) staff       (20)    27152 2023-06-27 02:58:52.000000 crown-0.3.1/crown/query.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-07-09 03:29:04.430524 crown-0.3.1/crown.egg-info/
+-rw-r--r--   0 machine    (501) staff       (20)    22502 2023-07-09 03:29:04.000000 crown-0.3.1/crown.egg-info/PKG-INFO
+-rw-r--r--   0 machine    (501) staff       (20)      319 2023-07-09 03:29:04.000000 crown-0.3.1/crown.egg-info/SOURCES.txt
+-rw-r--r--   0 machine    (501) staff       (20)        1 2023-07-09 03:29:04.000000 crown-0.3.1/crown.egg-info/dependency_links.txt
+-rw-r--r--   0 machine    (501) staff       (20)       17 2023-07-09 03:29:04.000000 crown-0.3.1/crown.egg-info/requires.txt
+-rw-r--r--   0 machine    (501) staff       (20)        6 2023-07-09 03:29:04.000000 crown-0.3.1/crown.egg-info/top_level.txt
+-rw-r--r--   0 machine    (501) staff       (20)       38 2023-07-09 03:29:04.431028 crown-0.3.1/setup.cfg
+-rw-r--r--   0 machine    (501) staff       (20)     1099 2023-07-09 03:27:59.000000 crown-0.3.1/setup.py
```

### Comparing `crown-0.3.0/LICENSE` & `crown-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crown-0.3.0/PKG-INFO` & `crown-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crown
-Version: 0.3.0
+Version: 0.3.1
 Summary: crown is a simple and small ORM for Time Series Database (TSDB) tdengine(taos), making it easy to learn and intuitive to use.
 Home-page: https://github.com/machine-w/crown
 Author: machine-w
 Author-email: steve2008.ma@gmail.com
 Keywords: orm,taos,TDengine,TSDB,Time Series Database,connector,python
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `crown-0.3.0/README.rst` & `crown-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `crown-0.3.0/crown/common.py` & `crown-0.3.1/crown/common.py`

 * *Files identical despite different names*

### Comparing `crown-0.3.0/crown/crown.py` & `crown-0.3.1/crown/crown.py`

 * *Files identical despite different names*

### Comparing `crown-0.3.0/crown/database.py` & `crown-0.3.1/crown/database.py`

 * *Files identical despite different names*

### Comparing `crown-0.3.0/crown/eng_taosrestful.py` & `crown-0.3.1/crown/eng_taosrestful.py`

 * *Files identical despite different names*

### Comparing `crown-0.3.0/crown/eng_taosrestful3.py` & `crown-0.3.1/crown/eng_taosrestful3.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,14 +94,14 @@
     
     def commit(self):
         pass
     def rollback(self):
         pass
 class TaosRestful():
     
-    def connect(self,database, host='localhost',port=6041,user='root',passwd='taosdata'):
-        conn = Conn(database,'http://%s:%s/%s' % (host,port,PATH),user,passwd)
+    def connect(self,database, host='localhost',port=6041,user='root',passwd='taosdata',timezone='Asia/Shanghai',db=''):
+        conn = Conn(database,'http://%s:%s/%s/%s?tz=%s' % (host,port,PATH,db,timezone),user,passwd)
         return conn
         
 taos_resetful = TaosRestful()
```

### Comparing `crown-0.3.0/crown/field.py` & `crown-0.3.1/crown/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,29 +241,30 @@
     def field_attributes(self):
         return {'max_length': 255}
 
     def coerce(self, value):
         value =  value or ''
         return value[:self.attributes['max_length']]
 def format_date_time(value, formats, post_process=None):
-    post_process = post_process or (lambda x: x)
+    post_process = post_process or (lambda x: x.astimezone(datetime.timezone.utc).replace(tzinfo=None))
     for fmt in formats:
         try:
             return post_process(datetime.datetime.strptime(value, fmt))
         except ValueError:
             pass
     return value
 class VarCharField(BinaryField):
     db_field = 'varchar'
 class DateTimeField(Field):
     db_field = 'datetime'
 
     def field_attributes(self):
         return {
             'formats': [
+                '%Y-%m-%dT%H:%M:%S.%f%z',
                 '%Y-%m-%dT%H:%M:%S.%fZ'
                 # '%Y-%m-%d %H:%M:%S.%f',
                 # '%Y-%m-%d %H:%M:%S',
                 # '%Y-%m-%d',
             ]
         }
```

### Comparing `crown-0.3.0/crown/query.py` & `crown-0.3.1/crown/query.py`

 * *Files identical despite different names*

### Comparing `crown-0.3.0/crown.egg-info/PKG-INFO` & `crown-0.3.1/crown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crown
-Version: 0.3.0
+Version: 0.3.1
 Summary: crown is a simple and small ORM for Time Series Database (TSDB) tdengine(taos), making it easy to learn and intuitive to use.
 Home-page: https://github.com/machine-w/crown
 Author: machine-w
 Author-email: steve2008.ma@gmail.com
 Keywords: orm,taos,TDengine,TSDB,Time Series Database,connector,python
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `crown-0.3.0/setup.py` & `crown-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     packages=['crown'],
     description="crown is a simple and small ORM for Time Series Database (TSDB) tdengine(taos), making it easy to learn and intuitive to use.",
     long_description=README,
     long_description_content_type='text/markdown',
     install_requires=[
         'requests>=2.23.0'
     ],
-    version='0.3.0',
+    version='0.3.1',
     url='https://github.com/machine-w/crown',
     author='machine-w',
     author_email='steve2008.ma@gmail.com',
     keywords=['orm','taos', 'TDengine', 'TSDB','Time Series Database','connector','python'],
     tests_require=[
         'pytest',
         'pytest-faker',
```

