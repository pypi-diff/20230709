# Comparing `tmp/WifiOrca-0.0.1.tar.gz` & `tmp/WifiOrca-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WifiOrca-0.0.1.tar", last modified: Sun Jul  9 02:53:25 2023, max compression
+gzip compressed data, was "WifiOrca-0.0.2.tar", last modified: Sun Jul  9 02:56:26 2023, max compression
```

## Comparing `WifiOrca-0.0.1.tar` & `WifiOrca-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:53:25.984936 WifiOrca-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 02:53:25.984936 WifiOrca-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      101 2023-07-07 21:24:23.000000 WifiOrca-0.0.1/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)      730 2023-07-09 02:53:01.000000 WifiOrca-0.0.1/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 02:53:25.984936 WifiOrca-0.0.1/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:53:25.980936 WifiOrca-0.0.1/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:53:25.980936 WifiOrca-0.0.1/src/WifiOrca/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.1/src/WifiOrca/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4015 2023-07-09 02:41:13.000000 WifiOrca-0.0.1/src/WifiOrca/elf.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:53:25.984936 WifiOrca-0.0.1/src/WifiOrca.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 02:53:25.000000 WifiOrca-0.0.1/src/WifiOrca.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      248 2023-07-09 02:53:25.000000 WifiOrca-0.0.1/src/WifiOrca.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 02:53:25.000000 WifiOrca-0.0.1/src/WifiOrca.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 02:53:25.000000 WifiOrca-0.0.1/src/WifiOrca.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 02:53:25.000000 WifiOrca-0.0.1/src/WifiOrca.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      101 2023-07-07 21:24:23.000000 WifiOrca-0.0.2/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      730 2023-07-09 02:55:48.000000 WifiOrca-0.0.2/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/src/WifiOrca/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-07-07 21:24:23.000000 WifiOrca-0.0.2/src/WifiOrca/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4027 2023-07-09 02:56:13.000000 WifiOrca-0.0.2/src/WifiOrca/elf.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-09 02:56:26.426658 WifiOrca-0.0.2/src/WifiOrca.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      648 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      248 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-07-09 02:56:26.000000 WifiOrca-0.0.2/src/WifiOrca.egg-info/top_level.txt
```

### Comparing `WifiOrca-0.0.1/PKG-INFO` & `WifiOrca-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WifiOrca
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wifi Orca contains free and open source tools similar to hak5! Requires nmap!
 Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/Wifi-Orca
 Project-URL: Bug Tracker, https://github.com/Invizabel/Wifi-Orca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `WifiOrca-0.0.1/pyproject.toml` & `WifiOrca-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WifiOrca"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Michael Mueller", email="michael.j.mueller.pro@gmail.com" },
 ]
 description = "Wifi Orca contains free and open source tools similar to hak5! Requires nmap!"
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.9"
```

### Comparing `WifiOrca-0.0.1/src/WifiOrca/elf.py` & `WifiOrca-0.0.2/src/WifiOrca/elf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from subprocess import run
 from TheSilent.clear import *
 from TheSilent.web_scanner import *
 
 CYAN = "\033[1;36m"
 
-def elf(save_file):
+def elf("report.txt"):
     start = time.time()
     clear()
     host_list = []
     ip_list = []
 
     print(CYAN + "running nmap")    
     ip_addr_command = str(run(["ip","addr"], capture_output=True).stdout)
@@ -34,15 +34,15 @@
             my_socket = socket.socket()
             my_socket.settimeout(5)
             try:
                 my_socket.connect((host, int(port)))
                 print(CYAN + f"getting banner: {host}:{port}")
                 banner = my_socket.recv(4096)
                 print(CYAN + banner)
-                with open(save_file, "a") as file:
+                with open("report.txt", "a") as file:
                     file.write(str(banner) + "\n")
 
                 my_socket.close()
 
             except:
                 my_socket.close()
                 continue
@@ -51,15 +51,15 @@
 
     for ip in ip_list:
         time.sleep(1)
         clear()
         print(CYAN + f"running TheSilent's web scanner against: http://{ip}")
         my_web_scanner = web_scanner(f"http://{ip}")
 
-        with open(save_file, "a") as file:
+        with open("report.txt", "a") as file:
             if my_web_scanner == "This server is secure!":
                 file.write(f"{ip}: This server is secure!\n")
                 print(CYAN + f"{ip}: This server is secure!")
 
             if my_web_scanner == "This website doesn't exist or is down!":
                 file.write(f"{ip}: This website doesn't exist or is down!\n")
                 print(CYAN + f"{ip}: This website doesn't exist or is down!")
@@ -73,15 +73,15 @@
                     file.write(f"{ip}: {vuln}\n")
                     print(RED + (f"{ip}: {vuln}"))
 
         clear()
         print(CYAN + f"running The Silent's web scanner against: https://{ip}")
         my_web_scanner = web_scanner(f"https://{ip}")
 
-        with open(save_file, "a") as file:
+        with open("report.txt", "a") as file:
             if my_web_scanner[0] == "This server is secure!":
                 file.write(f"{ip}: This server is secure!\n")
                 print(CYAN + f"{ip}: This server is secure!")
 
             if my_web_scanner == "This website doesn't exist or is down!":
                 file.write(f"{ip}: This website doesn't exist or is down!\n")
                 print(CYAN + f"{ip}: This website doesn't exist or is down!")
```

### Comparing `WifiOrca-0.0.1/src/WifiOrca.egg-info/PKG-INFO` & `WifiOrca-0.0.2/src/WifiOrca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WifiOrca
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wifi Orca contains free and open source tools similar to hak5! Requires nmap!
 Author-email: Michael Mueller <michael.j.mueller.pro@gmail.com>
 Project-URL: Homepage, https://github.com/Invizabel/Wifi-Orca
 Project-URL: Bug Tracker, https://github.com/Invizabel/Wifi-Orca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

