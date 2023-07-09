# Comparing `tmp/gwf_wrangler-0.0.2.tar.gz` & `tmp/gwf_wrangler-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwf_wrangler-0.0.2.tar", last modified: Sat Jul  1 21:20:56 2023, max compression
+gzip compressed data, was "gwf_wrangler-0.0.6.tar", last modified: Sun Jul  9 04:08:06 2023, max compression
```

## Comparing `gwf_wrangler-0.0.2.tar` & `gwf_wrangler-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1052 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.2/LICENSE
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.2/MANIFEST.in
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     4758 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/PKG-INFO
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     3023 2023-07-01 21:14:06.000000 gwf_wrangler-0.0.2/README.md
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.986256 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     4758 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/PKG-INFO
--rw-rw-r--   0 rlong     (1000) rlong     (1000)      614 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/SOURCES.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        1 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/dependency_links.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       47 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/entry_points.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       63 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/requires.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       29 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/top_level.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1460 2023-07-01 21:20:25.000000 gwf_wrangler-0.0.2/pyproject.toml
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       38 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/setup.cfg
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.986256 gwf_wrangler-0.0.2/src/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.2/src/__init__.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1727 2023-07-01 21:04:52.000000 gwf_wrangler-0.0.2/src/__main__.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1019 2023-07-01 21:10:39.000000 gwf_wrangler-0.0.2/src/cli.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     3577 2023-07-01 20:28:10.000000 gwf_wrangler-0.0.2/src/script.py
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.982257 gwf_wrangler-0.0.2/venv/
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/venv/bin/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1176 2023-07-01 20:23:27.000000 gwf_wrangler-0.0.2/venv/bin/activate_this.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      631 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2html.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      753 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2html4.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)     1088 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2html5.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      830 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2latex.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      653 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2man.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      819 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2odt.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      625 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      638 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      674 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2s5.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      910 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2xetex.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      639 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2xml.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      707 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rstpep2html.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1052 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.6/LICENSE
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.6/MANIFEST.in
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     4774 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/PKG-INFO
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     3031 2023-07-09 04:04:17.000000 gwf_wrangler-0.0.6/README.md
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     4774 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/PKG-INFO
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)      647 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/SOURCES.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        1 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/dependency_links.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       47 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/entry_points.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       63 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/requires.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       29 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/top_level.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1255 2023-07-09 04:07:56.000000 gwf_wrangler-0.0.6/pyproject.toml
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       38 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/setup.cfg
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/src/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.6/src/__init__.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     3848 2023-07-09 03:53:20.000000 gwf_wrangler-0.0.6/src/__main__.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1435 2023-07-09 03:08:58.000000 gwf_wrangler-0.0.6/src/cli.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     2014 2023-07-09 02:43:34.000000 gwf_wrangler-0.0.6/src/mapper.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1200 2023-07-09 02:56:07.000000 gwf_wrangler-0.0.6/src/script.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/tests/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1087 2023-07-09 03:51:36.000000 gwf_wrangler-0.0.6/tests/test_main.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/venv/
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/venv/bin/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1176 2023-07-01 20:23:27.000000 gwf_wrangler-0.0.6/venv/bin/activate_this.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      631 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2html.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      753 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2html4.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)     1088 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2html5.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      830 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2latex.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      653 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2man.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      819 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2odt.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      625 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      638 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      674 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2s5.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      910 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      639 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2xml.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      707 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rstpep2html.py
```

### Comparing `gwf_wrangler-0.0.2/LICENSE` & `gwf_wrangler-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/PKG-INFO` & `gwf_wrangler-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: gwf_wrangler
-Version: 0.0.2
+Version: 0.0.6
 Summary: A python package to convert yaml files to lua scripts for the Global Workflow Project.
 Author-email: Ryan Long <ryan.long@noaa.gov>
 License: Copyright 2023 NOAA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-Project-URL: Homepage, https://github.com/pypa/wrangler
-Project-URL: Bug Tracker, https://github.com/pypa/wrangler/issues
+Project-URL: Homepage, https://github.com/pypa/gwf-wrangler
+Project-URL: Bug Tracker, https://github.com/pypa/gwf-wrangler/issues
 Keywords: globalworkflow,global workflow,esmf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Wrangler (0.0.2)
+# Wrangler (0.0.5)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
 
 - DEBUG: You should use this level for debugging purposes in development.
 - INFO: You should use this level when something interesting—but expected—happens (e.g., a user starts a new project in a project management application).
 - WARNING: You should use this level when something unexpected or unusual happens. It’s not an error, but you should pay attention to it.
 - ERROR: This level is for things that go wrong but are usually recoverable (e.g., internal exceptions you can handle or APIs returning error results).
 - CRITICAL: You should use this level in a doomsday scenario. The application is unusable. At this level, someone should be woken up at 2 a.m.
-
+        
 ### Include a Timestamp for Each Log Entry
 
 Knowing something happened without knowing when it happened is only marginally better than not knowing about the event at all. Make sure to add a timestamp to your log entries to make the lives of the people who use logs for troubleshooting easier. Doing so also allows developers to analyze the log entries to obtain insights/analytics about user behavior.
 
 ### Adopt the ISO-8601 Format for Timestamps
 
 Timestamps are essential in log entries. Unfortunately, people can’t agree on the best way to express instants in time, so we came up with several conflicting formats.
```

### Comparing `gwf_wrangler-0.0.2/README.md` & `gwf_wrangler-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
-# Wrangler (0.0.2)
+# Wrangler (0.0.5)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
 
 - DEBUG: You should use this level for debugging purposes in development.
 - INFO: You should use this level when something interesting—but expected—happens (e.g., a user starts a new project in a project management application).
 - WARNING: You should use this level when something unexpected or unusual happens. It’s not an error, but you should pay attention to it.
 - ERROR: This level is for things that go wrong but are usually recoverable (e.g., internal exceptions you can handle or APIs returning error results).
 - CRITICAL: You should use this level in a doomsday scenario. The application is unusable. At this level, someone should be woken up at 2 a.m.
