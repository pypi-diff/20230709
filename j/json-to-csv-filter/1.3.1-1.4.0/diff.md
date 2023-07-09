# Comparing `tmp/json_to_csv_filter-1.3.1.tar.gz` & `tmp/json_to_csv_filter-1.4.0.tar.gz`

## Comparing `json_to_csv_filter-1.3.1.tar` & `json_to_csv_filter-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/deploy.sh
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/.gitignore
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/json_to_csv.iml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/src/json_to_csv_filter/__init__.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/src/json_to_csv_filter/json_to_csv.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/LICENSE
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 json_to_csv_filter-1.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/deploy.sh
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/.gitignore
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/json_to_csv.iml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/src/json_to_csv_filter/__init__.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/src/json_to_csv_filter/json_to_csv.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/README.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 json_to_csv_filter-1.4.0/PKG-INFO
```

### Comparing `json_to_csv_filter-1.3.1/.github/workflows/python-package.yml` & `json_to_csv_filter-1.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.3.1/.idea/workspace.xml` & `json_to_csv_filter-1.4.0/.idea/workspace.xml`

 * *Files 7% similar despite different names*

#### Comparing `json_to_csv_filter-1.3.1/.idea/workspace.xml` & `json_to_csv_filter-1.4.0/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment="renamed package"/>
+    <list default="true" id="3ce160a4-54f9-4e48-b828-419d5587133a" name="Changes" comment="renamed package">
+      <change beforePath="$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -40,29 +42,29 @@
 }</component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src"/>
       <recent name="$PROJECT_DIR$/json_to_csv"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python.json_to_csv_file_output">
+  <component name="RunManager" selected="Python.json_to_csv_stdout">
     <configuration name="json_to_csv_file_output" type="PythonConfigurationType" factoryName="Python">
       <module name="json_to_csv"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/src/json_to_csv/json_to_csv.py"/>
-      <option name="PARAMETERS" value="$USER_HOME$/ais_messages_2.json $USER_HOME$/ais_messages_2.csv -i rxtime nmea mmsi -o rxtime mmsi nmea -n 3 -d rxtime -df &quot;%x %X&quot;"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py"/>
+      <option name="PARAMETERS" value="$USER_HOME$/ais_messages_2.json $USER_HOME$/ais_messages_2.csv -i rxtime nmea mmsi -o rxtime mmsi nmea -n 3 -d rxtime"/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
@@ -74,16 +76,16 @@
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/src/json_to_csv/json_to_csv.py"/>
-      <option name="PARAMETERS" value="$USER_HOME$/ais_messages_2.json -i rxtime nmea mmsi -o rxtime mmsi nmea -n 3 -d rxtime -df %x"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/src/json_to_csv_filter/json_to_csv.py"/>
+      <option name="PARAMETERS" value="$USER_HOME$/ais_messages_2.json -i rxtime nmea mmsi -o rxtime mmsi nmea -n 3 -d rxtime -l none"/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
```

### Comparing `json_to_csv_filter-1.3.1/src/json_to_csv_filter/json_to_csv.py` & `json_to_csv_filter-1.4.0/src/json_to_csv_filter/json_to_csv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import argparse
-import os.path
 import sys
 import json
 import csv
 from typing import IO
-from dateutil.parser import parse
+
+import babel
+from dateutil.parser import parse, ParserError
+from babel.dates import format_datetime
 
 
 def _parse_args():
     parser = argparse.ArgumentParser(description='Convert list of json objects to csv')
+
     parser.add_argument('infile', nargs='?', type=str, default='-', help='Input file, defaults to STDIN')
     parser.add_argument('outfile', nargs='?', type=str, default='-', help='Output file, defaults to STDOUT')
     parser.add_argument('-i', '--include', nargs='*', default=set(), help='Include fields, defaults to all')
     parser.add_argument('-e', '--exclude', nargs='*', default=set(), help='Exclude fields, defaults to none')
     parser.add_argument('-o', '--order', nargs='*', default=[], help='Order fields, defaults to none')
     parser.add_argument('-n', '--number', nargs='?', default=-1, help='Number of records to process, defaults to all')
-
     parser.add_argument('-d', '--date-fields', nargs='*', default=set(), help='Date fields, defaults to none')
-    parser.add_argument('-df', '--date-format', nargs='?', default=None, help='Datetime format, defaults to none')
-    return parser.parse_args()
+    parser.add_argument('-df', '--date-format', nargs='?', default=None, help='Datetime format, defaults to nld short '
+                                                                              'date format')
+    parser.add_argument('-l', '--locale', nargs='?', default="nld", help='locale id, defaults to nld')
+
+    parser.epilog = 'See https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes for ' \
+                    'datetime format strings and https://babel.pocoo.org/en/latest/ for default nld locale datetime ' \
+                    'format'
+
+    return parser
 
 
 def _deserialize_json(json_input_file: IO, max_number_of_records: int):
     line_count = 0
     json_data = []
     json_keys = set()
 
