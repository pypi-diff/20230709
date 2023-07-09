# Comparing `tmp/wizproxy-0.1.0.tar.gz` & `tmp/wizproxy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizproxy-0.1.0.tar", max compression
+gzip compressed data, was "wizproxy-0.2.0.tar", max compression
```

## Comparing `wizproxy-0.1.0.tar` & `wizproxy-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.1.0/LICENSE
--rw-r--r--   0        0        0     4101 2023-07-08 22:07:00.506741 wizproxy-0.1.0/README.md
--rw-r--r--   0        0        0      564 2023-07-08 22:07:25.323022 wizproxy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-24 17:55:10.532607 wizproxy-0.1.0/wizproxy/__init__.py
--rw-r--r--   0        0        0     2075 2023-07-08 20:53:17.644557 wizproxy-0.1.0/wizproxy/__main__.py
--rw-r--r--   0        0        0     3510 2023-07-07 22:10:54.046310 wizproxy-0.1.0/wizproxy/aes.py
--rw-r--r--   0        0        0     2238 2023-07-08 21:38:01.265737 wizproxy-0.1.0/wizproxy/key_chain.py
--rw-r--r--   0        0        0      186 2023-07-08 20:52:07.212214 wizproxy-0.1.0/wizproxy/plugin/__init__.py
--rw-r--r--   0        0        0     3260 2023-07-08 19:14:33.867973 wizproxy-0.1.0/wizproxy/plugin/builtin.py
--rw-r--r--   0        0        0     1364 2023-07-08 17:35:40.141339 wizproxy-0.1.0/wizproxy/plugin/filter.py
--rw-r--r--   0        0        0     3746 2023-07-08 18:58:23.042352 wizproxy-0.1.0/wizproxy/plugin/interface.py
--rw-r--r--   0        0        0      432 2023-07-08 20:51:54.963279 wizproxy-0.1.0/wizproxy/plugin/log.py
--rw-r--r--   0        0        0     1812 2023-07-08 20:28:54.253293 wizproxy-0.1.0/wizproxy/plugin/scapy.py
--rw-r--r--   0        0        0      226 2023-07-08 15:33:47.151413 wizproxy-0.1.0/wizproxy/proto/__init__.py
--rw-r--r--   0        0        0     2475 2023-07-07 22:10:54.053311 wizproxy-0.1.0/wizproxy/proto/bytes.py
--rw-r--r--   0        0        0     1298 2023-07-07 22:10:54.053311 wizproxy-0.1.0/wizproxy/proto/dml.py
--rw-r--r--   0        0        0     1979 2023-07-08 17:28:54.299160 wizproxy-0.1.0/wizproxy/proto/frame.py
--rw-r--r--   0        0        0     2117 2023-07-07 22:10:54.059311 wizproxy-0.1.0/wizproxy/proto/handshake.py
--rw-r--r--   0        0        0     1807 2023-07-08 19:18:39.599952 wizproxy-0.1.0/wizproxy/proxy.py
--rw-r--r--   0        0        0     4019 2023-07-08 17:14:20.768084 wizproxy-0.1.0/wizproxy/session.py
--rw-r--r--   0        0        0     5034 2023-07-08 19:17:24.998553 wizproxy-0.1.0/wizproxy/shard.py
--rw-r--r--   0        0        0     4956 2023-07-07 22:10:54.060311 wizproxy-0.1.0/wizproxy/stream.py
--rw-r--r--   0        0        0     4653 1970-01-01 00:00:00.000000 wizproxy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      747 2023-06-24 18:52:44.129272 wizproxy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4341 2023-07-09 00:54:38.019365 wizproxy-0.2.0/README.md
+-rw-r--r--   0        0        0      564 2023-07-09 00:53:28.317839 wizproxy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 17:55:10.532607 wizproxy-0.2.0/wizproxy/__init__.py
+-rw-r--r--   0        0        0     2075 2023-07-08 20:53:17.644557 wizproxy-0.2.0/wizproxy/__main__.py
+-rw-r--r--   0        0        0     3510 2023-07-07 22:10:54.046310 wizproxy-0.2.0/wizproxy/aes.py
+-rw-r--r--   0        0        0     2238 2023-07-08 21:38:01.265737 wizproxy-0.2.0/wizproxy/key_chain.py
+-rw-r--r--   0        0        0      186 2023-07-08 20:52:07.212214 wizproxy-0.2.0/wizproxy/plugin/__init__.py
+-rw-r--r--   0        0        0     3260 2023-07-08 19:14:33.867973 wizproxy-0.2.0/wizproxy/plugin/builtin.py
+-rw-r--r--   0        0        0     1364 2023-07-08 17:35:40.141339 wizproxy-0.2.0/wizproxy/plugin/filter.py
+-rw-r--r--   0        0        0     3746 2023-07-08 18:58:23.042352 wizproxy-0.2.0/wizproxy/plugin/interface.py
+-rw-r--r--   0        0        0      432 2023-07-08 20:51:54.963279 wizproxy-0.2.0/wizproxy/plugin/log.py
+-rw-r--r--   0        0        0     1797 2023-07-09 00:39:09.063077 wizproxy-0.2.0/wizproxy/plugin/scapy.py
+-rw-r--r--   0        0        0      226 2023-07-08 15:33:47.151413 wizproxy-0.2.0/wizproxy/proto/__init__.py
+-rw-r--r--   0        0        0     2475 2023-07-07 22:10:54.053311 wizproxy-0.2.0/wizproxy/proto/bytes.py
+-rw-r--r--   0        0        0     1298 2023-07-07 22:10:54.053311 wizproxy-0.2.0/wizproxy/proto/dml.py
+-rw-r--r--   0        0        0     1979 2023-07-08 17:28:54.299160 wizproxy-0.2.0/wizproxy/proto/frame.py
+-rw-r--r--   0        0        0     2117 2023-07-07 22:10:54.059311 wizproxy-0.2.0/wizproxy/proto/handshake.py
+-rw-r--r--   0        0        0     1807 2023-07-08 19:18:39.599952 wizproxy-0.2.0/wizproxy/proxy.py
+-rw-r--r--   0        0        0     4019 2023-07-08 17:14:20.768084 wizproxy-0.2.0/wizproxy/session.py
+-rw-r--r--   0        0        0     5042 2023-07-08 23:16:29.087736 wizproxy-0.2.0/wizproxy/shard.py
+-rw-r--r--   0        0        0     4956 2023-07-07 22:10:54.060311 wizproxy-0.2.0/wizproxy/stream.py
+-rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 wizproxy-0.2.0/PKG-INFO
```

### Comparing `wizproxy-0.1.0/LICENSE` & `wizproxy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/README.md` & `wizproxy-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -108,7 +108,12 @@
 
 Injection as in arbitrarily injecting any amount of packets at any given time
 is not supported and, for many use cases where this would be considered, can
 get your account banned.
 
 Interception and manipulating the contents of specific packet types, however,
 is supported and is the encouraged way of interacting with the packet stream.
