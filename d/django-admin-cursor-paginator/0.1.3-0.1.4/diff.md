# Comparing `tmp/django-admin-cursor-paginator-0.1.3.tar.gz` & `tmp/django-admin-cursor-paginator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-cursor-paginator-0.1.3.tar", last modified: Sat Sep 17 18:55:29 2022, max compression
+gzip compressed data, was "django-admin-cursor-paginator-0.1.4.tar", last modified: Sun Jul  9 14:26:19 2023, max compression
```

## Comparing `django-admin-cursor-paginator-0.1.3.tar` & `django-admin-cursor-paginator-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 a1tus     (1000) a1tus     (1000)        0 2022-09-17 18:55:29.187339 django-admin-cursor-paginator-0.1.3/
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     1054 2021-03-10 18:30:54.000000 django-admin-cursor-paginator-0.1.3/LICENSE
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)       86 2021-03-10 19:19:41.000000 django-admin-cursor-paginator-0.1.3/MANIFEST.in
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     6321 2022-09-17 18:55:29.187339 django-admin-cursor-paginator-0.1.3/PKG-INFO
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     3864 2022-09-16 20:11:52.000000 django-admin-cursor-paginator-0.1.3/README.md
-drwxrwxr-x   0 a1tus     (1000) a1tus     (1000)        0 2022-09-17 18:55:29.187339 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)       54 2021-03-10 18:20:39.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/__init__.py
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     1140 2022-09-17 18:40:17.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/admin.py
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     1485 2021-08-07 17:00:47.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/cursor.py
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     3397 2022-02-26 22:22:27.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/paginator.py
-drwxrwxr-x   0 a1tus     (1000) a1tus     (1000)        0 2022-09-17 18:55:29.183339 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templates/
-drwxrwxr-x   0 a1tus     (1000) a1tus     (1000)        0 2022-09-17 18:55:29.187339 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templates/admin_cursor_paginator/
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)      149 2021-01-13 10:55:46.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templates/admin_cursor_paginator/change_list.html
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)      651 2021-02-14 14:53:41.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templates/admin_cursor_paginator/pagination.html
-drwxrwxr-x   0 a1tus     (1000) a1tus     (1000)        0 2022-09-17 18:55:29.187339 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templatetags/
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)        0 2021-03-10 19:41:13.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templatetags/__init__.py
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     1084 2021-01-13 10:55:46.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templatetags/admin_cursor_paginator_tags.py
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)       22 2022-09-17 18:18:00.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/version.py
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)      589 2021-01-13 10:55:46.000000 django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/views.py
-drwxrwxr-x   0 a1tus     (1000) a1tus     (1000)        0 2022-09-17 18:55:29.187339 django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     6321 2022-09-17 18:55:29.000000 django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/PKG-INFO
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)      826 2022-09-17 18:55:29.000000 django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/SOURCES.txt
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)        1 2022-09-17 18:55:29.000000 django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/dependency_links.txt
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)        1 2022-09-17 18:55:29.000000 django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/not-zip-safe
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)       12 2022-09-17 18:55:29.000000 django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/requires.txt
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)       23 2022-09-17 18:55:29.000000 django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/top_level.txt
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)     1576 2022-09-17 18:55:29.187339 django-admin-cursor-paginator-0.1.3/setup.cfg
--rw-rw-r--   0 a1tus     (1000) a1tus     (1000)       63 2021-03-10 19:06:26.000000 django-admin-cursor-paginator-0.1.3/setup.py
+drwxr-xr-x   0 a1tus      (501) staff       (20)        0 2023-07-09 14:26:19.508134 django-admin-cursor-paginator-0.1.4/
+-rw-r--r--   0 a1tus      (501) staff       (20)     1054 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/LICENSE
+-rw-r--r--   0 a1tus      (501) staff       (20)       86 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/MANIFEST.in
+-rw-r--r--   0 a1tus      (501) staff       (20)     5563 2023-07-09 14:26:19.508275 django-admin-cursor-paginator-0.1.4/PKG-INFO
+-rw-r--r--   0 a1tus      (501) staff       (20)     3864 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/README.md
+drwxr-xr-x   0 a1tus      (501) staff       (20)        0 2023-07-09 14:26:19.504463 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/
+-rw-r--r--   0 a1tus      (501) staff       (20)       54 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/__init__.py
+-rw-r--r--   0 a1tus      (501) staff       (20)     1140 2023-07-07 19:58:24.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/admin.py
+-rw-r--r--   0 a1tus      (501) staff       (20)     1489 2023-07-09 14:05:52.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/cursor.py
+-rw-r--r--   0 a1tus      (501) staff       (20)     3397 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/paginator.py
+drwxr-xr-x   0 a1tus      (501) staff       (20)        0 2023-07-09 14:26:19.499863 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templates/
+drwxr-xr-x   0 a1tus      (501) staff       (20)        0 2023-07-09 14:26:19.505519 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templates/admin_cursor_paginator/
+-rw-r--r--   0 a1tus      (501) staff       (20)      149 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templates/admin_cursor_paginator/change_list.html
+-rw-r--r--   0 a1tus      (501) staff       (20)      651 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templates/admin_cursor_paginator/pagination.html
+drwxr-xr-x   0 a1tus      (501) staff       (20)        0 2023-07-09 14:26:19.506181 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templatetags/
+-rw-r--r--   0 a1tus      (501) staff       (20)        0 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templatetags/__init__.py
+-rw-r--r--   0 a1tus      (501) staff       (20)     1084 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templatetags/admin_cursor_paginator_tags.py
+-rw-r--r--   0 a1tus      (501) staff       (20)       22 2023-07-07 19:57:12.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/version.py
+-rw-r--r--   0 a1tus      (501) staff       (20)      589 2023-07-07 18:44:51.000000 django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/views.py
+drwxr-xr-x   0 a1tus      (501) staff       (20)        0 2023-07-09 14:26:19.507896 django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/
+-rw-r--r--   0 a1tus      (501) staff       (20)     5563 2023-07-09 14:26:19.000000 django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/PKG-INFO
+-rw-r--r--   0 a1tus      (501) staff       (20)      826 2023-07-09 14:26:19.000000 django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/SOURCES.txt
+-rw-r--r--   0 a1tus      (501) staff       (20)        1 2023-07-09 14:26:19.000000 django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/dependency_links.txt
+-rw-r--r--   0 a1tus      (501) staff       (20)        1 2023-07-09 14:26:19.000000 django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/not-zip-safe
+-rw-r--r--   0 a1tus      (501) staff       (20)       12 2023-07-09 14:26:19.000000 django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/requires.txt
+-rw-r--r--   0 a1tus      (501) staff       (20)       23 2023-07-09 14:26:19.000000 django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/top_level.txt
+-rw-r--r--   0 a1tus      (501) staff       (20)     1585 2023-07-09 14:26:19.508823 django-admin-cursor-paginator-0.1.4/setup.cfg
+-rw-r--r--   0 a1tus      (501) staff       (20)      600 2023-07-09 14:25:48.000000 django-admin-cursor-paginator-0.1.4/setup.py
```

### Comparing `django-admin-cursor-paginator-0.1.3/LICENSE` & `django-admin-cursor-paginator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/README.md` & `django-admin-cursor-paginator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/admin.py` & `django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/cursor.py` & `django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from base64 import b64decode, b64encode
 from collections import namedtuple
 from datetime import datetime
 
 
 Cursor = namedtuple('Cursor', ['value', 'is_reverse', 'number'])
 
