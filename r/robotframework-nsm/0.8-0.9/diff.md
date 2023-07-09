# Comparing `tmp/robotframework-nsm-0.8.tar.gz` & `tmp/robotframework-nsm-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robotframework-nsm-0.8.tar", last modified: Sun May 31 09:41:01 2020, max compression
+gzip compressed data, was "dist/robotframework-nsm-0.9.tar", last modified: Wed Jun  3 16:36:01 2020, max compression
```

## Comparing `robotframework-nsm-0.8.tar` & `robotframework-nsm-0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2020-05-31 09:41:01.000000 robotframework-nsm-0.8/
-drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2020-05-31 09:41:01.000000 robotframework-nsm-0.8/nsm/
--rw-rw-r--   0 adam      (1000) adam      (1000)       59 2020-04-29 22:21:02.000000 robotframework-nsm-0.8/nsm/__init__.py
--rw-rw-r--   0 adam      (1000) adam      (1000)       26 2020-04-29 22:21:02.000000 robotframework-nsm-0.8/nsm/__main__.py
--rw-rw-r--   0 adam      (1000) adam      (1000)    30329 2020-05-31 09:38:42.000000 robotframework-nsm-0.8/nsm/nsm.py
--rw-rw-r--   0 adam      (1000) adam      (1000)       62 2020-04-29 22:21:02.000000 robotframework-nsm-0.8/setup.cfg
--rw-rw-r--   0 adam      (1000) adam      (1000)      865 2020-05-31 09:31:06.000000 robotframework-nsm-0.8/setup.py
--rw-rw-r--   0 adam      (1000) adam      (1000)      757 2020-05-31 09:41:01.000000 robotframework-nsm-0.8/PKG-INFO
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2020-06-03 16:36:01.000000 robotframework-nsm-0.9/
+drwxrwxr-x   0 adam      (1000) adam      (1000)        0 2020-06-03 16:36:01.000000 robotframework-nsm-0.9/nsm/
+-rw-rw-r--   0 adam      (1000) adam      (1000)       59 2020-04-29 22:21:02.000000 robotframework-nsm-0.9/nsm/__init__.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)       26 2020-04-29 22:21:02.000000 robotframework-nsm-0.9/nsm/__main__.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)    31002 2020-06-03 14:14:50.000000 robotframework-nsm-0.9/nsm/nsm.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)       62 2020-04-29 22:21:02.000000 robotframework-nsm-0.9/setup.cfg
+-rw-rw-r--   0 adam      (1000) adam      (1000)      865 2020-06-03 15:36:06.000000 robotframework-nsm-0.9/setup.py
+-rw-rw-r--   0 adam      (1000) adam      (1000)      757 2020-06-03 16:36:01.000000 robotframework-nsm-0.9/PKG-INFO
```

### Comparing `robotframework-nsm-0.8/nsm/nsm.py` & `robotframework-nsm-0.9/nsm/nsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -837,14 +837,16 @@
 ${DBPort}  3306
 ${DBFile}  w3schools.sql
 ${Furl}    https://raw.githubusercontent.com/AndrejPHP/w3schools-database/master/w3schools.sql
 ${gr}      /etc/apt/sources.list.d/google-chrome.list
 ${grep}    http://mirror.cs.uchicago.edu/google-chrome/pool/main/g/google-chrome-stable/
 #${chrome_version}  False
 ${chrome_version}  google-chrome-stable_81.0.4044.138-1_amd64.deb
+${chd81}  http://launchpadlibrarian.net/478575933/chromium-chromedriver_81.0.4044.138-0ubuntu0.18.04.1_amd64.deb
+
 
 *** Settings ***
 Library  Impansible
 library  Collections
 library  OperatingSystem
 library  String
 #Library  DatabaseLibrary
@@ -914,19 +916,28 @@
 	Should Contain  ${w}  google-chrome-stable
 
 The Chromedriver should be installed if needed
 	[Timeout]    600
 	${x}=  Convert To Lower Case  ${BROWSER}
 	${x}=  Run Keyword and return status  Should Contain  ${x}  chrome
 	Return from keyword if  not ${x}
-	${x}=	apt    localhost   package=chromium-chromedriver   state=present
-        ${x}=	get from dictionary  ${x}   invocation
-        ${y}=	get from dictionary  ${x}   module_args
-        ${s}=	get from dictionary  ${y}   state
-        Should be Equal  ${s}  present
+        ${x}=   package facts  localhost
+        ${x}=   get from dictionary  ${x}   ansible_facts
+        ${x}=   get from dictionary  ${x}   packages
+        ${x}=   get from dictionary  ${x}   google-chrome-stable
+        ${x}=   get from dictionary  ${x}[0]   version
+        ${xs}=  run keyword and return status  should start with  ${x}  81
+        ${x}=   run keyword if  not ${xs}  apt    localhost   package=chromium-chromedriver state=present
+        ${x}=   run keyword if  ${xs}  apt  localhost  deb="${chd81}"
+        #log to console   ${x}
+	#${x}=	apt    localhost   package=chromium-chromedriver   state=present
+        #${x}=	get from dictionary  ${x}   invocation
+        #${y}=	get from dictionary  ${x}   module_args
+        #${s}=	get from dictionary  ${y}   state
+        #Should be Equal  ${s}  present
 	${w}=	Run	which chromedriver
 	Should Contain  ${w}  chromedriver
 
 The MySQL server should be installed
 	[Timeout]    600
 	${x}=	apt    localhost   package=mysql-server   state=present
 	${x}=	get from dictionary  ${x}   invocation
```

### Comparing `robotframework-nsm-0.8/setup.py` & `robotframework-nsm-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'robotframework-nsm',
   packages = ['nsm'],
-  version = '0.8',
+  version = '0.9',
   license='MIT',
   description = 'Robotframework library for NSM',
   author = 'Adam Przybyla',
   author_email = 'adam.przybyla@gmail.com',
   url = 'https://github.com/AdamPrzybyla/robotframework-nsm',
-  download_url = 'https://github.com/AdamPrzybyla/robotframework-nsm/archive/v_08.tar.gz',
+  download_url = 'https://github.com/AdamPrzybyla/robotframework-nsm/archive/v_09.tar.gz',
   keywords = ['robotframework', 'nsm', 'automatisation', 'tests'],
   install_requires=[
           'robotframework',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Topic :: Software Development :: Build Tools',
```

### Comparing `robotframework-nsm-0.8/PKG-INFO` & `robotframework-nsm-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: robotframework-nsm
-Version: 0.8
+Version: 0.9
 Summary: Robotframework library for NSM
 Home-page: https://github.com/AdamPrzybyla/robotframework-nsm
 Author: Adam Przybyla
 Author-email: adam.przybyla@gmail.com
 License: MIT
-Download-URL: https://github.com/AdamPrzybyla/robotframework-nsm/archive/v_08.tar.gz
+Download-URL: https://github.com/AdamPrzybyla/robotframework-nsm/archive/v_09.tar.gz
 Description: UNKNOWN
 Keywords: robotframework,nsm,automatisation,tests
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

