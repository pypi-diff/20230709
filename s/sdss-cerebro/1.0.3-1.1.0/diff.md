# Comparing `tmp/sdss_cerebro-1.0.3.tar.gz` & `tmp/sdss_cerebro-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_cerebro-1.0.3.tar", max compression
+gzip compressed data, was "sdss_cerebro-1.1.0.tar", max compression
```

## Comparing `sdss_cerebro-1.0.3.tar` & `sdss_cerebro-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1504 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     2183 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/README.md
--rw-r--r--   0        0        0      273 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/__init__.py
--rw-r--r--   0        0        0     3481 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/__main__.py
--rw-r--r--   0        0        0    15275 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/cerebro.py
--rw-r--r--   0        0        0     3381 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/client.py
--rw-r--r--   0        0        0     7575 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/etc/cerebro.yaml
--rw-r--r--   0        0        0     3898 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/observer.py
--rw-r--r--   0        0        0     3064 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/protocols.py
--rw-r--r--   0        0        0        0 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/scripts/__init__.py
--rw-r--r--   0        0        0      735 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/scripts/tpm2influxdb.py
--rw-r--r--   0        0        0     5199 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/sources/AMQP.py
--rw-r--r--   0        0        0      453 2022-12-28 17:08:53.764801 sdss_cerebro-1.0.3/cerebro/sources/__init__.py
--rw-r--r--   0        0        0     5007 2022-12-28 17:08:53.768801 sdss_cerebro-1.0.3/cerebro/sources/drift.py
--rw-r--r--   0        0        0     5451 2022-12-28 17:08:53.768801 sdss_cerebro-1.0.3/cerebro/sources/lco.py
--rw-r--r--   0        0        0     7593 2022-12-28 17:08:53.768801 sdss_cerebro-1.0.3/cerebro/sources/lvm.py
--rw-r--r--   0        0        0     7292 2022-12-28 17:08:53.768801 sdss_cerebro-1.0.3/cerebro/sources/source.py
--rw-r--r--   0        0        0     2100 2022-12-28 17:08:53.768801 sdss_cerebro-1.0.3/cerebro/sources/tpm.py
--rw-r--r--   0        0        0    14219 2022-12-28 17:08:53.768801 sdss_cerebro-1.0.3/cerebro/sources/tron.py
--rw-r--r--   0        0        0     2436 2022-12-28 17:08:53.768801 sdss_cerebro-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 sdss_cerebro-1.0.3/setup.py
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 sdss_cerebro-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     2183 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/README.md
+-rw-r--r--   0        0        0      273 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/__init__.py
+-rw-r--r--   0        0        0     3583 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/__main__.py
+-rw-r--r--   0        0        0    15275 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/cerebro.py
+-rw-r--r--   0        0        0     3381 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/client.py
+-rw-r--r--   0        0        0     7575 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/etc/cerebro.yaml
+-rw-r--r--   0        0        0     3898 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/observer.py
+-rw-r--r--   0        0        0     3064 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/protocols.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/scripts/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/scripts/tpm2influxdb.py
+-rw-r--r--   0        0        0     5857 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/AMQP.py
+-rw-r--r--   0        0        0      453 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/__init__.py
+-rw-r--r--   0        0        0     5007 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/drift.py
+-rw-r--r--   0        0        0     5551 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/lco.py
+-rw-r--r--   0        0        0     7593 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/lvm.py
+-rw-r--r--   0        0        0     7292 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/source.py
+-rw-r--r--   0        0        0     2100 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/tpm.py
+-rw-r--r--   0        0        0    14219 2023-07-09 16:35:30.879619 sdss_cerebro-1.1.0/cerebro/sources/tron.py
+-rw-r--r--   0        0        0     2436 2023-07-09 16:35:30.883619 sdss_cerebro-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 sdss_cerebro-1.1.0/PKG-INFO
```

### Comparing `sdss_cerebro-1.0.3/LICENSE.md` & `sdss_cerebro-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/README.md` & `sdss_cerebro-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/__main__.py` & `sdss_cerebro-1.1.0/cerebro/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,17 @@
     else:
         config = os.path.realpath(config)
 
     sources = sources.split(",") if sources else []
 
     ctx.obj = {"sources": sources, "config": config, "profiles": profiles}
 
