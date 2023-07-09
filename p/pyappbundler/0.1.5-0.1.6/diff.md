# Comparing `tmp/pyappbundler-0.1.5.tar.gz` & `tmp/pyappbundler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappbundler-0.1.5.tar", last modified: Sun Jul  9 02:08:41 2023, max compression
+gzip compressed data, was "pyappbundler-0.1.6.tar", last modified: Sun Jul  9 05:49:49 2023, max compression
```

## Comparing `pyappbundler-0.1.5.tar` & `pyappbundler-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.928820 pyappbundler-0.1.5/
--rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      730 2023-07-09 02:08:41.928820 pyappbundler-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.922819 pyappbundler-0.1.5/pyappbundler/
--rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.5/pyappbundler/__init__.py
--rw-rw-rw-   0        0        0     2518 2023-07-07 08:42:32.000000 pyappbundler-0.1.5/pyappbundler/__main__.py
--rw-rw-rw-   0        0        0       22 2023-07-08 10:54:23.000000 pyappbundler-0.1.5/pyappbundler/_version.py
--rw-rw-rw-   0        0        0     5062 2023-07-08 10:56:52.000000 pyappbundler-0.1.5/pyappbundler/pyappbundler.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.927820 pyappbundler-0.1.5/pyappbundler/templates/
--rw-rw-rw-   0        0        0     1705 2023-07-08 10:54:08.000000 pyappbundler-0.1.5/pyappbundler/templates/iss.tmpl
-drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.926821 pyappbundler-0.1.5/pyappbundler.egg-info/
--rw-rw-rw-   0        0        0      730 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 02:08:41.928820 pyappbundler-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.264960 pyappbundler-0.1.6/
+-rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      730 2023-07-09 05:49:49.264960 pyappbundler-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.259959 pyappbundler-0.1.6/pyappbundler/
+-rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.6/pyappbundler/__init__.py
+-rw-rw-rw-   0        0        0     2518 2023-07-07 08:42:32.000000 pyappbundler-0.1.6/pyappbundler/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-07-09 05:48:46.000000 pyappbundler-0.1.6/pyappbundler/_version.py
+-rw-rw-rw-   0        0        0     5182 2023-07-09 05:48:02.000000 pyappbundler-0.1.6/pyappbundler/pyappbundler.py
+drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.263959 pyappbundler-0.1.6/pyappbundler/templates/
+-rw-rw-rw-   0        0        0     1705 2023-07-08 10:54:08.000000 pyappbundler-0.1.6/pyappbundler/templates/iss.tmpl
+drwxrwxrwx   0        0        0        0 2023-07-09 05:49:49.262958 pyappbundler-0.1.6/pyappbundler.egg-info/
+-rw-rw-rw-   0        0        0      730 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-09 05:49:49.000000 pyappbundler-0.1.6/pyappbundler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 05:49:49.264960 pyappbundler-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.6/setup.py
```

### Comparing `pyappbundler-0.1.5/LICENSE` & `pyappbundler-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.5/PKG-INFO` & `pyappbundler-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.5
+Version: 0.1.6
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.5/pyappbundler/__main__.py` & `pyappbundler-0.1.6/pyappbundler/__main__.py`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.5/pyappbundler/pyappbundler.py` & `pyappbundler-0.1.6/pyappbundler/pyappbundler.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,15 +105,19 @@
 
         if self.icon:
             args.extend(['--icon', str(self.icon)])
         else:
             args.extend(['--icon', 'NONE'])
 
         if self.pyinst_flags:
-            args.extend([f'--{flag}' for flag in self.pyinst_flags])
+            for flag in self.pyinst_flags:
+                if len(flag) == 1:
+                    args.append(f'-{flag}')
+                else:
+                    args.append(f'--{flag}')
 
         if self.res_dirs:
             for directory in self.res_dirs:
                 directory_path = Path(directory).resolve()
                 if not directory_path.is_dir():
                     raise FileNotFoundError(
                         f'Directory expected, but "{directory_path}" is not!')
```

### Comparing `pyappbundler-0.1.5/pyappbundler/templates/iss.tmpl` & `pyappbundler-0.1.6/pyappbundler/templates/iss.tmpl`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.5/pyappbundler.egg-info/PKG-INFO` & `pyappbundler-0.1.6/pyappbundler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.5
+Version: 0.1.6
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.5/pyproject.toml` & `pyappbundler-0.1.6/pyproject.toml`

 * *Files identical despite different names*

