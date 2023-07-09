# Comparing `tmp/wizproxy-0.2.0.tar.gz` & `tmp/wizproxy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizproxy-0.2.0.tar", max compression
+gzip compressed data, was "wizproxy-0.3.0.tar", max compression
```

## Comparing `wizproxy-0.2.0.tar` & `wizproxy-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.2.0/LICENSE
--rw-r--r--   0        0        0     4341 2023-07-09 00:54:38.019365 wizproxy-0.2.0/README.md
--rw-r--r--   0        0        0      564 2023-07-09 00:53:28.317839 wizproxy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 17:55:10.532607 wizproxy-0.2.0/wizproxy/__init__.py
--rw-r--r--   0        0        0     2075 2023-07-08 20:53:17.644557 wizproxy-0.2.0/wizproxy/__main__.py
--rw-r--r--   0        0        0     3510 2023-07-07 22:10:54.046310 wizproxy-0.2.0/wizproxy/aes.py
--rw-r--r--   0        0        0     2238 2023-07-08 21:38:01.265737 wizproxy-0.2.0/wizproxy/key_chain.py
--rw-r--r--   0        0        0      186 2023-07-08 20:52:07.212214 wizproxy-0.2.0/wizproxy/plugin/__init__.py
--rw-r--r--   0        0        0     3260 2023-07-08 19:14:33.867973 wizproxy-0.2.0/wizproxy/plugin/builtin.py
--rw-r--r--   0        0        0     1364 2023-07-08 17:35:40.141339 wizproxy-0.2.0/wizproxy/plugin/filter.py
--rw-r--r--   0        0        0     3746 2023-07-08 18:58:23.042352 wizproxy-0.2.0/wizproxy/plugin/interface.py
--rw-r--r--   0        0        0      432 2023-07-08 20:51:54.963279 wizproxy-0.2.0/wizproxy/plugin/log.py
--rw-r--r--   0        0        0     1797 2023-07-09 00:39:09.063077 wizproxy-0.2.0/wizproxy/plugin/scapy.py
--rw-r--r--   0        0        0      226 2023-07-08 15:33:47.151413 wizproxy-0.2.0/wizproxy/proto/__init__.py
--rw-r--r--   0        0        0     2475 2023-07-07 22:10:54.053311 wizproxy-0.2.0/wizproxy/proto/bytes.py
--rw-r--r--   0        0        0     1298 2023-07-07 22:10:54.053311 wizproxy-0.2.0/wizproxy/proto/dml.py
--rw-r--r--   0        0        0     1979 2023-07-08 17:28:54.299160 wizproxy-0.2.0/wizproxy/proto/frame.py
--rw-r--r--   0        0        0     2117 2023-07-07 22:10:54.059311 wizproxy-0.2.0/wizproxy/proto/handshake.py
--rw-r--r--   0        0        0     1807 2023-07-08 19:18:39.599952 wizproxy-0.2.0/wizproxy/proxy.py
--rw-r--r--   0        0        0     4019 2023-07-08 17:14:20.768084 wizproxy-0.2.0/wizproxy/session.py
--rw-r--r--   0        0        0     5042 2023-07-08 23:16:29.087736 wizproxy-0.2.0/wizproxy/shard.py
--rw-r--r--   0        0        0     4956 2023-07-07 22:10:54.060311 wizproxy-0.2.0/wizproxy/stream.py
--rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 wizproxy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4341 2023-07-09 00:54:38.019365 wizproxy-0.3.0/README.md
+-rw-r--r--   0        0        0      564 2023-07-09 01:03:28.499986 wizproxy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 17:55:10.532607 wizproxy-0.3.0/wizproxy/__init__.py
+-rw-r--r--   0        0        0     2102 2023-07-09 01:02:56.982040 wizproxy-0.3.0/wizproxy/__main__.py
+-rw-r--r--   0        0        0     3510 2023-07-07 22:10:54.046310 wizproxy-0.3.0/wizproxy/aes.py
+-rw-r--r--   0        0        0     2238 2023-07-08 21:38:01.265737 wizproxy-0.3.0/wizproxy/key_chain.py
+-rw-r--r--   0        0        0      186 2023-07-08 20:52:07.212214 wizproxy-0.3.0/wizproxy/plugin/__init__.py
+-rw-r--r--   0        0        0     3260 2023-07-08 19:14:33.867973 wizproxy-0.3.0/wizproxy/plugin/builtin.py
+-rw-r--r--   0        0        0     1364 2023-07-08 17:35:40.141339 wizproxy-0.3.0/wizproxy/plugin/filter.py
+-rw-r--r--   0        0        0     3746 2023-07-08 18:58:23.042352 wizproxy-0.3.0/wizproxy/plugin/interface.py
+-rw-r--r--   0        0        0      432 2023-07-08 20:51:54.963279 wizproxy-0.3.0/wizproxy/plugin/log.py
+-rw-r--r--   0        0        0     1797 2023-07-09 00:39:09.063077 wizproxy-0.3.0/wizproxy/plugin/scapy.py
+-rw-r--r--   0        0        0      226 2023-07-08 15:33:47.151413 wizproxy-0.3.0/wizproxy/proto/__init__.py
+-rw-r--r--   0        0        0     2475 2023-07-07 22:10:54.053311 wizproxy-0.3.0/wizproxy/proto/bytes.py
+-rw-r--r--   0        0        0     1298 2023-07-07 22:10:54.053311 wizproxy-0.3.0/wizproxy/proto/dml.py
+-rw-r--r--   0        0        0     1979 2023-07-08 17:28:54.299160 wizproxy-0.3.0/wizproxy/proto/frame.py
+-rw-r--r--   0        0        0     2117 2023-07-07 22:10:54.059311 wizproxy-0.3.0/wizproxy/proto/handshake.py
+-rw-r--r--   0        0        0     1807 2023-07-08 19:18:39.599952 wizproxy-0.3.0/wizproxy/proxy.py
+-rw-r--r--   0        0        0     4019 2023-07-08 17:14:20.768084 wizproxy-0.3.0/wizproxy/session.py
+-rw-r--r--   0        0        0     5042 2023-07-08 23:16:29.087736 wizproxy-0.3.0/wizproxy/shard.py
+-rw-r--r--   0        0        0     4956 2023-07-07 22:10:54.060311 wizproxy-0.3.0/wizproxy/stream.py
+-rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 wizproxy-0.3.0/PKG-INFO
```

### Comparing `wizproxy-0.2.0/LICENSE` & `wizproxy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/README.md` & `wizproxy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/pyproject.toml` & `wizproxy-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizproxy"
-version = "0.2.0"
+version = "0.3.0"
 description = "A proxy for handling encrypted Wizard101 traffic"
 authors = ["Valentin B. <valentin.be@protonmail.com>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `wizproxy-0.2.0/wizproxy/__main__.py` & `wizproxy-0.3.0/wizproxy/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "keys", type=Path, help="The directory with the two key JSON files"
     )
     parser.add_argument(
         "--host",
         type=str,
+        default="0.0.0.0",
         help="The host interface to bind shard sockets to",
     )
     parser.add_argument(
         "-l",
         "--login",
         type=str,
         default="login.us.wizard101.com",
```

### Comparing `wizproxy-0.2.0/wizproxy/aes.py` & `wizproxy-0.3.0/wizproxy/aes.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/key_chain.py` & `wizproxy-0.3.0/wizproxy/key_chain.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/plugin/builtin.py` & `wizproxy-0.3.0/wizproxy/plugin/builtin.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/plugin/filter.py` & `wizproxy-0.3.0/wizproxy/plugin/filter.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/plugin/interface.py` & `wizproxy-0.3.0/wizproxy/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/plugin/scapy.py` & `wizproxy-0.3.0/wizproxy/plugin/scapy.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/proto/bytes.py` & `wizproxy-0.3.0/wizproxy/proto/bytes.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/proto/dml.py` & `wizproxy-0.3.0/wizproxy/proto/dml.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/proto/frame.py` & `wizproxy-0.3.0/wizproxy/proto/frame.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/proto/handshake.py` & `wizproxy-0.3.0/wizproxy/proto/handshake.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/proxy.py` & `wizproxy-0.3.0/wizproxy/proxy.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/session.py` & `wizproxy-0.3.0/wizproxy/session.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/shard.py` & `wizproxy-0.3.0/wizproxy/shard.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/wizproxy/stream.py` & `wizproxy-0.3.0/wizproxy/stream.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.2.0/PKG-INFO` & `wizproxy-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizproxy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A proxy for handling encrypted Wizard101 traffic
 License: ISC
 Author: Valentin B.
 Author-email: valentin.be@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