@@ -56,16 +65,16 @@
         else:
             msg = 'argument "-" with mode %r' % mode
             raise ValueError(msg)
 
     # all other arguments are used as file names
     try:
         return open(filename, mode=mode, newline=newline)
-    except OSError as e:
-        args = {'filename': filename, 'error': e}
+    except OSError as os_error:
+        args = {'filename': filename, 'error': os_error}
         message = "can't open '%(filename)s': %(error)s"
         raise argparse.ArgumentTypeError(message % args)
 
 
 def include_fields(fields: set, include_list: set):
     if not include_list:
         return fields  # include all fields by default
@@ -82,48 +91,59 @@
 
 def order_fields(header: set, order_list: list):
     ordered_header_part = [h for h in order_list if h in header]
     unordered_header_part = header - set(ordered_header_part)
     return ordered_header_part + list(unordered_header_part)
 
 
-def format_datetime_fields(_data: list, datetime_fields: set, datetime_format: str):
+def format_datetime_fields(_data: list, datetime_fields: set, datetime_format: str, locale: str):
     formatted_list = []
     for row in _data:
         for key, value in row.items():
             if key in datetime_fields:
-                if datetime_format:
+                try:
                     datetime_value = parse(value)
-                    formatted_datetime_value = datetime_value.strftime(datetime_format)
-                else:
+
+                    if datetime_format:
+                        formatted_datetime_value = datetime_value.strftime(datetime_format)
+                    else:
+                        formatted_datetime_value = format_datetime(datetime_value, format='short', locale=locale)
+                except ParserError:
                     formatted_datetime_value = value
 
                 row[key] = formatted_datetime_value
 
         formatted_list.append(row)
 
     return formatted_list
 
 
 def main():
     # parse arguments from program options
-    args = _parse_args()
+    parser = _parse_args()
+    args = parser.parse_args()
+
+    try:
+        datetime_locale = babel.Locale.parse(args.locale)
+    except babel.UnknownLocaleError:
+        datetime_locale = parser.get_default('locale')
+        print("Unknown locale, using default: {0}\n".format(datetime_locale))
 
     # read json records from file
     with open_filename_arg(args.infile, mode='rt', newline='') as infile:
         data, header = _deserialize_json(infile, int(args.number))
 
     # include fields
     header = include_fields(header, set(args.include))
 
     # exclude fields
     header = exclude_fields(header, set(args.exclude))
 
     # format datetime fields
-    data = format_datetime_fields(data, set(args.date_fields), args.date_format)
+    data = format_datetime_fields(data, set(args.date_fields), args.date_format, datetime_locale)
 
     # order fields
     header = order_fields(header, args.order)
 
     # serialize python objects as csv file
     with open_filename_arg(args.outfile, mode='w', newline='') as outfile:
         _serialize_csv(outfile, list(header), data)
```

### Comparing `json_to_csv_filter-1.3.1/.gitignore` & `json_to_csv_filter-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.3.1/LICENSE` & `json_to_csv_filter-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_to_csv_filter-1.3.1/pyproject.toml` & `json_to_csv_filter-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'python-dateutil ~= 2.8.2'
+    'python-dateutil ~= 2.8.2',
+    'babel ~= 2.12.1'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hylkefoeken/json-to-csv"
 "Bug Tracker" = "https://github.com/hylkefoeken/json-to-csv/issues"
 
 [project.scripts]
```

### Comparing `json_to_csv_filter-1.3.1/PKG-INFO` & `json_to_csv_filter-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: json_to_csv_filter
-Version: 1.3.1
+Version: 1.4.0
 Summary: Convert list of json objects to csv with optional filters
 Project-URL: Homepage, https://github.com/hylkefoeken/json-to-csv
 Project-URL: Bug Tracker, https://github.com/hylkefoeken/json-to-csv/issues
 Author-email: Hylke Foeken <h.foeken@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: babel~=2.12.1
 Requires-Dist: python-dateutil~=2.8.2
 Description-Content-Type: text/markdown
 
 # Description
 Converts a list of json objects to a csv with optional filtering, sorting and date formatting.
 
+# installation
+This commands installs the package and an application script: json2csv. 
+```bash
+pip install json-to-csv-filter
+```
+
 # Usage
 ```bash
 usage: json_to_csv.py [-h] [-i [INCLUDE ...]] [-e [EXCLUDE ...]] [-o [ORDER ...]] [-n [NUMBER]] [-d [DATE_FIELDS ...]] [-df [DATE_FORMAT]]
                       [infile] [outfile]
 
 Convert list of json objects to csv
 
@@ -37,8 +44,14 @@
                         Order fields, defaults to none
   -n [NUMBER], --number [NUMBER]
                         Number of records to process, defaults to all
   -d [DATE_FIELDS ...], --date-fields [DATE_FIELDS ...]
                         Date fields, defaults to none
   -df [DATE_FORMAT], --date-format [DATE_FORMAT]
                         Datetime format, defaults to none
-```
+```
+
+# Examples
+## convert a json file to standard out
+```bash
+json2csv -i ais-messages.txt
+```
```

