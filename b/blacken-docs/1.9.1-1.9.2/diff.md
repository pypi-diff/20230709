# Comparing `tmp/blacken_docs-1.9.1.tar.gz` & `tmp/blacken_docs-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blacken_docs-1.9.1.tar", last modified: Sun Dec 20 04:51:55 2020, max compression
+gzip compressed data, was "dist/blacken_docs-1.9.2.tar", last modified: Mon Jan 25 22:07:57 2021, max compression
```

## Comparing `blacken_docs-1.9.1.tar` & `blacken_docs-1.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2020-12-20 04:51:55.841843 blacken_docs-1.9.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2020-12-20 04:51:14.000000 blacken_docs-1.9.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3900 2020-12-20 04:51:55.841843 blacken_docs-1.9.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2281 2020-12-20 04:51:31.000000 blacken_docs-1.9.1/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2020-12-20 04:51:55.841843 blacken_docs-1.9.1/blacken_docs.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3900 2020-12-20 04:51:55.000000 blacken_docs-1.9.1/blacken_docs.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      270 2020-12-20 04:51:55.000000 blacken_docs-1.9.1/blacken_docs.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2020-12-20 04:51:55.000000 blacken_docs-1.9.1/blacken_docs.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2020-12-20 04:51:55.000000 blacken_docs-1.9.1/blacken_docs.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       14 2020-12-20 04:51:55.000000 blacken_docs-1.9.1/blacken_docs.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2020-12-20 04:51:55.000000 blacken_docs-1.9.1/blacken_docs.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7147 2020-12-20 04:51:14.000000 blacken_docs-1.9.1/blacken_docs.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1243 2020-12-20 04:51:55.841843 blacken_docs-1.9.1/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2020-12-20 04:51:14.000000 blacken_docs-1.9.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-01-25 22:07:57.639977 blacken_docs-1.9.2/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2021-01-25 22:07:18.000000 blacken_docs-1.9.2/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3900 2021-01-25 22:07:57.639977 blacken_docs-1.9.2/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2281 2021-01-25 22:07:39.000000 blacken_docs-1.9.2/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-01-25 22:07:57.639977 blacken_docs-1.9.2/blacken_docs.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3900 2021-01-25 22:07:57.000000 blacken_docs-1.9.2/blacken_docs.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      270 2021-01-25 22:07:57.000000 blacken_docs-1.9.2/blacken_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2021-01-25 22:07:57.000000 blacken_docs-1.9.2/blacken_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       52 2021-01-25 22:07:57.000000 blacken_docs-1.9.2/blacken_docs.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       14 2021-01-25 22:07:57.000000 blacken_docs-1.9.2/blacken_docs.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2021-01-25 22:07:57.000000 blacken_docs-1.9.2/blacken_docs.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7200 2021-01-25 22:07:18.000000 blacken_docs-1.9.2/blacken_docs.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1243 2021-01-25 22:07:57.639977 blacken_docs-1.9.2/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2021-01-25 22:07:18.000000 blacken_docs-1.9.2/setup.py
```

### Comparing `blacken_docs-1.9.1/LICENSE` & `blacken_docs-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blacken_docs-1.9.1/PKG-INFO` & `blacken_docs-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacken_docs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Run `black` on python code blocks in documentation files
 Home-page: https://github.com/asottile/blacken-docs
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Description: [![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.blacken-docs?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=36&branchName=master)
         [![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/36/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=36&branchName=master)
@@ -98,15 +98,15 @@
         See [pre-commit](https://pre-commit.com) for instructions
         
         Sample `.pre-commit-config.yaml`:
         
         
         ```yaml
         -   repo: https://github.com/asottile/blacken-docs
-            rev: v1.9.1
+            rev: v1.9.2
             hooks:
             -   id: blacken-docs
                 additional_dependencies: [black==...]
         ```
         
         Since `black` is currently a moving target, it is suggested to pin `black`
         to a specific version using `additional_dependencies`.
```

### Comparing `blacken_docs-1.9.1/README.md` & `blacken_docs-1.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 See [pre-commit](https://pre-commit.com) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 
 ```yaml
 -   repo: https://github.com/asottile/blacken-docs
-    rev: v1.9.1
+    rev: v1.9.2
     hooks:
     -   id: blacken-docs
         additional_dependencies: [black==...]
 ```
 
 Since `black` is currently a moving target, it is suggested to pin `black`
 to a specific version using `additional_dependencies`.
```

### Comparing `blacken_docs-1.9.1/blacken_docs.egg-info/PKG-INFO` & `blacken_docs-1.9.2/blacken_docs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacken-docs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Run `black` on python code blocks in documentation files
 Home-page: https://github.com/asottile/blacken-docs
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Description: [![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.blacken-docs?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=36&branchName=master)
         [![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/36/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=36&branchName=master)
@@ -98,15 +98,15 @@
         See [pre-commit](https://pre-commit.com) for instructions
         
         Sample `.pre-commit-config.yaml`:
         
         
         ```yaml
         -   repo: https://github.com/asottile/blacken-docs
-            rev: v1.9.1
+            rev: v1.9.2
             hooks:
             -   id: blacken-docs
                 additional_dependencies: [black==...]
         ```
         
         Since `black` is currently a moving target, it is suggested to pin `black`
         to a specific version using `additional_dependencies`.
```

### Comparing `blacken_docs-1.9.1/blacken_docs.py` & `blacken_docs-1.9.2/blacken_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 )
 RST_PYCON_RE = re.compile(
     r'(?P<before>'
     r'(?P<indent> *)\.\. (code|code-block):: pycon\n'
     r'((?P=indent) +:.*\n)*'
     r'\n*'
     r')'
-    r'(?P<code>(^((?P=indent) +.*)?\n)+)',
+    r'(?P<code>(^((?P=indent) +.*)?(\n|$))+)',
     re.MULTILINE,
 )
 PYCON_PREFIX = '>>> '
 PYCON_CONTINUATION_PREFIX = '...'
 PYCON_CONTINUATION_RE = re.compile(
     rf'^{re.escape(PYCON_CONTINUATION_PREFIX)}( |$)',
 )
@@ -120,24 +120,25 @@
                     # ...
                     if line:
                         code += f'{PYCON_CONTINUATION_PREFIX} {line}\n'
                 if fragment_lines[-1].startswith(' '):
                     code += f'{PYCON_CONTINUATION_PREFIX}\n'
                 fragment = None
 
+        indentation = None
         for line in match['code'].splitlines():
             orig_line, line = line, line.lstrip()
+            if indentation is None and line:
+                indentation = len(orig_line) - len(line)
             continuation_match = PYCON_CONTINUATION_RE.match(line)
-            if continuation_match:
-                assert fragment is not None
+            if continuation_match and fragment is not None:
                 fragment += line[continuation_match.end():] + '\n'
             else:
                 finish_fragment()
                 if line.startswith(PYCON_PREFIX):
-                    indentation = len(orig_line) - len(line)
                     fragment = line[len(PYCON_PREFIX):] + '\n'
                 else:
                     code += orig_line[indentation:] + '\n'
         finish_fragment()
 
         min_indent = min(INDENT_RE.findall(match['code']))
         code = textwrap.indent(code, min_indent)
```

### Comparing `blacken_docs-1.9.1/setup.cfg` & `blacken_docs-1.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = blacken_docs
-version = 1.9.1
+version = 1.9.2
 description = Run `black` on python code blocks in documentation files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/blacken-docs
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