-
+        
 ### Include a Timestamp for Each Log Entry
 
 Knowing something happened without knowing when it happened is only marginally better than not knowing about the event at all. Make sure to add a timestamp to your log entries to make the lives of the people who use logs for troubleshooting easier. Doing so also allows developers to analyze the log entries to obtain insights/analytics about user behavior.
 
 ### Adopt the ISO-8601 Format for Timestamps
 
 Timestamps are essential in log entries. Unfortunately, people can’t agree on the best way to express instants in time, so we came up with several conflicting formats.
```

### Comparing `gwf_wrangler-0.0.2/gwf_wrangler.egg-info/PKG-INFO` & `gwf_wrangler-0.0.6/gwf_wrangler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: gwf-wrangler
-Version: 0.0.2
+Version: 0.0.6
 Summary: A python package to convert yaml files to lua scripts for the Global Workflow Project.
 Author-email: Ryan Long <ryan.long@noaa.gov>
 License: Copyright 2023 NOAA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-Project-URL: Homepage, https://github.com/pypa/wrangler
-Project-URL: Bug Tracker, https://github.com/pypa/wrangler/issues
+Project-URL: Homepage, https://github.com/pypa/gwf-wrangler
+Project-URL: Bug Tracker, https://github.com/pypa/gwf-wrangler/issues
 Keywords: globalworkflow,global workflow,esmf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Wrangler (0.0.2)
+# Wrangler (0.0.5)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
 
 - DEBUG: You should use this level for debugging purposes in development.
 - INFO: You should use this level when something interesting—but expected—happens (e.g., a user starts a new project in a project management application).
 - WARNING: You should use this level when something unexpected or unusual happens. It’s not an error, but you should pay attention to it.
 - ERROR: This level is for things that go wrong but are usually recoverable (e.g., internal exceptions you can handle or APIs returning error results).
 - CRITICAL: You should use this level in a doomsday scenario. The application is unusable. At this level, someone should be woken up at 2 a.m.
-
+        
 ### Include a Timestamp for Each Log Entry
 
 Knowing something happened without knowing when it happened is only marginally better than not knowing about the event at all. Make sure to add a timestamp to your log entries to make the lives of the people who use logs for troubleshooting easier. Doing so also allows developers to analyze the log entries to obtain insights/analytics about user behavior.
 
 ### Adopt the ISO-8601 Format for Timestamps
 
 Timestamps are essential in log entries. Unfortunately, people can’t agree on the best way to express instants in time, so we came up with several conflicting formats.
```

### Comparing `gwf_wrangler-0.0.2/gwf_wrangler.egg-info/SOURCES.txt` & `gwf_wrangler-0.0.6/gwf_wrangler.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 gwf_wrangler.egg-info/dependency_links.txt
 gwf_wrangler.egg-info/entry_points.txt
 gwf_wrangler.egg-info/requires.txt
 gwf_wrangler.egg-info/top_level.txt
 src/__init__.py
 src/__main__.py
 src/cli.py
+src/mapper.py
 src/script.py
+tests/test_main.py
 venv/bin/activate_this.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
 venv/bin/rst2html5.py
 venv/bin/rst2latex.py
 venv/bin/rst2man.py
 venv/bin/rst2odt.py
```

### Comparing `gwf_wrangler-0.0.2/pyproject.toml` & `gwf_wrangler-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "versioneer[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gwf_wrangler"
 description = "A python package to convert yaml files to lua scripts for the Global Workflow Project."
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.6"
 dependencies = ["PyYAML"]
 authors = [{ name = "Ryan Long", email = "ryan.long@noaa.gov" }]
 keywords = ["globalworkflow", "global workflow", "esmf"]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -22,32 +22,23 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "twine", "build"]
 
 
 [project.scripts]
 wrangler = "src.__main__:main"
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/wrangler"
-"Bug Tracker" = "https://github.com/pypa/wrangler/issues"
+"Homepage" = "https://github.com/pypa/gwf-wrangler"
+"Bug Tracker" = "https://github.com/pypa/gwf-wrangler/issues"
 
 [tool.setuptools.packages]
 find = {} # Scan the project directory with the default parameters
 
-[tool.versioneer]
-VCS = "git"
-style = "pep440"
-versionfile_source = "src/wrangler/_version.py"
-versionfile_build = "wrangler/_version.py"
-tag_prefix = ""
-# parentdir_prefix = "myproject-"
-
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
-"pyproject.toml" = ['']
 "README.md" = ["{pep440_version}"]
```

### Comparing `gwf_wrangler-0.0.2/venv/bin/activate_this.py` & `gwf_wrangler-0.0.6/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2html.py` & `gwf_wrangler-0.0.6/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2html4.py` & `gwf_wrangler-0.0.6/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2html5.py` & `gwf_wrangler-0.0.6/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2latex.py` & `gwf_wrangler-0.0.6/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2man.py` & `gwf_wrangler-0.0.6/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2odt.py` & `gwf_wrangler-0.0.6/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2odt_prepstyles.py` & `gwf_wrangler-0.0.6/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2pseudoxml.py` & `gwf_wrangler-0.0.6/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2s5.py` & `gwf_wrangler-0.0.6/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2xetex.py` & `gwf_wrangler-0.0.6/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rst2xml.py` & `gwf_wrangler-0.0.6/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.2/venv/bin/rstpep2html.py` & `gwf_wrangler-0.0.6/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

