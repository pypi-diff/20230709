# Comparing `tmp/memphis-py-beta-1.0.6.tar.gz` & `tmp/memphis-py-beta-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-beta-1.0.6.tar", last modified: Tue Jun 27 07:00:11 2023, max compression
+gzip compressed data, was "dist/memphis-py-beta-1.0.7.tar", last modified: Sun Jul  9 15:31:27 2023, max compression
```

## Comparing `memphis-py-beta-1.0.6.tar` & `memphis-py-beta-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16856 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12847 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    34977 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13568 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16856 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/memphis_py_beta.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-06-27 07:00:03.000000 memphis-py-beta-1.0.6/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-06-27 07:00:11.000000 memphis-py-beta-1.0.6/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16852 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12843 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9588 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    34977 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13667 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16852 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/memphis_py_beta.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-07-09 15:31:20.000000 memphis-py-beta-1.0.7/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-07-09 15:31:27.000000 memphis-py-beta-1.0.7/setup.py
```

### Comparing `memphis-py-beta-1.0.6/PKG-INFO` & `memphis-py-beta-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.6
+Version: 1.0.7
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.7.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
@@ -70,18 +70,18 @@
         ```python
         async def main():
           try:
             memphis = Memphis()
             await memphis.connect(
               host="<memphis-host>",
               username="<application-type username>",
-              account_id="<account_id>", # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
+              account_id=<account_id>, # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
               connection_token="<broker-token>", # you will get it on application type user creation
               password="<string>", # depends on how Memphis deployed - default is connection token-based authentication
-              port="<port>", # defaults to 6666
+              port=<port>, # defaults to 6666
               reconnect=True, # defaults to True
               max_reconnect=3, # defaults to 3
               reconnect_interval_ms=1500, # defaults to 1500
               timeout_ms=1500, # defaults to 1500
               # for TLS connection:
               key_file='<key-client.pem>', 
               cert_file='<cert-client.pem>',
```

### Comparing `memphis-py-beta-1.0.6/README.md` & `memphis-py-beta-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,18 @@
 ```python
 async def main():
   try:
     memphis = Memphis()
     await memphis.connect(
       host="<memphis-host>",
       username="<application-type username>",
-      account_id="<account_id>", # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
+      account_id=<account_id>, # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
       connection_token="<broker-token>", # you will get it on application type user creation
       password="<string>", # depends on how Memphis deployed - default is connection token-based authentication
-      port="<port>", # defaults to 6666
+      port=<port>, # defaults to 6666
       reconnect=True, # defaults to True
       max_reconnect=3, # defaults to 3
       reconnect_interval_ms=1500, # defaults to 1500
       timeout_ms=1500, # defaults to 1500
       # for TLS connection:
       key_file='<key-client.pem>', 
       cert_file='<cert-client.pem>',
```

### Comparing `memphis-py-beta-1.0.6/memphis/__init__.py` & `memphis-py-beta-1.0.7/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis/consumer.py` & `memphis-py-beta-1.0.7/memphis/consumer.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.consumer_name = consumer_name.lower()
         self.consumer_group = consumer_group.lower()
         self.pull_interval_ms = pull_interval_ms
         self.batch_size = batch_size
         self.batch_max_time_to_wait_ms = batch_max_time_to_wait_ms
         self.max_ack_time_ms = max_ack_time_ms
         self.max_msg_deliveries = max_msg_deliveries
-        self.ping_consumer_invterval_ms = 30000
+        self.ping_consumer_interval_ms = 30000
         if error_callback is None:
             error_callback = default_error_handler
         self.t_ping = asyncio.create_task(self.__ping_consumer(error_callback))
         self.start_consume_from_sequence = start_consume_from_sequence
         self.last_messages = last_messages
         self.context = {}
         self.dls_messages = []
@@ -112,15 +112,53 @@
                     )
         except Exception as e:
             if self.dls_callback_func != None:
                 await self.dls_callback_func([], MemphisError(str(e)), self.context)
                 return
 
     async def fetch(self, batch_size: int = 10):
