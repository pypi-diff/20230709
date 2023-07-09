# Comparing `tmp/objdictgen-3.3.tar.gz` & `tmp/objdictgen-3.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objdictgen-3.3.tar", last modified: Sat Apr 15 17:06:25 2023, max compression
+gzip compressed data, was "objdictgen-3.3.post1.tar", last modified: Sun Jul  9 09:24:42 2023, max compression
```

## Comparing `objdictgen-3.3.tar` & `objdictgen-3.3.post1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.614698 objdictgen-3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-04-15 17:06:13.000000 objdictgen-3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-15 17:06:25.614698 objdictgen-3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-15 17:06:13.000000 objdictgen-3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-15 17:06:13.000000 objdictgen-3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 17:06:25.614698 objdictgen-3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-15 17:06:13.000000 objdictgen-3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.606698 objdictgen-3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.606698 objdictgen-3.3/src/objdictgen/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.610698 objdictgen-3.3/src/objdictgen/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-302.prf
--rw-r--r--   0 runner    (1001) docker     (123)    28344 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-401.prf
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-402.prf
--rw-r--r--   0 runner    (1001) docker     (123)    96871 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-404.prf
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-406.prf
--rw-r--r--   0 runner    (1001) docker     (123)   133352 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-408.prf
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-410.prf
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-418.prf
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/config/DS-419.prf
--rw-r--r--   0 runner    (1001) docker     (123)    39039 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/eds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/gen_cfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    48127 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/jsonod.py
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/nodelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    47919 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/nodemanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.610698 objdictgen-3.3/src/objdictgen/nosis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/nosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24885 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/nosis/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/nosis/xtoy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.610698 objdictgen-3.3/src/objdictgen/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/schema/od.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.610698 objdictgen-3.3/src/objdictgen/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69984 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/commondialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/networkedit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/networkeditortemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/nodeeditortemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    27274 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/objdictedit.py
--rw-r--r--   0 runner    (1001) docker     (123)    42378 2023-04-15 17:06:13.000000 objdictgen-3.3/src/objdictgen/ui/subindextable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.610698 objdictgen-3.3/src/objdictgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-15 17:06:25.000000 objdictgen-3.3/src/objdictgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-15 17:06:25.000000 objdictgen-3.3/src/objdictgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:06:25.000000 objdictgen-3.3/src/objdictgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-15 17:06:25.000000 objdictgen-3.3/src/objdictgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-15 17:06:25.000000 objdictgen-3.3/src/objdictgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 17:06:25.000000 objdictgen-3.3/src/objdictgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:06:25.614698 objdictgen-3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-15 17:06:13.000000 objdictgen-3.3/tests/test_knownfailures.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-15 17:06:13.000000 objdictgen-3.3/tests/test_nodelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-15 17:06:13.000000 objdictgen-3.3/tests/test_nodemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-15 17:06:13.000000 objdictgen-3.3/tests/test_objdictgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-04-15 17:06:13.000000 objdictgen-3.3/tests/test_odcompare.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-15 17:06:13.000000 objdictgen-3.3/tests/test_odg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.252383 objdictgen-3.3.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.252383 objdictgen-3.3.post1/src/objdictgen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/src/objdictgen/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-302.prf
+-rw-r--r--   0 runner    (1001) docker     (123)    28344 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-401.prf
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-402.prf
+-rw-r--r--   0 runner    (1001) docker     (123)    96871 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-404.prf
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-406.prf
+-rw-r--r--   0 runner    (1001) docker     (123)   133352 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-408.prf
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-410.prf
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-418.prf
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/config/DS-419.prf
+-rw-r--r--   0 runner    (1001) docker     (123)    39039 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/eds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/gen_cfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48127 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/jsonod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/nodelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47919 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/nodemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/src/objdictgen/nosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/nosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24885 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/nosis/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/nosis/xtoy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/src/objdictgen/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/schema/od.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/src/objdictgen/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69984 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/commondialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/networkedit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/networkeditortemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/nodeeditortemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27274 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/objdictedit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42378 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/src/objdictgen/ui/subindextable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.252383 objdictgen-3.3.post1/src/objdictgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-09 09:24:42.000000 objdictgen-3.3.post1/src/objdictgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-09 09:24:42.000000 objdictgen-3.3.post1/src/objdictgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:24:42.000000 objdictgen-3.3.post1/src/objdictgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 09:24:42.000000 objdictgen-3.3.post1/src/objdictgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-09 09:24:42.000000 objdictgen-3.3.post1/src/objdictgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 09:24:42.000000 objdictgen-3.3.post1/src/objdictgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:24:42.256383 objdictgen-3.3.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/tests/test_knownfailures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/tests/test_nodelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/tests/test_nodemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/tests/test_objdictgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/tests/test_odcompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-09 09:24:31.000000 objdictgen-3.3.post1/tests/test_odg.py
```

### Comparing `objdictgen-3.3/LICENSE` & `objdictgen-3.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/PKG-INFO` & `objdictgen-3.3.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objdictgen
-Version: 3.3
+Version: 3.3.post1
 Summary: CanFestival object dictionary tools
 Home-page: https://github.com/laerdal-svg/python-objdictgen
 Author: Svein Seldal
 Author-email: sveinse@seldal.com
 Keywords: build,development,canfestival,canopen,objdictgen
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -34,21 +34,21 @@
 This is python tools for working with Object Dictionary (OD) files for
 the CanFestival communication library. CanFestival is an open source
 implementation of the [CANopen](https://www.can-cia.org/canopen/)
 communication protocol.
 
 This repo is located:
 
-> https://github.com/laerdal-svg/python-objdictgen
+> https://github.com/laerdal/python-objdictgen
 
 objdictgen includes tools to generate c code that works in tandem with a
 canfestival library. This tool has been built to work together with the
 Laerdal Medical fork for the canfestival library:
 
-> https://github.com/laerdal-svg/canfestival-laerdal
+> https://github.com/laerdal/canfestival-laerdal
 
 objdictgen is a tool to parse, view and manipulate files containing object
 dictionary (OD). An object dictionary is entries with data and configuration
 in CANopen devices. The `odg` executable is installed. It supports
 reading and writing OD files in `.json` format, in legacy XML `.od` and `.eds`
 files. It can generate c code for use with the canfestival library.
 
@@ -64,15 +64,15 @@
 
 The original objdictedit and objdictgen tool were written in legacy python2 and
 and this is a port to python3. The package still remains compatible with
 python2, as python2 is required for running the UI tools.
 
 This tool is a fork from upstream canfestival-3-asc repo:
 
-> https://github.com/laerdal-svg/canfestival-3-asc
+> https://github.com/laerdal/canfestival-3-asc
 
 
 ## Install
 
 To install into a virtual environment `venv`. Check out this repo and go to
 the top in a command-prompt (here assuming Windows and git bash):
 
@@ -90,17 +90,17 @@
 for Python 2.7. Download and install both.
 
    * https://www.python.org/downloads/release/python-2716/
    * https://sourceforge.net/projects/wxpython/files/wxPython/2.8.12.1/
 
 To setup the virtual environment run (assuming git bash):
 
-    $ py.exe -2 -mvirtualenv --system-site-packages venv
-    $ venv/Scripts/python -mpip install --upgrade pip wheel setuptools
-    $ venv/Scripts/pip install .
+    $ py.exe -2 -mvirtualenv --system-site-packages venv-27
+    $ venv-27/Scripts/python -mpip install --upgrade pip wheel setuptools
+    $ venv-27/Scripts/pip install .
 
 NOTE: The `py.exe` tool is only shipped with recent Python 3.
 
 
 ## `odg` command-line tool
 
 `odg` is a command-line tool which is installed when the python package
@@ -171,8 +171,8 @@
 Objdictgen has been based on the python tool included in CanFestival. This
 original work from CanFestival is:
 
     Copyright (C): Edouard TISSERANT, Francis DUPIN and Laurent BESSARD
 
 The Python 3 port and tool improvements have been implemented under
 
-    Copyright (C) 2022 Svein Seldal, Laerdal Medical AS
+    Copyright (C) 2022-2023 Svein Seldal, Laerdal Medical AS
```

### Comparing `objdictgen-3.3/README.md` & `objdictgen-3.3.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 This is python tools for working with Object Dictionary (OD) files for
 the CanFestival communication library. CanFestival is an open source
 implementation of the [CANopen](https://www.can-cia.org/canopen/)
 communication protocol.
 
 This repo is located:
 
-> https://github.com/laerdal-svg/python-objdictgen
+> https://github.com/laerdal/python-objdictgen
 
 objdictgen includes tools to generate c code that works in tandem with a
 canfestival library. This tool has been built to work together with the
 Laerdal Medical fork for the canfestival library:
 
-> https://github.com/laerdal-svg/canfestival-laerdal
+> https://github.com/laerdal/canfestival-laerdal
 
 objdictgen is a tool to parse, view and manipulate files containing object
 dictionary (OD). An object dictionary is entries with data and configuration
 in CANopen devices. The `odg` executable is installed. It supports
 reading and writing OD files in `.json` format, in legacy XML `.od` and `.eds`
 files. It can generate c code for use with the canfestival library.
 
@@ -33,15 +33,15 @@
 
 The original objdictedit and objdictgen tool were written in legacy python2 and
 and this is a port to python3. The package still remains compatible with
 python2, as python2 is required for running the UI tools.
 
 This tool is a fork from upstream canfestival-3-asc repo:
 
-> https://github.com/laerdal-svg/canfestival-3-asc
+> https://github.com/laerdal/canfestival-3-asc
 
 
 ## Install
 
 To install into a virtual environment `venv`. Check out this repo and go to
 the top in a command-prompt (here assuming Windows and git bash):
 
@@ -59,17 +59,17 @@
 for Python 2.7. Download and install both.
 
    * https://www.python.org/downloads/release/python-2716/
    * https://sourceforge.net/projects/wxpython/files/wxPython/2.8.12.1/
 
 To setup the virtual environment run (assuming git bash):
 
-    $ py.exe -2 -mvirtualenv --system-site-packages venv
-    $ venv/Scripts/python -mpip install --upgrade pip wheel setuptools
-    $ venv/Scripts/pip install .
+    $ py.exe -2 -mvirtualenv --system-site-packages venv-27
+    $ venv-27/Scripts/python -mpip install --upgrade pip wheel setuptools
+    $ venv-27/Scripts/pip install .
 
 NOTE: The `py.exe` tool is only shipped with recent Python 3.
 
 
 ## `odg` command-line tool
 
 `odg` is a command-line tool which is installed when the python package
@@ -140,8 +140,8 @@
 Objdictgen has been based on the python tool included in CanFestival. This
 original work from CanFestival is:
 
     Copyright (C): Edouard TISSERANT, Francis DUPIN and Laurent BESSARD
 
 The Python 3 port and tool improvements have been implemented under
 
-    Copyright (C) 2022 Svein Seldal, Laerdal Medical AS
+    Copyright (C) 2022-2023 Svein Seldal, Laerdal Medical AS
```

### Comparing `objdictgen-3.3/setup.py` & `objdictgen-3.3.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='3.3',  # Required
+    version='3.3.post1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='CanFestival object dictionary tools',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `objdictgen-3.3/src/objdictgen/__init__.py` & `objdictgen-3.3.post1/src/objdictgen/__init__.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/__main__.py` & `objdictgen-3.3.post1/src/objdictgen/__main__.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-302.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-302.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-401.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-401.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-402.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-402.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-404.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-404.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-406.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-406.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-408.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-408.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-410.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-410.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-418.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-418.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/config/DS-419.prf` & `objdictgen-3.3.post1/src/objdictgen/config/DS-419.prf`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/eds_utils.py` & `objdictgen-3.3.post1/src/objdictgen/eds_utils.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/gen_cfile.py` & `objdictgen-3.3.post1/src/objdictgen/gen_cfile.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/jsonod.py` & `objdictgen-3.3.post1/src/objdictgen/jsonod.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/maps.py` & `objdictgen-3.3.post1/src/objdictgen/maps.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/node.py` & `objdictgen-3.3.post1/src/objdictgen/node.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/nodelist.py` & `objdictgen-3.3.post1/src/objdictgen/nodelist.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/nodemanager.py` & `objdictgen-3.3.post1/src/objdictgen/nodemanager.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/nosis/pickle.py` & `objdictgen-3.3.post1/src/objdictgen/nosis/pickle.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/nosis/xtoy.py` & `objdictgen-3.3.post1/src/objdictgen/nosis/xtoy.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/schema/od.schema.json` & `objdictgen-3.3.post1/src/objdictgen/schema/od.schema.json`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/ui/commondialogs.py` & `objdictgen-3.3.post1/src/objdictgen/ui/commondialogs.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/ui/exception.py` & `objdictgen-3.3.post1/src/objdictgen/ui/exception.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/ui/networkedit.py` & `objdictgen-3.3.post1/src/objdictgen/ui/networkedit.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/ui/networkeditortemplate.py` & `objdictgen-3.3.post1/src/objdictgen/ui/networkeditortemplate.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/ui/nodeeditortemplate.py` & `objdictgen-3.3.post1/src/objdictgen/ui/nodeeditortemplate.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/ui/objdictedit.py` & `objdictgen-3.3.post1/src/objdictgen/ui/objdictedit.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen/ui/subindextable.py` & `objdictgen-3.3.post1/src/objdictgen/ui/subindextable.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/src/objdictgen.egg-info/PKG-INFO` & `objdictgen-3.3.post1/src/objdictgen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objdictgen
-Version: 3.3
+Version: 3.3.post1
 Summary: CanFestival object dictionary tools
 Home-page: https://github.com/laerdal-svg/python-objdictgen
 Author: Svein Seldal
 Author-email: sveinse@seldal.com
 Keywords: build,development,canfestival,canopen,objdictgen
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -34,21 +34,21 @@
 This is python tools for working with Object Dictionary (OD) files for
 the CanFestival communication library. CanFestival is an open source
 implementation of the [CANopen](https://www.can-cia.org/canopen/)
 communication protocol.
 
 This repo is located:
 
-> https://github.com/laerdal-svg/python-objdictgen
+> https://github.com/laerdal/python-objdictgen
 
 objdictgen includes tools to generate c code that works in tandem with a
 canfestival library. This tool has been built to work together with the
 Laerdal Medical fork for the canfestival library:
 
-> https://github.com/laerdal-svg/canfestival-laerdal
+> https://github.com/laerdal/canfestival-laerdal
 
 objdictgen is a tool to parse, view and manipulate files containing object
 dictionary (OD). An object dictionary is entries with data and configuration
 in CANopen devices. The `odg` executable is installed. It supports
 reading and writing OD files in `.json` format, in legacy XML `.od` and `.eds`
 files. It can generate c code for use with the canfestival library.
 
@@ -64,15 +64,15 @@
 
 The original objdictedit and objdictgen tool were written in legacy python2 and
 and this is a port to python3. The package still remains compatible with
 python2, as python2 is required for running the UI tools.
 
 This tool is a fork from upstream canfestival-3-asc repo:
 
-> https://github.com/laerdal-svg/canfestival-3-asc
+> https://github.com/laerdal/canfestival-3-asc
 
 
 ## Install
 
 To install into a virtual environment `venv`. Check out this repo and go to
 the top in a command-prompt (here assuming Windows and git bash):
 
@@ -90,17 +90,17 @@
 for Python 2.7. Download and install both.
 
    * https://www.python.org/downloads/release/python-2716/
    * https://sourceforge.net/projects/wxpython/files/wxPython/2.8.12.1/
 
 To setup the virtual environment run (assuming git bash):
 
-    $ py.exe -2 -mvirtualenv --system-site-packages venv
-    $ venv/Scripts/python -mpip install --upgrade pip wheel setuptools
-    $ venv/Scripts/pip install .
+    $ py.exe -2 -mvirtualenv --system-site-packages venv-27
+    $ venv-27/Scripts/python -mpip install --upgrade pip wheel setuptools
+    $ venv-27/Scripts/pip install .
 
 NOTE: The `py.exe` tool is only shipped with recent Python 3.
 
 
 ## `odg` command-line tool
 
 `odg` is a command-line tool which is installed when the python package
@@ -171,8 +171,8 @@
 Objdictgen has been based on the python tool included in CanFestival. This
 original work from CanFestival is:
 
     Copyright (C): Edouard TISSERANT, Francis DUPIN and Laurent BESSARD
 
 The Python 3 port and tool improvements have been implemented under
 
-    Copyright (C) 2022 Svein Seldal, Laerdal Medical AS
+    Copyright (C) 2022-2023 Svein Seldal, Laerdal Medical AS
```

### Comparing `objdictgen-3.3/src/objdictgen.egg-info/SOURCES.txt` & `objdictgen-3.3.post1/src/objdictgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/tests/test_knownfailures.py` & `objdictgen-3.3.post1/tests/test_knownfailures.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/tests/test_nodemanager.py` & `objdictgen-3.3.post1/tests/test_nodemanager.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/tests/test_objdictgen.py` & `objdictgen-3.3.post1/tests/test_objdictgen.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/tests/test_odcompare.py` & `objdictgen-3.3.post1/tests/test_odcompare.py`

 * *Files identical despite different names*

### Comparing `objdictgen-3.3/tests/test_odg.py` & `objdictgen-3.3.post1/tests/test_odg.py`

 * *Files identical despite different names*