+
+> I'm getting `json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)`
+
+This is because you are on Windows and the JSON files you dumped are UTF-16
+encoded. Use any text editor of your preference to convert them to UTF-8.
```

### Comparing `wizproxy-0.1.0/pyproject.toml` & `wizproxy-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizproxy"
-version = "0.1.0"
+version = "0.2.0"
 description = "A proxy for handling encrypted Wizard101 traffic"
 authors = ["Valentin B. <valentin.be@protonmail.com>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `wizproxy-0.1.0/wizproxy/__main__.py` & `wizproxy-0.2.0/wizproxy/__main__.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/aes.py` & `wizproxy-0.2.0/wizproxy/aes.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/key_chain.py` & `wizproxy-0.2.0/wizproxy/key_chain.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/plugin/builtin.py` & `wizproxy-0.2.0/wizproxy/plugin/builtin.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/plugin/filter.py` & `wizproxy-0.2.0/wizproxy/plugin/filter.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/plugin/interface.py` & `wizproxy-0.2.0/wizproxy/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/plugin/scapy.py` & `wizproxy-0.2.0/wizproxy/plugin/scapy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import trio
 from scapy.layers.inet import Ether, IP, TCP
 from scapy.utils import PcapNgWriter
 
-from ..proto import Bytes, Frame
+from ..proto import Bytes, Frame, SocketAddress
 from . import Context, Direction, Plugin, listen
 
 
 class ScapyPlugin(Plugin):
     """
     A plugin which writes frame data to pcapng files.
 
@@ -25,32 +25,37 @@
         self.writer = writer
 
     @classmethod
     def from_file(cls, path: Path):
         writer = PcapNgWriter(str(path.resolve()))
         return cls(writer)
 
-    async def write_to_file(self, ctx: Context, tcp: TCP, ip: IP, raw: bytes):
+    async def write_to_file(
+        self, ctx: Context, source: SocketAddress, dest: SocketAddress, raw: bytes
+    ):
         shard = ctx.shard()
 
-        packet = Ether() / ip / tcp / raw
+        packet = (
+            Ether()
+            / IP(src=source.ip, dst=dest.ip)
+            / TCP(sport=source.port, dport=dest.port)
+            / raw
+        )
         packet.comment = f"Shard {shard.ip}:{shard.port}, client {ctx.session.sid}"
 
         await trio.to_thread.run_sync(self.writer.write, packet)
 
     @listen(Direction.CLIENT_TO_SERVER)
     async def clientbound(self, ctx: Context, frame: Frame):
         bytes = Bytes()
         frame.write(bytes)
 
-        ip = IP(src=ctx.session.client.ip, dst=ctx.session.server.ip)
-        tcp = TCP(sport=ctx.session.client.port, dport=ctx.session.server.port)
-        await self.write_to_file(ctx, tcp, ip, bytes.getvalue())
+        session = ctx.session
+        await self.write_to_file(ctx, session.client, session.server, bytes.getvalue())
 
     @listen(Direction.SERVER_TO_CLIENT)
     async def serverbound(self, ctx: Context, frame: Frame):
         bytes = Bytes()
         frame.write(bytes)
 
-        ip = IP(src=ctx.session.server.ip, dst=ctx.session.client.ip)
-        tcp = TCP(sport=ctx.session.server.port, dport=ctx.session.client.port)
-        await self.write_to_file(ctx, tcp, ip, bytes.getvalue())
+        session = ctx.session
+        await self.write_to_file(ctx, session.server, session.client, bytes.getvalue())
```

### Comparing `wizproxy-0.1.0/wizproxy/proto/bytes.py` & `wizproxy-0.2.0/wizproxy/proto/bytes.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/proto/dml.py` & `wizproxy-0.2.0/wizproxy/proto/dml.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/proto/frame.py` & `wizproxy-0.2.0/wizproxy/proto/frame.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/proto/handshake.py` & `wizproxy-0.2.0/wizproxy/proto/handshake.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/proxy.py` & `wizproxy-0.2.0/wizproxy/proxy.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/session.py` & `wizproxy-0.2.0/wizproxy/session.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/wizproxy/shard.py` & `wizproxy-0.2.0/wizproxy/shard.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     async def run(
         self, host: Optional[str], nursery: trio.Nursery, remote: SocketAddress
     ) -> SocketAddress:
         async def accept_tcp_client(stream: trio.SocketStream):
             outward = await trio.open_tcp_stream(*remote)
 
-            client = SocketAddress(*stream.socket.getsockname())  # type:ignore
+            client = SocketAddress(*stream.socket.getsockname()[:2])  # type:ignore
             sid = next(self._id_generator)
             session = Session(client, remote, sid, self.key_chain)
 
             context = Context(self, session)
 
             logger.info(
                 f"[{self.socket()}] Client {sid} ({client.ip}:{client.port}) connected"
@@ -147,12 +147,12 @@
                 for e in eg.exceptions:
                     logger.error(f"[{self.socket()}] Client {sid} crashed: {e}")
 
         # Port 0 makes the OS pick for us. So we need to remember the real socket
         # address after the server has started.
         serve_tcp = partial(trio.serve_tcp, host=host, handler_nursery=nursery)
         listeners = await nursery.start(serve_tcp, accept_tcp_client, 0)
-        self.addr = SocketAddress(*listeners[0].socket.getsockname())  # type:ignore
+        self.addr = SocketAddress(*listeners[0].socket.getsockname()[:2])  # type:ignore
 
         logger.info(f"[{self.socket()}] Spawning shard to {remote}...")
 
         return self.addr
```

### Comparing `wizproxy-0.1.0/wizproxy/stream.py` & `wizproxy-0.2.0/wizproxy/stream.py`

 * *Files identical despite different names*

### Comparing `wizproxy-0.1.0/PKG-INFO` & `wizproxy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizproxy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A proxy for handling encrypted Wizard101 traffic
 License: ISC
 Author: Valentin B.
 Author-email: valentin.be@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -126,7 +126,12 @@
 Injection as in arbitrarily injecting any amount of packets at any given time
 is not supported and, for many use cases where this would be considered, can
 get your account banned.
 
 Interception and manipulating the contents of specific packet types, however,
 is supported and is the encouraged way of interacting with the packet stream.
 
+> I'm getting `json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)`
+
+This is because you are on Windows and the JSON files you dumped are UTF-16
+encoded. Use any text editor of your preference to convert them to UTF-8.
+
```

