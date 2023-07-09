# Comparing `tmp/asyncpg_stubs-0.27.0.tar.gz` & `tmp/asyncpg_stubs-0.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpg_stubs-0.27.0.tar", max compression
+gzip compressed data, was "asyncpg_stubs-0.27.1.tar", max compression
```

## Comparing `asyncpg_stubs-0.27.0.tar` & `asyncpg_stubs-0.27.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1501 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/LICENSE
--rw-r--r--   0        0        0     1503 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/README.md
--rw-r--r--   0        0        0      263 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/__init__.pyi
--rw-r--r--   0        0        0     2739 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/_testbase/__init__.pyi
--rw-r--r--   0        0        0     1915 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/_testbase/fuzzer.pyi
--rw-r--r--   0        0        0       61 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/_version.pyi
--rw-r--r--   0        0        0     3246 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/cluster.pyi
--rw-r--r--   0        0        0      410 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/compat.pyi
--rw-r--r--   0        0        0     1548 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/connect_utils.pyi
--rw-r--r--   0        0        0    12796 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/connection.pyi
--rw-r--r--   0        0        0      358 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/connresource.pyi
--rw-r--r--   0        0        0     3233 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/cursor.pyi
--rw-r--r--   0        0        0    30328 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/exceptions/__init__.pyi
--rw-r--r--   0        0        0     2869 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/exceptions/_base.pyi
--rw-r--r--   0        0        0      394 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/introspection.pyi
--rw-r--r--   0        0        0        0 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/pgproto/__init__.pyi
--rw-r--r--   0        0        0      347 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/pgproto/pgproto.pyi
--rw-r--r--   0        0        0     3259 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/pgproto/types.pyi
--rw-r--r--   0        0        0    18118 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/pool.pyi
--rw-r--r--   0        0        0     1800 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/prepared_stmt.pyi
--rw-r--r--   0        0        0      156 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/protocol/__init__.pyi
--rw-r--r--   0        0        0        0 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/protocol/codecs/__init__.pyi
--rw-r--r--   0        0        0     9796 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/protocol/protocol.pyi
--rw-r--r--   0        0        0      209 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/serverversion.pyi
--rw-r--r--   0        0        0     1159 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/transaction.pyi
--rw-r--r--   0        0        0     2335 2022-10-26 22:38:40.837294 asyncpg_stubs-0.27.0/asyncpg-stubs/types.pyi
--rw-r--r--   0        0        0      250 2022-10-26 22:38:40.841294 asyncpg_stubs-0.27.0/asyncpg-stubs/utils.pyi
--rw-r--r--   0        0        0     1466 2022-10-26 22:39:00.574707 asyncpg_stubs-0.27.0/pyproject.toml
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 asyncpg_stubs-0.27.0/setup.py
--rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 asyncpg_stubs-0.27.0/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/LICENSE
+-rw-r--r--   0        0        0     1503 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/README.md
+-rw-r--r--   0        0        0      263 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2732 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/_testbase/__init__.pyi
+-rw-r--r--   0        0        0     1783 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/_testbase/fuzzer.pyi
+-rw-r--r--   0        0        0       61 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/_version.pyi
+-rw-r--r--   0        0        0     3246 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/cluster.pyi
+-rw-r--r--   0        0        0      410 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/compat.pyi
+-rw-r--r--   0        0        0     1548 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/connect_utils.pyi
+-rw-r--r--   0        0        0    12796 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/connection.pyi
+-rw-r--r--   0        0        0      358 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/connresource.pyi
+-rw-r--r--   0        0        0     3233 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/cursor.pyi
+-rw-r--r--   0        0        0    30376 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/__init__.pyi
+-rw-r--r--   0        0        0     2869 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/_base.pyi
+-rw-r--r--   0        0        0      394 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/introspection.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/__init__.pyi
+-rw-r--r--   0        0        0      347 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/pgproto.pyi
+-rw-r--r--   0        0        0     3254 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/types.pyi
+-rw-r--r--   0        0        0    18090 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/pool.pyi
+-rw-r--r--   0        0        0     1800 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/prepared_stmt.pyi
+-rw-r--r--   0        0        0      156 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/codecs/__init__.pyi
+-rw-r--r--   0        0        0     9672 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/protocol.pyi
+-rw-r--r--   0        0        0      205 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/serverversion.pyi
+-rw-r--r--   0        0        0     1159 2023-07-09 19:00:47.420211 asyncpg_stubs-0.27.1/asyncpg-stubs/transaction.pyi
+-rw-r--r--   0        0        0     2335 2023-07-09 19:00:47.424211 asyncpg_stubs-0.27.1/asyncpg-stubs/types.pyi
+-rw-r--r--   0        0        0      250 2023-07-09 19:00:47.424211 asyncpg_stubs-0.27.1/asyncpg-stubs/utils.pyi
+-rw-r--r--   0        0        0     2179 2023-07-09 19:01:06.420640 asyncpg_stubs-0.27.1/pyproject.toml
+-rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 asyncpg_stubs-0.27.1/PKG-INFO
```

### Comparing `asyncpg_stubs-0.27.0/LICENSE` & `asyncpg_stubs-0.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/README.md` & `asyncpg_stubs-0.27.1/README.md`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/_testbase/__init__.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/_testbase/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     @classmethod
     def get_proxy_settings(cls) -> Any: ...
     @classmethod
     def setUpClass(cls) -> None: ...
     @classmethod
     def tearDownClass(cls) -> None: ...
     @classmethod
-    def get_connection_spec(cls, kwargs: Any) -> Any: ...  # type: ignore[override] # noqa
+    def get_connection_spec(cls, kwargs: Any) -> Any: ...  # type: ignore[override]
     def tearDown(self) -> None: ...
 
 def with_connection_options(**options: Any) -> Any: ...
 
 class ConnectedTestCase(ClusterTestCase):
     con: Any = ...
     server_version: Any = ...
```

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/cluster.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/cluster.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/connect_utils.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/connect_utils.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/connection.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/cursor.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/cursor.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/exceptions/__init__.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -884,15 +884,15 @@
     'GroupingError',
     'HeldCursorRequiresSameIsolationLevelError',
     'IdleInTransactionSessionTimeoutError',
     'IdleSessionTimeoutError',
     'ImplicitZeroBitPadding',
     'InFailedSQLTransactionError',
     'InappropriateAccessModeForBranchTransactionError',