+    print("Using config file", config)
+    print("Profiles", profiles)
+
 
 @cerebro.group(
     cls=DaemonGroup,
     prog="cerebro_daemon",
     workdir=os.getcwd(),
     pidfile=pidfile,
 )
@@ -137,12 +140,12 @@
         print(color_text("FAILED", "red"))
 
     w.close()
     await w.wait_closed()
 
 
 def main():
-    cerebro(obj={})
+    cerebro(obj={}, auto_envvar_prefix="CEREBRO")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sdss_cerebro-1.0.3/cerebro/cerebro.py` & `sdss_cerebro-1.1.0/cerebro/cerebro.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/client.py` & `sdss_cerebro-1.1.0/cerebro/client.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/etc/cerebro.yaml` & `sdss_cerebro-1.1.0/cerebro/etc/cerebro.yaml`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/observer.py` & `sdss_cerebro-1.1.0/cerebro/observer.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/protocols.py` & `sdss_cerebro-1.1.0/cerebro/protocols.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/scripts/tpm2influxdb.py` & `sdss_cerebro-1.1.0/cerebro/scripts/tpm2influxdb.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/sources/AMQP.py` & `sdss_cerebro-1.1.0/cerebro/sources/AMQP.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,87 @@
 # @Date: 2021-05-04
 # @Filename: AMQP.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
+from collections.abc import MutableMapping
 from contextlib import suppress
 
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Callable, Coroutine, Optional
 
-from clu import AMQPClient
-
-from cerebro import log
+from clu import AMQPClient, AMQPReply
 
 from .source import DataPoints, Source
 
 
+if TYPE_CHECKING:
+    from aio_pika import IncomingMessage
+
 __all__ = ["AMQPSource"]
 
 
+def flatten_dict(
+    d: MutableMapping,
+    parent_key: str = "",
+    sep: str = ".",
+    groupers: list[str] = [],
+) -> tuple[MutableMapping, dict]:
+    """From https://bit.ly/3KN9v3G."""
+
+    groupings = {}
+
+    items = []
+    for k, v in d.items():
+        if isinstance(v, (tuple, list)):
+            continue
+
+        new_key = parent_key + sep + k if parent_key else k
+        if isinstance(v, MutableMapping):
+            flattened, new_groupings = flatten_dict(
+                v,
+                new_key,
+                groupers=groupers,
+                sep=sep,
+            )
+            items.extend(flattened.items())
+            groupings.update(new_groupings)
+        else:
+            items.append((new_key, v))
+            if k in groupers:
+                groupings[k] = v
+
+    return dict(items), groupings
+
+
+class ReplyClient(AMQPClient):
+    """A client that monitors all the replies."""
+
+    def __init__(
+        self,
+        *args,
+        callback: Callable[[AMQPReply], Coroutine] | None = None,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+
+        self.callback = callback
+
+    async def handle_reply(self, message: IncomingMessage):
+        """Prints the formatted reply."""
+
+        reply = await super().handle_reply(message)
+
+        if self.callback:
+            asyncio.create_task(self.callback(reply))
+
+        return reply
+
+
 class AMQPSource(Source):
     """A source for AMQP actors.
 
     Parameters
     ----------
     name
         The name of the data source.
@@ -41,19 +100,21 @@
     user
         The username to use to use to connect to RabbitMQ.
     password
         The password to use to use to connect to RabbitMQ.
     keywords
         A list of keyword values to output. The format must be
         ``actor.keyword.subkeyword.subsubkeyword``. The final value extracted
-        must be a scalar.
+        must be a scalar. If `None`, all keywords will be stored.
     groupers
         A list of subkeywords that, if found, will be added as tags to the
         measurement. These are useful when the same keyword can be output
         for different devices or controllers.
+    internal
+        Mark commands sent to the actor as internal.
     commands
         A mapping of commands to be issued to the interval, in seconds. For
         example ``{"archon status": 5}``.
 
     """
 
     source_type = "amqp"
@@ -64,58 +125,48 @@
         name: str,
         bucket: Optional[str] = None,
         tags: dict[str, Any] = {},
         host: str = "localhost",
         port: int = 5672,
         user: str = "guest",
         password: str = "guest",
-        keywords: list[str] = [],
+        keywords: list[str] | None = None,
         groupers: list[str] = [],
+        internal: bool = False,
         commands: dict[str, float] = {},
     ):
         super().__init__(name, bucket=bucket, tags=tags)
 
-        key_actors = list(set([key.split(".")[0] for key in keywords]))
-
-        self.client = AMQPClient(
+        self.client = ReplyClient(
             f"cerebro_client_{name}",
             user=user,
             password=password,
             host=host,
             port=port,
-            models=key_actors,
+            callback=self.process_keyword,
         )
 
         self.keywords = keywords
         self.groupers = groupers
-        self._actor_keys = {
-            actor: [key.split(".")[1] for key in keywords if key.startswith(actor)]
-            for actor in key_actors
-        }
+        self.internal = internal
 
         self.commands = commands
         self._command_tasks: list[asyncio.Task] = []
 
     async def start(self):
         """Starts the connection to RabbitMQ."""
 
         await self.client.start()
 
         for model in self.client.models.values():
             model.register_callback(self.process_keyword)
 
         for command in self.commands:
-            self._command_tasks.append(
-                asyncio.create_task(
-                    self.schedule_command(
-                        command,
-                        self.commands[command],
-                    )
-                )
-            )
+            task = self.schedule_command(command, self.commands[command])
+            self._command_tasks.append(asyncio.create_task(task))
 
         self.running = True
 
     async def stop(self):
         """Closes the connection to Tron."""
 
         for task in self._command_tasks:
@@ -131,54 +182,35 @@
     async def schedule_command(self, command: str, interval: float):
         """Schedules a command to be executed on an interval."""
 
         actor = command.split(" ")[0]
         cmd_str = " ".join(command.split(" ")[1:])
 
         while True:
-            await (await self.client.send_command(actor, cmd_str))
+            await self.client.send_command(actor, cmd_str, internal=self.internal)
             await asyncio.sleep(interval)
 
-    async def process_keyword(self, model, keyword):
-        """Processes a keyword received from Tron."""
+    async def process_keyword(self, reply: AMQPReply):
+        """Processes a keyword received from an actor."""
 
-        name = keyword.name
-        actor = keyword.model.name
+        actor = reply.sender
+        body = reply.body
 
-        if name not in self._actor_keys[actor]:
-            return
+        fields, grouppings = flatten_dict(body, groupers=self.groupers)
 
-        points = []
-
-        for key in self.keywords:
-            if not key.startswith(actor) or key.split(".")[1] != name:
-                continue
-
-            value = keyword.value  # In case it's a scalar.
-            try:
-                subchunks = key.split(".")[2:]
-                field_name = ".".join(subchunks)
-                for chunk in subchunks:
-                    value = value.get(chunk, None)
-                    if value is None:
-                        return
-            except Exception as err:
-                log.warning(f"{self.name}: {err}")
-                return
-
-            tags = self.tags.copy()
-            if isinstance(keyword.value, dict):
-                for grouper in self.groupers:
-                    if grouper in keyword.value:
-                        tags[grouper] = keyword.value[grouper]
-
-            points.append(
-                {
-                    "measurement": actor,
-                    "tags": tags,
-                    "fields": {field_name: value},
-                }
-            )
+        if self.keywords:
+            fields = {k: fields[k] for k in fields if k in self.keywords}
+
+        tags = self.tags.copy()
+        tags.update(grouppings)
+
+        points = [
+            {
+                "measurement": actor,
+                "tags": tags,
+                "fields": fields,
+            }
+        ]
 
         data_points = DataPoints(data=points, bucket=self.bucket)
 
         self.on_next(data_points)
```

