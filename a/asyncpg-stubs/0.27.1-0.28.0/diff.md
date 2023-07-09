# Comparing `tmp/asyncpg_stubs-0.27.1.tar.gz` & `tmp/asyncpg_stubs-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpg_stubs-0.27.1.tar", max compression
+gzip compressed data, was "asyncpg_stubs-0.28.0.tar", max compression
```

## Comparing `asyncpg_stubs-0.27.1.tar` & `asyncpg_stubs-0.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1501 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/LICENSE
--rw-r--r--   0        0        0     1503 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/README.md
--rw-r--r--   0        0        0      263 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/__init__.pyi
--rw-r--r--   0        0        0     2732 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/_testbase/__init__.pyi
--rw-r--r--   0        0        0     1783 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/_testbase/fuzzer.pyi
--rw-r--r--   0        0        0       61 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/_version.pyi
--rw-r--r--   0        0        0     3246 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/cluster.pyi
--rw-r--r--   0        0        0      410 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/compat.pyi
--rw-r--r--   0        0        0     1548 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/connect_utils.pyi
--rw-r--r--   0        0        0    12796 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/connection.pyi
--rw-r--r--   0        0        0      358 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/connresource.pyi
--rw-r--r--   0        0        0     3233 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/cursor.pyi
--rw-r--r--   0        0        0    30376 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/__init__.pyi
--rw-r--r--   0        0        0     2869 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/_base.pyi
--rw-r--r--   0        0        0      394 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/introspection.pyi
--rw-r--r--   0        0        0        0 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/__init__.pyi
--rw-r--r--   0        0        0      347 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/pgproto.pyi
--rw-r--r--   0        0        0     3254 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/types.pyi
--rw-r--r--   0        0        0    18090 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pool.pyi
--rw-r--r--   0        0        0     1800 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/prepared_stmt.pyi
--rw-r--r--   0        0        0      156 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/__init__.pyi
--rw-r--r--   0        0        0        0 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/codecs/__init__.pyi
--rw-r--r--   0        0        0     9672 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/protocol.pyi
--rw-r--r--   0        0        0      205 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/serverversion.pyi
--rw-r--r--   0        0        0     1159 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/transaction.pyi
--rw-r--r--   0        0        0     2335 2023-07-09 19:00:47.424211 asyncpg_stubs-0.27.1/asyncpg-stubs/types.pyi
--rw-r--r--   0        0        0      250 2023-07-09 19:00:47.424211 asyncpg_stubs-0.27.1/asyncpg-stubs/utils.pyi
--rw-r--r--   0        0        0     2179 2023-07-09 19:01:06.420640 asyncpg_stubs-0.27.1/pyproject.toml
--rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 asyncpg_stubs-0.27.1/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/LICENSE
+-rw-r--r--   0        0        0     1503 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/README.md
+-rw-r--r--   0        0        0      263 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/__init__.pyi
+-rw-r--r--   0        0        0     3163 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/_testbase/__init__.pyi
+-rw-r--r--   0        0        0     1783 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/_testbase/fuzzer.pyi
+-rw-r--r--   0        0        0       61 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/_version.pyi
+-rw-r--r--   0        0        0     3246 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/cluster.pyi
+-rw-r--r--   0        0        0      410 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/compat.pyi
+-rw-r--r--   0        0        0     1876 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/connect_utils.pyi
+-rw-r--r--   0        0        0    13009 2023-07-09 19:09:45.858612 asyncpg_stubs-0.28.0/asyncpg-stubs/connection.pyi
+-rw-r--r--   0        0        0      358 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/connresource.pyi
+-rw-r--r--   0        0        0     3233 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/cursor.pyi
+-rw-r--r--   0        0        0    30376 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/exceptions/__init__.pyi
+-rw-r--r--   0        0        0     2972 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/exceptions/_base.pyi
+-rw-r--r--   0        0        0      394 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/introspection.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/pgproto/__init__.pyi
+-rw-r--r--   0        0        0      347 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/pgproto/pgproto.pyi
+-rw-r--r--   0        0        0     3254 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/pgproto/types.pyi
+-rw-r--r--   0        0        0    18128 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/pool.pyi
+-rw-r--r--   0        0        0     1800 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/prepared_stmt.pyi
+-rw-r--r--   0        0        0      156 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/protocol/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/protocol/codecs/__init__.pyi
+-rw-r--r--   0        0        0     9672 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/protocol/protocol.pyi
+-rw-r--r--   0        0        0      205 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/serverversion.pyi
+-rw-r--r--   0        0        0     1179 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/transaction.pyi
+-rw-r--r--   0        0        0     2335 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/types.pyi
+-rw-r--r--   0        0        0      250 2023-07-09 19:09:45.862612 asyncpg_stubs-0.28.0/asyncpg-stubs/utils.pyi
+-rw-r--r--   0        0        0     2179 2023-07-09 19:10:06.894957 asyncpg_stubs-0.28.0/pyproject.toml
+-rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 asyncpg_stubs-0.28.0/PKG-INFO
```

### Comparing `asyncpg_stubs-0.27.1/LICENSE` & `asyncpg_stubs-0.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/README.md` & `asyncpg_stubs-0.28.0/README.md`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/_testbase/__init__.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/_testbase/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -81,7 +81,19 @@
 def with_connection_options(**options: Any) -> Any: ...
 
 class ConnectedTestCase(ClusterTestCase):
     con: Any = ...
     server_version: Any = ...
     def setUp(self) -> None: ...
     def tearDown(self) -> None: ...
+
+class HotStandbyTestCase(ClusterTestCase):
+    @classmethod
+    def setup_cluster(cls) -> None: ...
+    @classmethod
+    def get_cluster_connection_spec(cls, cluster: Any, kwargs: Any = ...) -> Any: ...
+    @classmethod
+    def get_connection_spec(cls, kwargs: Any = ...) -> Any: ...
+    @classmethod
+    def connect_primary(cls, **kwargs: Any) -> Any: ...
+    @classmethod
+    def connect_standby(cls, **kwargs: Any) -> Any: ...
```

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/_testbase/fuzzer.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/_testbase/fuzzer.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/cluster.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/cluster.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/connect_utils.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/connect_utils.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from _typeshed import Self
 from asyncio import AbstractEventLoop, Future, Protocol
 from collections.abc import Awaitable, Callable
