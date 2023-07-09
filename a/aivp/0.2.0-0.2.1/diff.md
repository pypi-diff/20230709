# Comparing `tmp/aivp-0.2.0.tar.gz` & `tmp/aivp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aivp-0.2.0.tar", last modified: Sat Jul  8 22:37:15 2023, max compression
+gzip compressed data, was "aivp-0.2.1.tar", last modified: Sun Jul  9 16:37:10 2023, max compression
```

## Comparing `aivp-0.2.0.tar` & `aivp-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 calebcosta   (501) staff       (20)        0 2023-07-08 22:37:15.853559 aivp-0.2.0/
--rw-r--r--   0 calebcosta   (501) staff       (20)     1036 2023-07-08 22:13:50.000000 aivp-0.2.0/LICENSE
--rw-r--r--   0 calebcosta   (501) staff       (20)      517 2023-07-08 22:37:15.853433 aivp-0.2.0/PKG-INFO
--rw-r--r--   0 calebcosta   (501) staff       (20)       35 2023-07-08 22:01:25.000000 aivp-0.2.0/README.md
-drwxr-xr-x   0 calebcosta   (501) staff       (20)        0 2023-07-08 22:37:15.852606 aivp-0.2.0/aivp/
--rw-r--r--   0 calebcosta   (501) staff       (20)       37 2023-07-08 22:12:49.000000 aivp-0.2.0/aivp/__init__.py
--rw-r--r--   0 calebcosta   (501) staff       (20)     2215 2023-07-08 22:12:23.000000 aivp-0.2.0/aivp/aivp.py
-drwxr-xr-x   0 calebcosta   (501) staff       (20)        0 2023-07-08 22:37:15.853261 aivp-0.2.0/aivp.egg-info/
--rw-r--r--   0 calebcosta   (501) staff       (20)      517 2023-07-08 22:37:15.000000 aivp-0.2.0/aivp.egg-info/PKG-INFO
--rw-r--r--   0 calebcosta   (501) staff       (20)      195 2023-07-08 22:37:15.000000 aivp-0.2.0/aivp.egg-info/SOURCES.txt
--rw-r--r--   0 calebcosta   (501) staff       (20)        1 2023-07-08 22:37:15.000000 aivp-0.2.0/aivp.egg-info/dependency_links.txt
--rw-r--r--   0 calebcosta   (501) staff       (20)       45 2023-07-08 22:37:15.000000 aivp-0.2.0/aivp.egg-info/requires.txt
--rw-r--r--   0 calebcosta   (501) staff       (20)        5 2023-07-08 22:37:15.000000 aivp-0.2.0/aivp.egg-info/top_level.txt
--rw-r--r--   0 calebcosta   (501) staff       (20)       38 2023-07-08 22:37:15.853604 aivp-0.2.0/setup.cfg
--rw-r--r--   0 calebcosta   (501) staff       (20)      806 2023-07-08 22:35:13.000000 aivp-0.2.0/setup.py
+drwxr-xr-x   0 calebcosta   (501) staff       (20)        0 2023-07-09 16:37:10.963965 aivp-0.2.1/
+-rw-r--r--   0 calebcosta   (501) staff       (20)     1036 2023-07-08 22:13:50.000000 aivp-0.2.1/LICENSE
+-rw-r--r--   0 calebcosta   (501) staff       (20)      517 2023-07-09 16:37:10.963835 aivp-0.2.1/PKG-INFO
+-rw-r--r--   0 calebcosta   (501) staff       (20)       35 2023-07-08 22:01:25.000000 aivp-0.2.1/README.md
+drwxr-xr-x   0 calebcosta   (501) staff       (20)        0 2023-07-09 16:37:10.962937 aivp-0.2.1/aivp/
+-rw-r--r--   0 calebcosta   (501) staff       (20)       37 2023-07-08 22:12:49.000000 aivp-0.2.1/aivp/__init__.py
+-rw-r--r--   0 calebcosta   (501) staff       (20)     2170 2023-07-09 16:36:03.000000 aivp-0.2.1/aivp/aivp.py
+drwxr-xr-x   0 calebcosta   (501) staff       (20)        0 2023-07-09 16:37:10.963662 aivp-0.2.1/aivp.egg-info/
+-rw-r--r--   0 calebcosta   (501) staff       (20)      517 2023-07-09 16:37:10.000000 aivp-0.2.1/aivp.egg-info/PKG-INFO
+-rw-r--r--   0 calebcosta   (501) staff       (20)      195 2023-07-09 16:37:10.000000 aivp-0.2.1/aivp.egg-info/SOURCES.txt
+-rw-r--r--   0 calebcosta   (501) staff       (20)        1 2023-07-09 16:37:10.000000 aivp-0.2.1/aivp.egg-info/dependency_links.txt
+-rw-r--r--   0 calebcosta   (501) staff       (20)       45 2023-07-09 16:37:10.000000 aivp-0.2.1/aivp.egg-info/requires.txt
+-rw-r--r--   0 calebcosta   (501) staff       (20)        5 2023-07-09 16:37:10.000000 aivp-0.2.1/aivp.egg-info/top_level.txt
+-rw-r--r--   0 calebcosta   (501) staff       (20)       38 2023-07-09 16:37:10.964003 aivp-0.2.1/setup.cfg
+-rw-r--r--   0 calebcosta   (501) staff       (20)      806 2023-07-09 16:36:50.000000 aivp-0.2.1/setup.py
```

### Comparing `aivp-0.2.0/LICENSE` & `aivp-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aivp-0.2.0/PKG-INFO` & `aivp-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aivp
-Version: 0.2.0
+Version: 0.2.1
 Summary: AI and Voice Processing Library
 Home-page: https://github.com/removeableox/aivp
 Author: Caleb Costa
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aivp-0.2.0/aivp/aivp.py` & `aivp-0.2.1/aivp/aivp.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def speak(self, text):
         if text:
             tts = gTTS(text=text, lang="en")
             tts.save("output.mp3")
             playsound.playsound("output.mp3")
             os.remove("output.mp3")
         else:
-            self.speak("There was no response from the API.")
+            pass
 
 class Listener:
     def __init__(self):
         # sets the default minimum of volume for the microphone to pick up input
         self.power_min = sr.Recognizer().energy_threshold = 5000
         self.mic = sr.Microphone()
     def record(self, source, duration):
```

### Comparing `aivp-0.2.0/aivp.egg-info/PKG-INFO` & `aivp-0.2.1/aivp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aivp
-Version: 0.2.0
+Version: 0.2.1
 Summary: AI and Voice Processing Library
 Home-page: https://github.com/removeableox/aivp
 Author: Caleb Costa
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aivp-0.2.0/setup.py` & `aivp-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='aivp',
-    version='0.2.0',
+    version='0.2.1',
     description='AI and Voice Processing Library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['aivp'],
     install_requires=[
         'SpeechRecognition',
         'gTTS',
```

