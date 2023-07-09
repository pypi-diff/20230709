# Comparing `tmp/json_to_csv_filter-1.4.0.tar.gz` & `tmp/json_to_csv_filter-1.4.1.tar.gz`

## Comparing `json_to_csv_filter-1.4.0.tar` & `json_to_csv_filter-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/deploy.sh
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/.gitignore
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/json_to_csv.iml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/vcs.xml
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/src/json_to_csv_filter/__init__.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/src/json_to_csv_filter/json_to_csv.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/LICENSE
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/README.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/deploy.sh
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.idea/.gitignore
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.idea/json_to_csv.iml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/src/json_to_csv_filter/__init__.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/src/json_to_csv_filter/json_to_csv.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/README.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.1/PKG-INFO
```

### Comparing `json_to_csv_filter-1.4.0/.github/workflows/python-package.yml` & `json_to_csv_filter-1.4.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.4.0/.idea/workspace.xml` & `json_to_csv_filter-1.4.1/.idea/workspace.xml`

 * *Files 11% similar despite different names*

#### Comparing `json_to_csv_filter-1.4.0/.idea/workspace.xml` & `json_to_csv_filter-1.4.1/.idea/workspace.xml`

```diff
@@ -1,14 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment="renamed package">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -124,8 +125,19 @@
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="renamed package"/>
     <option name="LAST_COMMIT_MESSAGE" value="renamed package"/>
   </component>
+  <component name="XDebuggerManager">
+    <breakpoint-manager>
+      <breakpoints>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py</url>
+          <line>127</line>
+          <option name="timeStamp" value="4"/>
+        </line-breakpoint>
+      </breakpoints>
+    </breakpoint-manager>
+  </component>
 </project>
```

### Comparing `json_to_csv_filter-1.4.0/src/json_to_csv_filter/json_to_csv.py` & `json_to_csv_filter-1.4.1/src/json_to_csv_filter/json_to_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     parser.add_argument('infile', nargs='?', type=str, default='-', help='Input file, defaults to STDIN')
     parser.add_argument('outfile', nargs='?', type=str, default='-', help='Output file, defaults to STDOUT')
     parser.add_argument('-i', '--include', nargs='*', default=set(), help='Include fields, defaults to all')
     parser.add_argument('-e', '--exclude', nargs='*', default=set(), help='Exclude fields, defaults to none')
     parser.add_argument('-o', '--order', nargs='*', default=[], help='Order fields, defaults to none')
     parser.add_argument('-n', '--number', nargs='?', default=-1, help='Number of records to process, defaults to all')
     parser.add_argument('-d', '--date-fields', nargs='*', default=set(), help='Date fields, defaults to none')
-    parser.add_argument('-df', '--date-format', nargs='?', default=None, help='Datetime format, defaults to nld short '
-                                                                              'date format')
+    parser.add_argument('-df', '--date-format', nargs='?', default=None, help='Custom datetime format')
     parser.add_argument('-l', '--locale', nargs='?', default="nld", help='locale id, defaults to nld')
 
     parser.epilog = 'See https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes for ' \
                     'datetime format strings and https://babel.pocoo.org/en/latest/ for default nld locale datetime ' \
                     'format'
 
     return parser
```

### Comparing `json_to_csv_filter-1.4.0/.gitignore` & `json_to_csv_filter-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.4.0/LICENSE` & `json_to_csv_filter-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.4.0/README.md` & `json_to_csv_filter-1.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 This commands installs the package and an application script: json2csv. 
 ```bash
 pip install json-to-csv-filter
 ```
 
 # Usage
 ```bash
-usage: json_to_csv.py [-h] [-i [INCLUDE ...]] [-e [EXCLUDE ...]] [-o [ORDER ...]] [-n [NUMBER]] [-d [DATE_FIELDS ...]] [-df [DATE_FORMAT]]
-                      [infile] [outfile]
+usage: json_to_csv.py [-h] [-i [INCLUDE ...]] [-e [EXCLUDE ...]] [-o [ORDER ...]] [-n [NUMBER]] [-d [DATE_FIELDS ...]] [-df [DATE_FORMAT]] [-l [LOCALE]] [infile] [outfile]
 
 Convert list of json objects to csv
 
 positional arguments:
   infile                Input file, defaults to STDIN
   outfile               Output file, defaults to STDOUT
 
@@ -27,15 +26,19 @@
   -o [ORDER ...], --order [ORDER ...]
                         Order fields, defaults to none
   -n [NUMBER], --number [NUMBER]
                         Number of records to process, defaults to all
   -d [DATE_FIELDS ...], --date-fields [DATE_FIELDS ...]
                         Date fields, defaults to none
   -df [DATE_FORMAT], --date-format [DATE_FORMAT]
-                        Datetime format, defaults to none
+                        Custom datetime format
+  -l [LOCALE], --locale [LOCALE]
+                        locale id, defaults to nld
+
+See https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes for datetime format strings and https://babel.pocoo.org/en/latest/ for default nld locale datetime format
 ```
 
 # Examples
 ## convert a json file to standard out
 ```bash
 json2csv -i ais-messages.txt
 ```
```

### Comparing `json_to_csv_filter-1.4.0/pyproject.toml` & `json_to_csv_filter-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.4.0/PKG-INFO` & `json_to_csv_filter-1.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_to_csv_filter
-Version: 1.4.0
+Version: 1.4.1
 Summary: Convert list of json objects to csv with optional filters
 Project-URL: Homepage, https://github.com/hylkefoeken/json-to-csv
 Project-URL: Bug Tracker, https://github.com/hylkefoeken/json-to-csv/issues
 Author-email: Hylke Foeken <h.foeken@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,15 @@
 This commands installs the package and an application script: json2csv. 
 ```bash
 pip install json-to-csv-filter
 ```
 
 # Usage
 ```bash
-usage: json_to_csv.py [-h] [-i [INCLUDE ...]] [-e [EXCLUDE ...]] [-o [ORDER ...]] [-n [NUMBER]] [-d [DATE_FIELDS ...]] [-df [DATE_FORMAT]]
-                      [infile] [outfile]
+usage: json_to_csv.py [-h] [-i [INCLUDE ...]] [-e [EXCLUDE ...]] [-o [ORDER ...]] [-n [NUMBER]] [-d [DATE_FIELDS ...]] [-df [DATE_FORMAT]] [-l [LOCALE]] [infile] [outfile]
 
 Convert list of json objects to csv
 
 positional arguments:
   infile                Input file, defaults to STDIN
   outfile               Output file, defaults to STDOUT
 
@@ -43,15 +42,19 @@
   -o [ORDER ...], --order [ORDER ...]
                         Order fields, defaults to none
   -n [NUMBER], --number [NUMBER]
                         Number of records to process, defaults to all
   -d [DATE_FIELDS ...], --date-fields [DATE_FIELDS ...]
                         Date fields, defaults to none
   -df [DATE_FORMAT], --date-format [DATE_FORMAT]
-                        Datetime format, defaults to none
+                        Custom datetime format
+  -l [LOCALE], --locale [LOCALE]
+                        locale id, defaults to nld
+
+See https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes for datetime format strings and https://babel.pocoo.org/en/latest/ for default nld locale datetime format
 ```
 
 # Examples
 ## convert a json file to standard out
 ```bash
 json2csv -i ais-messages.txt
 ```
```

