# Comparing `tmp/overfast-py-1.1.tar.gz` & `tmp/overfast-py-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overfast-py-1.1.tar", last modified: Thu Jul  6 12:14:42 2023, max compression
+gzip compressed data, was "overfast-py-1.2.tar", last modified: Sun Jul  9 21:22:28 2023, max compression
```

## Comparing `overfast-py-1.1.tar` & `overfast-py-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:14:42.236767 overfast-py-1.1/
--rw-rw-rw-   0        0        0     1083 2023-07-05 12:29:57.000000 overfast-py-1.1/LICENSE
--rw-rw-rw-   0        0        0      485 2023-07-06 12:14:42.237260 overfast-py-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      119 2023-07-05 12:47:29.000000 overfast-py-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:14:42.214368 overfast-py-1.1/overfast/
--rw-rw-rw-   0        0        0     3306 2023-07-06 12:09:10.000000 overfast-py-1.1/overfast/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:14:42.235772 overfast-py-1.1/overfast_py.egg-info/
--rw-rw-rw-   0        0        0      485 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 12:14:42.000000 overfast-py-1.1/overfast_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      433 2023-07-06 12:14:10.000000 overfast-py-1.1/pyproject.toml
--rw-rw-rw-   0        0        0      212 2023-07-06 12:14:42.238748 overfast-py-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 21:22:28.408619 overfast-py-1.2/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 12:29:57.000000 overfast-py-1.2/LICENSE
+-rw-rw-rw-   0        0        0      485 2023-07-09 21:22:28.409114 overfast-py-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      119 2023-07-05 12:47:29.000000 overfast-py-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 21:22:28.380347 overfast-py-1.2/overfast/
+-rw-rw-rw-   0        0        0     3401 2023-07-09 20:18:28.000000 overfast-py-1.2/overfast/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 21:22:28.407131 overfast-py-1.2/overfast_py.egg-info/
+-rw-rw-rw-   0        0        0      485 2023-07-09 21:22:28.000000 overfast-py-1.2/overfast_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-09 21:22:28.000000 overfast-py-1.2/overfast_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 21:22:28.000000 overfast-py-1.2/overfast_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 21:22:28.000000 overfast-py-1.2/overfast_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 21:22:28.000000 overfast-py-1.2/overfast_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      433 2023-07-09 21:21:22.000000 overfast-py-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      212 2023-07-09 21:22:28.411595 overfast-py-1.2/setup.cfg
```

### Comparing `overfast-py-1.1/LICENSE` & `overfast-py-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `overfast-py-1.1/overfast/__init__.py` & `overfast-py-1.2/overfast/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         else:
             type = "heroes/" + key
     if type in ['hero', 'heroes', 'gamemodes']:
         params["locale"] : locale
     if type == "maps":
         if key:
             params["gamemode"] = key
+    if type == "heroes":
+        params['role'] = key
     
     data = requests.get(url + type, params)
     response = data.json()
 
     if data.status_code != 200:
         if data.status_code == 422:
             return "Validation error"
@@ -84,8 +86,10 @@
     if data.status_code != 200:
         if data.status_code == 422:
             return "Validation error: " + str(response)
         else:
             return response["error"]
     else:
         return response
-        
+        
+
+print(get(type='heroes', key=None))
```

