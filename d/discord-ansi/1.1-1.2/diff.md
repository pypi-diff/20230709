# Comparing `tmp/discord-ansi-1.1.tar.gz` & `tmp/discord-ansi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ansi-1.1.tar", last modified: Wed Jul  5 11:46:24 2023, max compression
+gzip compressed data, was "discord-ansi-1.2.tar", last modified: Sun Jul  9 09:50:13 2023, max compression
```

## Comparing `discord-ansi-1.1.tar` & `discord-ansi-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 11:46:14.000000 discord-ansi-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-05 11:46:24.667755 discord-ansi-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-05 11:46:14.000000 discord-ansi-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/discord_ansi/
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-07-05 11:46:14.000000 discord-ansi-1.1/discord_ansi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/discord_ansi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 11:46:24.000000 discord-ansi-1.1/discord_ansi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-05 11:46:14.000000 discord-ansi-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:46:24.667755 discord-ansi-1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:46:24.667755 discord-ansi-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-05 11:46:14.000000 discord-ansi-1.1/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:50:13.747153 discord-ansi-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 09:50:02.000000 discord-ansi-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-09 09:50:13.747153 discord-ansi-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-09 09:50:02.000000 discord-ansi-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:50:13.743153 discord-ansi-1.2/discord_ansi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-07-09 09:50:02.000000 discord-ansi-1.2/discord_ansi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:50:13.747153 discord-ansi-1.2/discord_ansi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-09 09:50:13.000000 discord-ansi-1.2/discord_ansi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-09 09:50:13.000000 discord-ansi-1.2/discord_ansi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:50:13.000000 discord-ansi-1.2/discord_ansi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 09:50:13.000000 discord-ansi-1.2/discord_ansi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 09:50:13.000000 discord-ansi-1.2/discord_ansi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-09 09:50:02.000000 discord-ansi-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:50:13.747153 discord-ansi-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:50:13.747153 discord-ansi-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-09 09:50:02.000000 discord-ansi-1.2/tests/test1.py
```

### Comparing `discord-ansi-1.1/LICENSE` & `discord-ansi-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ansi-1.1/PKG-INFO` & `discord-ansi-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 1.1
+Version: 1.2
 Summary: Discord messages with ANSI (message builder + ANSI Art)
 Author-email: GEOEGII555 <geoegii2001555@gmail.com>, "GEOEGII555 (Alternative email)" <webmaster@geoegii555.eu.org>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `discord-ansi-1.1/README.md` & `discord-ansi-1.2/README.md`

 * *Files identical despite different names*

### Comparing `discord-ansi-1.1/discord_ansi/__init__.py` & `discord-ansi-1.2/discord_ansi/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-ansi-1.1/discord_ansi.egg-info/PKG-INFO` & `discord-ansi-1.2/discord_ansi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ansi
-Version: 1.1
+Version: 1.2
 Summary: Discord messages with ANSI (message builder + ANSI Art)
 Author-email: GEOEGII555 <geoegii2001555@gmail.com>, "GEOEGII555 (Alternative email)" <webmaster@geoegii555.eu.org>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `discord-ansi-1.1/pyproject.toml` & `discord-ansi-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "discord-ansi"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="GEOEGII555", email="geoegii2001555@gmail.com" },
   { name="GEOEGII555 (Alternative email)", email="webmaster@geoegii555.eu.org" },
 ]
 description = "Discord messages with ANSI (message builder + ANSI Art)"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `discord-ansi-1.1/tests/test1.py` & `discord-ansi-1.2/tests/test1.py`

 * *Files identical despite different names*

