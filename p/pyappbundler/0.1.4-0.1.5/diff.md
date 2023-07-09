# Comparing `tmp/pyappbundler-0.1.4.tar.gz` & `tmp/pyappbundler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappbundler-0.1.4.tar", last modified: Fri Jul  7 08:46:32 2023, max compression
+gzip compressed data, was "pyappbundler-0.1.5.tar", last modified: Sun Jul  9 02:08:41 2023, max compression
```

## Comparing `pyappbundler-0.1.4.tar` & `pyappbundler-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 08:46:32.794634 pyappbundler-0.1.4/
--rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      730 2023-07-07 08:46:32.794634 pyappbundler-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 08:46:32.790634 pyappbundler-0.1.4/pyappbundler/
--rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.4/pyappbundler/__init__.py
--rw-rw-rw-   0        0        0     2518 2023-07-07 08:42:32.000000 pyappbundler-0.1.4/pyappbundler/__main__.py
--rw-rw-rw-   0        0        0       22 2023-07-07 08:38:52.000000 pyappbundler-0.1.4/pyappbundler/_version.py
--rw-rw-rw-   0        0        0     5002 2023-07-07 08:31:58.000000 pyappbundler-0.1.4/pyappbundler/pyappbundler.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:46:32.793634 pyappbundler-0.1.4/pyappbundler/templates/
--rw-rw-rw-   0        0        0     1582 2023-07-07 08:41:22.000000 pyappbundler-0.1.4/pyappbundler/templates/iss.tmpl
-drwxrwxrwx   0        0        0        0 2023-07-07 08:46:32.793634 pyappbundler-0.1.4/pyappbundler.egg-info/
--rw-rw-rw-   0        0        0      730 2023-07-07 08:46:32.000000 pyappbundler-0.1.4/pyappbundler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-07 08:46:32.000000 pyappbundler-0.1.4/pyappbundler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 08:46:32.000000 pyappbundler-0.1.4/pyappbundler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-07 08:46:32.000000 pyappbundler-0.1.4/pyappbundler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-07 08:46:32.000000 pyappbundler-0.1.4/pyappbundler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 08:46:32.794634 pyappbundler-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.928820 pyappbundler-0.1.5/
+-rw-rw-rw-   0        0        0     1074 2023-07-05 03:17:37.000000 pyappbundler-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      730 2023-07-09 02:08:41.928820 pyappbundler-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-05 14:55:05.000000 pyappbundler-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.922819 pyappbundler-0.1.5/pyappbundler/
+-rw-rw-rw-   0        0        0       79 2023-07-06 12:55:47.000000 pyappbundler-0.1.5/pyappbundler/__init__.py
+-rw-rw-rw-   0        0        0     2518 2023-07-07 08:42:32.000000 pyappbundler-0.1.5/pyappbundler/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-07-08 10:54:23.000000 pyappbundler-0.1.5/pyappbundler/_version.py
+-rw-rw-rw-   0        0        0     5062 2023-07-08 10:56:52.000000 pyappbundler-0.1.5/pyappbundler/pyappbundler.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.927820 pyappbundler-0.1.5/pyappbundler/templates/
+-rw-rw-rw-   0        0        0     1705 2023-07-08 10:54:08.000000 pyappbundler-0.1.5/pyappbundler/templates/iss.tmpl
+drwxrwxrwx   0        0        0        0 2023-07-09 02:08:41.926821 pyappbundler-0.1.5/pyappbundler.egg-info/
+-rw-rw-rw-   0        0        0      730 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-09 02:08:41.000000 pyappbundler-0.1.5/pyappbundler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      776 2023-07-06 12:57:21.000000 pyappbundler-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 02:08:41.928820 pyappbundler-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-07-05 16:21:35.000000 pyappbundler-0.1.5/setup.py
```

### Comparing `pyappbundler-0.1.4/LICENSE` & `pyappbundler-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.4/PKG-INFO` & `pyappbundler-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.4
+Version: 0.1.5
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.4/pyappbundler/__main__.py` & `pyappbundler-0.1.5/pyappbundler/__main__.py`

 * *Files identical despite different names*

### Comparing `pyappbundler-0.1.4/pyappbundler/pyappbundler.py` & `pyappbundler-0.1.5/pyappbundler/pyappbundler.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
 
         iss_config = {
             'app_name': self.app_name,
             'app_ico': str(self.icon),
             'app_guid': self.app_guid,
             'app_ver': self.app_ver,
             'dist': str(self.dist),
+            'is_onefile': ('onefile' in self.pyinst_flags),
         }
 
         tmpl_path = Path(__file__).parent / 'templates/iss.tmpl'
         env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(tmpl_path.parent),
             keep_trailing_newline=True,
             block_start_string='{%%',
```

### Comparing `pyappbundler-0.1.4/pyappbundler/templates/iss.tmpl` & `pyappbundler-0.1.5/pyappbundler/templates/iss.tmpl`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,20 @@
 Name: "russian"; MessagesFile: "compiler:Languages\Russian.isl"
 Name: "ukrainian"; MessagesFile: "compiler:Languages\Ukrainian.isl"
 
 [Tasks]
 Name: "desktopicon"; Description: "{cm:CreateDesktopIcon}"; GroupDescription: "{cm:AdditionalIcons}"; Flags: unchecked
 
 [Files]
+{%% if is_onefile %%}
+Source: "{#Dist}\{#MyAppExeName}"; DestDir: "{app}"; Flags: ignoreversion
+{%% else %%}
 Source: "{#Dist}\{#MyAppName}\{#MyAppExeName}"; DestDir: "{app}"; Flags: ignoreversion
 Source: "{#Dist}\{#MyAppName}\*"; DestDir: "{app}"; Flags: ignoreversion recursesubdirs createallsubdirs
+{%% endif %%}
 ; NOTE: Don't use "Flags: ignoreversion" on any shared system files
 
 [Icons]
 Name: "{autoprograms}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"
 Name: "{autodesktop}\{#MyAppName}"; Filename: "{app}\{#MyAppExeName}"; Tasks: desktopicon
 
 [Run]
```

### Comparing `pyappbundler-0.1.4/pyappbundler.egg-info/PKG-INFO` & `pyappbundler-0.1.5/pyappbundler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappbundler
-Version: 0.1.4
+Version: 0.1.5
 Summary: automate bundle a Python application into a single package
 Author-email: inerject <kumbalup@gmail.com>
 Project-URL: Homepage, https://github.com/inerject/pyappbundler
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyappbundler-0.1.4/pyproject.toml` & `pyappbundler-0.1.5/pyproject.toml`

 * *Files identical despite different names*