### Comparing `sdss_cerebro-1.0.3/cerebro/sources/drift.py` & `sdss_cerebro-1.1.0/cerebro/sources/drift.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/sources/lco.py` & `sdss_cerebro-1.1.0/cerebro/sources/lco.py`

 * *Files 7% similar despite different names*

```diff
@@ -141,57 +141,56 @@
 
     async def dimm_data(self):
         """Gathers data from DIMM."""
 
         if self.connection.is_closed():
             raise RuntimeError("Database connection is not open.")
 
+        time_str = self.last_data.strftime("'%Y-%m-%d %H:%M:%S'")
         qdata = self.connection.execute_sql(
-            "SELECT tm, se FROM dimm_data ORDER BY tm DESC LIMIT 10"
+            f"SELECT tm, se, el FROM dimm_data WHERE tm > {time_str} ORDER BY tm DESC"
         )
 
-        valid = list(filter(lambda x: x[0] > self.last_data, qdata))
-
         points = [
             {
                 "measurement": "dimm",
-                "fields": {"seeing": vv[1]},
+                "fields": {"seeing": vv[1], "altitude": vv[2]},
                 "time": vv[0],
                 "tags": self.tags.copy(),
             }
-            for vv in valid
+            for vv in qdata
         ]
 
         return points
 
     async def magellan_data(self):
         """Gathers data from the Magellans."""
 
         if self.connection.is_closed():
             raise RuntimeError("Database connection is not open.")
 
+        time_str = self.last_data.strftime("'%Y-%m-%d %H:%M:%S'")
         qdata = self.connection.execute_sql(
-            "SELECT tm, un, fw FROM magellan_data WHERE fw IS NOT NULL AND fw > 0 "
-            "ORDER BY tm DESC LIMIT 10"
+            "SELECT tm, un, fw, az, el FROM magellan_data "
+            f"WHERE fw IS NOT NULL AND fw > 0 AND tm > {time_str}"
+            "ORDER BY tm DESC"
         )
 
-        valid = list(filter(lambda x: x[0] > self.last_data, qdata))
-
         points = []
         tags = self.tags.copy()
 
-        for vv in valid:
+        for vv in qdata:
             if vv[1] == 0:
                 telescope = "baade"
             else:
                 telescope = "clay"
 
             points.append(
                 {
                     "measurement": "magellan",
-                    "fields": {"seeing": vv[2]},
+                    "fields": {"seeing": vv[2], "azimuth": vv[3], "altitude": vv[4]},
                     "time": vv[0],
                     "tags": {**tags, "telescope": telescope},
                 }
             )
 
         return points
```

