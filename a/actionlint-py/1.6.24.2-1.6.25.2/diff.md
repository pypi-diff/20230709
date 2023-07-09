# Comparing `tmp/actionlint_py-1.6.24.2.tar.gz` & `tmp/actionlint_py-1.6.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionlint_py-1.6.24.2.tar", last modified: Wed May  3 17:38:33 2023, max compression
+gzip compressed data, was "actionlint_py-1.6.25.2.tar", last modified: Sun Jul  9 19:21:18 2023, max compression
```

## Comparing `actionlint_py-1.6.24.2.tar` & `actionlint_py-1.6.25.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/
--rw-rw-rw-   0        0        0     1087 2023-05-03 15:51:52.000000 actionlint_py-1.6.24.2/LICENSE
--rw-rw-rw-   0        0        0     1958 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/PKG-INFO
--rw-rw-rw-   0        0        0     1257 2023-05-03 16:11:35.000000 actionlint_py-1.6.24.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/actionlint_py.egg-info/
--rw-rw-rw-   0        0        0     1958 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 17:38:33.000000 actionlint_py-1.6.24.2/actionlint_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1737 2023-05-03 17:38:33.453090 actionlint_py-1.6.24.2/setup.cfg
--rw-rw-rw-   0        0        0     5099 2023-05-03 17:13:49.000000 actionlint_py-1.6.24.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 19:21:18.577056 actionlint_py-1.6.25.2/
+-rw-rw-rw-   0        0        0     1087 2023-05-03 15:51:52.000000 actionlint_py-1.6.25.2/LICENSE
+-rw-rw-rw-   0        0        0     2081 2023-07-09 19:21:18.577056 actionlint_py-1.6.25.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-07-09 19:19:45.000000 actionlint_py-1.6.25.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 19:21:18.576054 actionlint_py-1.6.25.2/actionlint_py.egg-info/
+-rw-rw-rw-   0        0        0     2081 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1737 2023-07-09 19:21:18.578389 actionlint_py-1.6.25.2/setup.cfg
+-rw-rw-rw-   0        0        0     5099 2023-05-03 17:13:49.000000 actionlint_py-1.6.25.2/setup.py
```

### Comparing `actionlint_py-1.6.24.2/LICENSE` & `actionlint_py-1.6.25.2/LICENSE`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.24.2/PKG-INFO` & `actionlint_py-1.6.25.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.6.24.2
+Version: 1.6.25.2
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Home-page: https://github.com/Mateusz-Grzelinski/actionlint-py
 Author: Ryan Rhee, Mateusz Grzeliński
 Author-email: grzelinskimat@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,50 +18,55 @@
 # actionlint-py
 
 A python wrapper to provide a pip-installable [actionlint] binary.
 
 Internally this package provides a convenient way to download the pre-built
 actionlint binary for your particular platform.
 
-### installation
+### Installation
 
 ```bash
 pip install actionlint-py
 ```
 
-### usage
+### Usage
 
 After installation, the `actionlint` binary should be available in your
 environment (or `actionlint.exe` on windows).
 
 ### As a pre-commit hook
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.22
+  rev: v1.6.25
   hooks:
-  - id: actionlint
+    - id: actionlint
 ```
 
 or to avoid going twice to internet (might help with proxy):
 
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Test yaml scripts with actionlint
-#      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
-      additional_dependencies: [actionlint-py]
+      #      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
+      additional_dependencies: [ actionlint-py ]
       entry: actionlint
-#      args: [-ignore "*.set-output. was depracated.*"]
+      #      args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
 [actionlint]: https://github.com/rhysd/actionlint
+
 [pre-commit]: https://pre-commit.com
+
+# Development
+
+Development of wrapper and releasing new version: see [README-DEV.md](README-DEV.md)
```

### Comparing `actionlint_py-1.6.24.2/README.md` & `actionlint_py-1.6.25.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 # actionlint-py
 
 A python wrapper to provide a pip-installable [actionlint] binary.
 
 Internally this package provides a convenient way to download the pre-built
 actionlint binary for your particular platform.
 
-### installation
+### Installation
 
 ```bash
 pip install actionlint-py
 ```
 
-### usage
+### Usage
 
 After installation, the `actionlint` binary should be available in your
 environment (or `actionlint.exe` on windows).
 
 ### As a pre-commit hook
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.22
+  rev: v1.6.25
   hooks:
-  - id: actionlint
+    - id: actionlint
 ```
 
 or to avoid going twice to internet (might help with proxy):
 
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Test yaml scripts with actionlint
-#      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
-      additional_dependencies: [actionlint-py]
+      #      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
+      additional_dependencies: [ actionlint-py ]
       entry: actionlint
-#      args: [-ignore "*.set-output. was depracated.*"]
+      #      args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
 [actionlint]: https://github.com/rhysd/actionlint
+
 [pre-commit]: https://pre-commit.com
+
+# Development
+
+Development of wrapper and releasing new version: see [README-DEV.md](README-DEV.md)
```

### Comparing `actionlint_py-1.6.24.2/actionlint_py.egg-info/PKG-INFO` & `actionlint_py-1.6.25.2/actionlint_py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint-py
-Version: 1.6.24.2
+Version: 1.6.25.2
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Home-page: https://github.com/Mateusz-Grzelinski/actionlint-py
 Author: Ryan Rhee, Mateusz Grzeliński
 Author-email: grzelinskimat@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,50 +18,55 @@
 # actionlint-py
 
 A python wrapper to provide a pip-installable [actionlint] binary.
 
 Internally this package provides a convenient way to download the pre-built
 actionlint binary for your particular platform.
 
-### installation
+### Installation
 
 ```bash
 pip install actionlint-py
 ```
 
-### usage
+### Usage
 
 After installation, the `actionlint` binary should be available in your
 environment (or `actionlint.exe` on windows).
 
 ### As a pre-commit hook
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.22
+  rev: v1.6.25
   hooks:
-  - id: actionlint
+    - id: actionlint
 ```
 
 or to avoid going twice to internet (might help with proxy):
 
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Test yaml scripts with actionlint
-#      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
-      additional_dependencies: [actionlint-py]
+      #      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
+      additional_dependencies: [ actionlint-py ]
       entry: actionlint
-#      args: [-ignore "*.set-output. was depracated.*"]
+      #      args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
 [actionlint]: https://github.com/rhysd/actionlint
+
 [pre-commit]: https://pre-commit.com
+
+# Development
+
+Development of wrapper and releasing new version: see [README-DEV.md](README-DEV.md)
```

### Comparing `actionlint_py-1.6.24.2/setup.py` & `actionlint_py-1.6.25.2/setup.py`

 * *Files identical despite different names*