-delimiter = '|||'
+_delimiter = '|||'
 
 
 def encode_cursor(cursor):
     parts = [encode_value(x) for x in cursor]
-    return b64encode(delimiter.join(parts).encode('utf8')).decode('ascii')
+    return b64encode(_delimiter.join(parts).encode('utf8')).decode('ascii')
 
 
 def decode_cursor(encoded_cursor):
     try:
         cursor_str = b64decode(encoded_cursor.encode('ascii')).decode('utf8')
-        parts = cursor_str.split(delimiter)
+        parts = cursor_str.split(_delimiter)
         return Cursor(
             value=decode_value(parts[0]),
             is_reverse=bool(parts[1]),
             number=int(parts[2]),
         )
     except (TypeError, ValueError):
         return None
 
 
 def encode_value(val):
     if not val:
         return ''
-    # datetime.__str__ applies `isoformat()` under the hood
+    # datetime.__str__ applies `isoformat()` under the hood,
     # but we do this explicitly for the sake of clarity
     if isinstance(val, datetime):
         return val.isoformat()
     return str(val)
 
 
 def decode_value(val):
```

### Comparing `django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/paginator.py` & `django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/paginator.py`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templates/admin_cursor_paginator/pagination.html` & `django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templates/admin_cursor_paginator/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/templatetags/admin_cursor_paginator_tags.py` & `django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/templatetags/admin_cursor_paginator_tags.py`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/admin_cursor_paginator/views.py` & `django-admin-cursor-paginator-0.1.4/admin_cursor_paginator/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/django_admin_cursor_paginator.egg-info/SOURCES.txt` & `django-admin-cursor-paginator-0.1.4/django_admin_cursor_paginator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-cursor-paginator-0.1.3/setup.cfg` & `django-admin-cursor-paginator-0.1.4/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = django-admin-cursor-paginator
-version = attr: admin_cursor_paginator.version.__version__
 description = Drop-in replacement for django admin default pagination that works fast with huge tables.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Ilya Melnitskiy
 author_email = mortas.11@gmail.com
 url = https://github.com/a1tus/django-admin-cursor-paginator
 download_url = https://pypi.org/project/django-admin-cursor-paginator/
@@ -18,27 +17,29 @@
 	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.4
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 python_requires = >=3.4
 install_requires = 
 	Django >= 2.0
 packages = find:
```