-from enum import IntEnum
+from enum import Enum, IntEnum
 from ssl import SSLContext
-from typing import NamedTuple
+from typing import Any, NamedTuple
 from typing_extensions import Final, Literal, TypeAlias
 
+from . import connection
+
 _ParsedSSLType: TypeAlias = SSLContext | Literal[False]
 _PasswordType: TypeAlias = str | Callable[[], str] | Callable[[], Awaitable[str]]
 
 PGPASSFILE: Final[str]
 
 class SSLMode(IntEnum):
     disable: int
@@ -26,14 +28,15 @@
     password: _PasswordType | None
     database: str
     ssl: _ParsedSSLType | None
     sslmode: SSLMode | None
     direct_tls: bool
     connect_timeout: float
     server_settings: dict[str, str] | None
+    target_session_attrs: SessionAttribute
 
 class _ClientConfiguration(NamedTuple):
     command_timeout: float | None
     statement_cache_size: int
     max_cached_statement_lifetime: int
     max_cacheable_statement_size: int
 
@@ -49,7 +52,19 @@
         host: str,
         port: int,
         ssl_context: SSLContext,
         ssl_is_advisory: bool | None,
     ) -> None: ...
     def data_received(self, data: bytes) -> None: ...
     def connection_lost(self, exc: Exception | None) -> None: ...
+
+class SessionAttribute(str, Enum):
+    any: str
+    primary: str
+    standby: str
+    prefer_standby: str
+    read_write: str
+    read_only: str
+
+target_attrs_check: Final[
+    dict[SessionAttribute, Callable[[connection.Connection[Any]], Any]]
+]
```

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/connection.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/connection.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -358,14 +358,15 @@
     max_cached_statement_lifetime: int = ...,
     max_cacheable_statement_size: int = ...,
     command_timeout: float | None = ...,
     ssl: _SSLType | None = ...,
     direct_tls: bool = ...,
     record_class: type[_Record],
     server_settings: dict[str, str] | None = ...,
+    target_session_attrs: connect_utils.SessionAttribute | None = ...,
 ) -> Connection[_Record]: ...
 @overload
 async def connect(
     dsn: str | None = ...,
     *,
     host: _HostType | None = ...,
     port: _PortType | None = ...,
@@ -380,14 +381,15 @@
     max_cacheable_statement_size: int = ...,
     command_timeout: float | None = ...,
     ssl: _SSLType | None = ...,
     direct_tls: bool = ...,
     connection_class: type[_Connection],
     record_class: type[_Record] = ...,
     server_settings: dict[str, str] | None = ...,
+    target_session_attrs: connect_utils.SessionAttribute | None = ...,
 ) -> _Connection: ...
 @overload
 async def connect(
     dsn: str | None = ...,
     *,
     host: _HostType | None = ...,
     port: _PortType | None = ...,
@@ -400,14 +402,15 @@
     statement_cache_size: int = ...,
     max_cached_statement_lifetime: int = ...,
     max_cacheable_statement_size: int = ...,
     command_timeout: float | None = ...,
     ssl: _SSLType | None = ...,
     direct_tls: bool = ...,
     server_settings: dict[str, str] | None = ...,
+    target_session_attrs: connect_utils.SessionAttribute | None = ...,
 ) -> Connection[protocol.Record]: ...
 
 class _ConnectionProxy(Generic[_Record]):
     __slots__ = ()
 
 class ServerCapabilities(NamedTuple):
     advisory_locks: bool
```

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/cursor.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/cursor.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/__init__.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/exceptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/_base.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/exceptions/_base.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     'InterfaceError',
     'InterfaceWarning',
     'PostgresLogMessage',
     'InternalClientError',
     'OutdatedSchemaCacheError',
     'ProtocolError',
     'UnsupportedClientFeatureError',
