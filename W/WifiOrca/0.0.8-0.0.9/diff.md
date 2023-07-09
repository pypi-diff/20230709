# Comparing `tmp/WifiOrca-0.0.8.tar.gz` & `tmp/WifiOrca-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WifiOrca-0.0.8.tar", last modified: Sun Jul  9 11:28:39 2023, max compression
+gzip compressed data, was "WifiOrca-0.0.9.tar", last modified: Sun Jul  9 11:31:38 2023, max compression
```

## Comparing `WifiOrca-0.0.8.tar` & `WifiOrca-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:28:39.102964 WifiOrca-0.0.8/
--rw-r--r--   0 kali      (1000) kali      (1000)     2070 2023-07-09 11:28:39.102964 WifiOrca-0.0.8/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1505 2023-07-09 11:28:12.000000 WifiOrca-0.0.8/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      748 2023-07-09 11:23:47.000000 WifiOrca-0.0.8/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 11:28:39.102964 WifiOrca-0.0.8/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:28:39.098964 WifiOrca-0.0.8/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:28:39.102964 WifiOrca-0.0.8/src/WifiOrca/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.8/src/WifiOrca/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      281 2023-07-09 11:08:22.000000 WifiOrca-0.0.8/src/WifiOrca/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6036 2023-07-09 11:26:59.000000 WifiOrca-0.0.8/src/WifiOrca/packet_fox_client.py
--rw-r--r--   0 kali      (1000) kali      (1000)      846 2023-07-09 11:07:38.000000 WifiOrca-0.0.8/src/WifiOrca/packet_fox_server.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:28:39.102964 WifiOrca-0.0.8/src/WifiOrca.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2070 2023-07-09 11:28:39.000000 WifiOrca-0.0.8/src/WifiOrca.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      317 2023-07-09 11:28:39.000000 WifiOrca-0.0.8/src/WifiOrca.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 11:28:39.000000 WifiOrca-0.0.8/src/WifiOrca.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 11:28:39.000000 WifiOrca-0.0.8/src/WifiOrca.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 11:28:39.000000 WifiOrca-0.0.8/src/WifiOrca.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:31:38.440373 WifiOrca-0.0.9/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2070 2023-07-09 11:31:38.440373 WifiOrca-0.0.9/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1505 2023-07-09 11:28:12.000000 WifiOrca-0.0.9/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      748 2023-07-09 11:31:06.000000 WifiOrca-0.0.9/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 11:31:38.440373 WifiOrca-0.0.9/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:31:38.440373 WifiOrca-0.0.9/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:31:38.440373 WifiOrca-0.0.9/src/WifiOrca/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.9/src/WifiOrca/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      281 2023-07-09 11:08:22.000000 WifiOrca-0.0.9/src/WifiOrca/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6041 2023-07-09 11:31:26.000000 WifiOrca-0.0.9/src/WifiOrca/packet_fox_client.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      846 2023-07-09 11:07:38.000000 WifiOrca-0.0.9/src/WifiOrca/packet_fox_server.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 11:31:38.440373 WifiOrca-0.0.9/src/WifiOrca.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2070 2023-07-09 11:31:38.000000 WifiOrca-0.0.9/src/WifiOrca.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      317 2023-07-09 11:31:38.000000 WifiOrca-0.0.9/src/WifiOrca.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 11:31:38.000000 WifiOrca-0.0.9/src/WifiOrca.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 11:31:38.000000 WifiOrca-0.0.9/src/WifiOrca.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 11:31:38.000000 WifiOrca-0.0.9/src/WifiOrca.egg-info/top_level.txt
```

### Comparing `WifiOrca-0.0.8/PKG-INFO` & `WifiOrca-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WifiOrca
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wifi Orca contains free and open source tools similar to hak5! Please see github for more info!
 Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/Wifi-Orca
 Project-URL: Bug Tracker, https://github.com/Invizabel/Wifi-Orca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `WifiOrca-0.0.8/README.md` & `WifiOrca-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `WifiOrca-0.0.8/pyproject.toml` & `WifiOrca-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WifiOrca"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Michael Mueller", email="michael.j.mueller.pro@gmail.com" },
 ]
 description = "Wifi Orca contains free and open source tools similar to hak5! Please see github for more info!"
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.9"
```

### Comparing `WifiOrca-0.0.8/src/WifiOrca/packet_fox_client.py` & `WifiOrca-0.0.9/src/WifiOrca/packet_fox_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 def packet_fox_client():
     with open("server.txt","r") as file:
         server = file.read()
         server = re.sub("[\s\t\r\n]","",server)
 
     with open("payloads.txt", "r") as file:
         payloads = file.read()
-        payloads = re.sub("[\s\t\r\n]","",lan)
+        payloads = re.sub("[\s\t\r\n]","",payloads)
 
     clear()
     if platform != "linux":
         print("Unsupported platform! Linux is required for this tool!")
         sys.exit()
 
     if payloads == "01":
```

### Comparing `WifiOrca-0.0.8/src/WifiOrca/packet_fox_server.py` & `WifiOrca-0.0.9/src/WifiOrca/packet_fox_server.py`

 * *Files identical despite different names*

### Comparing `WifiOrca-0.0.8/src/WifiOrca.egg-info/PKG-INFO` & `WifiOrca-0.0.9/src/WifiOrca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WifiOrca
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wifi Orca contains free and open source tools similar to hak5! Please see github for more info!
 Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/Wifi-Orca
 Project-URL: Bug Tracker, https://github.com/Invizabel/Wifi-Orca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

