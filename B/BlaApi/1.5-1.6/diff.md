# Comparing `tmp/BlaApi-1.5.tar.gz` & `tmp/BlaApi-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlaApi-1.5.tar", last modified: Mon Jun 26 11:39:50 2023, max compression
+gzip compressed data, was "BlaApi-1.6.tar", last modified: Sun Jul  9 14:31:05 2023, max compression
```

## Comparing `BlaApi-1.5.tar` & `BlaApi-1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-06-26 11:39:50.371933 BlaApi-1.5/
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-06-26 11:39:50.367933 BlaApi-1.5/BlaApi/
--rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.5/BlaApi/__init__.py
--rw-r--r--   0 muddi     (1000) muddi     (1001)     7825 2023-06-26 11:15:42.000000 BlaApi-1.5/BlaApi/client.py
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-06-26 11:39:50.370932 BlaApi-1.5/BlaApi.egg-info/
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-06-26 11:39:50.000000 BlaApi-1.5/BlaApi.egg-info/SOURCES.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/dependency_links.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)       21 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/requires.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/top_level.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.5/LICENSE
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-06-26 11:39:50.370932 BlaApi-1.5/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.5/README.md
--rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-06-26 11:39:50.371933 BlaApi-1.5/setup.cfg
--rw-r--r--   0 muddi     (1000) muddi     (1001)     3583 2023-06-26 11:39:28.000000 BlaApi-1.5/setup.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-09 14:31:05.427710 BlaApi-1.6/
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-09 14:31:05.422710 BlaApi-1.6/BlaApi/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.6/BlaApi/__init__.py
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     8018 2023-07-09 14:29:50.000000 BlaApi-1.6/BlaApi/client.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-09 14:31:05.425710 BlaApi-1.6/BlaApi.egg-info/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-07-09 14:31:05.000000 BlaApi-1.6/BlaApi.egg-info/SOURCES.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/dependency_links.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       21 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/requires.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/top_level.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.6/LICENSE
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-09 14:31:05.426710 BlaApi-1.6/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.6/README.md
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-07-09 14:31:05.427710 BlaApi-1.6/setup.cfg
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     3583 2023-07-09 14:30:21.000000 BlaApi-1.6/setup.py
```

### Comparing `BlaApi-1.5/BlaApi/client.py` & `BlaApi-1.6/BlaApi/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,20 +39,24 @@
 
         pattern=r'\((\d+[A-Z])\s+[A-Z]+\)'
 
         # seperate student name and section from name and class string.
         students=[]
 
         for student in student_data:
-            string=student.get('studentName') # name, class and section string eg. 'Foo bar (69C M)'
-            match = re.search(pattern, string)
-            student_section=match.group(1)[-1]
-            student_class= match.group(1).strip(student_section) # remove section to get class
-            student_name = re.sub(pattern, '', string).strip()  # Remove the class and section part from the string
+            string=student.get('studentName') # name, class and section string eg. 'Foo bar (69C M)'    
+            pattern=r'\((.*?)\)' # match values inside parenthesis
+            match = re.search(pattern, string) 
+
+            student_name=string.replace(match.group(0), '')
             student_name = student_name.replace('  ', ' ') # remove double spaces from name
+
+            student_class_section = match.group(1).split()[0] # will select '69C' from '69C M'
+            student_section = student_class_section[-1] # will select 'C' from '69C'
+            student_class=student_class_section.strip(student_section)# student_class=student_class_section.replace(student_section, '')
             students.append(
                 {
                 'student_name': student_name,
                 'section': student_section,
                 'class': student_class,
                 'student_id': student.get('id'),
                 'gr_number': student.get('grNo'),
```

### Comparing `BlaApi-1.5/BlaApi.egg-info/PKG-INFO` & `BlaApi-1.6/BlaApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.5
+Version: 1.6
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.5/LICENSE` & `BlaApi-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BlaApi-1.5/PKG-INFO` & `BlaApi-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.5
+Version: 1.6
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.5/README.md` & `BlaApi-1.6/README.md`

 * *Files identical despite different names*

### Comparing `BlaApi-1.5/setup.py` & `BlaApi-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'BlaApi'
 DESCRIPTION = 'A wrapper for the beacon light api.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'deaddogfuneral@gmail.com'
 AUTHOR = 'Omer-Farooqui'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.5'
+VERSION = '1.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
      'httpx', 'fake_useragent',
 ]
 
 # What packages are optional?
```

