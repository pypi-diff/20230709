# Comparing `tmp/pygmailsorter-0.0.5.tar.gz` & `tmp/pygmailsorter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmailsorter-0.0.5.tar", last modified: Sun Jul  9 15:12:34 2023, max compression
+gzip compressed data, was "pygmailsorter-0.0.6.tar", last modified: Sun Jul  9 17:57:42 2023, max compression
```

## Comparing `pygmailsorter-0.0.5.tar` & `pygmailsorter-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.540314 pygmailsorter-0.0.5/pygmailsorter/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-09 15:12:34.540314 pygmailsorter-0.0.5/pygmailsorter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.532314 pygmailsorter-0.0.5/pygmailsorter/base/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/base/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/base/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/pygmailsorter/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/daemon/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/pygmailsorter/google/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/google/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/pygmailsorter/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/pygmailsorter/ml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.532314 pygmailsorter-0.0.5/pygmailsorter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/pygmailsorter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-09 15:12:34.000000 pygmailsorter-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:12:34.536314 pygmailsorter-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/tests/test_google_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-09 15:12:28.000000 pygmailsorter-0.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/pygmailsorter/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/pygmailsorter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.413447 pygmailsorter-0.0.6/pygmailsorter/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/base/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/base/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.417447 pygmailsorter-0.0.6/pygmailsorter/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/daemon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/daemon/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/daemon/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/daemon/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.417447 pygmailsorter-0.0.6/pygmailsorter/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/google/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/google/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/google/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/google/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.417447 pygmailsorter-0.0.6/pygmailsorter/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/ml/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/ml/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/ml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.417447 pygmailsorter-0.0.6/pygmailsorter/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/googleapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.413447 pygmailsorter-0.0.6/pygmailsorter/webapp/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.417447 pygmailsorter-0.0.6/pygmailsorter/webapp/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9241 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/css/main.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    83821 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/css/util.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.413447 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   139056 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-Black.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   155956 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-BlackItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   141260 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-Bold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   160224 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-BoldItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   140220 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   158708 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-ExtraBoldItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   147952 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLight.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   170912 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-ExtraLightItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   167140 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-Italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   146472 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-Light.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   168944 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-LightItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   143516 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-Medium.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   165512 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-MediumItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   145312 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-Regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   142148 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-SemiBold.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   161896 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-SemiBoldItalic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   148976 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-Thin.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   172308 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/fonts/poppins/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/pygmailsorter/webapp/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114272 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/images/bg-01.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/pygmailsorter/webapp/static/images/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32038 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/static/images/icons/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/pygmailsorter/webapp/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/templates/login.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1873 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/templates/user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/pygmailsorter/webapp/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.413447 pygmailsorter-0.0.6/pygmailsorter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-09 17:57:42.000000 pygmailsorter-0.0.6/pygmailsorter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-09 17:57:42.000000 pygmailsorter-0.0.6/pygmailsorter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:57:42.000000 pygmailsorter-0.0.6/pygmailsorter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-09 17:57:42.000000 pygmailsorter-0.0.6/pygmailsorter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-09 17:57:42.000000 pygmailsorter-0.0.6/pygmailsorter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 17:57:42.000000 pygmailsorter-0.0.6/pygmailsorter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-09 17:57:42.000000 pygmailsorter-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:57:42.425447 pygmailsorter-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/tests/test_google_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-09 17:57:39.000000 pygmailsorter-0.0.6/versioneer.py
```

### Comparing `pygmailsorter-0.0.5/LICENSE` & `pygmailsorter-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/PKG-INFO` & `pygmailsorter-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pygmailsorter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Assign labels to emails in Google Mail based on their similarity to other emails assigned to the same label.
 Home-page: https://github.com/mailsort/pygmailsorter
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 Description-Content-Type: text/markdown
+Provides-Extra: webapp
 License-File: LICENSE
 
 # Sort your emails automatically 
 [![Python package](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/mailsort/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/mailsort/pygmailsorter?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pygmailsorter-0.0.5/README.md` & `pygmailsorter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/__main__.py` & `pygmailsorter-0.0.6/pygmailsorter/__main__.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/base/database.py` & `pygmailsorter-0.0.6/pygmailsorter/base/database.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/base/message.py` & `pygmailsorter-0.0.6/pygmailsorter/base/message.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/daemon/__main__.py` & `pygmailsorter-0.0.6/pygmailsorter/daemon/__main__.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/daemon/daemon.py` & `pygmailsorter-0.0.6/pygmailsorter/daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/daemon/shared.py` & `pygmailsorter-0.0.6/pygmailsorter/daemon/shared.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/daemon/tasks.py` & `pygmailsorter-0.0.6/pygmailsorter/daemon/tasks.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/google/authentication.py` & `pygmailsorter-0.0.6/pygmailsorter/google/authentication.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/google/database.py` & `pygmailsorter-0.0.6/pygmailsorter/google/database.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/google/mail.py` & `pygmailsorter-0.0.6/pygmailsorter/google/mail.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/google/message.py` & `pygmailsorter-0.0.6/pygmailsorter/google/message.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/local.py` & `pygmailsorter-0.0.6/pygmailsorter/local.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/ml/database.py` & `pygmailsorter-0.0.6/pygmailsorter/ml/database.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/ml/encoding.py` & `pygmailsorter-0.0.6/pygmailsorter/ml/encoding.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter/ml/model.py` & `pygmailsorter-0.0.6/pygmailsorter/ml/model.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/pygmailsorter.egg-info/PKG-INFO` & `pygmailsorter-0.0.6/pygmailsorter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pygmailsorter
-Version: 0.0.5
+Version: 0.0.6
 Summary: Assign labels to emails in Google Mail based on their similarity to other emails assigned to the same label.
 Home-page: https://github.com/mailsort/pygmailsorter
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 Description-Content-Type: text/markdown
+Provides-Extra: webapp
 License-File: LICENSE
 
 # Sort your emails automatically 
 [![Python package](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml/badge.svg?branch=main)](https://github.com/mailsort/pygmailsorter/actions/workflows/unittest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/mailsort/pygmailsorter/badge.svg?branch=main)](https://coveralls.io/github/mailsort/pygmailsorter?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pygmailsorter-0.0.5/setup.py` & `pygmailsorter-0.0.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,21 +17,25 @@
     author_email="jan.janssen@outlook.com",
     license="BSD",
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
         "google-api-python-client>=2.92.0",
         "google-auth>=2.21.0",
         "google-auth-oauthlib>=1.0.0",
-        "numpy>=1.25.0",
+        "numpy>=1.25.1",
         "tqdm>=4.65.0",
         "pandas>=2.0.3",
         "scikit-learn>=1.3.0",
         "sqlalchemy>=2.0.18",
     ],
+    extras_require={
+        "webapp": ['gunicorn>=20.1.0', "flask>=2.3.2", "flask-login>=0.6.2"],
+    },
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
             "console_scripts": [
                 'pygmailsorter=pygmailsorter.__main__:command_line_parser',
-                'pygmailsorter-daemon=pygmailsorter.__main__:command_line_parser'
+                'pygmailsorter-daemon=pygmailsorter.daemon.__main__:command_line_parser',
+                'pygmailsorter-app=pygmailsorter.webapp.app:run_app'
             ]
     }
 )
```

### Comparing `pygmailsorter-0.0.5/tests/test_database.py` & `pygmailsorter-0.0.6/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/tests/test_google_message.py` & `pygmailsorter-0.0.6/tests/test_google_message.py`

 * *Files identical despite different names*

### Comparing `pygmailsorter-0.0.5/versioneer.py` & `pygmailsorter-0.0.6/versioneer.py`

 * *Files identical despite different names*

