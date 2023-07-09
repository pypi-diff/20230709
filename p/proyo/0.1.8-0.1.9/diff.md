# Comparing `tmp/proyo-0.1.8.tar.gz` & `tmp/proyo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/proyo-0.1.8.tar", last modified: Wed Oct 30 08:49:12 2019, max compression
+gzip compressed data, was "proyo-0.1.9.tar", last modified: Wed Aug 10 03:09:35 2022, max compression
```

## Comparing `proyo-0.1.8.tar` & `proyo-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2019-10-30 08:49:12.000000 proyo-0.1.8/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1075 2019-10-30 08:48:47.000000 proyo-0.1.8/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2019-07-14 22:41:48.000000 proyo-0.1.8/proyo/templates/_subparsers_
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/cpp/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      240 2019-07-26 05:12:58.000000 proyo-0.1.8/proyo/templates/create/cpp/_subparsers_
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/cpp/app/
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/cpp/app/source/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      201 2019-07-26 05:25:37.000000 proyo-0.1.8/proyo/templates/create/cpp/app/source/main.cpp
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       82 2019-07-31 04:23:04.000000 proyo-0.1.8/proyo/templates/create/cpp/app/source/meson.build
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      169 2019-07-31 04:23:04.000000 proyo-0.1.8/proyo/templates/create/cpp/app/CMakeLists.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      146 2019-07-31 04:23:04.000000 proyo-0.1.8/proyo/templates/create/cpp/app/meson.build
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      400 2019-07-26 05:19:49.000000 proyo-0.1.8/proyo/templates/create/cpp/_
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/python/
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/python/{{package_name}}/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2019-07-14 23:22:47.000000 proyo-0.1.8/proyo/templates/create/python/{{package_name}}/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      332 2019-08-07 04:50:31.000000 proyo-0.1.8/proyo/templates/create/python/{{package_name}}/__main__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1206 2019-08-07 05:41:33.000000 proyo-0.1.8/proyo/templates/create/python/setup.py~
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1207 2019-10-30 08:47:01.000000 proyo-0.1.8/proyo/templates/create/python/setup.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      568 2019-08-07 04:50:19.000000 proyo-0.1.8/proyo/templates/create/python/{{module_name}}.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1162 2019-08-07 04:48:28.000000 proyo-0.1.8/proyo/templates/create/python/_
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      300 2019-08-07 05:40:55.000000 proyo-0.1.8/proyo/templates/create/_subparsers_
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/react/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2019-07-14 22:41:48.000000 proyo-0.1.8/proyo/templates/create/react/_subparsers_
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/react/app/
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/react/app/public/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      561 2019-07-23 06:31:02.000000 proyo-0.1.8/proyo/templates/create/react/app/public/index.html
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3870 2019-07-18 15:01:19.000000 proyo-0.1.8/proyo/templates/create/react/app/public/favicon.ico
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      313 2019-07-23 06:31:34.000000 proyo-0.1.8/proyo/templates/create/react/app/public/manifest.json
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/templates/create/react/app/src/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      248 2019-07-18 15:01:19.000000 proyo-0.1.8/proyo/templates/create/react/app/src/App.test.js
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       34 2019-07-23 05:47:05.000000 proyo-0.1.8/proyo/templates/create/react/app/src/App.css
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      216 2019-07-23 05:52:29.000000 proyo-0.1.8/proyo/templates/create/react/app/src/index.js
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      256 2019-07-23 06:32:16.000000 proyo-0.1.8/proyo/templates/create/react/app/src/App.js
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       63 2019-07-18 15:01:19.000000 proyo-0.1.8/proyo/templates/create/react/app/src/index.css
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      269 2019-07-23 06:32:33.000000 proyo-0.1.8/proyo/templates/create/react/app/package.json
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       63 2019-07-23 06:38:41.000000 proyo-0.1.8/proyo/templates/create/react/app/_
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       83 2019-08-07 05:40:55.000000 proyo-0.1.8/proyo/templates/create/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    42126 2019-08-07 05:58:07.000000 proyo-0.1.8/proyo/templates/create/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     2696 2019-08-07 04:41:31.000000 proyo-0.1.8/proyo/templates/create/_
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       57 2019-07-15 00:04:45.000000 proyo-0.1.8/proyo/macros.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2019-07-25 07:34:32.000000 proyo-0.1.8/proyo/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     4785 2019-07-25 07:36:31.000000 proyo-0.1.8/proyo/misc.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo/macros/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      563 2019-08-04 00:41:59.000000 proyo-0.1.8/proyo/macros/_subparsers_
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1906 2019-08-07 05:59:47.000000 proyo-0.1.8/proyo/__main__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    12139 2019-08-07 05:58:38.000000 proyo-0.1.8/proyo/proyo.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1039 2019-07-25 07:45:32.000000 proyo-0.1.8/README.md
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        6 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo.egg-info/top_level.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       47 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo.egg-info/entry_points.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1471 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      605 2019-10-30 08:49:12.000000 proyo-0.1.8/proyo.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      605 2019-10-30 08:49:12.000000 proyo-0.1.8/PKG-INFO
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.248628 proyo-0.1.9/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1063 2022-08-10 03:08:38.000000 proyo-0.1.9/LICENSE
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      616 2022-08-10 03:09:35.248628 proyo-0.1.9/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1039 2022-08-10 03:08:38.000000 proyo-0.1.9/README.md
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1906 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/__main__.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo/macros/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      563 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/macros/_subparsers_
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       57 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/macros.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     4785 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/misc.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    12139 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/proyo.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo/templates/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/_subparsers_
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo/templates/create/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)    42126 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/LICENSE
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       83 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/README.md
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     2696 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/_
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      300 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/_subparsers_
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo/templates/create/cpp/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      400 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/cpp/_
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      240 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/cpp/_subparsers_
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo/templates/create/cpp/app/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      169 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/cpp/app/CMakeLists.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      146 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/cpp/app/meson.build
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo/templates/create/cpp/app/source/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      201 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/cpp/app/source/main.cpp
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       82 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/cpp/app/source/meson.build
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.248628 proyo-0.1.9/proyo/templates/create/python/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1162 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/python/_
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1208 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/python/setup.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      568 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/python/{{module_name}}.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.248628 proyo-0.1.9/proyo/templates/create/python/{{package_name}}/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/python/{{package_name}}/__init__.py
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      332 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/python/{{package_name}}/__main__.py
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.248628 proyo-0.1.9/proyo/templates/create/react/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/_subparsers_
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.248628 proyo-0.1.9/proyo/templates/create/react/app/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       63 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/_
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      269 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/package.json
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.248628 proyo-0.1.9/proyo/templates/create/react/app/public/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     3870 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/public/favicon.ico
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      561 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/public/index.html
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      313 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/public/manifest.json
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.248628 proyo-0.1.9/proyo/templates/create/react/app/src/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       34 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/src/App.css
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      256 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/src/App.js
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      248 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/src/App.test.js
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       63 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/src/index.css
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      216 2022-08-10 03:08:38.000000 proyo-0.1.9/proyo/templates/create/react/app/src/index.js
+drwxr-xr-x   0 matthew   (1000) matthew   (1000)        0 2022-08-10 03:09:35.238628 proyo-0.1.9/proyo.egg-info/
+-rw-r--r--   0 matthew   (1000) matthew   (1000)      616 2022-08-10 03:09:35.000000 proyo-0.1.9/proyo.egg-info/PKG-INFO
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1439 2022-08-10 03:09:35.000000 proyo-0.1.9/proyo.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        1 2022-08-10 03:09:35.000000 proyo-0.1.9/proyo.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       47 2022-08-10 03:09:35.000000 proyo-0.1.9/proyo.egg-info/entry_points.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)        6 2022-08-10 03:09:35.000000 proyo-0.1.9/proyo.egg-info/top_level.txt
+-rw-r--r--   0 matthew   (1000) matthew   (1000)       38 2022-08-10 03:09:35.248628 proyo-0.1.9/setup.cfg
+-rw-r--r--   0 matthew   (1000) matthew   (1000)     1075 2022-08-10 03:08:53.000000 proyo-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `proyo-0.1.8/setup.py` & `proyo-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     for root, dirnames, filenames in os.walk(join(
         dirname(abspath(__file__)), 'proyo', folder
     ))
 ]
 
 setup(
     name='proyo',
-    version='0.1.8',
+    version='0.1.9',
     description='A tool to broadcast notifications across various interfaces',
     url='https://github.com/matthewscholefield/proyo',
     author='Matthew Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `proyo-0.1.8/proyo/templates/create/python/setup.py~` & `proyo-0.1.9/proyo/templates/create/python/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     author='{{git_author or "AUTHOR"}}',
     author_email='{{git_email or "AUTHOR_EMAIL"}}',
     classifiers=[
         'Development Status :: 3 - Alpha',
 
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     keywords='{{project_name.replace("-", " ")}}',
     # ~ if is_package:
-    packages=['{{module_name}}'],
+    packages=['{{package_name}}'],
     # ~ #
     # ~ else:
     py_modules=['{{module_name}}'],
     # ~ #
     install_requires=[],
     # ~ if project_type == 'script':
     entry_points={
```

### Comparing `proyo-0.1.8/proyo/templates/create/python/{{module_name}}.py` & `proyo-0.1.9/proyo/templates/create/python/{{module_name}}.py`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/templates/create/python/_` & `proyo-0.1.9/proyo/templates/create/python/_`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/templates/create/react/app/public/index.html` & `proyo-0.1.9/proyo/templates/create/react/app/public/index.html`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/templates/create/react/app/public/favicon.ico` & `proyo-0.1.9/proyo/templates/create/react/app/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/templates/create/LICENSE` & `proyo-0.1.9/proyo/templates/create/LICENSE`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/templates/create/_` & `proyo-0.1.9/proyo/templates/create/_`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/misc.py` & `proyo-0.1.9/proyo/misc.py`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/macros/_subparsers_` & `proyo-0.1.9/proyo/macros/_subparsers_`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/__main__.py` & `proyo-0.1.9/proyo/__main__.py`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo/proyo.py` & `proyo-0.1.9/proyo/proyo.py`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/README.md` & `proyo-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `proyo-0.1.8/proyo.egg-info/SOURCES.txt` & `proyo-0.1.9/proyo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 proyo/__init__.py
 proyo/__main__.py
 proyo/macros.py
 proyo/misc.py
 proyo/proyo.py
@@ -20,15 +21,14 @@
 proyo/templates/create/cpp/_subparsers_
 proyo/templates/create/cpp/app/CMakeLists.txt
 proyo/templates/create/cpp/app/meson.build
 proyo/templates/create/cpp/app/source/main.cpp
 proyo/templates/create/cpp/app/source/meson.build
 proyo/templates/create/python/_
 proyo/templates/create/python/setup.py
-proyo/templates/create/python/setup.py~
 proyo/templates/create/python/{{module_name}}.py
 proyo/templates/create/python/{{package_name}}/__init__.py
 proyo/templates/create/python/{{package_name}}/__main__.py
 proyo/templates/create/react/_subparsers_
 proyo/templates/create/react/app/_
 proyo/templates/create/react/app/package.json
 proyo/templates/create/react/app/public/favicon.ico
```

### Comparing `proyo-0.1.8/proyo.egg-info/PKG-INFO` & `proyo-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: proyo
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to broadcast notifications across various interfaces
 Home-page: https://github.com/matthewscholefield/proyo
 Author: Matthew Scholefield
 Author-email: matthew331199@gmail.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: notify server
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `proyo-0.1.8/PKG-INFO` & `proyo-0.1.9/proyo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: proyo
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to broadcast notifications across various interfaces
 Home-page: https://github.com/matthewscholefield/proyo
 Author: Matthew Scholefield
 Author-email: matthew331199@gmail.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: notify server
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+
+UNKNOWN
+
```