+    'TargetServerAttributeNotMatched',
 )
 
 _PM = TypeVar('_PM', bound=PostgresMessage)
 
 class PostgresMessageMeta(type): ...
 
 class PostgresMessage(metaclass=PostgresMessageMeta):
@@ -78,14 +79,15 @@
         *,
         detail: str | None = ...,
         hint: str | None = ...,
     ) -> None: ...
 
 class InternalClientError(Exception): ...
 class ProtocolError(InternalClientError): ...
+class TargetServerAttributeNotMatched(InternalClientError): ...
 
 class OutdatedSchemaCacheError(InternalClientError):
     schema_name: str | None
     data_type_name: str | None
     position: str | None
     def __init__(
         self,
```

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/types.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/pgproto/types.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/pool.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/pool.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -336,14 +336,15 @@
         setup: _SetupCallback[_Record] | None,
         init: _InitCallback[_Record] | None,
         loop: AbstractEventLoop | None,
         connection_class: type[_Connection],
         record_class: type[_Record],
         **connect_kwargs: object,
     ) -> None: ...
+    def is_closing(self) -> bool: ...
     def get_size(self) -> int: ...
     def get_min_size(self) -> int: ...
     def get_max_size(self) -> int: ...
     def get_idle_size(self) -> int: ...
     def set_connect_args(
         self,
         dsn: str | None = ...,
```

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/prepared_stmt.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/prepared_stmt.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/protocol.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/protocol/protocol.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/transaction.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/transaction.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     NEW: int
     STARTED: int
     COMMITTED: int
     ROLLEDBACK: int
     FAILED: int
 
 _IsolationLevels: TypeAlias = Literal[
-    'read_committed', 'serializable', 'repeatable_read'
+    'read_committed', 'read_uncommitted', 'serializable', 'repeatable_read'
 ]
 ISOLATION_LEVELS: Final[set[_IsolationLevels]]
 ISOLATION_LEVELS_BY_VALUE: Final[dict[str, _IsolationLevels]]
 
 class Transaction(connresource.ConnectionResource):
     __slots__ = (
         '_connection',
```

### Comparing `asyncpg_stubs-0.27.1/asyncpg-stubs/types.pyi` & `asyncpg_stubs-0.28.0/asyncpg-stubs/types.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.1/pyproject.toml` & `asyncpg_stubs-0.28.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpg-stubs"
-version = "0.27.1"
+version = "0.28.0"
 description = "asyncpg stubs"
 homepage = "https://github.com/bryanforbes/asyncpg-stubs"
 authors = ["Bryan Forbes <bryan@reigndropsfall.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [
   { include = "asyncpg-stubs" }
@@ -13,15 +13,15 @@
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-asyncpg = ">=0.27,<0.28"
+asyncpg = ">=0.28,<0.29"
 typing-extensions = "^4.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 pre-commit = "2.21.0"
 mypy = "1.4.1"
 ruff = "0.0.277"
```

### Comparing `asyncpg_stubs-0.27.1/PKG-INFO` & `asyncpg_stubs-0.28.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpg-stubs
-Version: 0.27.1
+Version: 0.28.0
 Summary: asyncpg stubs
 Home-page: https://github.com/bryanforbes/asyncpg-stubs
 License: BSD-3-Clause
 Author: Bryan Forbes
 Author-email: bryan@reigndropsfall.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Dist: asyncpg (>=0.27,<0.28)
+Requires-Dist: asyncpg (>=0.28,<0.29)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # asyncpg-stubs
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/bryanforbes/asyncpg-stubs/blob/master/LICENSE)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
```

