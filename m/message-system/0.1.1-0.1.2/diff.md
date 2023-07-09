# Comparing `tmp/message_system-0.1.1.tar.gz` & `tmp/message_system-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message_system-0.1.1.tar", max compression
+gzip compressed data, was "message_system-0.1.2.tar", max compression
```

## Comparing `message_system-0.1.1.tar` & `message_system-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-07-08 05:28:51.234196 message_system-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-08 05:30:22.488449 message_system-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-08 05:30:22.488449 message_system-0.1.1/message_system/__init__.py
--rw-r--r--   0        0        0     7473 2023-07-08 05:52:30.970874 message_system-0.1.1/message_system/message_system.py
--rw-r--r--   0        0        0      432 2023-07-08 05:52:07.494604 message_system-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 message_system-0.1.1/setup.py
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 message_system-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-08 05:28:51.234196 message_system-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-08 05:30:22.488449 message_system-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-08 05:30:22.488449 message_system-0.1.2/message_system/__init__.py
+-rw-r--r--   0        0        0     7472 2023-07-09 00:38:53.958869 message_system-0.1.2/message_system/message_system.py
+-rw-r--r--   0        0        0      432 2023-07-09 00:39:02.921957 message_system-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 message_system-0.1.2/setup.py
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 message_system-0.1.2/PKG-INFO
```

### Comparing `message_system-0.1.1/LICENSE` & `message_system-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `message_system-0.1.1/message_system/message_system.py` & `message_system-0.1.2/message_system/message_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         except socket.error:
             return False  # Socket is closed
 
     def stop_listening(self, sock, duration=3):
         threading.Timer(duration, self.close_sock, [sock]).start()
 
     def close_sock(self, sock: socket.socket):
-        if Message_System.is_socket_open(sock):
+        if MessageSystem.is_socket_open(sock):
             logger.debug(f"closing socket, {str(sock)}")
             try:
                 if sys.platform.startswith("linux"):
                     sock.shutdown(SHUT_RDWR)
                 sock.close()
             except OSError:
                 pass
```

### Comparing `message_system-0.1.1/setup.py` & `message_system-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces>=0.11.0,<0.12.0']
 
 setup_kwargs = {
     'name': 'message-system',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '',
     'author': 'JavierOramas',
     'author_email': 'javiale2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

