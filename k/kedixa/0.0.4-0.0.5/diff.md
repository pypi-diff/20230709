# Comparing `tmp/kedixa-0.0.4-py3-none-any.whl.zip` & `tmp/kedixa-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 39768 bytes, number of entries: 43
+Zip file size: 40264 bytes, number of entries: 44
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-28 08:01 kedixa/__init__.py
 -rw-r--r--  2.0 unx       46 b- defN 23-Mar-12 13:18 kedixa/compat.py
 -rw-r--r--  2.0 unx      877 b- defN 23-Feb-28 08:01 kedixa/file_loader.py
--rw-r--r--  2.0 unx     3967 b- defN 23-Apr-26 03:12 kedixa/mprocess.py
--rw-r--r--  2.0 unx      145 b- defN 23-May-07 13:56 kedixa/version.py
+-rw-r--r--  2.0 unx     4353 b- defN 23-Jul-08 16:47 kedixa/mprocess.py
+-rw-r--r--  2.0 unx      769 b- defN 23-Jul-09 15:25 kedixa/qps_pool.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Jul-09 15:37 kedixa/version.py
 -rw-r--r--  2.0 unx      345 b- defN 23-May-07 13:50 kedixa/comm/__init__.py
 -rw-r--r--  2.0 unx     1711 b- defN 23-Apr-27 04:13 kedixa/comm/address.py
 -rw-r--r--  2.0 unx     6678 b- defN 23-Apr-07 10:56 kedixa/comm/basic.py
 -rw-r--r--  2.0 unx     1785 b- defN 23-Apr-21 04:04 kedixa/comm/bridge.py
 -rw-r--r--  2.0 unx     3336 b- defN 23-Apr-26 03:22 kedixa/comm/connection.py
 -rw-r--r--  2.0 unx     1082 b- defN 23-Mar-18 17:04 kedixa/comm/debug_filter.py
 -rw-r--r--  2.0 unx     1215 b- defN 23-May-05 03:49 kedixa/comm/debug_transformer.py
@@ -34,12 +35,12 @@
 -rw-r--r--  2.0 unx     2437 b- defN 23-Apr-07 14:31 kedixa/comm/http/http_proxy_upgrader.py
 -rw-r--r--  2.0 unx      135 b- defN 23-Apr-08 15:33 kedixa/comm/websocket/__init__.py
 -rw-r--r--  2.0 unx     4524 b- defN 23-Apr-08 08:17 kedixa/comm/websocket/websocket_client.py
 -rw-r--r--  2.0 unx     4903 b- defN 23-Apr-09 03:17 kedixa/comm/websocket/websocket_handler.py
 -rw-r--r--  2.0 unx     3860 b- defN 23-Apr-01 03:14 kedixa/comm/websocket/websocket_message.py
 -rw-r--r--  2.0 unx     6166 b- defN 23-Apr-15 08:48 kedixa/comm/websocket/websocket_processor.py
 -rw-r--r--  2.0 unx     2603 b- defN 23-Apr-09 02:01 kedixa/comm/websocket/websocket_upgrader.py
--rw-r--r--  2.0 unx      227 b- defN 23-May-08 03:37 kedixa-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 03:37 kedixa-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-08 03:37 kedixa-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3683 b- defN 23-May-08 03:37 kedixa-0.0.4.dist-info/RECORD
-43 files, 113485 bytes uncompressed, 33874 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-09 15:37 kedixa-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 15:37 kedixa-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-09 15:37 kedixa-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3757 b- defN 23-Jul-09 15:37 kedixa-0.0.5.dist-info/RECORD
+44 files, 114714 bytes uncompressed, 34258 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: kedixa/file_loader.py
 Comment: 
 
 Filename: kedixa/mprocess.py
 Comment: 
 
+Filename: kedixa/qps_pool.py
+Comment: 
+
 Filename: kedixa/version.py
 Comment: 
 
 Filename: kedixa/comm/__init__.py
 Comment: 
 
 Filename: kedixa/comm/address.py
@@ -111,20 +114,20 @@
 
 Filename: kedixa/comm/websocket/websocket_processor.py
 Comment: 
 
 Filename: kedixa/comm/websocket/websocket_upgrader.py
 Comment: 
 
-Filename: kedixa-0.0.4.dist-info/METADATA
+Filename: kedixa-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: kedixa-0.0.4.dist-info/WHEEL
+Filename: kedixa-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: kedixa-0.0.4.dist-info/top_level.txt
+Filename: kedixa-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: kedixa-0.0.4.dist-info/RECORD
+Filename: kedixa-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kedixa/mprocess.py

```diff
@@ -30,42 +30,49 @@
         self._sem: asyncio.Semaphore = None
         self._loop: asyncio.AbstractEventLoop = None
 
     def __iter__(self):
         return self
 
     def __next__(self):
+        finished = self._finished
+
         while True:
             try:
                 return self.get_task(timeout=0.05)
             except queue.Empty:
-                if self.finished():
+                if finished:
                     raise StopIteration
+                finished = self.finished()
 
     async def __aiter__(self):
         if self._pool is None:
             self._pool = fut.ThreadPoolExecutor(1)
             self._sem = asyncio.Semaphore(1)
             self._loop = asyncio.get_event_loop()
         return self
 
     async def __anext__(self):
-        try_sync = True
+        finished = self._finished
+
+        try:
+            return self.get_task(False, None)
+        except queue.Empty:
+            if finished:
+                raise StopAsyncIteration
+            finished = self.finished()
+
         while True:
             try:
-                if try_sync:
-                    return self.get_task(False, None)
                 async with self._sem:
-                    if self._finished:
-                        raise StopAsyncIteration
                     return await self._loop.run_in_executor(self._pool, self.get_task, True, 0.05)
             except queue.Empty:
-                try_sync = False
-                if self.finished():
+                if finished:
                     raise StopAsyncIteration
+                finished = self.finished()
 
     @property
     def procid(self) -> int:
         return self._procid
 
     def wait_start(self) -> int:
         self._barrier.wait()
@@ -126,14 +133,25 @@
             self._procs.append(mp.Process(target=_worker, args=cur_args, kwargs=kwargs))
 
     def start(self):
         for p in self._procs:
             p.start()
         self._barrier.wait()
 
+    def alive_count(self) -> int:
+        cnt = 0
+        if self._procs:
+            for proc in self._procs:
+                if proc.is_alive():
+                    cnt += 1
+        return cnt
+
+    def all_alive(self) -> bool:
+        return self.alive_count() == self._nproc
+
     def stop(self):
         self._que.close()
         self._que.join_thread()
         self._stopevent.set()
         for p in self._procs:
             p.join()
```