-        """Fetch a batch of messages."""
+        """
+        Fetch a batch of messages.
+
+        Returns a list of Message objects. If the connection is
+        not active or no messages are recieved before timing out,
+        an empty list is returned.
+
+        Example:
+
+            import asyncio
+            
+            from memphis import Memphis
+
+            async def main(/, host, username, password, station):
+                memphis = Memphis()
+                await memphis.connect(host=host,
+                                      username=username,
+                                      password=password)
+            
+                consumer = await memphis.consumer(station_name=station,
+                                                  consumer_name="test-consumer",
+                                                  consumer_group="test-consumer-group")
+            
+                while True:
+                    batch = await consumer.fetch()
+                    print("Recieved {} messages".format(len(batch)))
+                    for msg in batch:
+                        serialized_record = msg.get_data()
+                        print("Message:", serialized_record)
+            
+                await memphis.close()
+
+            if __name__ == '__main__':
+                asyncio.run(main(host=host,
+                                 username=username,
+                                 password=password,
+                                 station=station))
+        
+        """
         messages = []
         if self.connection.is_connection_active:
             try:
                 if batch_size > self.MAX_BATCH_SIZE:
                     raise MemphisError(
                         f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
                 self.batch_size = batch_size
@@ -146,23 +184,23 @@
                 )
                 msgs = await self.psub.fetch(batch_size)
                 for msg in msgs:
                     messages.append(
                         Message(msg, self.connection, self.consumer_group))
                 return messages
             except Exception as e:
-                if "timeout" not in str(e):
+                if "timeout" not in str(e).lower():
                     raise MemphisError(str(e)) from e
-        else:
-            return messages
+
+        return messages
 
     async def __ping_consumer(self, callback):
         while True:
             try:
-                await asyncio.sleep(self.ping_consumer_invterval_ms / 1000)
+                await asyncio.sleep(self.ping_consumer_interval_ms / 1000)
                 consumer_group = get_internal_name(self.consumer_group)
                 await self.connection.broker_connection.consumer_info(
                     self.station_name, consumer_group, timeout=30
                 )
 
             except Exception as e:
                 callback(MemphisError(str(e)))
@@ -176,15 +214,17 @@
         if self.t_ping is not None:
             self.t_ping.cancel()
         self.pull_interval_ms = None
         try:
             destroy_consumer_req = {
                 "name": self.consumer_name,
                 "station_name": self.station_name,
-                "username": self.connection.username
+                "username": self.connection.username,
+                "connection_id": self.connection.connection_id,
+                "req_version": 1,
             }
             consumer_name = json.dumps(
                 destroy_consumer_req, indent=2).encode("utf-8")
             res = await self.connection.broker_manager.request(
                 "$memphis_consumer_destructions", consumer_name, timeout=5
             )
             error = res.data.decode("utf-8")
```

### Comparing `memphis-py-beta-1.0.6/memphis/exceptions.py` & `memphis-py-beta-1.0.7/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis/headers.py` & `memphis-py-beta-1.0.7/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis/memphis.py` & `memphis-py-beta-1.0.7/memphis/memphis.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis/message.py` & `memphis-py-beta-1.0.7/memphis/message.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis/producer.py` & `memphis-py-beta-1.0.7/memphis/producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,17 @@
 
     async def destroy(self):
         """Destroy the producer."""
         try:
             destroy_producer_req = {
                 "name": self.producer_name,
                 "station_name": self.station_name,
-                "username": self.connection.username
+                "username": self.connection.username,
+                "connection_id": self.connection.connection_id,
+                "req_version": 1,
             }
 
             producer_name = json.dumps(destroy_producer_req).encode("utf-8")
             res = await self.connection.broker_manager.request(
                 "$memphis_producer_destructions", producer_name, timeout=5
             )
             error = res.data.decode("utf-8")
```

### Comparing `memphis-py-beta-1.0.6/memphis/station.py` & `memphis-py-beta-1.0.7/memphis/station.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis/types.py` & `memphis-py-beta-1.0.7/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis/utils.py` & `memphis-py-beta-1.0.7/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.6/memphis_py_beta.egg-info/PKG-INFO` & `memphis-py-beta-1.0.7/memphis_py_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.6
+Version: 1.0.7
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.7.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
@@ -70,18 +70,18 @@
         ```python
         async def main():
           try:
             memphis = Memphis()
             await memphis.connect(
               host="<memphis-host>",
               username="<application-type username>",
-              account_id="<account_id>", # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
+              account_id=<account_id>, # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
               connection_token="<broker-token>", # you will get it on application type user creation
               password="<string>", # depends on how Memphis deployed - default is connection token-based authentication
-              port="<port>", # defaults to 6666
+              port=<port>, # defaults to 6666
               reconnect=True, # defaults to True
               max_reconnect=3, # defaults to 3
               reconnect_interval_ms=1500, # defaults to 1500
               timeout_ms=1500, # defaults to 1500
               # for TLS connection:
               key_file='<key-client.pem>', 
               cert_file='<cert-client.pem>',
```

### Comparing `memphis-py-beta-1.0.6/setup.py` & `memphis-py-beta-1.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py-beta",
     packages=["memphis"],
-    version="1.0.6",
+    version="1.0.7",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.7.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