### Comparing `sdss_cerebro-1.0.3/cerebro/sources/lvm.py` & `sdss_cerebro-1.1.0/cerebro/sources/lvm.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/sources/source.py` & `sdss_cerebro-1.1.0/cerebro/sources/source.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/sources/tpm.py` & `sdss_cerebro-1.1.0/cerebro/sources/tpm.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/cerebro/sources/tron.py` & `sdss_cerebro-1.1.0/cerebro/sources/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_cerebro-1.0.3/pyproject.toml` & `sdss_cerebro-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-cerebro"
-version = "1.0.3"
+version = "1.1.0"
 description = "Telemetry management and time series for SDSS-V"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/cerebro"
 repository = "https://github.com/sdss/cerebro"
 documentation = "https://sdss-cerebro.readthedocs.io/en/latest/"
@@ -28,15 +28,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8,<4.0"
 numpy = "^1.17.4"
 sdsstools = ">=0.5.1"
 influxdb-client = {version="^1.9.0", extras=["extra"]}
 click = "^8.0.0"
-sdss-clu = "^1.5.5"
+sdss-clu = "^2.0.0"
 ntplib = "^0.3.4"
 daemonocle = "^1.0.2"
 click-default-group = "^1.2.2"
 sdss-drift = "^1.0.1"
 rx = "^3.2.0"
 pymysql = "^1.0.2"
 peewee = "^3.15.4"
```

### Comparing `sdss_cerebro-1.0.3/PKG-INFO` & `sdss_cerebro-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-cerebro
-Version: 1.0.3
+Version: 1.1.0
 Summary: Telemetry management and time series for SDSS-V
 Home-page: https://github.com/sdss/cerebro
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
@@ -25,15 +25,15 @@
 Requires-Dist: daemonocle (>=1.0.2,<2.0.0)
 Requires-Dist: influxdb-client[extra] (>=1.9.0,<2.0.0)
 Requires-Dist: ntplib (>=0.3.4,<0.4.0)
 Requires-Dist: numpy (>=1.17.4,<2.0.0)
 Requires-Dist: peewee (>=3.15.4,<4.0.0)
 Requires-Dist: pymysql (>=1.0.2,<2.0.0)
 Requires-Dist: rx (>=3.2.0,<4.0.0)
-Requires-Dist: sdss-clu (>=1.5.5,<2.0.0)
+Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
 Requires-Dist: sdss-drift (>=1.0.1,<2.0.0)
 Requires-Dist: sdsstools (>=0.5.1)
 Project-URL: Documentation, https://sdss-cerebro.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sdss/cerebro
 Description-Content-Type: text/markdown
 
 # cerebro
```

