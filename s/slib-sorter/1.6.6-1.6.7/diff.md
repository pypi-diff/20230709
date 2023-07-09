# Comparing `tmp/slib-sorter-1.6.6.tar.gz` & `tmp/slib-sorter-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slib-sorter-1.6.6.tar", last modified: Sat Jul  8 20:49:07 2023, max compression
+gzip compressed data, was "slib-sorter-1.6.7.tar", last modified: Sun Jul  9 13:11:16 2023, max compression
```

## Comparing `slib-sorter-1.6.6.tar` & `slib-sorter-1.6.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 20:49:07.949220 slib-sorter-1.6.6/
--rw-rw-rw-   0        0        0    11558 2023-07-08 14:57:30.000000 slib-sorter-1.6.6/LICENSE
--rw-rw-rw-   0        0        0     2332 2023-07-08 20:49:07.948225 slib-sorter-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     1856 2023-07-08 20:46:53.000000 slib-sorter-1.6.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 20:49:07.949220 slib-sorter-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     2931 2023-07-08 20:03:34.000000 slib-sorter-1.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 20:49:07.946193 slib-sorter-1.6.6/slib_sorter.egg-info/
--rw-rw-rw-   0        0        0     2332 2023-07-08 20:49:07.000000 slib-sorter-1.6.6/slib_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-08 20:49:07.000000 slib-sorter-1.6.6/slib_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 20:49:07.000000 slib-sorter-1.6.6/slib_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-08 20:49:07.000000 slib-sorter-1.6.6/slib_sorter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 20:49:07.000000 slib-sorter-1.6.6/slib_sorter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 20:49:07.000000 slib-sorter-1.6.6/slib_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 20:49:07.947193 slib-sorter-1.6.6/src/
--rw-rw-rw-   0        0        0        0 2023-07-08 14:57:30.000000 slib-sorter-1.6.6/src/__init__.py
--rw-rw-rw-   0        0        0    67590 2023-07-08 20:30:50.000000 slib-sorter-1.6.6/src/slib_sorter.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:11:16.843866 slib-sorter-1.6.7/
+-rw-rw-rw-   0        0        0    11558 2023-07-09 13:09:56.000000 slib-sorter-1.6.7/LICENSE
+-rw-rw-rw-   0        0        0     7571 2023-07-09 13:11:16.843866 slib-sorter-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7095 2023-07-09 13:09:56.000000 slib-sorter-1.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:11:16.843866 slib-sorter-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     2931 2023-07-09 13:09:56.000000 slib-sorter-1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:11:16.833863 slib-sorter-1.6.7/slib_sorter.egg-info/
+-rw-rw-rw-   0        0        0     7571 2023-07-09 13:11:16.000000 slib-sorter-1.6.7/slib_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-09 13:11:16.000000 slib-sorter-1.6.7/slib_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:11:16.000000 slib-sorter-1.6.7/slib_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-09 13:11:16.000000 slib-sorter-1.6.7/slib_sorter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 13:11:16.000000 slib-sorter-1.6.7/slib_sorter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-09 13:11:16.000000 slib-sorter-1.6.7/slib_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 13:11:16.842862 slib-sorter-1.6.7/src/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:09:56.000000 slib-sorter-1.6.7/src/__init__.py
+-rw-rw-rw-   0        0        0    67590 2023-07-09 13:09:56.000000 slib-sorter-1.6.7/src/slib_sorter.py
```

### Comparing `slib-sorter-1.6.6/LICENSE` & `slib-sorter-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slib-sorter-1.6.6/setup.py` & `slib-sorter-1.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "Prompt Color": "dark_grey",
         "Statistics Value Color": "light_red",
         "Successfully Sorted File Color": "green",
         "Unsorted File Color": "yellow",
         "Rejected Filetype Color": "red"
     },
     "Show Top Title Bar": true,
-    "Top Title Bar": ">_Sample Library Sorter v1.6.6",
+    "Top Title Bar": ">_Sample Library Sorter v1.6.7",
     "Show More Console Logs": true,
     "Show Statistics": true,
     "Console Log Seperator": "  >>--->  ",
     "Prompt": "$ ",
     "Max files per Dir": 50,
     "Run Shell Command On Startup": false,
     "Command On Startup": "cls"
@@ -48,15 +48,15 @@
     if not os.path.exists(settings_folder):
         os.makedirs(settings_folder)
     if not os.path.exists(settings):
         with open(settings, 'w') as f:
             f.write(default_config)
     setuptools.setup(
         name="slib-sorter",
-        version="1.6.6",
+        version="1.6.7",
         author="Lukas H",
         author_email="fettkindasindauchoke@gmail.com",
         description="A Python package for sorting Sample Libraries",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/nrdrch/slib-sorter",
         packages=setuptools.find_packages(),
```

### Comparing `slib-sorter-1.6.6/src/slib_sorter.py` & `slib-sorter-1.6.7/src/slib_sorter.py`

 * *Files identical despite different names*

