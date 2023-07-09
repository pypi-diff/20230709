# Comparing `tmp/vocalhost-1.0.9.tar.gz` & `tmp/vocalhost-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalhost-1.0.9.tar", last modified: Fri Jul  7 19:44:25 2023, max compression
+gzip compressed data, was "vocalhost-1.1.0.tar", last modified: Sun Jul  9 18:22:25 2023, max compression
```

## Comparing `vocalhost-1.0.9.tar` & `vocalhost-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:44:25.862002 vocalhost-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-07 19:44:25.862002 vocalhost-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-07 19:44:14.000000 vocalhost-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:44:25.862002 vocalhost-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-07 19:44:14.000000 vocalhost-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:44:25.862002 vocalhost-1.0.9/vocalhost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-07 19:44:14.000000 vocalhost-1.0.9/vocalhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:22:25.258284 vocalhost-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-09 18:22:25.258284 vocalhost-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-09 18:22:15.000000 vocalhost-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:22:25.258284 vocalhost-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-09 18:22:15.000000 vocalhost-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:22:25.258284 vocalhost-1.1.0/vocalhost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-09 18:22:25.000000 vocalhost-1.1.0/vocalhost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-09 18:22:25.000000 vocalhost-1.1.0/vocalhost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:22:25.000000 vocalhost-1.1.0/vocalhost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 18:22:25.000000 vocalhost-1.1.0/vocalhost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 18:22:25.000000 vocalhost-1.1.0/vocalhost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-09 18:22:15.000000 vocalhost-1.1.0/vocalhost.py
```

### Comparing `vocalhost-1.0.9/PKG-INFO` & `vocalhost-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.0.9
+Version: 1.1.0
 Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.0.9/README.md` & `vocalhost-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vocalhost-1.0.9/vocalhost.egg-info/PKG-INFO` & `vocalhost-1.1.0/vocalhost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.0.9
+Version: 1.1.0
 Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.0.9/vocalhost.py` & `vocalhost-1.1.0/vocalhost.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,15 @@
         asyncio.run(Receiver._connect_to_server(client_id=client_id))
 
 
 class Request:
     def send(message, receiver_id, timeout=60):
         receiver_id = str(receiver_id)
         url = 'https://vocalhost.reiserx.com/connect/'+ receiver_id +'/'
-        data = {
-            'message': message
-        }
         
         headers = {
             'Timeout': str(timeout),
             'Authorization': API_KEY
         }
         
-        response = requests.post(url, headers=headers, json=data)
+        response = requests.post(url, headers=headers, data=message)
         return response
```