-    'InappropriateIsolationLevelForBranchTransactionError',
+    'InappropriateIsolationLevelForBranchTransactionError',  # noqa: PYI053
     'IndeterminateCollationError',
     'IndeterminateDatatypeError',
     'IndexCorruptedError',
     'IndicatorOverflowError',
     'InsufficientPrivilegeError',
     'InsufficientResourcesError',
     'IntegrityConstraintViolationError',
@@ -990,15 +990,15 @@
     'PostgresIOError',
     'PostgresSyntaxError',
     'PostgresSystemError',
     'PostgresWarning',
     'PrivilegeNotGranted',
     'PrivilegeNotRevoked',
     'ProgramLimitExceededError',
-    'ProhibitedExternalRoutineSQLStatementAttemptedError',
+    'ProhibitedExternalRoutineSQLStatementAttemptedError',  # noqa: PYI053
     'ProhibitedSQLStatementAttemptedError',
     'ProtocolViolationError',
     'QueryCanceledError',
     'RaiseError',
     'ReadOnlySQLTransactionError',
     'ReadingExternalRoutineSQLDataNotPermittedError',
     'ReadingSQLDataNotPermittedError',
@@ -1014,15 +1014,15 @@
     'SavepointError',
     'SchemaAndDataStatementMixingNotSupportedError',
     'SequenceGeneratorLimitExceededError',
     'SerializationError',
     'SingletonSQLJsonItemRequiredError',
     'SnapshotTooOldError',
     'SrfProtocolViolatedError',
-    'StackedDiagnosticsAccessedWithoutActiveHandlerError',
+    'StackedDiagnosticsAccessedWithoutActiveHandlerError',  # noqa: PYI053
     'StatementCompletionUnknownError',
     'StatementTooComplexError',
     'StringDataLengthMismatchError',
     'StringDataRightTruncation',
     'StringDataRightTruncationError',
     'SubstringError',
     'SyntaxOrAccessError',
```

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/exceptions/_base.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/exceptions/_base.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/pgproto/types.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/pgproto/types.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import builtins
 from _typeshed import Self
 from collections.abc import Iterator, Sequence
-from typing import Any, SupportsFloat, overload
+from typing import SupportsFloat, overload
 from typing_extensions import Literal, SupportsIndex, TypeAlias
 
 __all__ = (
     'BitString',
     'Point',
     'Path',
     'Polygon',
```

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/pool.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/pool.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     transaction,
     types,
 )
 from .protocol import protocol as _cprotocol
 
 _Connection = TypeVar('_Connection', bound=connection.Connection[Any])
 _Record = TypeVar('_Record', bound=protocol.Record)
