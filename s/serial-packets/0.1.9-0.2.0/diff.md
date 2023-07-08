# Comparing `tmp/serial_packets-0.1.9.tar.gz` & `tmp/serial_packets-0.2.0.tar.gz`

## Comparing `serial_packets-0.1.9.tar` & `serial_packets-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/client.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/packet_decoder.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/packet_encoder.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.9/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.9/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.9/LICENSE
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.9/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17761 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/packet_decoder.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/packet_encoder.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.2.0/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.2.0/LICENSE
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.2.0/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.2.0/PKG-INFO
```

### Comparing `serial_packets-0.1.9/src/serial_packets/_packets.py` & `serial_packets-0.2.0/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.9/src/serial_packets/client.py` & `serial_packets-0.2.0/src/serial_packets/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         self.__work_queue.put_nowait(event)
 
     async def connect(self) -> bool:
         """Connect to serial port. Returns True if connected to port."""
         logger.debug("Connecting to port [%s]", self.__port)
         try:
             self.__transport, self.__protocol = await serial_asyncio.create_serial_connection(
-                asyncio.get_event_loop(), _SerialProtocol, self.__port, baudrate=self.__baudrate)
+                asyncio.get_running_loop(), _SerialProtocol, self.__port, baudrate=self.__baudrate)
         except Exception as e:
             logger.error("%s", e)
             if logging.DEBUG >= logger.getEffectiveLevel():
                 traceback.print_exception(e)
             return False
         self.__protocol.set(self, self.__port, self.__packet_decoder, self.__work_queue)
         return True
```

### Comparing `serial_packets-0.1.9/src/serial_packets/packet_decoder.py` & `serial_packets-0.2.0/src/serial_packets/packet_decoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.9/src/serial_packets/packet_encoder.py` & `serial_packets-0.2.0/src/serial_packets/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.9/src/serial_packets/packets.py` & `serial_packets-0.2.0/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.9/LICENSE` & `serial_packets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.9/README.md` & `serial_packets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.9/pyproject.toml` & `serial_packets-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.9/PKG-INFO` & `serial_packets-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

