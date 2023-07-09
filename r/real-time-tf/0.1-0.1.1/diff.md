# Comparing `tmp/real-time-tf-0.1.tar.gz` & `tmp/real-time-tf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real-time-tf-0.1.tar", last modified: Sun Jul  9 15:10:26 2023, max compression
+gzip compressed data, was "real-time-tf-0.1.1.tar", last modified: Sun Jul  9 15:14:39 2023, max compression
```

## Comparing `real-time-tf-0.1.tar` & `real-time-tf-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:10:26.287398 real-time-tf-0.1/
--rw-r--r--   0 diganta.eth   (501) staff       (20)     1514 2023-07-09 15:08:42.000000 real-time-tf-0.1/LICENSE
--rw-r--r--   0 diganta.eth   (501) staff       (20)      344 2023-07-09 15:10:26.287517 real-time-tf-0.1/PKG-INFO
--rw-r--r--   0 diganta.eth   (501) staff       (20)     1317 2023-07-09 14:31:17.000000 real-time-tf-0.1/README.md
-drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:10:26.285845 real-time-tf-0.1/real_time_tf.egg-info/
--rw-r--r--   0 diganta.eth   (501) staff       (20)      344 2023-07-09 15:10:26.000000 real-time-tf-0.1/real_time_tf.egg-info/PKG-INFO
--rw-r--r--   0 diganta.eth   (501) staff       (20)      360 2023-07-09 15:10:26.000000 real-time-tf-0.1/real_time_tf.egg-info/SOURCES.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)        1 2023-07-09 15:10:26.000000 real-time-tf-0.1/real_time_tf.egg-info/dependency_links.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)       61 2023-07-09 15:10:26.000000 real-time-tf-0.1/real_time_tf.egg-info/entry_points.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)       29 2023-07-09 15:10:26.000000 real-time-tf-0.1/real_time_tf.egg-info/requires.txt
--rw-r--r--   0 diganta.eth   (501) staff       (20)       12 2023-07-09 15:10:26.000000 real-time-tf-0.1/real_time_tf.egg-info/top_level.txt
-drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:10:26.287007 real-time-tf-0.1/realtime_tf/
--rw-r--r--   0 diganta.eth   (501) staff       (20)       33 2023-07-09 15:02:30.000000 real-time-tf-0.1/realtime_tf/__init__.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)       58 2023-07-09 14:24:52.000000 real-time-tf-0.1/realtime_tf/constants.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)     5392 2023-07-09 15:03:05.000000 real-time-tf-0.1/realtime_tf/realtime_tf.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)     3013 2023-07-09 14:24:25.000000 real-time-tf-0.1/realtime_tf/time_frequency.py
--rw-r--r--   0 diganta.eth   (501) staff       (20)       79 2023-07-09 15:10:26.287879 real-time-tf-0.1/setup.cfg
--rw-r--r--   0 diganta.eth   (501) staff       (20)      893 2023-07-09 11:25:57.000000 real-time-tf-0.1/setup.py
+drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:14:39.001421 real-time-tf-0.1.1/
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1514 2023-07-09 15:08:42.000000 real-time-tf-0.1.1/LICENSE
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1704 2023-07-09 15:14:39.001534 real-time-tf-0.1.1/PKG-INFO
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1317 2023-07-09 14:31:17.000000 real-time-tf-0.1.1/README.md
+drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:14:38.999666 real-time-tf-0.1.1/real_time_tf.egg-info/
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1704 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/PKG-INFO
+-rw-r--r--   0 diganta.eth   (501) staff       (20)      360 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/SOURCES.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)        1 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/dependency_links.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       61 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/entry_points.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       29 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/requires.txt
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       12 2023-07-09 15:14:38.000000 real-time-tf-0.1.1/real_time_tf.egg-info/top_level.txt
+drwxr-xr-x   0 diganta.eth   (501) staff       (20)        0 2023-07-09 15:14:39.001024 real-time-tf-0.1.1/realtime_tf/
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       33 2023-07-09 15:02:30.000000 real-time-tf-0.1.1/realtime_tf/__init__.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       58 2023-07-09 14:24:52.000000 real-time-tf-0.1.1/realtime_tf/constants.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     5392 2023-07-09 15:03:05.000000 real-time-tf-0.1.1/realtime_tf/realtime_tf.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     3013 2023-07-09 14:24:25.000000 real-time-tf-0.1.1/realtime_tf/time_frequency.py
+-rw-r--r--   0 diganta.eth   (501) staff       (20)       79 2023-07-09 15:14:39.001930 real-time-tf-0.1.1/setup.cfg
+-rw-r--r--   0 diganta.eth   (501) staff       (20)     1151 2023-07-09 15:14:36.000000 real-time-tf-0.1.1/setup.py
```

### Comparing `real-time-tf-0.1/LICENSE` & `real-time-tf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `real-time-tf-0.1/README.md` & `real-time-tf-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `real-time-tf-0.1/realtime_tf/realtime_tf.py` & `real-time-tf-0.1.1/realtime_tf/realtime_tf.py`

 * *Files identical despite different names*

### Comparing `real-time-tf-0.1/realtime_tf/time_frequency.py` & `real-time-tf-0.1.1/realtime_tf/time_frequency.py`

 * *Files identical despite different names*

### Comparing `real-time-tf-0.1/setup.py` & `real-time-tf-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup, find_packages
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="real-time-tf",
-    version="0.1",
+    version="0.1.1",
     description="Real time time frequency plotting of EEG data from the Muse headset.",
     keywords="muse time-frequency eeg fft neuroscience",
     url="https://github.com/dxganta/real-time-tf",
     author="Diganta Kalita",
     author_email="digantakalita.ai@gmail.com",
     license="BSD (3-clause)",
     packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'realtime_tf = realtime_tf.realtime_tf:main',
         ],
     },
     install_requires=[
         'pylsl',
```