-_OtherRecord = TypeVar("_OtherRecord", bound=protocol.Record)
+_OtherRecord = TypeVar('_OtherRecord', bound=protocol.Record)
 
 class _SetupCallback(Protocol[_Record]):
     async def __call__(self, __proxy: PoolConnectionProxy[_Record]) -> None: ...
 
 class _InitCallback(Protocol[_Record]):
     async def __call__(self, __con: connection.Connection[_Record]) -> None: ...
 
@@ -522,53 +522,52 @@
 def create_pool(
     dsn: str | None = ...,
     *,
     min_size: int = ...,
     max_size: int = ...,
     max_queries: int = ...,
     max_inactive_connection_lifetime: float = ...,
-    setup: _SetupCallback[protocol.Record] | None = ...,
-    init: _InitCallback[protocol.Record] | None = ...,
+    setup: _SetupCallback[_Record] | None = ...,
+    init: _InitCallback[_Record] | None = ...,
     loop: AbstractEventLoop | None = ...,
-    connection_class: type[connection.Connection[protocol.Record]] = ...,
-    record_class: type[protocol.Record] = ...,
+    connection_class: type[connection.Connection[_Record]] = ...,
+    record_class: type[_Record],
     host: connection._HostType | None = ...,
     port: connection._PortType | None = ...,
     user: str | None = ...,
     password: connect_utils._PasswordType | None = ...,
     passfile: str | None = ...,
     database: str | None = ...,
     timeout: float = ...,
     statement_cache_size: int = ...,
     max_cached_statement_lifetime: int = ...,
     max_cacheable_statement_size: int = ...,
     command_timeout: float | None = ...,
     ssl: connection._SSLType | None = ...,
     server_settings: dict[str, str] | None = ...,
-) -> Pool[protocol.Record]: ...
+) -> Pool[_Record]: ...
 @overload
 def create_pool(
     dsn: str | None = ...,
     *,
     min_size: int = ...,
     max_size: int = ...,
     max_queries: int = ...,
     max_inactive_connection_lifetime: float = ...,
-    setup: _SetupCallback[_Record] | None = ...,
-    init: _InitCallback[_Record] | None = ...,
+    setup: _SetupCallback[protocol.Record] | None = ...,
+    init: _InitCallback[protocol.Record] | None = ...,
     loop: AbstractEventLoop | None = ...,
-    connection_class: type[_Connection] = ...,
-    record_class: type[_Record],
+    connection_class: type[connection.Connection[protocol.Record]] = ...,
     host: connection._HostType | None = ...,
     port: connection._PortType | None = ...,
     user: str | None = ...,
     password: connect_utils._PasswordType | None = ...,
     passfile: str | None = ...,
     database: str | None = ...,
     timeout: float = ...,
     statement_cache_size: int = ...,
     max_cached_statement_lifetime: int = ...,
     max_cacheable_statement_size: int = ...,
     command_timeout: float | None = ...,
     ssl: connection._SSLType | None = ...,
     server_settings: dict[str, str] | None = ...,
-) -> Pool[_Record]: ...
+) -> Pool[protocol.Record]: ...
```

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/prepared_stmt.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/prepared_stmt.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/protocol/protocol.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/protocol/protocol.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 
 import asyncpg.pgproto.pgproto
 
 from ..connect_utils import _ConnectionParameters
 from ..pgproto.pgproto import WriteBuffer
 from ..types import Attribute, Type
 
-_T = TypeVar("_T")
-_Record = TypeVar("_Record", bound=Record)
-_OtherRecord = TypeVar("_OtherRecord", bound=Record)
+_T = TypeVar('_T')
+_Record = TypeVar('_Record', bound=Record)
+_OtherRecord = TypeVar('_OtherRecord', bound=Record)
 _PreparedStatementState = TypeVar(
-    "_PreparedStatementState", bound=PreparedStatementState[Any]
+    '_PreparedStatementState', bound=PreparedStatementState[Any]
 )
 
-_NoTimeoutType = NewType("_NoTimeoutType", object)
+_NoTimeoutType = NewType('_NoTimeoutType', object)
 _TimeoutType: TypeAlias = float | None | _NoTimeoutType
 
 BUILTIN_TYPE_NAME_MAP: Final[dict[str, int]]
 BUILTIN_TYPE_OID_MAP: Final[dict[int, str]]
 NO_TIMEOUT: Final[_NoTimeoutType]
 
-hashlib_md5 = md5  # noqa: Y026
+hashlib_md5 = md5
 
 @final
 class ConnectionSettings(asyncpg.pgproto.pgproto.CodecContext):
-    __pyx_vtable__: Any = ...
+    __pyx_vtable__: Any
     def __init__(self, conn_key: object) -> None: ...
     def add_python_codec(
         self,
         typeoid: int,
         typename: str,
         typeschema: str,
         typekind: str,
@@ -62,21 +62,21 @@
         format: object = ...,
     ) -> Any: ...
     def __getattr__(self, name: str) -> Any: ...
     def __reduce__(self) -> Any: ...
 
 @final
 class PreparedStatementState(Generic[_Record]):
-    closed: bool = ...
-    name: str = ...
-    query: str = ...
-    refs: int = ...
-    record_class: type[_Record] = ...
-    ignore_custom_codec: bool = ...
-    __pyx_vtable__: Any = ...
+    closed: bool
+    name: str
+    query: str
+    refs: int
+    record_class: type[_Record]
+    ignore_custom_codec: bool
+    __pyx_vtable__: Any
     def __init__(
         self,
         name: str,
         query: str,
         protocol: BaseProtocol[Any],
         record_class: type[_Record],
         ignore_custom_codec: bool,
@@ -87,25 +87,25 @@
     def _init_codecs(self) -> None: ...
     def attach(self) -> None: ...
     def detach(self) -> None: ...
     def mark_closed(self) -> None: ...
     def __reduce__(self) -> Any: ...
 
 class CoreProtocol:
-    backend_pid: Any = ...
-    backend_secret: Any = ...
-    __pyx_vtable__: Any = ...
+    backend_pid: Any
+    backend_secret: Any
+    __pyx_vtable__: Any
     def __init__(self, con_params: _ConnectionParameters) -> None: ...
     def is_in_transaction(self) -> bool: ...
     def __reduce__(self) -> Any: ...
 
 class BaseProtocol(CoreProtocol, Generic[_Record]):
-    queries_count: Any = ...
-    is_ssl: bool = ...
-    __pyx_vtable__: Any = ...
+    queries_count: Any
+    is_ssl: bool
+    __pyx_vtable__: Any
     def __init__(
         self,
         addr: object,
         connected_fut: object,
         con_params: _ConnectionParameters,
         record_class: type[_Record],
         loop: object,
@@ -199,29 +199,29 @@
     ) -> PreparedStatementState[_OtherRecord]: ...
     async def query(self, *args: object, **kwargs: object) -> str: ...
     def resume_writing(self, *args: object, **kwargs: object) -> Any: ...
     def __reduce__(self) -> Any: ...
 
 @final
 class Codec:
-    __pyx_vtable__: Any = ...
+    __pyx_vtable__: Any
     def __init__(
         self,
         name: str,
         schema: str,
         kind: str,
         type: int,
         format: int,
         xformat: int,
         c_encoder: object,
     ) -> None: ...
     def __reduce__(self) -> Any: ...
 
 class DataCodecConfig:
-    __pyx_vtable__: Any = ...
+    __pyx_vtable__: Any
     def __init__(self, cache_key: object) -> None: ...
     def add_python_codec(
         self,
         typeoid: int,
         typename: str,
         typeschema: str,
         typekind: str,
@@ -274,15 +274,15 @@
     def get_remaining_budget(self) -> float: ...
     def has_budget_greater_than(self, amount: float) -> bool: ...
 
 @final
 class SCRAMAuthentication:
     AUTHENTICATION_METHODS: ClassVar[list[str]]
     DEFAULT_CLIENT_NONCE_BYTES: ClassVar[int]
-    DIGEST = sha256  # noqa: Y026
+    DIGEST = sha256
     REQUIREMENTS_CLIENT_FINAL_MESSAGE: ClassVar[list[str]]
     REQUIREMENTS_CLIENT_PROOF: ClassVar[list[str]]
     SASLPREP_PROHIBITED: ClassVar[tuple[Callable[[str], bool], ...]]
     authentication_method: bytes
     authorization_message: bytes | None
     client_channel_binding: bytes
     client_first_message_bare: bytes | None
```

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/transaction.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/transaction.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/asyncpg-stubs/types.pyi` & `asyncpg_stubs-0.27.1/asyncpg-stubs/types.pyi`

 * *Files identical despite different names*

### Comparing `asyncpg_stubs-0.27.0/PKG-INFO` & `asyncpg_stubs-0.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpg-stubs
-Version: 0.27.0
+Version: 0.27.1
 Summary: asyncpg stubs
 Home-page: https://github.com/bryanforbes/asyncpg-stubs
 License: BSD-3-Clause
 Author: Bryan Forbes
 Author-email: bryan@reigndropsfall.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

