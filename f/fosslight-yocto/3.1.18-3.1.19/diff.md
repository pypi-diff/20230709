# Comparing `tmp/fosslight_yocto-3.1.18.tar.gz` & `tmp/fosslight_yocto-3.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_yocto-3.1.18.tar", last modified: Mon Mar  6 04:30:58 2023, max compression
+gzip compressed data, was "fosslight_yocto-3.1.19.tar", last modified: Sun Jul  9 07:00:28 2023, max compression
```

## Comparing `fosslight_yocto-3.1.18.tar` & `fosslight_yocto-3.1.19.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 04:30:58.810312 fosslight_yocto-3.1.18/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      101 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2973 2023-03-06 04:30:58.810312 fosslight_yocto-3.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2062 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 04:30:58.806311 fosslight_yocto-3.1.18/files_for_preparation/
--rw-r--r--   0 runner    (1001) docker     (116)     2663 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/files_for_preparation/bom.bbclass
--rw-r--r--   0 runner    (1001) docker     (116)      184 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-06 04:30:58.810312 fosslight_yocto-3.1.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 04:30:58.806311 fosslight_yocto-3.1.18/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 04:30:58.810312 fosslight_yocto-3.1.18/src/fosslight_yocto/
--rwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1953 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5691 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/_overwrite_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8959 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/_package_item.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2596 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/_write_result_file.py
--rw-r--r--   0 runner    (1001) docker     (116)     6216 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/_zip_source_works.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    43127 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/create_oss_report_for_yocto.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8200 2023-03-06 04:30:43.000000 fosslight_yocto-3.1.18/src/fosslight_yocto/parsing_meta_doubleopen.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 04:30:58.810312 fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2973 2023-03-06 04:30:58.000000 fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      667 2023-03-06 04:30:58.000000 fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-06 04:30:58.000000 fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      154 2023-03-06 04:30:58.000000 fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      184 2023-03-06 04:30:58.000000 fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-06 04:30:58.000000 fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:00:28.698814 fosslight_yocto-3.1.19/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-09 07:00:28.698814 fosslight_yocto-3.1.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:00:28.694814 fosslight_yocto-3.1.19/files_for_preparation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/files_for_preparation/bom.bbclass
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 07:00:28.698814 fosslight_yocto-3.1.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:00:28.694814 fosslight_yocto-3.1.19/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:00:28.694814 fosslight_yocto-3.1.19/src/fosslight_yocto/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5691 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/_overwrite_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9496 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/_package_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3601 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/_write_result_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/_zip_source_works.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43781 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/create_oss_report_for_yocto.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8200 2023-07-09 07:00:17.000000 fosslight_yocto-3.1.19/src/fosslight_yocto/parsing_meta_doubleopen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:00:28.694814 fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-09 07:00:28.000000 fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-09 07:00:28.000000 fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:00:28.000000 fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-09 07:00:28.000000 fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-09 07:00:28.000000 fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 07:00:28.000000 fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/top_level.txt
```

### Comparing `fosslight_yocto-3.1.18/LICENSE` & `fosslight_yocto-3.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.18/PKG-INFO` & `fosslight_yocto-3.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_yocto
-Version: 3.1.18
+Version: 3.1.19
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.18 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.19 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        [Korean]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.] [Current python package version.] [https://img.shields.io/
 pypi/pyversions/fosslight_yocto] [![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.18/README.md` & `fosslight_yocto-3.1.19/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.18/files_for_preparation/bom.bbclass` & `fosslight_yocto-3.1.19/files_for_preparation/bom.bbclass`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.18/setup.py` & `fosslight_yocto-3.1.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_yocto',
-        version='3.1.18',
+        version='3.1.19',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Yocto',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto/_help.py` & `fosslight_yocto-3.1.19/src/fosslight_yocto/_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
             -a <path>\t\t\t   Path to analyze the binaries
             -n\t\t\t\t   Print result in BIN(Android) format
             -d\t\t\t\t   Change license to declared license
             -s\t\t\t\t   Analyze source code for unconfirmed Open Source
             -c\t\t\t\t   Analyze all the source code
             -e\t\t\t\t   Compress all the source code
             -o <path>\t\t\t   Output Path
-            -f <format>\t\t\t   Output file format (excel, csv, opossum)"""
+            -f <format>\t\t\t   Output file format (excel, csv, opossum)
+            -pr\t\t\t\t   Print all data of bom.json"""
 
 _HELP_MESSAGE_META_DOUBLE = """
     Usage: fosslight_doubleopen [option1] <arg1> [option2] <arg2>...
 
     FOSSLight Yocto for parsing meta-doubleopen's result file
 
     Options:
```

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto/_overwrite_yaml.py` & `fosslight_yocto-3.1.19/src/fosslight_yocto/_overwrite_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto/_package_item.py` & `fosslight_yocto-3.1.19/src/fosslight_yocto/_package_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self._package_name = ""  # Installed Package name
         self.src_path = ""
         self.file_path = ""
         self.spdx_id = ""
         self._yocto_recipe = []
         self._yocto_package = []
         self.relative_path = ""
+        self.additional_data = {}
 
     def __eq__(self, value):
         return self.spdx_id == value
 
     def __del__(self):
         pass
 
@@ -167,36 +168,43 @@
     @declared_licenses.setter
     def declared_licenses(self, value):
         if value != "" and isinstance(value, list):
             if len(value) > 0:
                 self.comment = "License changed to the license registered in OSC System DB."
                 self._declared_licenses = value
 
-    def get_print_item(self, bin_android_format=False):
+    def get_print_item(self, bin_android_format=False, additional_column=[]):
         print_items = []
         license_to_print = self.license
         exclude = EXCLUDE_TRUE_VALUE if self.exclude else ""
         if len(self.declared_licenses) > 0:
             license_to_print = self.declared_licenses
         if bin_android_format:  # BIN(Android) Sheet
-            print_items.append(
-                [self.parent_package_name, self.oss_name, "", self.name, self.version,
-                 ','.join(license_to_print),
-                 self.download_location, self.homepage, self.copyright, exclude, self.comment])
+            row = [self.parent_package_name, self.oss_name, "", self.name, self.version,
+                   ','.join(license_to_print),
+                   self.download_location, self.homepage, self.copyright, exclude, self.comment]
+            for column_name in additional_column:
+                row.append(self.additional_data.get(column_name, ''))
+            print_items.append(row)
         else:
             if len(self.source_name_or_path) > 0:  # BIN Sheet
                 for file in self.source_name_or_path:
-                    print_items.append(
-                        [file, self.name, self.version, ','.join(license_to_print), self.download_location,
-                         self.homepage, self.copyright, exclude, self.comment])
+                    row = [file, self.name, self.version, ','.join(license_to_print), self.download_location,
+                           self.homepage, self.copyright, exclude, self.comment]
+                    for column_name in additional_column:
+                        row.append(self.additional_data.get(column_name, ''))
+                    print_items.append(row)
+
             else:  # SRC Sheet
-                print_items.append(
-                    [self.parent_package_name, self.name, self.version, ','.join(license_to_print),
-                     self.download_location,
-                     self.homepage, self.copyright, exclude, self.comment])
+                row = [self.parent_package_name, self.name, self.version, ','.join(license_to_print),
+                       self.download_location,
+                       self.homepage, self.copyright, exclude, self.comment]
+                for column_name in additional_column:
+                    row.append(self.additional_data.get(column_name, ''))
+                print_items.append(row)
         return print_items
 
 
 def update_license(license_name):
     license_map_list = {"bsd": "bsd-3-clause", "closed": const_other_proprietary_license, "mit-style": "mit-like license",
                         "bsd-style": "bsd-like license"}
 
@@ -238,14 +246,16 @@
         oss.set_license_flags(value)
     elif key == 'package':
         update_package_name(oss, value, nested_pkg_name)
     elif key == 'yocto_package':
         oss.yocto_package = value
     elif key == 'yocto_recipe':
         oss.yocto_recipe = value
+    elif key == 'additional_data':
+        oss.additional_data = value
 
 
 def update_package_name(oss, value, nested_pkg_name):
     if oss.package_name != value:
         if value in nested_pkg_name:
             oss.parent_package_name = nested_pkg_name[value]
             oss.comment = f"Installed Package Name: {value}"
```

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto/_zip_source_works.py` & `fosslight_yocto-3.1.19/src/fosslight_yocto/_zip_source_works.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto/create_oss_report_for_yocto.py` & `fosslight_yocto-3.1.19/src/fosslight_yocto/create_oss_report_for_yocto.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                                        'agpl-3.0': ['agplv3', 'agplv3.0'],
                                        'apache-2.0': ['apachev2'], 'afl-2.0': ['aflv2'], 'afl-1.2': ['aflv1'],
                                        'bsd-new': ['bsd-3-clause'], 'bsd-simplified': ['bsd-3-clause'],
                                        'cddl-1.0': ['cddlv1'], 'epl-1.0': ['eplv1.0'],
                                        'mpl-1.1': ['mplv1.1', 'mplv1'], 'mpl-2.0': ['mpl2.0', 'mplv2'],
                                        'x11': ['mit-x']}
 _skip_to_check_scancode_licenses = ['proprietary-license']
+additional_columns = []
+printall = False  # Print all values in bom.json
 
 
 def read_installed_pkg_file(installed_pkg_names_file):
     global installed_packages_src
     installed_packages_src = []
 
     try:
@@ -115,32 +117,35 @@
             file_content += "]"
         json_obj = get_json_object(file_content)
 
     return json_obj
 
 
 def read_bom_file(bom_file, buildhistory_latest_pkg_list):
-    global bom_pkg_data
+    global bom_pkg_data, additional_columns
 
     json_array = check_json_validate(bom_file)
     bom_pkg_data = {}
 
     for item in json_array:
         oss_item = {"package": "", "license": "", "version": "", "source": "", "oss_name": "", "license_flags": "",
                     "src_path": "", "file_path": ""}
-
-        # Set Data
-        if 'src_path' in item:
-            oss_item['src_path'] = item['src_path']
-        oss_item['version'] = item['pv']
-        recipe_name = item['recipe']
-        # oss_item['package'] = recipe_name
+        additional_column = {}
+        recipe_name = item.get('recipe', '')
         oss_item['oss_name'] = recipe_name
+        oss_item['version'] = item.get('pv', '')
+        oss_item['src_path'] = item.get('src_path', '')
+
+        if printall:
+            for key, value in item.items():
+                if key not in ['src_path', 'pv', 'recipe', 'packages', 'license_flags', 'license', 'pkg_lic', 'src_uri', 'file_path']:
+                    additional_column[key] = value if value else ''
+                    additional_columns.append(key)
 
-        bom_packages = item['packages']
+        bom_packages = item.get('packages', '')
         if recipe_name in buildhistory_latest_pkg_list:
             bom_packages += " " + buildhistory_latest_pkg_list[recipe_name]
             bom_packages = bom_packages.strip()
 
         oss_item['license_flags'] = item['license_flags']
         recipe_license = item['license']
         oss_item['license'] = recipe_license
@@ -164,19 +169,21 @@
             packages = bom_packages.split()
             packages = list(set(packages))
             for package in packages:
                 oss_item['package'] = package
                 oss_item['license'] = recipe_license
                 if bom_pkg_licenses != "":
                     oss_item['license'] = bom_pkg_licenses.get(package, recipe_license)
+                oss_item['additional_data'] = additional_column
                 bom_pkg_data[package] = copy.deepcopy(oss_item)
         # else: # Do not save data for the recipe without packages. (ex- *-native)
         #    bom_pkg_data[recipe_name] = oss_item
     if len(bom_pkg_data) == 0:
         logger.critical("The bom.json file is not json validated.")
+    additional_columns = list(set(additional_columns))
 
 
 def read_file(file_name_with_path, read_as_one_line=False):
     encodings = ["utf-8", "latin-1", "utf-16"]
     read_line = "" if read_as_one_line else []
     read_success = False
     for encoding_option in encodings:
@@ -896,15 +903,15 @@
         cur.close()
         conn.close()
     except Exception:
         pass
 
 
 def main():
-    global installed_packages_src, installed_packages_bin
+    global installed_packages_src, installed_packages_bin, printall
 
     bom_file = "bom.json"
     installed_pkgs = "installed-package-names.txt"
     oss_pkg_yaml_file = ""
     buildhistory_path = ""
     bin_analysis_path = ""
     _print_bin_android = False
@@ -927,14 +934,15 @@
     parser.add_argument('-o', '--output', type=str, required=False)
     parser.add_argument('-f', '--format', type=str, required=False)
     parser.add_argument('-n', '--another', action='store_true', required=False)
     parser.add_argument('-d', '--declared', action='store_true', required=False)
     parser.add_argument('-s', '--source', action='store_true', required=False)
     parser.add_argument('-c', '--complete', action='store_true', required=False)
     parser.add_argument('-e', '--compress', action='store_true', required=False)
+    parser.add_argument('-pr', '--printall', action='store_true', required=False)
 
     args = parser.parse_args()
     if args.help:
         print_help_msg_bom()
     if args.version:
         print_version(_PKG_NAME)
     if args.istalled:
@@ -959,14 +967,16 @@
     if args.source:
         _analyze_source = True
     if args.complete:
         _analyze_source = True
         _analyze_source_all = True
     if args.compress:
         _compress_source_all = True
+    if args.printall:
+        printall = True
 
     # Output file names
     start_time = datetime.now().strftime('%y%m%d_%H%M')
     success, msg, output_path, output_file, output_extension = check_output_format(output_path, file_format)
     output_path = os.path.abspath(output_path)
     if output_file == "":
         if output_extension == '.json':
@@ -1005,15 +1015,15 @@
         declare_license_by_osc_db()
 
     # Source Code Analysis
     if _analyze_source:
         run_source_code_analysis_multiprocessing(_analyze_source_all, output_path, os.path.join(output_path, output_src_analysis_file))
 
     # Write the result to excel file
-    write_result_from_bom(output_file, installed_packages_src, installed_packages_bin, _print_bin_android, output_extension)
+    write_result_from_bom(output_file, installed_packages_src, installed_packages_bin, _print_bin_android, output_extension, additional_columns)
 
     if _compress_source_all:
         try:
             logger.info("* Enable zip option")
             collect_source(installed_packages_src, output_path)
         except Exception as ex:
             logger.error(f"Collecting source code: {ex}")
```

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto/parsing_meta_doubleopen.py` & `fosslight_yocto-3.1.19/src/fosslight_yocto/parsing_meta_doubleopen.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/PKG-INFO` & `fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-yocto
-Version: 3.1.18
+Version: 3.1.19
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.18 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.19 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        [Korean]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.] [Current python package version.] [https://img.shields.io/
 pypi/pyversions/fosslight_yocto] [![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.18/src/fosslight_yocto.egg-info/SOURCES.txt` & `fosslight_yocto-3.1.19/src/fosslight_yocto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

