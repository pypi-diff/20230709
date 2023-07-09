# Comparing `tmp/django-script-1.0.0.tar.gz` & `tmp/django-script-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-script-1.0.0.tar", last modified: Sun Jul  9 09:04:47 2023, max compression
+gzip compressed data, was "dist\django-script-1.0.1.tar", last modified: Sun Jul  9 12:57:44 2023, max compression
```

## Comparing `django-script-1.0.0.tar` & `django-script-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 09:04:47.744775 django-script-1.0.0/
--rw-rw-rw-   0        0        0       34 2023-06-24 13:12:33.000000 django-script-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      510 2023-07-09 09:04:47.743783 django-script-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-09 09:04:47.698954 django-script-1.0.0/django_script.egg-info/
--rw-rw-rw-   0        0        0      510 2023-07-09 09:04:47.000000 django-script-1.0.0/django_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-07-09 09:04:47.000000 django-script-1.0.0/django_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 09:04:47.000000 django-script-1.0.0/django_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-09 09:04:47.000000 django-script-1.0.0/django_script.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-07-09 09:04:47.000000 django-script-1.0.0/django_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 09:04:47.000000 django-script-1.0.0/django_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 09:04:47.745773 django-script-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-07-09 09:04:41.000000 django-script-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 09:04:47.725991 django-script-1.0.0/starts/
--rw-rw-rw-   0        0        0        0 2023-06-24 03:57:34.000000 django-script-1.0.0/starts/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-07-06 13:14:23.000000 django-script-1.0.0/starts/addCodeSettings.py
--rw-rw-rw-   0        0        0      509 2023-06-24 09:46:24.000000 django-script-1.0.0/starts/addHost.py
--rw-rw-rw-   0        0        0      703 2023-06-24 09:04:55.000000 django-script-1.0.0/starts/addInstallApp.py
--rw-rw-rw-   0        0        0        0 2023-06-26 03:29:19.000000 django-script-1.0.0/starts/addMail.py
--rw-rw-rw-   0        0        0      712 2023-06-24 09:44:35.000000 django-script-1.0.0/starts/addMiddleware.py
--rw-rw-rw-   0        0        0     1050 2023-06-26 06:56:19.000000 django-script-1.0.0/starts/addSecret.py
--rw-rw-rw-   0        0        0      522 2023-06-25 05:01:05.000000 django-script-1.0.0/starts/fileCheck.py
--rw-rw-rw-   0        0        0     1680 2023-06-25 07:44:18.000000 django-script-1.0.0/starts/multiUser.py
-drwxrwxrwx   0        0        0        0 2023-07-09 09:04:47.730995 django-script-1.0.0/starts/react/
--rw-rw-rw-   0        0        0   672155 2023-06-24 13:24:36.000000 django-script-1.0.0/starts/react/package-lock.json
--rw-rw-rw-   0        0        0      808 2023-06-24 13:24:04.000000 django-script-1.0.0/starts/react/package.json
-drwxrwxrwx   0        0        0        0 2023-07-09 09:04:47.733998 django-script-1.0.0/starts/react/public/
--rw-rw-rw-   0        0        0      238 2023-06-24 11:50:39.000000 django-script-1.0.0/starts/react/public/index.html
-drwxrwxrwx   0        0        0        0 2023-07-09 09:04:47.741772 django-script-1.0.0/starts/react/src/
--rw-rw-rw-   0        0        0      564 2023-03-08 08:12:50.000000 django-script-1.0.0/starts/react/src/App.css
--rw-rw-rw-   0        0        0      473 2023-06-24 11:48:31.000000 django-script-1.0.0/starts/react/src/App.js
--rw-rw-rw-   0        0        0      366 2023-03-08 08:12:52.000000 django-script-1.0.0/starts/react/src/index.css
--rw-rw-rw-   0        0        0      254 2023-06-24 11:38:58.000000 django-script-1.0.0/starts/react/src/index.js
--rw-rw-rw-   0        0        0      829 2023-06-24 13:47:59.000000 django-script-1.0.0/starts/react.py
--rw-rw-rw-   0        0        0     3280 2023-06-25 08:11:06.000000 django-script-1.0.0/starts/scheduler.py
--rw-rw-rw-   0        0        0     4297 2023-06-27 14:00:27.000000 django-script-1.0.0/starts/starts.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:44.956455 django-script-1.0.1/
+-rw-rw-rw-   0        0        0       34 2023-06-24 13:12:33.000000 django-script-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3016 2023-07-09 12:57:44.955455 django-script-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2137 2023-07-09 10:37:13.000000 django-script-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:44.876661 django-script-1.0.1/django_script.egg-info/
+-rw-rw-rw-   0        0        0     3016 2023-07-09 12:57:44.000000 django-script-1.0.1/django_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-07-09 12:57:44.000000 django-script-1.0.1/django_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:57:44.000000 django-script-1.0.1/django_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-09 12:57:44.000000 django-script-1.0.1/django_script.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-07-09 12:57:44.000000 django-script-1.0.1/django_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 12:57:44.000000 django-script-1.0.1/django_script.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:44.954454 django-script-1.0.1/master/
+-rw-rw-rw-   0        0        0        0 2023-06-24 03:57:34.000000 django-script-1.0.1/master/__init__.py
+-rw-rw-rw-   0        0        0     2982 2023-07-06 13:14:23.000000 django-script-1.0.1/master/addCodeSettings.py
+-rw-rw-rw-   0        0        0      509 2023-06-24 09:46:24.000000 django-script-1.0.1/master/addHost.py
+-rw-rw-rw-   0        0        0      703 2023-06-24 09:04:55.000000 django-script-1.0.1/master/addInstallApp.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 03:29:19.000000 django-script-1.0.1/master/addMail.py
+-rw-rw-rw-   0        0        0      712 2023-06-24 09:44:35.000000 django-script-1.0.1/master/addMiddleware.py
+-rw-rw-rw-   0        0        0     1050 2023-06-26 06:56:19.000000 django-script-1.0.1/master/addSecret.py
+-rw-rw-rw-   0        0        0      522 2023-06-25 05:01:05.000000 django-script-1.0.1/master/fileCheck.py
+-rw-rw-rw-   0        0        0     4296 2023-07-09 09:24:08.000000 django-script-1.0.1/master/main.py
+-rw-rw-rw-   0        0        0     1680 2023-06-25 07:44:18.000000 django-script-1.0.1/master/multiUser.py
+-rw-rw-rw-   0        0        0      829 2023-06-24 13:47:59.000000 django-script-1.0.1/master/react.py
+-rw-rw-rw-   0        0        0     3280 2023-06-25 08:11:06.000000 django-script-1.0.1/master/scheduler.py
+-rw-rw-rw-   0        0        0       42 2023-07-09 12:57:44.956455 django-script-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1398 2023-07-09 12:51:44.000000 django-script-1.0.1/setup.py
```

### Comparing `django-script-1.0.0/starts/addCodeSettings.py` & `django-script-1.0.1/master/addCodeSettings.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/addInstallApp.py` & `django-script-1.0.1/master/addInstallApp.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/addMiddleware.py` & `django-script-1.0.1/master/addMiddleware.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/addSecret.py` & `django-script-1.0.1/master/addSecret.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/fileCheck.py` & `django-script-1.0.1/master/fileCheck.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/multiUser.py` & `django-script-1.0.1/master/multiUser.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/react.py` & `django-script-1.0.1/master/react.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/scheduler.py` & `django-script-1.0.1/master/scheduler.py`

 * *Files identical despite different names*

### Comparing `django-script-1.0.0/starts/starts.py` & `django-script-1.0.1/master/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .react import react
 from .fileCheck import *
 from .multiUser import multiUser
 from .scheduler import scheduler
 #from .addMail import addMail
 
 
-def create_folder():
+def djangoScript():
     callName = sys.argv[1]
     status = 2
     manage_py_path = findCurrentFile('manage.py')
     project_check = findFile('manage.py')
     if manage_py_path:
         status=0
     elif project_check:
```