## kedixa/version.py

```diff
@@ -1,4 +1,4 @@
 __major_version__ = 0
 __minor_version__ = 0
-__bugfix_version__ = 4
+__bugfix_version__ = 5
 __version__ = f'{__major_version__}.{__minor_version__}.{__bugfix_version__}'
```

## Comparing `kedixa-0.0.4.dist-info/RECORD` & `kedixa-0.0.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 kedixa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kedixa/compat.py,sha256=G87n6iIZ0Xbvt87mnYLymfrZxluXYYL7lxjC99a4CTo,46
 kedixa/file_loader.py,sha256=2wfU05ozidmTn9LD7zdxljlLJbIFroBvk58RUltEQ-A,877
-kedixa/mprocess.py,sha256=Dv5Dg8BkIcdEHxDYd5vjkXryu0d9V-CTFep9Ke2V5r8,3967
-kedixa/version.py,sha256=bvngniCAzmNl7d7SDAxVv9irMT_m1tFY7R0_eEkClxI,145
+kedixa/mprocess.py,sha256=48f6zPV_mFO5ryPxcnMaBYNqzT4v6q5ChxATzHLTjaA,4353
+kedixa/qps_pool.py,sha256=dPBWNBTYLnS0JwJNbapoHzMJAiC-VYK7o3OZfTRISlk,769
+kedixa/version.py,sha256=ah8WK5x5bx-pCL9k4yEYd5IZH8lyPLIVGqeZWs_gQBU,145
 kedixa/comm/__init__.py,sha256=VtWimM0FbaqkuarlA7fHK90R4C7UD84a1hYLxZ_eSLA,345
 kedixa/comm/address.py,sha256=MNt3sl6rglbeNrdUb82FpqxpQrPcsy24z1PQGaQSY9Y,1711
 kedixa/comm/basic.py,sha256=HOVBqA1o0mFVz-2eQPaRrwSp-YjD9Eo_QXQVUyV_v1A,6678
 kedixa/comm/bridge.py,sha256=1OJ80lBUxFrCLMydM9aMDjNSBOpfouqQc8Hs4V79_PY,1785
 kedixa/comm/connection.py,sha256=DsJjeCifyMm3UOpmjW7NJ5b4DarFV2eBxK4UE0nLKY0,3336
 kedixa/comm/debug_filter.py,sha256=SdCROn1CACYZjlO_ZDiDgwHSg09DHb-0qlUaTUAdWYw,1082
 kedixa/comm/debug_transformer.py,sha256=_uJj0kVgv7kKrxxinpY4uSesag5GILKDgj6aQ_9aUBQ,1215
@@ -33,11 +34,11 @@
 kedixa/comm/http/http_proxy_upgrader.py,sha256=ZpMNLBDAcSvHOq-O8_YGObbPFTOM13f_1e4t-WxRo7s,2437
 kedixa/comm/websocket/__init__.py,sha256=ZCdKPpz9RuNMrgAAoILMI7EniexKVAYuHPfsLTI1f9s,135
 kedixa/comm/websocket/websocket_client.py,sha256=FrQtQ-vInrrqJ-B6oAtvzXr01Yqb2MZR1cIAqxLdWlA,4524
 kedixa/comm/websocket/websocket_handler.py,sha256=UmQ6MjBjz7vj3Oz5n5OmOgVeFGn2Gu5NcbiKNWehVY8,4903
 kedixa/comm/websocket/websocket_message.py,sha256=9GRqZLuHwDiNxhYF8vD8VfPjV-vsfQJ6GeDpzWZCDUM,3860
 kedixa/comm/websocket/websocket_processor.py,sha256=F_iM6TdCJlujFzUV3mBfhQirZL38uxKaNWAklkl_UZs,6166
 kedixa/comm/websocket/websocket_upgrader.py,sha256=SbGwmY-WV8keiW-Pk0oZtqvB3j1QCl1_Ejt-JO4llfo,2603
-kedixa-0.0.4.dist-info/METADATA,sha256=yuIsOisf3IN_AvUl387Mac8WDDI2eoyKDX8ljWOgz3E,227
-kedixa-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kedixa-0.0.4.dist-info/top_level.txt,sha256=ONvTJADmljVaMUydvaC_uUZc5p_aUq5Z3GNuwTlhHpw,7
-kedixa-0.0.4.dist-info/RECORD,,
+kedixa-0.0.5.dist-info/METADATA,sha256=jH5kQFbQF2rwLcPqDe3Y19Czfwx6o0VwPtr2qNnqa68,227
+kedixa-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+kedixa-0.0.5.dist-info/top_level.txt,sha256=ONvTJADmljVaMUydvaC_uUZc5p_aUq5Z3GNuwTlhHpw,7
+kedixa-0.0.5.dist-info/RECORD,,
```

