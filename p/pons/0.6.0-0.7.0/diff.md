# Comparing `tmp/pons-0.6.0.tar.gz` & `tmp/pons-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pons-0.6.0.tar", last modified: Thu May 11 22:24:26 2023, max compression
+gzip compressed data, was "pons-0.7.0.tar", last modified: Sun Jul  9 20:57:11 2023, max compression
```

## Comparing `pons-0.6.0.tar` & `pons-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
--rw-r--r--   0        0        0      177 2022-04-23 23:56:47.860000 pons-0.6.0/.coveragerc
--rw-r--r--   0        0        0     1055 2022-02-27 04:36:26.110000 pons-0.6.0/LICENSE.md
--rw-r--r--   0        0        0     1051 2022-06-06 01:00:07.570000 pons-0.6.0/README.md
--rw-r--r--   0        0        0      638 2022-02-28 05:30:25.300000 pons-0.6.0/docs/Makefile
--rw-r--r--   0        0        0     4503 2022-08-06 01:36:45.100000 pons-0.6.0/docs/api.rst
--rw-r--r--   0        0        0     4366 2023-05-11 22:23:05.214707 pons-0.6.0/docs/changelog.rst
--rw-r--r--   0        0        0     2565 2023-02-05 09:02:39.350000 pons-0.6.0/docs/conf.py
--rw-r--r--   0        0        0     3177 2022-09-14 20:33:08.940000 pons-0.6.0/docs/index.rst
--rw-r--r--   0        0        0     6890 2022-11-10 22:51:25.580000 pons-0.6.0/docs/tutorial.rst
--rw-r--r--   0        0        0      164 2023-01-21 08:19:29.290000 pons-0.6.0/mypy.ini
--rw-r--r--   0        0        0      617 2022-08-25 00:47:15.620000 pons-0.6.0/pons/__init__.py
--rw-r--r--   0        0        0    18449 2023-05-07 07:14:33.518659 pons-0.6.0/pons/_abi_types.py
--rw-r--r--   0        0        0    29113 2022-11-11 23:30:57.740000 pons-0.6.0/pons/_client.py
--rw-r--r--   0        0        0     7317 2022-08-17 18:47:24.899999 pons-0.6.0/pons/_contract.py
--rw-r--r--   0        0        0    27975 2023-05-07 07:14:33.518858 pons-0.6.0/pons/_contract_abi.py
--rw-r--r--   0        0        0    19283 2023-02-05 00:19:21.360000 pons-0.6.0/pons/_entities.py
--rw-r--r--   0        0        0     5431 2022-08-17 18:47:24.899999 pons-0.6.0/pons/_provider.py
--rw-r--r--   0        0        0     1227 2022-08-17 18:47:24.899999 pons-0.6.0/pons/_signer.py
--rw-r--r--   0        0        0      757 2022-04-24 22:22:36.230000 pons-0.6.0/pons/abi.py
--rw-r--r--   0        0        0        0 2022-04-23 23:56:47.860000 pons-0.6.0/pons/py.typed
--rw-r--r--   0        0        0     1215 2023-05-11 22:22:15.121564 pons-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       26 2022-04-25 23:59:46.280000 pons-0.6.0/pytest.ini
--rw-r--r--   0        0        0     2399 2022-06-05 01:05:34.940000 pons-0.6.0/tests/TestClient.sol
--rw-r--r--   0        0        0      939 2022-05-25 05:17:34.620000 pons-0.6.0/tests/TestContract.sol
--rw-r--r--   0        0        0     2045 2022-05-29 07:42:02.330000 pons-0.6.0/tests/TestContractFunctionality.sol
--rw-r--r--   0        0        0      343 2022-03-06 23:50:17.740000 pons-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      640 2022-05-24 03:06:04.490000 pons-0.6.0/tests/compile.py
--rw-r--r--   0        0        0      585 2022-06-05 01:05:34.940000 pons-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0    10942 2023-02-05 00:19:21.180000 pons-0.6.0/tests/provider.py
--rw-r--r--   0        0        0     2648 2022-09-14 20:33:08.940000 pons-0.6.0/tests/provider_server.py
--rw-r--r--   0        0        0    11696 2023-02-05 00:19:21.410000 pons-0.6.0/tests/test_abi_types.py
--rw-r--r--   0        0        0    34366 2023-05-07 07:14:33.519168 pons-0.6.0/tests/test_client.py
--rw-r--r--   0        0        0     4556 2022-06-05 06:14:54.790000 pons-0.6.0/tests/test_contract.py
--rw-r--r--   0        0        0    24721 2023-05-07 07:14:33.519340 pons-0.6.0/tests/test_contract_abi.py
--rw-r--r--   0        0        0     5030 2023-02-05 00:19:21.100000 pons-0.6.0/tests/test_contract_functionality.py
--rw-r--r--   0        0        0    12097 2023-02-05 00:19:21.350000 pons-0.6.0/tests/test_entities.py
--rw-r--r--   0        0        0     6662 2023-02-05 00:19:21.149999 pons-0.6.0/tests/test_provider.py
--rw-r--r--   0        0        0     1209 2022-06-05 01:05:34.950000 pons-0.6.0/tests/test_signer.py
--rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 pons-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      177 2022-04-23 23:56:47.860000 pons-0.7.0/.coveragerc
+-rw-r--r--   0        0        0     1055 2022-02-27 04:36:26.110000 pons-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     1051 2022-06-06 01:00:07.570000 pons-0.7.0/README.md
+-rw-r--r--   0        0        0      638 2022-02-28 05:30:25.300000 pons-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0     4665 2023-06-01 23:14:39.716552 pons-0.7.0/docs/api.rst
+-rw-r--r--   0        0        0     5097 2023-07-09 20:51:06.297956 pons-0.7.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2565 2023-02-05 09:02:39.350000 pons-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0     3177 2022-09-14 20:33:08.940000 pons-0.7.0/docs/index.rst
+-rw-r--r--   0        0        0     7116 2023-06-01 23:14:39.717149 pons-0.7.0/docs/tutorial.rst
+-rw-r--r--   0        0        0      164 2023-06-02 00:42:13.657633 pons-0.7.0/mypy.ini
+-rw-r--r--   0        0        0      768 2023-06-01 23:14:39.717416 pons-0.7.0/pons/__init__.py
+-rw-r--r--   0        0        0    18498 2023-05-31 23:30:41.956540 pons-0.7.0/pons/_abi_types.py
+-rw-r--r--   0        0        0    29885 2023-06-01 23:14:39.717747 pons-0.7.0/pons/_client.py
+-rw-r--r--   0        0        0     6174 2023-06-01 23:14:39.717918 pons-0.7.0/pons/_contract.py
+-rw-r--r--   0        0        0    26702 2023-06-01 23:14:39.718290 pons-0.7.0/pons/_contract_abi.py
+-rw-r--r--   0        0        0    19703 2023-05-31 23:30:41.957089 pons-0.7.0/pons/_entities.py
+-rw-r--r--   0        0        0     6384 2023-05-31 23:30:41.957231 pons-0.7.0/pons/_fallback_provider.py
+-rw-r--r--   0        0        0     6329 2023-05-31 23:30:41.957394 pons-0.7.0/pons/_provider.py
+-rw-r--r--   0        0        0     1227 2022-08-17 18:47:24.899999 pons-0.7.0/pons/_signer.py
+-rw-r--r--   0        0        0      757 2022-04-24 22:22:36.230000 pons-0.7.0/pons/abi.py
+-rw-r--r--   0        0        0        0 2022-04-23 23:56:47.860000 pons-0.7.0/pons/py.typed
+-rw-r--r--   0        0        0     1215 2023-07-09 20:51:35.471942 pons-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2022-04-25 23:59:46.280000 pons-0.7.0/pytest.ini
+-rw-r--r--   0        0        0      887 2023-06-01 05:58:07.212219 pons-0.7.0/tests/MockMulticall.sol
+-rw-r--r--   0        0        0     2399 2022-06-05 01:05:34.940000 pons-0.7.0/tests/TestClient.sol
+-rw-r--r--   0        0        0      939 2022-05-25 05:17:34.620000 pons-0.7.0/tests/TestContract.sol
+-rw-r--r--   0        0        0     2165 2023-06-01 23:14:39.718768 pons-0.7.0/tests/TestContractFunctionality.sol
+-rw-r--r--   0        0        0      343 2022-03-06 23:50:17.740000 pons-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      640 2022-05-24 03:06:04.490000 pons-0.7.0/tests/compile.py
+-rw-r--r--   0        0        0      585 2022-06-05 01:05:34.940000 pons-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0    10957 2023-06-01 23:14:39.718925 pons-0.7.0/tests/provider.py
+-rw-r--r--   0        0        0     2648 2022-09-14 20:33:08.940000 pons-0.7.0/tests/provider_server.py
+-rw-r--r--   0        0        0    11849 2023-05-31 23:30:41.957552 pons-0.7.0/tests/test_abi_types.py
+-rw-r--r--   0        0        0    35138 2023-06-01 23:14:39.719144 pons-0.7.0/tests/test_client.py
+-rw-r--r--   0        0        0     4513 2023-06-01 23:14:39.719300 pons-0.7.0/tests/test_contract.py
+-rw-r--r--   0        0        0    22359 2023-06-01 23:14:39.719514 pons-0.7.0/tests/test_contract_abi.py
+-rw-r--r--   0        0        0     6520 2023-06-01 23:14:39.719775 pons-0.7.0/tests/test_contract_functionality.py
+-rw-r--r--   0        0        0    12207 2023-05-26 17:16:32.160667 pons-0.7.0/tests/test_entities.py
+-rw-r--r--   0        0        0     7854 2023-05-31 23:30:41.957944 pons-0.7.0/tests/test_fallback_provider.py
+-rw-r--r--   0        0        0     1982 2023-06-01 22:02:43.711692 pons-0.7.0/tests/test_multicall.py
+-rw-r--r--   0        0        0     7389 2023-05-31 23:30:41.958172 pons-0.7.0/tests/test_provider.py
+-rw-r--r--   0        0        0     1209 2022-06-05 01:05:34.950000 pons-0.7.0/tests/test_signer.py
+-rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 pons-0.7.0/PKG-INFO
```

### Comparing `pons-0.6.0/LICENSE.md` & `pons-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/README.md` & `pons-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/docs/Makefile` & `pons-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/docs/api.rst` & `pons-0.7.0/docs/api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,33 @@
 
 .. autoclass:: pons._provider.Provider
 
 .. autoclass:: HTTPProvider
    :show-inheritance:
 
 
+Fallback providers
+------------------
+
+.. autoclass:: FallbackProvider
+   :show-inheritance:
+
+.. autoclass:: CycleFallback
+   :show-inheritance:
+
+.. autoclass:: PriorityFallback
+   :show-inheritance:
+
+.. autoclass:: FallbackStrategyFactory
+   :members:
+
+.. autoclass:: FallbackStrategy
+   :members:
+
+
 Errors
 ------
 
 .. autoclass:: pons.ABIDecodingError
 
 .. autoclass:: pons.RemoteError
 
@@ -69,25 +88,22 @@
 
 Contract ABI
 ------------
 
 .. autoclass:: ContractABI
    :members:
 
-.. autoclass:: Constructor
+.. autoclass:: Mutability
    :members:
-   :special-members: __call__
 
-.. autoclass:: ReadMethod
-   :show-inheritance:
+.. autoclass:: Constructor
    :members:
    :special-members: __call__
 
-.. autoclass:: WriteMethod
-   :show-inheritance:
+.. autoclass:: Method
    :members:
    :special-members: __call__
 
 .. autoclass:: Event
    :members:
 
 .. autoclass:: Error
@@ -102,42 +118,32 @@
 
 Secondary classes
 -----------------
 
 .. autoclass:: pons._contract_abi.ConstructorCall()
    :members:
 
-.. autoclass:: pons._contract_abi.ReadCall()
-   :members:
-
-.. autoclass:: pons._contract_abi.WriteCall()
+.. autoclass:: pons._contract_abi.MethodCall()
    :members:
 
 .. autoclass:: pons._contract_abi.EventFilter()
    :members:
 
 .. autoclass:: pons._contract.BoundConstructor()
    :members:
    :special-members: __call__
 
 .. autoclass:: pons._contract.BoundConstructorCall()
    :members:
 
-.. autoclass:: pons._contract.BoundReadMethod()
+.. autoclass:: pons._contract.BoundMethod()
    :members:
    :special-members: __call__
 
-.. autoclass:: pons._contract.BoundReadCall()
-   :members:
-
-.. autoclass:: pons._contract.BoundWriteMethod()
-   :members:
-   :special-members: __call__
-
-.. autoclass:: pons._contract.BoundWriteCall()
+.. autoclass:: pons._contract.BoundMethodCall()
    :members:
 
 .. autoclass:: pons._contract.BoundEvent()
    :members:
    :special-members: __call__
 
 .. autoclass:: pons._contract.BoundEventFilter()
@@ -214,14 +220,19 @@
 .. autoclass:: pons._entities.LogFilter()
 
 .. autoclass:: pons._entities.LogTopic()
 
 .. autoclass:: pons._entities.LogEntry()
    :members:
 
+.. class:: JSON
+
+   A JSON-ifiable object (``bool``, ``int``, ``float``, ``str``, ``None``,
+   iterable of ``JSON``, or mapping of ``str`` to ``JSON``).
+
 
 Solidity types
 --------------
 
 Type aliases are exported from the ``abi`` submodule.
 Arrays can be obtained from ``Type`` objects by indexing them (either with an integer for a fixed-size array, or with ``...`` for a variable-sized array).
```

### Comparing `pons-0.6.0/docs/changelog.rst` & `pons-0.7.0/docs/changelog.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 Changelog
 ---------
 
 
+0.7.0 (09-07-2023)
+~~~~~~~~~~~~~~~~~~
+
+Changed
+^^^^^^^
+
+- ``ReadMethod`` and ``WriteMethod`` were merged into ``Method`` (with the corresponding merge of ``ContractABI`` routing objects and various bound calls). (PR_50_)
+
+
+Added
+^^^^^
+
+- ``Block.SAFE`` and ``Block.FINALIZED`` values. (PR_48_)
+- ``FallbackProvider``, two strategies for it (``CycleFallback`` and ``PriorityFallback``), and a framework for creating user-defined strategies (``FallbackStrategy`` and ``FallbackStrategyFactory``). (PR_49_)
+- ``Mutability`` enum for defining contract method mutability. (PR_50_)
+
+
+.. _PR_48: https://github.com/fjarri/pons/pull/48
+.. _PR_49: https://github.com/fjarri/pons/pull/49
+.. _PR_50: https://github.com/fjarri/pons/pull/50
+
+
+
 0.6.0 (11-05-2023)
 ~~~~~~~~~~~~~~~~~~
 
 Changed
 ^^^^^^^
 
 - Parameter names and fields coinciding with Python keywords have ``_`` appended to them on the creation of ABI objects. (PR_47_)
```

### Comparing `pons-0.6.0/docs/conf.py` & `pons-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/docs/index.rst` & `pons-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/docs/tutorial.rst` & `pons-0.7.0/docs/tutorial.rst`

 * *Files 4% similar despite different names*

```diff
@@ -54,93 +54,99 @@
 
 ::
 
     {
         constructor(uint256 _v1, uint256 _v2) nonpayable
         fallback() nonpayable
         receive() payable
-        function getState(uint256 _x) returns (uint256)
-        function testStructs((uint256,uint256) inner_in, ((uint256,uint256),uint256) outer_in) returns ((uint256,uint256) inner_out, ((uint256,uint256),uint256) outer_out)
-        function v1() returns (uint256)
-        function v2() returns (uint256)
+        function getState(uint256 _x) view returns (uint256)
+        function testStructs((uint256,uint256) inner_in, ((uint256,uint256),uint256) outer_in) view returns ((uint256,uint256) inner_out, ((uint256,uint256),uint256) outer_out)
+        function v1() view returns (uint256)
+        function v2() view returns (uint256)
         function setState(uint256 _v1) nonpayable
     }
 
 Alternatively, one can define only the methods they need directly in Python code:
 
 ::
 
-    from pons import ContractABI, abi, Constructor, WriteMethod, ReadMethod
+    from pons import ContractABI, abi, Constructor, Method, Mutability
 
     inner_struct = abi.struct(inner1=abi.uint(256), inner2=abi.uint(256))
     outer_struct = abi.struct(inner=inner_struct, outer1=abi.uint(256))
     cabi = ContractABI(
         constructor=Constructor(inputs=dict(_v1=abi.uint(256), _v2=abi.uint(256))),
-        write=[
-            WriteMethod(name='setState', inputs=dict(_v1=abi.uint(256)))
-        ],
-        read=[
-            ReadMethod(name='getState', inputs=dict(_x=abi.uint(256)), outputs=abi.uint(256)),
-            ReadMethod(
+        methods=[
+            Method(
+                name='setState',
+                mutability=Mutability.NONPAYABLE,
+                inputs=dict(_v1=abi.uint(256)))
+            Method(
+                name='getState',
+                mutability=Mutability.VIEW,
+                inputs=dict(_x=abi.uint(256)),
+                outputs=abi.uint(256)),
+            Method(
                 name='testStructs',
+                mutability=Mutability.VIEW,
                 inputs=dict(inner_in=inner_struct, outer_in=outer_struct),
                 outputs=dict(inner_out=inner_struct, outer_out=outer_struct),
                 )
             ]
         )
 
     print(cabi)
 
 ::
 
     {
         constructor(uint256 _v1, uint256 _v2) nonpayable
-        function getState(uint256 _x) returns (uint256)
-        function testStructs((uint256,uint256) inner_in, ((uint256,uint256),uint256) outer_in) returns ((uint256,uint256) inner_out, ((uint256,uint256),uint256) outer_out)
+        function getState(uint256 _x) view returns (uint256)
+        function testStructs((uint256,uint256) inner_in, ((uint256,uint256),uint256) outer_in) view returns ((uint256,uint256) inner_out, ((uint256,uint256),uint256) outer_out)
         function setState(uint256 _v1) nonpayable
     }
 
 
 Contract methods
 ----------------
 
 All the enumerated methods have corresponding objects that can be accessed via :py:class:`~pons.ContractABI` fields (see the API reference for details).
 For example,
 
 ::
 
-    print(cabi.read.getState)
+    print(cabi.method.getState)
 
 ::
 
-    function getState(uint256 _x) returns (uint256)
+    function getState(uint256 _x) view returns (uint256)
 
 With a specific method object one can create a contract call by, naturally, calling the object.
 The arguments are processed the same as in Python functions, so one can either use positional arguments, keyword ones (if the parameter names are present in the contract ABI), or mix the two.
 
 ::
 
-    call = cabi.read.getState(1)
-    call = cabi.read.getState(_x=1)
+    call = cabi.method.getState(1)
+    call = cabi.method.getState(_x=1)
 
 Note that the arguments are checked and encoded on call creation, so any inconsistency will result in a raised exception:
 
 ::
 
-    call = cabi.read.getState(1, 2)
+    call = cabi.method.getState(1, 2)
 
 ::
 
     Traceback (most recent call last):
     ...
     TypeError: too many positional arguments
 
 ::
 
-    call = cabi.read.getState("a")
+    call = cabi.method.getState("a")
 
 ::
 
     Traceback (most recent call last):
     ...
     TypeError: `uint256` must correspond to an integer, got str
 
@@ -172,19 +178,19 @@
 A :py:class:`~pons.DeployedContract` object wraps all ABI method objects into "bound" state, similarly to how Python methods are bound to class instances.
 It means that all the method calls created from this object have the contract address inside them, so that it does not need to be provided every time.
 
 For example, to call a non-mutating contract method via :py:meth:`~pons._client.ClientSession.eth_call`:
 
 ::
 
-    call = deployed_contract.read.getState(1)
+    call = deployed_contract.method.getState(1)
     result = await session.eth_call(call)
 
 Note that when the :py:class:`~pons.ContractABI` object is created from the JSON ABI, even if the method returns a single value, it is still represented as a list of one element in the JSON, so the ``result`` will be a list too.
 If the ABI is declared programmatically, one can provide a single output value instead of the list, and then ``pons`` will unpack that list.
 
 Naturally, a mutating call requires a signer to be provided:
 
 ::
 
-    call = deployed_contract.write.setState(1)
+    call = deployed_contract.method.setState(1)
     await session.transact(signer, call)
```

### Comparing `pons-0.6.0/pons/__init__.py` & `pons-0.7.0/pons/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,25 +8,32 @@
     ContractError,
     TransactionFailed,
     ProviderError,
 )
 from ._contract_abi import (
     ContractABI,
     Constructor,
-    ReadMethod,
-    WriteMethod,
+    Method,
     Event,
     Error,
     Fallback,
     Receive,
     Either,
+    Mutability,
 )
 from ._contract import CompiledContract, DeployedContract
 from ._entities import (
     Amount,
     Address,
     Block,
     TxHash,
     BlockHash,
 )
-from ._provider import HTTPProvider, Unreachable
+from ._fallback_provider import (
+    FallbackProvider,
+    FallbackStrategy,
+    FallbackStrategyFactory,
+    CycleFallback,
+    PriorityFallback,
+)
+from ._provider import HTTPProvider, Unreachable, JSON
 from ._signer import Signer, AccountSigner
```

### Comparing `pons-0.6.0/pons/_abi_types.py` & `pons-0.7.0/pons/_abi_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,18 @@
 
 class ABIDecodingError(Exception):
     """
     Raised on an error when decoding a value in an Eth ABI encoded bytestring.
     """
 
 
-# TODO: currently mypy does not support recursive type aliases,
-# make it recursive when it's possible.
-# See https://github.com/python/mypy/issues/731
-ABIType = Any
+ABIType = Union[int, str, bytes, bool, List["ABIType"]]
 """
-Represents the type that can be received from ``eth_decode()``.
-``ABIType = Union[int, str, bytes, bool, List[ABIType]]``
+Represents the argument type that can be received from ``eth_abi.decode()``,
+or passed to ``eth_abi.encode()``.
 """
 
 
 def encode_typed(types: Iterable[str], args: Iterable[ABIType]) -> bytes:
     # ``eth_abi.encode()`` does not have type annotations.
     # This is a typed wrapper (easier than making custom stubs).
     # Remove when typing is added in ``eth_abi``.
@@ -164,15 +161,15 @@
                 f"under {self._bits} bits, got {val}"
             )
         return int(val)
 
     def _normalize(self, val: Any) -> int:
         return self._check_val(val)
 
-    def _denormalize(self, val: Any) -> int:
+    def _denormalize(self, val: ABIType) -> int:
         return self._check_val(val)
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, UInt) and self._bits == other._bits
 
 
 class Int(Type):
@@ -202,15 +199,15 @@
                 f"under {self._bits} bits, got {val}"
             )
         return int(val)
 
     def _normalize(self, val: Any) -> int:
         return self._check_val(val)
 
-    def _denormalize(self, val: Any) -> int:
+    def _denormalize(self, val: ABIType) -> int:
         return self._check_val(val)
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, Int) and self._bits == other._bits
 
 
 class Bytes(Type):
@@ -236,15 +233,15 @@
         if self._size is not None and len(val) != self._size:
             raise ValueError(f"Expected {self._size} bytes, got {len(val)}")
         return val
 
     def _normalize(self, val: Any) -> bytes:
         return self._check_val(val)
 
-    def _denormalize(self, val: Any) -> bytes:
+    def _denormalize(self, val: ABIType) -> bytes:
         return self._check_val(val)
 
     def _encode_to_topic_outer(self, val: bytes) -> bytes:
         if self._size is None:
             # Dynamic `bytes` is a reference type and is therefore hashed.
             return keccak(val)
         # Sized `bytes` is a value type, falls back to the base implementation.
@@ -274,23 +271,25 @@
     Not to be confused with :py:class:`~pons.Address` which represents an address value.
     """
 
     @property
     def canonical_form(self) -> str:
         return "address"
 
-    def _normalize(self, val: Any) -> bytes:
+    def _normalize(self, val: Any) -> str:
         if not isinstance(val, Address):
             raise TypeError(
                 f"`address` must correspond to an `Address`-type value, "
                 f"got {type(val).__name__}"
             )
-        return bytes(val)
+        return val.checksum
 
-    def _denormalize(self, val: str) -> Address:
+    def _denormalize(self, val: ABIType) -> Address:
+        if not isinstance(val, str):
+            raise TypeError(f"Expected a string to convert to `Address`, got {type(val).__name__}")
         return Address.from_hex(val)
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, AddressType)
 
 
 class String(Type):
@@ -308,15 +307,15 @@
                 f"`string` must correspond to a `str`-type value, got {type(val).__name__}"
             )
         return val
 
     def _normalize(self, val: Any) -> str:
         return self._check_val(val)
 
-    def _denormalize(self, val: Any) -> str:
+    def _denormalize(self, val: ABIType) -> str:
         return self._check_val(val)
 
     def _encode_to_topic_outer(self, val: str) -> bytes:
         # `string` is encoded and treated as dynamic `bytes`
         return Bytes()._encode_to_topic_outer(val.encode())
 
     def _encode_to_topic_inner(self, val: str) -> bytes:
@@ -346,15 +345,15 @@
                 f"`bool` must correspond to a `bool`-type value, got {type(val).__name__}"
             )
         return val
 
     def _normalize(self, val: Any) -> bool:
         return self._check_val(val)
 
-    def _denormalize(self, val: Any) -> bool:
+    def _denormalize(self, val: ABIType) -> bool:
         return self._check_val(val)
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, Bool)
 
 
 class Array(Type):
@@ -378,15 +377,15 @@
         if self._size is not None and len(val) != self._size:
             raise ValueError(f"Expected {self._size} elements, got {len(val)}")
         return val
 
     def _normalize(self, val: Any) -> List[ABIType]:
         return [self._element_type._normalize(item) for item in self._check_val(val)]
 
-    def _denormalize(self, val: Any) -> List[ABIType]:
+    def _denormalize(self, val: ABIType) -> List[ABIType]:
         return [self._element_type._denormalize(item) for item in self._check_val(val)]
 
     def _encode_to_topic_outer(self, val: Any) -> bytes:
         return keccak(self._encode_to_topic_inner(val))
 
     def _encode_to_topic_inner(self, val: Any) -> bytes:
         return b"".join(self._element_type._encode_to_topic_inner(elem) for elem in val)
@@ -428,15 +427,15 @@
                     f"Expected fields {list(self._fields.keys())}, got {list(val.keys())}"
                 )
             return [tp._normalize(val[name]) for name, tp in self._fields.items()]
         return [
             tp._normalize(item) for item, tp in zip(self._check_val(val), self._fields.values())
         ]
 
-    def _denormalize(self, val: Any) -> Dict[str, ABIType]:
+    def _denormalize(self, val: ABIType) -> Dict[str, ABIType]:
         return {
             name: tp._denormalize(item)
             for item, (name, tp) in zip(self._check_val(val), self._fields.items())
         }
 
     def _encode_to_topic_outer(self, val: Any) -> bytes:
         return keccak(self._encode_to_topic_inner(val))
```

### Comparing `pons-0.6.0/pons/_client.py` & `pons-0.7.0/pons/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,15 @@
     ParamSpec = lambda _: [Any]  # pragma: no cover
 
 import anyio
 
 from ._contract import (
     DeployedContract,
     BoundConstructorCall,
-    BoundReadCall,
-    BoundWriteCall,
+    BoundMethodCall,
     BoundEventFilter,
 )
 from ._contract_abi import EventFilter, PANIC_ERROR, LEGACY_ERROR, UnknownError, ContractABI, Error
 from ._provider import (
     Provider,
     ProviderSession,
     UnexpectedResponse,
@@ -50,14 +49,17 @@
 from ._entities import (
     Address,
     Amount,
     Block,
     BlockFilter,
     PendingTransactionFilter,
     LogFilter,
+    BlockFilterId,
+    PendingTransactionFilterId,
+    LogFilterId,
     LogEntry,
     BlockHash,
     TxHash,
     BlockInfo,
     TxReceipt,
     TxInfo,
     rpc_encode_quantity,
@@ -416,15 +418,15 @@
         while True:
             receipt = await self.eth_get_transaction_receipt(tx_hash)
             if receipt is not None:
                 return receipt
             await anyio.sleep(poll_latency)
 
     @rpc_call("eth_call")
-    async def eth_call(self, call: BoundReadCall, block: Union[int, Block] = Block.LATEST) -> Any:
+    async def eth_call(self, call: BoundMethodCall, block: Union[int, Block] = Block.LATEST) -> Any:
         """
         Sends a prepared contact method call to the provided address.
         Returns the decoded output.
         """
         result = await self._provider_session.rpc(
             "eth_call",
             {
@@ -483,15 +485,15 @@
         tx = {
             "from": source_address.rpc_encode(),
             "to": destination_address.rpc_encode(),
             "value": amount.rpc_encode(),
         }
         return await self._estimate_gas(tx)
 
-    async def estimate_transact(self, call: BoundWriteCall, amount: Amount = Amount(0)) -> int:
+    async def estimate_transact(self, call: BoundMethodCall, amount: Amount = Amount(0)) -> int:
         """
         Estimates the amount of gas required to transact with a contract.
 
         Raises :py:class:`ContractPanic`, :py:class:`ContractLegacyError`,
         or :py:class:`ContractError` if a known error was caught during the dry run.
         If the error was unknown, falls back to :py:class:`ProviderError`.
         """
@@ -654,18 +656,21 @@
             )
 
         return DeployedContract(call.contract_abi, receipt.contract_address)
 
     async def broadcast_transact(
         self,
         signer: Signer,
-        call: BoundWriteCall,
+        call: BoundMethodCall,
         amount: Amount = Amount(0),
         gas: Optional[int] = None,
     ) -> TxHash:
+        if not call.mutating:
+            raise ValueError("This method is non-mutating, use `eth_call` to invoke it")
+
         if not call.payable and amount.as_wei() != 0:
             raise ValueError("This method does not accept an associated payment")
 
         chain_id = await self.eth_chain_id()
         if gas is None:
             gas = await self.estimate_transact(call, amount=amount)
         # TODO: implement gas strategies
@@ -685,15 +690,15 @@
         }
         signed_tx = signer.sign_transaction(tx)
         return await self._eth_send_raw_transaction(signed_tx)
 
     async def transact(
         self,
         signer: Signer,
-        call: BoundWriteCall,
+        call: BoundMethodCall,
         amount: Amount = Amount(0),
         gas: Optional[int] = None,
     ) -> None:
         """
         Transacts with the contract using a prepared method call.
         If ``gas`` is ``None``, the required amount of gas is estimated first,
         otherwise the provided value is used.
@@ -710,24 +715,28 @@
             raise TransactionFailed(f"Transact failed (receipt: {receipt})")
 
     @rpc_call("eth_newBlockFilter")
     async def eth_new_block_filter(self) -> BlockFilter:
         """
         Calls the ``eth_newBlockFilter`` RPC method.
         """
-        result = await self._provider_session.rpc("eth_newBlockFilter")
-        return BlockFilter.rpc_decode(result)
+        result, provider_path = await self._provider_session.rpc_and_pin("eth_newBlockFilter")
+        filter_id = BlockFilterId.rpc_decode(result)
+        return BlockFilter(id=filter_id, provider_path=provider_path)
 
     @rpc_call("eth_newPendingTransactionFilter")
     async def eth_new_pending_transaction_filter(self) -> PendingTransactionFilter:
         """
         Calls the ``eth_newPendingTransactionFilter`` RPC method.
         """
-        result = await self._provider_session.rpc("eth_newPendingTransactionFilter")
-        return PendingTransactionFilter.rpc_decode(result)
+        result, provider_path = await self._provider_session.rpc_and_pin(
+            "eth_newPendingTransactionFilter"
+        )
+        filter_id = PendingTransactionFilterId.rpc_decode(result)
+        return PendingTransactionFilter(id=filter_id, provider_path=provider_path)
 
     @rpc_call("eth_newFilter")
     async def eth_new_filter(
         self,
         source: Optional[Union[Address, Iterable[Address]]] = None,
         event_filter: Optional[EventFilter] = None,
         from_block: Union[int, Block] = Block.LATEST,
@@ -749,27 +758,34 @@
             for topic in event_filter.topics:
                 if topic is None:
                     encoded_topics.append(None)
                 else:
                     encoded_topics.append([elem.rpc_encode() for elem in topic])
             params["topics"] = encoded_topics
 
-        result = await self._provider_session.rpc("eth_newFilter", params)
-        return LogFilter.rpc_decode(result)
+        result, provider_path = await self._provider_session.rpc_and_pin("eth_newFilter", params)
+        filter_id = LogFilterId.rpc_decode(result)
+        return LogFilter(id=filter_id, provider_path=provider_path)
 
     @rpc_call("eth_getFilterChangers")
     async def eth_get_filter_changes(
         self, filter_: Union[BlockFilter, PendingTransactionFilter, LogFilter]
     ) -> Union[Tuple[BlockHash, ...], Tuple[TxHash, ...], Tuple[LogEntry, ...]]:
         """
         Calls the ``eth_getFilterChangers`` RPC method.
         Depending on what ``filter_`` was, returns a tuple of corresponding results.
         """
         # TODO: split into separate functions wiht specific return types?
-        results = await self._provider_session.rpc("eth_getFilterChanges", filter_.rpc_encode())
+        results = await self._provider_session.rpc_at_pin(
+            filter_.provider_path, "eth_getFilterChanges", filter_.id.rpc_encode()
+        )
+
+        # TODO: this will go away with generalized RPC decoding.
+        if not isinstance(results, list):
+            raise UnexpectedResponse(f"Expected a list as a response, got {type(results).__name__}")
 
         if isinstance(filter_, BlockFilter):
             return tuple(BlockHash.rpc_decode(elem) for elem in results)
         if isinstance(filter_, PendingTransactionFilter):
             return tuple(TxHash.rpc_decode(elem) for elem in results)
         return tuple(LogEntry.rpc_decode(ResponseDict(elem)) for elem in results)
```

### Comparing `pons-0.6.0/pons/_contract.py` & `pons-0.7.0/pons/_contract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from typing import Any, Dict, Tuple, Optional, List
 
 from ._contract_abi import (
     ContractABI,
     Methods,
-    ReadMethod,
-    WriteMethod,
+    Method,
     Event,
     EventFilter,
     Error,
-    Any,
 )
 from ._entities import Address, LogEntry, LogTopic
 from ._provider import JSON
 
 
 class BoundConstructor:
     """
@@ -49,98 +47,73 @@
 
     def __init__(self, contract_abi: ContractABI, data_bytes: bytes, payable: bool):
         self.contract_abi = contract_abi
         self.payable = payable
         self.data_bytes = data_bytes
 
 
-class BoundReadMethod:
+class BoundMethod:
     """
-    A non-mutating method bound to a specific contract's address.
+    A regular method bound to a specific contract's address.
     """
 
-    def __init__(self, contract_address: Address, method: ReadMethod):
-        self._contract_address = contract_address
-        self._method = method
-
-    def __call__(self, *args: Any, **kwargs: Any) -> "BoundReadCall":
-        """
-        Returns a contract call with encoded arguments bound to a specific address.
-        """
-        call = self._method(*args, **kwargs)
-        return BoundReadCall(self._method, self._contract_address, call.data_bytes)
-
-
-class BoundReadCall:
-    """
-    A non-mutating method call with encoded arguments bound to a specific contract address.
-    """
-
-    contract_address: Address
-    """The contract address."""
-
-    data_bytes: bytes
-    """Encoded call arguments with the selector."""
-
-    def __init__(self, method: ReadMethod, contract_address: Address, data_bytes: bytes):
-        self._method = method
-        self.contract_address = contract_address
-        self.data_bytes = data_bytes
-
-    def decode_output(self, output_bytes: bytes) -> Any:
-        """
-        Decodes contract output packed into the bytestring.
-        """
-        return self._method.decode_output(output_bytes)
-
-
-class BoundWriteMethod:
-    """
-    A mutating method bound to a specific contract's address.
-    """
-
-    def __init__(self, contract_abi: ContractABI, contract_address: Address, method: WriteMethod):
+    def __init__(self, contract_abi: ContractABI, contract_address: Address, method: Method):
         self._contract_abi = contract_abi
         self._contract_address = contract_address
         self._method = method
 
-    def __call__(self, *args: Any, **kwargs: Any) -> "BoundWriteCall":
+    def __call__(self, *args: Any, **kwargs: Any) -> "BoundMethodCall":
         """
         Returns a contract call with encoded arguments bound to a specific address.
         """
         call = self._method(*args, **kwargs)
-        return BoundWriteCall(
-            self._contract_abi, self._contract_address, call.data_bytes, self._method.payable
+        return BoundMethodCall(
+            self._contract_abi, self._method, self._contract_address, call.data_bytes
         )
 
 
-class BoundWriteCall:
+class BoundMethodCall:
     """
-    A mutating method call with encoded arguments bound to a specific contract address.
+    A regular method call with encoded arguments bound to a specific contract address.
     """
 
     contract_abi: ContractABI
     """The corresponding contract's ABI"""
 
     contract_address: Address
     """The contract address."""
 
-    payable: bool
-    """Whether this call is payable."""
-
     data_bytes: bytes
     """Encoded call arguments with the selector."""
 
+    payable: bool
+    """Whether this method is marked as ``payable``."""
+
+    mutating: bool
+    """Whether this method is marked as ``payable`` or ``nonpayable``."""
+
     def __init__(
-        self, contract_abi: ContractABI, contract_address: Address, data_bytes: bytes, payable: bool
+        self,
+        contract_abi: ContractABI,
+        method: Method,
+        contract_address: Address,
+        data_bytes: bytes,
     ):
+        self._method = method
         self.contract_abi = contract_abi
-        self.payable = payable
         self.contract_address = contract_address
         self.data_bytes = data_bytes
+        self.payable = self._method.payable
+        self.mutating = self._method.mutating
+
+    def decode_output(self, output_bytes: bytes) -> Any:
+        """
+        Decodes contract output packed into the bytestring.
+        """
+        return self._method.decode_output(output_bytes)
 
 
 class BoundEvent:
     """
     An event creation call with encoded topics bound to a specific contract address.
     """
 
@@ -217,36 +190,27 @@
 
     abi: ContractABI
     """Contract's ABI."""
 
     address: Address
     """Contract's address."""
 
-    read: Methods[BoundReadMethod]
-    """Contract's non-mutating methods bound to the address."""
-
-    write: Methods[BoundWriteMethod]
-    """Contract's mutating methods bound to the address."""
+    method: Methods[BoundMethod]
+    """Contract's regular methods bound to the address."""
 
     event: Methods[BoundEvent]
     """Contract's events bound to the address."""
 
     error: Methods[Error]
     """Contract's errors."""
 
     def __init__(self, abi: ContractABI, address: Address):
         self.abi = abi
         self.address = address
 
-        self.read = Methods(
-            {method.name: BoundReadMethod(self.address, method) for method in self.abi.read}
-        )
-        self.write = Methods(
-            {
-                method.name: BoundWriteMethod(self.abi, self.address, method)
-                for method in self.abi.write
-            }
+        self.method = Methods(
+            {method.name: BoundMethod(self.abi, self.address, method) for method in self.abi.method}
         )
         self.event = Methods(
             {event.name: BoundEvent(self.address, event) for event in self.abi.event}
         )
         self.error = self.abi.error
```

### Comparing `pons-0.6.0/pons/_contract_abi.py` & `pons-0.7.0/pons/_contract_abi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from enum import Enum
 from functools import cached_property
 import inspect
 from itertools import chain
 from keyword import iskeyword
 from typing import (
     Any,
     AbstractSet,
@@ -57,14 +58,18 @@
                     inspect.Parameter(f"_{i}", inspect.Parameter.POSITIONAL_ONLY)
                     for i in range(len(parameters))
                 ]
             )
             self._types = list(parameters)
             self._named_parameters = False
 
+    @property
+    def empty(self) -> bool:
+        return not bool(self._types)
+
     @cached_property
     def canonical_form(self) -> str:
         """
         Returns the signature serialized in the canonical form as a string.
         """
         return "(" + ",".join(tp.canonical_form for tp in self._types) + ")"
 
@@ -208,47 +213,14 @@
         params = []
         for name, tp in self._types.items():
             indexed = "indexed " if name in self._indexed else ""
             params.append(f"{tp.canonical_form} {indexed}{name}")
         return "(" + ", ".join(params) + ")"
 
 
-class Method(ABC):
-    """
-    An abstract type for a method (mutating or non-mutating).
-    """
-
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """
-        Method name.
-        """
-        ...
-
-    @property
-    @abstractmethod
-    def inputs(self) -> Signature:
-        """
-        Method's input signature.
-        """
-        ...
-
-    @cached_property
-    def selector(self) -> bytes:
-        """
-        Method's selector.
-        """
-        return keccak(self.name.encode() + self.inputs.canonical_form.encode())[:4]
-
-    def _encode_call(self, *args: Any, **kwargs: Any) -> bytes:
-        input_bytes = self.inputs.encode(*args, **kwargs)
-        return self.selector + input_bytes
-
-
 class Constructor:
     """
     Contract constructor.
 
     .. note::
 
        If the name of a parameter given to the constructor matches a Python keyword,
@@ -293,61 +265,110 @@
         input_bytes = self.inputs.encode(*args, **kwargs)
         return ConstructorCall(input_bytes)
 
     def __str__(self) -> str:
         return f"constructor{self.inputs} " + ("payable" if self.payable else "nonpayable")
 
 
-class ReadMethod(Method):
+class Mutability(Enum):
+    """
+    Possible states of a contract's method mutability.
+    """
+
+    PURE = "pure"
+    """Solidity's ``pure`` (does not read or write the contract state)."""
+    VIEW = "view"
+    """Solidity's ``view`` (may read the contract state)."""
+    NONPAYABLE = "nonpayable"
+    """Solidity's ``nonpayable`` (may write the contract state)."""
+    PAYABLE = "payable"
+    """
+    Solidity's ``payable`` (may write the contract state
+    and accept associated funds with transactions).
+    """
+
+    @classmethod
+    def from_json(cls, entry: str) -> "Mutability":
+        values = dict(
+            pure=Mutability.PURE,
+            view=Mutability.VIEW,
+            nonpayable=Mutability.NONPAYABLE,
+            payable=Mutability.PAYABLE,
+        )
+        if entry not in values:
+            raise ValueError(f"Unknown mutability identifier: {entry}")
+        return values[entry]
+
+    @property
+    def payable(self) -> bool:
+        return self == Mutability.PAYABLE
+
+    @property
+    def mutating(self) -> bool:
+        return self == Mutability.PAYABLE or self == Mutability.NONPAYABLE
+
+
+class Method:
     """
     A non-mutating contract method.
 
     .. note::
 
        If the name of a parameter (input or output) given to the constructor
        matches a Python keyword, ``_`` will be appended to it.
     """
 
     outputs: Signature
     """Method's output signature."""
 
+    payable: bool
+    """Whether this method is marked as payable."""
+
+    mutating: bool
+    """Whether this method may mutate the contract state."""
+
     @classmethod
-    def from_json(cls, method_entry: Dict[str, Any]) -> "ReadMethod":
+    def from_json(cls, method_entry: Dict[str, Any]) -> "Method":
         """
         Creates this object from a JSON ABI method entry.
         """
         if method_entry["type"] != "function":
-            raise ValueError(
-                "ReadMethod object must be created from a JSON entry with type='function'"
-            )
+            raise ValueError("Method object must be created from a JSON entry with type='function'")
 
         name = method_entry["name"]
         inputs = dispatch_types(method_entry["inputs"])
-        if method_entry["stateMutability"] not in ("pure", "view"):
-            raise ValueError(
-                "Non-mutating method's JSON entry state mutability must be `pure` or `view`"
-            )
+
+        mutability = Mutability.from_json(method_entry["stateMutability"])
 
         # Outputs can be anonymous
         outputs: Union[Dict[str, Type], List[Type]]
-        if all(entry["name"] == "" for entry in method_entry["outputs"]):
+        if "outputs" not in method_entry:
+            outputs = []
+        elif all(entry["name"] == "" for entry in method_entry["outputs"]):
             outputs = [dispatch_type(entry) for entry in method_entry["outputs"]]
         else:
             outputs = dispatch_types(method_entry["outputs"])
 
-        return cls(name=name, inputs=inputs, outputs=outputs)
+        return cls(name=name, inputs=inputs, outputs=outputs, mutability=mutability)
 
     def __init__(
         self,
         name: str,
+        mutability: Mutability,
         inputs: Union[Mapping[str, Type], Sequence[Type]],
-        outputs: Union[Mapping[str, Type], Sequence[Type], Type],
+        outputs: Union[Mapping[str, Type], Sequence[Type], Type, None] = None,
     ):
         self._name = name
         self._inputs = Signature(inputs)
+        self._mutability = mutability
+        self.payable = mutability.payable
+        self.mutating = mutability.mutating
+
+        if outputs is None:
+            outputs = []
 
         if isinstance(outputs, Type):
             outputs = [outputs]
             self._single_output = True
         else:
             self._single_output = False
 
@@ -357,91 +378,46 @@
     def name(self) -> str:
         return self._name
 
     @property
     def inputs(self) -> Signature:
         return self._inputs
 
-    def __call__(self, *args: Any, **kwargs: Any) -> "ReadCall":
+    def __call__(self, *args: Any, **kwargs: Any) -> "MethodCall":
         """
         Returns an encoded call with given arguments.
         """
-        return ReadCall(self._encode_call(*args, **kwargs))
+        return MethodCall(self._encode_call(*args, **kwargs))
+
+    @cached_property
+    def selector(self) -> bytes:
+        """
+        Method's selector.
+        """
+        return keccak(self.name.encode() + self.inputs.canonical_form.encode())[:4]
+
+    def _encode_call(self, *args: Any, **kwargs: Any) -> bytes:
+        input_bytes = self.inputs.encode(*args, **kwargs)
+        return self.selector + input_bytes
 
     def decode_output(self, output_bytes: bytes) -> Any:
         """
         Decodes the output from ABI-packed bytes.
         """
         results = self.outputs.decode_into_tuple(output_bytes)
         if self._single_output:
             results = results[0]
         return results
 
     def __str__(self) -> str:
-        return f"function {self.name}{self.inputs} returns {self.outputs}"
-
-
-class WriteMethod(Method):
-    """
-    A mutating contract method.
-
-    .. note::
-
-       If the name of a parameter given to the constructor matches a Python keyword,
-       ``_`` will be appended to it.
-    """
-
-    payable: bool
-    """Whether this method is marked as payable"""
-
-    @classmethod
-    def from_json(cls, method_entry: Dict[str, Any]) -> "WriteMethod":
-        """
-        Creates this object from a JSON ABI method entry.
-        """
-        if method_entry["type"] != "function":
-            raise ValueError(
-                "WriteMethod object must be created from a JSON entry with type='function'"
-            )
-
-        name = method_entry["name"]
-        inputs = dispatch_types(method_entry["inputs"])
-        if method_entry["stateMutability"] not in ("nonpayable", "payable"):
-            raise ValueError(
-                "Mutating method's JSON entry state mutability must be `nonpayable` or `payable`"
-            )
-        payable = method_entry["stateMutability"] == "payable"
-        return cls(name=name, inputs=inputs, payable=payable)
-
-    def __init__(
-        self,
-        name: str,
-        inputs: Union[Mapping[str, Type], Sequence[Type]],
-        payable: bool = False,
-    ):
-        self._name = name
-        self._inputs = Signature(inputs)
-        self.payable = payable
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def inputs(self) -> Signature:
-        return self._inputs
-
-    def __call__(self, *args: Any, **kwargs: Any) -> "WriteCall":
-        """
-        Returns an encoded call with given arguments.
-        """
-        return WriteCall(self._encode_call(*args, **kwargs))
-
-    def __str__(self) -> str:
-        return f"function {self.name}{self.inputs} " + ("payable" if self.payable else "nonpayable")
+        if self.outputs.empty:
+            returns = ""
+        else:
+            returns = f" returns {self.outputs}"
+        return f"function {self.name}{self.inputs} {self._mutability.value}{returns}"
 
 
 class Event:
     """
     A contract event.
 
     .. note::
@@ -652,29 +628,17 @@
     input_bytes: bytes
     """Encoded call arguments."""
 
     def __init__(self, input_bytes: bytes):
         self.input_bytes = input_bytes
 
 
-class ReadCall:
+class MethodCall:
     """
-    A call to a contract's non-mutating method.
-    """
-
-    data_bytes: bytes
-    """Encoded call arguments with the selector."""
-
-    def __init__(self, data_bytes: bytes):
-        self.data_bytes = data_bytes
-
-
-class WriteCall:
-    """
-    A call to a contract's mutating method.
+    A call to a contract's regular method.
     """
 
     data_bytes: bytes
     """Encoded call arguments with the selector."""
 
     def __init__(self, data_bytes: bytes):
         self.data_bytes = data_bytes
@@ -736,19 +700,16 @@
 
     fallback: Optional[Fallback]
     """Contract's fallback method."""
 
     receive: Optional[Receive]
     """Contract's receive method."""
 
-    read: Methods[ReadMethod]
-    """Contract's non-mutating methods."""
-
-    write: Methods[WriteMethod]
-    """Contract's mutating methods."""
+    method: Methods[Method]
+    """Contract's regular methods."""
 
     event: Methods[Event]
     """Contract's events."""
 
     error: Methods[Error]
     """Contract's errors."""
 
@@ -756,17 +717,15 @@
     def from_json(cls, json_abi: List[Dict[str, JSON]]) -> "ContractABI":
         """
         Creates this object from a JSON ABI (e.g. generated by a Solidity compiler).
         """
         constructor = None
         fallback = None
         receive = None
-        read = []
-        write = []
-        methods = set()
+        methods = {}
         events = {}
         errors = {}
 
         for entry in json_abi:
             if entry["type"] == "constructor":
                 if constructor:
                     raise ValueError("JSON ABI contains more than one constructor declarations")
@@ -774,21 +733,15 @@
 
             elif entry["type"] == "function":
                 if entry["name"] in methods:
                     # TODO: add support for overloaded methods
                     raise ValueError(
                         f"JSON ABI contains more than one declarations of `{entry['name']}`"
                     )
-
-                methods.add(entry["name"])
-
-                if entry["stateMutability"] in ("pure", "view"):
-                    read.append(ReadMethod.from_json(entry))
-                else:
-                    write.append(WriteMethod.from_json(entry))
+                methods[entry["name"]] = Method.from_json(entry)
 
             elif entry["type"] == "fallback":
                 if fallback:
                     raise ValueError("JSON ABI contains more than one fallback declarations")
                 fallback = Fallback.from_json(entry)
 
             elif entry["type"] == "receive":
@@ -813,38 +766,35 @@
             else:
                 raise ValueError(f"Unknown ABI entry type: {entry['type']}")
 
         return cls(
             constructor=constructor,
             fallback=fallback,
             receive=receive,
-            read=read,
-            write=write,
+            methods=methods.values(),
             events=events.values(),
             errors=errors.values(),
         )
 
     def __init__(
         self,
         constructor: Optional[Constructor] = None,
         fallback: Optional[Fallback] = None,
         receive: Optional[Receive] = None,
-        read: Optional[Iterable[ReadMethod]] = None,
-        write: Optional[Iterable[WriteMethod]] = None,
+        methods: Optional[Iterable[Method]] = None,
         events: Optional[Iterable[Event]] = None,
         errors: Optional[Iterable[Error]] = None,
     ):
         if constructor is None:
             constructor = Constructor(inputs=[])
 
         self.fallback = fallback
         self.receive = receive
         self.constructor = constructor
-        self.read = Methods({method.name: method for method in (read or [])})
-        self.write = Methods({method.name: method for method in (write or [])})
+        self.method = Methods({method.name: method for method in (methods or [])})
         self.event = Methods({event.name: event for event in (events or [])})
         self.error = Methods({error.name: error for error in (errors or [])})
 
         self._error_by_selector = {
             error.selector: error for error in chain([PANIC_ERROR, LEGACY_ERROR], self.error)
         }
 
@@ -862,20 +812,17 @@
             error = self._error_by_selector[selector]
             decoded = error.decode_fields(data)
             return error, decoded
 
         raise UnknownError(f"Could not find an error with selector {selector.hex()} in the ABI")
 
     def __str__(self) -> str:
-        all_methods: Iterable[
-            Union[Constructor, Fallback, Receive, ReadMethod, WriteMethod, Event, Error]
-        ] = chain(
+        all_methods: Iterable[Union[Constructor, Fallback, Receive, Method, Event, Error]] = chain(
             [self.constructor] if self.constructor else [],
             [self.fallback] if self.fallback else [],
             [self.receive] if self.receive else [],
-            self.read,
-            self.write,
+            self.method,
             self.event,
             self.error,
         )
         method_list = ["    " + str(method) for method in all_methods]
         return "{\n" + "\n".join(method_list) + "\n}"
```

### Comparing `pons-0.6.0/pons/_entities.py` & `pons-0.7.0/pons/_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,33 +235,54 @@
 
     EARLIEST = "earliest"
     """The earliest block"""
 
     PENDING = "pending"
     """Currently pending block"""
 
+    SAFE = "safe"
+    """The latest safe head block"""
 
-class BlockFilter(TypedQuantity):
+    FINALIZED = "finalized"
+    """The latest finalized block"""
+
+
+class BlockFilterId(TypedQuantity):
     """
     A block filter identifier (returned by ``eth_newBlockFilter``).
     """
 
 
-class PendingTransactionFilter(TypedQuantity):
+class PendingTransactionFilterId(TypedQuantity):
     """
     A pending transaction filter identifier (returned by ``eth_newPendingTransactionFilter``).
     """
 
 
-class LogFilter(TypedQuantity):
+class LogFilterId(TypedQuantity):
     """
     A log filter identifier (returned by ``eth_newFilter``).
     """
 
 
+class BlockFilter(NamedTuple):
+    id: BlockFilterId
+    provider_path: Tuple[int, ...]
+
+
+class PendingTransactionFilter(NamedTuple):
+    id: PendingTransactionFilterId
+    provider_path: Tuple[int, ...]
+
+
+class LogFilter(NamedTuple):
+    id: LogFilterId
+    provider_path: Tuple[int, ...]
+
+
 class LogTopic(TypedData):
     """
     A log topic for log filtering.
     """
 
     def _length(self) -> int:
         return 32
```

### Comparing `pons-0.6.0/pons/_provider.py` & `pons-0.7.0/pons/_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from abc import ABC, abstractmethod
 from contextlib import asynccontextmanager
 from http import HTTPStatus
-from typing import Any, AsyncIterator, Dict, Optional, Union, cast, Iterable, Mapping
+from typing import Any, AsyncIterator, Dict, Optional, Union, cast, Iterable, Mapping, Tuple
 
 import httpx
 
 
-# TODO: currently mypy does not support recursive type aliases,
-# make it recursive when it's possible.
-# See https://github.com/python/mypy/issues/731
-JSON = Union[bool, int, float, str, None, Iterable[Any], Mapping[str, Any]]
+# TODO: the doc entry had to be written manually for this type because of Sphinx limitations.
+JSON = Union[bool, int, float, str, None, Iterable["JSON"], Mapping[str, "JSON"]]
 
 
 class Provider(ABC):
     """
     The base class for JSON RPC providers.
     """
 
@@ -63,21 +61,41 @@
 
 class ProviderSession(ABC):
     """
     The base class for provider sessions.
     """
 
     @abstractmethod
-    async def rpc(self, method: str, *args: JSON) -> Any:
+    async def rpc(self, method: str, *args: JSON) -> JSON:
         """
         Calls the given RPC method with the already json-ified arguments.
         """
         ...
 
+    async def rpc_and_pin(self, method: str, *args: JSON) -> Tuple[JSON, Tuple[int, ...]]:
+        """
+        Calls the given RPC method and returns the path to the provider it succeded on.
+        This method will be typically overriden by multi-provider implementations.
+        """
+        return await self.rpc(method, *args), ()
+
+    async def rpc_at_pin(self, path: Tuple[int, ...], method: str, *args: JSON) -> JSON:
+        """
+        Calls the given RPC method at the provider by the given path
+        (obtained previously from ``rpc_and_pin()``).
+        This method will be typically overriden by multi-provider implementations.
+        """
+        if path != ():
+            raise ValueError(f"Unexpected provider path: {path}")
+        return await self.rpc(method, *args)
+
     async def rpc_dict(self, method: str, *args: JSON) -> Optional[ResponseDict]:
+        """
+        Calls the given RPC method expecting to get a dictionary (or ``null``) in response.
+        """
         result = await self.rpc(method, *args)
         if result is None:
             return None
         return ResponseDict(result)
 
 
 class HTTPProvider(Provider):
@@ -97,15 +115,15 @@
 class RPCError(Exception):
     """
     A wrapper for a server error returned either as a proper RPC response,
     or as an HTTP error code response.
     """
 
     @classmethod
-    def from_json(cls, response: Dict[str, JSON]) -> "RPCError":
+    def from_json(cls, response: JSON) -> "RPCError":
         error = ResponseDict(response)
         if "data" in error:
             data = error["data"]
             if data is not None and not isinstance(data, str):
                 raise UnexpectedResponse(
                     f"Error data must be a string or None, got {type(data)} ({data})"
                 )
@@ -154,16 +172,17 @@
         try:
             response = await self._client.post(self._url, json=json)
         except Exception as exc:
             raise Unreachable(str(exc)) from exc
         if response.status_code != HTTPStatus.OK:
             raise RPCError(response.status_code, response.content.decode())
 
-        response_json = cast(JSON, response.json())
-        if not isinstance(response_json, dict):
+        response_json = response.json()
+        if not isinstance(response_json, Mapping):
             raise UnexpectedResponse(f"RPC response must be a dictionary, got: {response_json}")
+        # Assuming that the HTTP client knows what it's doing, and gives us a valid JSON dict
+        response_json = cast(Mapping[str, JSON], response_json)
         if "error" in response_json:
             raise RPCError.from_json(response_json["error"])
         if "result" not in response_json:
             raise UnexpectedResponse(f"`result` is not present in the response: {response_json}")
-        # TODO: see the TODO above; when JSON is recursive, this cast won't be necessary.
-        return cast(JSON, response_json["result"])
+        return response_json["result"]
```

### Comparing `pons-0.6.0/pons/_signer.py` & `pons-0.7.0/pons/_signer.py`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/pons/abi.py` & `pons-0.7.0/pons/abi.py`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/pyproject.toml` & `pons-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pons"
-version = "0.6.0"
+version = "0.7.0"
 description = "Async RPC client for Ethereum"
 authors = [
     { name = "Bogdan Opanchuk", email = "bogdan@opanchuk.net" },
 ]
 dependencies = [
     "httpx>=0.22",
     "eth-account>=0.6",
```

### Comparing `pons-0.6.0/tests/TestClient.sol` & `pons-0.7.0/tests/TestClient.sol`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/tests/TestContract.sol` & `pons-0.7.0/tests/TestContract.sol`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/tests/TestContractFunctionality.sol` & `pons-0.7.0/tests/TestContractFunctionality.sol`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     }
 
     fallback(bytes calldata) external returns (bytes memory) {
         v1 = 1;
         v2 = 2;
     }
 
+    function setStateAndReturn(uint256 _v1) public returns (uint256) {
+        v1 = v1 + _v1;
+        return v1;
+    }
+
     function setState(uint256 _v1) public {
         v1 = _v1;
     }
 
     function getState(uint256 _x) public view returns (uint256) {
         return v1 + _x;
     }
```

### Comparing `pons-0.6.0/tests/compile.py` & `pons-0.7.0/tests/compile.py`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/tests/conftest.py` & `pons-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/tests/provider.py` & `pons-0.7.0/tests/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
             # Have to go through this procedure because eth-tester doesn't bother
             # to discriminate between legacy (string) reverts and reverts with custom types.
             try:
                 # raises ValueError if it is not a Python literal
                 reason_data = ast.literal_eval(reason)
                 assert isinstance(reason_data, bytes)  # sanity check
-            except ValueError:
+            except (ValueError, SyntaxError):
                 assert isinstance(reason, str)  # sanity check
                 # Bring `reason_data` to what a `Revert` instance would contain in this case
                 reason_data = _ERROR_SELECTOR + encode_args((abi.string, reason))
 
         else:
             # Shouldn't happen unless the API of eth-tester changes
             raise NotImplementedError() from exc  # pragma: no cover
```

### Comparing `pons-0.6.0/tests/provider_server.py` & `pons-0.7.0/tests/provider_server.py`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/tests/test_abi_types.py` & `pons-0.7.0/tests/test_abi_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,27 +91,30 @@
     with pytest.raises(TypeError, match="`bytes` must correspond to a bytestring, got str"):
         abi.bytes()._normalize("foo")
     with pytest.raises(ValueError, match="Expected 4 bytes, got 3"):
         abi.bytes(4)._normalize(b"foo")
 
 
 def test_address():
-    addr_bytes = b"\x01" * 20
+    addr_bytes = os.urandom(20)
     addr = Address(addr_bytes)
 
-    assert abi.address._normalize(addr) == addr_bytes
-    assert abi.address._denormalize(addr_bytes) == addr
+    assert abi.address._normalize(addr) == addr.checksum
+    assert abi.address._denormalize(addr.checksum) == addr
 
     assert abi.address.canonical_form == "address"
 
     with pytest.raises(
         TypeError, match="`address` must correspond to an `Address`-type value, got str"
     ):
         abi.address._normalize("0x" + "01" * 20)
 
+    with pytest.raises(TypeError, match="Expected a string to convert to `Address`, got bytes"):
+        abi.address._denormalize(addr_bytes)
+
 
 def test_string():
     assert abi.string._normalize("foo") == "foo"
     assert abi.string._denormalize("foo") == "foo"
 
     assert abi.string.canonical_form == "string"
 
@@ -235,15 +238,15 @@
         field4=abi.struct(inner1=abi.bool, inner2=abi.string),
     )
 
     addr = Address(b"\x01" * 20)
 
     value = dict(field1=1, field2=[2, 3], field3=addr, field4=dict(inner2="abcd", inner1=True))
 
-    expected_normalized = [1, [2, 3], bytes(addr), [True, "abcd"]]
+    expected_normalized = [1, [2, 3], addr.checksum, [True, "abcd"]]
 
     # normalize() loses info on struct field names
     assert struct._normalize(value) == expected_normalized
 
     # denormalize() should recover struct field names
     assert struct._denormalize(expected_normalized) == value
```

### Comparing `pons-0.6.0/tests/test_client.py` & `pons-0.7.0/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from pons import (
     abi,
     ABIDecodingError,
     Address,
     Amount,
     ContractABI,
     DeployedContract,
-    ReadMethod,
+    Method,
     TxHash,
     BlockHash,
     Block,
     Either,
     ContractPanic,
     ContractLegacyError,
     ContractError,
+    Mutability,
 )
 from pons._abi_types import keccak, encode_args
 from pons._contract_abi import PANIC_ERROR
 from pons._client import BadResponseFormat, ProviderError, TransactionFailed
 from pons._entities import rpc_encode_data
 from pons._provider import RPCError
 
@@ -155,45 +156,46 @@
 
     assert receipt.succeeded
 
 
 async def test_eth_call(session, compiled_contracts, root_signer):
     compiled_contract = compiled_contracts["BasicContract"]
     deployed_contract = await session.deploy(root_signer, compiled_contract.constructor(123))
-    result = await session.eth_call(deployed_contract.read.getState(456))
+    result = await session.eth_call(deployed_contract.method.getState(456))
     assert result == (123 + 456,)
 
 
 async def test_eth_call_decoding_error(session, compiled_contracts, root_signer):
     """
     Tests that `eth_call()` propagates an error on mismatch of the declared output signature
     and the bytestring received from the provider (as opposed to wrapping it in another exception).
     """
     compiled_contract = compiled_contracts["BasicContract"]
     deployed_contract = await session.deploy(root_signer, compiled_contract.constructor(123))
 
     wrong_abi = ContractABI(
-        read=[
-            ReadMethod(
+        methods=[
+            Method(
                 name="getState",
+                mutability=Mutability.VIEW,
                 inputs=[abi.uint(256)],
                 # the actual method in in BasicContract returns only one uint256
                 outputs=[abi.uint(256), abi.uint(256)],
             )
         ]
     )
     wrong_contract = DeployedContract(abi=wrong_abi, address=deployed_contract.address)
 
     expected_message = (
         r"Could not decode the return value with the expected signature \(uint256,uint256\): "
         r"Tried to read 32 bytes.  Only got 0 bytes"
     )
 
     with pytest.raises(ABIDecodingError, match=expected_message):
-        await session.eth_call(wrong_contract.read.getState(456))
+        await session.eth_call(wrong_contract.method.getState(456))
 
 
 async def test_estimate_deploy(session, compiled_contracts):
     compiled_contract = compiled_contracts["BasicContract"]
     gas = await session.estimate_deploy(compiled_contract.constructor(1))
     assert isinstance(gas, int) and gas > 0
 
@@ -212,15 +214,15 @@
             root_signer.address, another_signer.address, Amount.ether(1000)
         )
 
 
 async def test_estimate_transact(session, compiled_contracts, root_signer):
     compiled_contract = compiled_contracts["BasicContract"]
     deployed_contract = await session.deploy(root_signer, compiled_contract.constructor(1))
-    gas = await session.estimate_transact(deployed_contract.write.setState(456))
+    gas = await session.estimate_transact(deployed_contract.method.setState(456))
     assert isinstance(gas, int) and gas > 0
 
 
 async def test_eth_gas_price(session):
     gas_price = await session.eth_gas_price()
     assert isinstance(gas_price, Amount)
 
@@ -282,15 +284,15 @@
 async def test_deploy(test_provider, session, compiled_contracts, root_signer):
     basic_contract = compiled_contracts["BasicContract"]
     construction_error = compiled_contracts["TestErrors"]
     payable_constructor = compiled_contracts["PayableConstructor"]
 
     # Normal deploy
     deployed_contract = await session.deploy(root_signer, basic_contract.constructor(123))
-    result = await session.eth_call(deployed_contract.read.getState(456))
+    result = await session.eth_call(deployed_contract.method.getState(456))
     assert result == (123 + 456,)
 
     with pytest.raises(ValueError, match="This constructor does not accept an associated payment"):
         await session.deploy(root_signer, basic_contract.constructor(1), Amount.ether(1))
 
     # Explicit payment equal to zero is the same as no payment
     await session.deploy(root_signer, basic_contract.constructor(1), Amount.ether(0))
@@ -327,34 +329,39 @@
 
 
 async def test_transact(test_provider, session, compiled_contracts, root_signer):
     basic_contract = compiled_contracts["BasicContract"]
 
     # Normal transact
     deployed_contract = await session.deploy(root_signer, basic_contract.constructor(123))
-    await session.transact(root_signer, deployed_contract.write.setState(456))
-    result = await session.eth_call(deployed_contract.read.getState(789))
+    await session.transact(root_signer, deployed_contract.method.setState(456))
+    result = await session.eth_call(deployed_contract.method.getState(789))
     assert result == (456 + 789,)
 
+    with pytest.raises(
+        ValueError, match="This method is non-mutating, use `eth_call` to invoke it"
+    ):
+        await session.transact(root_signer, deployed_contract.method.getState(456))
+
     with pytest.raises(ValueError, match="This method does not accept an associated payment"):
-        await session.transact(root_signer, deployed_contract.write.setState(456), Amount.ether(1))
+        await session.transact(root_signer, deployed_contract.method.setState(456), Amount.ether(1))
 
     # Explicit payment equal to zero is the same as no payment
-    await session.transact(root_signer, deployed_contract.write.setState(456), Amount.ether(0))
+    await session.transact(root_signer, deployed_contract.method.setState(456), Amount.ether(0))
 
     # Payable transact
     await session.transact(
-        root_signer, deployed_contract.write.payableSetState(456), Amount.ether(1)
+        root_signer, deployed_contract.method.payableSetState(456), Amount.ether(1)
     )
     balance = await session.eth_get_balance(deployed_contract.address)
     assert balance == Amount.ether(1)
 
     # Not enough gas
     with pytest.raises(TransactionFailed, match="Transact failed"):
-        await session.transact(root_signer, deployed_contract.write.faultySetState(0), gas=300000)
+        await session.transact(root_signer, deployed_contract.method.faultySetState(0), gas=300000)
 
 
 async def test_get_block(test_provider, session, root_signer, another_signer):
     to_transfer = Amount.ether(10)
     await session.transfer(root_signer, another_signer.address, to_transfer)
 
     block_info = await session.eth_get_block_by_number(1, with_transactions=True)
@@ -384,14 +391,25 @@
     assert tx_info.value == to_transfer
 
     non_existent = TxHash(b"abcd" * 8)
     tx_info = await session.eth_get_transaction_by_hash(non_existent)
     assert tx_info is None
 
 
+async def test_eth_get_filter_changes_bad_response(test_provider, session, monkeypatch):
+    monkeypatch.setattr(test_provider, "eth_get_filter_changes", lambda filter_id: {"foo": 1})
+
+    block_filter = await session.eth_new_block_filter()
+
+    with pytest.raises(
+        BadResponseFormat, match=r"eth_getFilterChangers: Expected a list as a response, got dict"
+    ):
+        await session.eth_get_filter_changes(block_filter)
+
+
 async def test_block_filter(test_provider, session, root_signer, another_signer):
     to_transfer = Amount.ether(1)
 
     await session.transfer(root_signer, another_signer.address, to_transfer)
 
     block_filter = await session.eth_new_block_filter()
 
@@ -428,16 +446,16 @@
 async def test_log_filter_all(session, compiled_contracts, root_signer, another_signer):
     basic_contract = compiled_contracts["BasicContract"]
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
     contract2 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     log_filter = await session.eth_new_filter()
-    await session.transact(root_signer, contract1.write.deposit(b"1234"))
-    await session.transact(another_signer, contract2.write.deposit2(b"4567"))
+    await session.transact(root_signer, contract1.method.deposit(b"1234"))
+    await session.transact(another_signer, contract2.method.deposit2(b"4567"))
 
     entries = await session.eth_get_filter_changes(log_filter)
     assert len(entries) == 2
     assert entries[0].address == contract1.address
     assert entries[1].address == contract2.address
 
     assert (
@@ -455,33 +473,33 @@
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
     contract2 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     # Filter by a single address
 
     log_filter = await session.eth_new_filter(source=contract2.address)
-    await session.transact(root_signer, contract1.write.deposit(b"1234"))
-    await session.transact(root_signer, contract2.write.deposit2(b"4567"))
+    await session.transact(root_signer, contract1.method.deposit(b"1234"))
+    await session.transact(root_signer, contract2.method.deposit2(b"4567"))
 
     entries = await session.eth_get_filter_changes(log_filter)
     assert len(entries) == 1
     assert entries[0].address == contract2.address
     assert (
         normalize_topics(entries[0].topics)
         == contract2.abi.event.Deposit2(root_signer.address, b"4567").topics
     )
 
     # Filter by several addresses
 
     contract3 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     log_filter = await session.eth_new_filter(source=[contract1.address, contract3.address])
-    await session.transact(root_signer, contract1.write.deposit(b"1111"))
-    await session.transact(root_signer, contract2.write.deposit(b"2222"))
-    await session.transact(root_signer, contract3.write.deposit(b"3333"))
+    await session.transact(root_signer, contract1.method.deposit(b"1111"))
+    await session.transact(root_signer, contract2.method.deposit(b"2222"))
+    await session.transact(root_signer, contract3.method.deposit(b"3333"))
 
     entries = await session.eth_get_filter_changes(log_filter)
     assert len(entries) == 2
     assert entries[0].address == contract1.address
     assert (
         normalize_topics(entries[0].topics)
         == contract1.abi.event.Deposit(root_signer.address, b"1111").topics
@@ -499,21 +517,21 @@
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
     contract2 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     # Filter by a specific topic or None at each position
 
     log_filter = await session.eth_new_filter(event_filter=contract2.abi.event.Deposit2(id=b"4567"))
     # filtered out, wrong event type
-    await session.transact(root_signer, contract1.write.deposit(b"4567"))
+    await session.transact(root_signer, contract1.method.deposit(b"4567"))
     # matches the filter
-    await session.transact(root_signer, contract1.write.deposit2(b"4567"))
+    await session.transact(root_signer, contract1.method.deposit2(b"4567"))
     # filtered out, wrong value
-    await session.transact(another_signer, contract2.write.deposit2(b"7890"))
+    await session.transact(another_signer, contract2.method.deposit2(b"7890"))
     # matches the filter
-    await session.transact(another_signer, contract2.write.deposit2(b"4567"))
+    await session.transact(another_signer, contract2.method.deposit2(b"4567"))
 
     entries = await session.eth_get_filter_changes(log_filter)
     assert len(entries) == 2
     assert entries[0].address == contract1.address
     assert (
         normalize_topics(entries[0].topics)
         == contract1.abi.event.Deposit2(root_signer.address, b"4567").topics
@@ -524,18 +542,18 @@
         == contract2.abi.event.Deposit2(another_signer.address, b"4567").topics
     )
 
     # Filter by a list of topics
 
     event_filter = contract1.abi.event.Deposit(id=Either(b"1111", b"3333"))
     log_filter = await session.eth_new_filter(event_filter=event_filter)
-    await session.transact(root_signer, contract1.write.deposit(b"1111"))
-    await session.transact(root_signer, contract1.write.deposit2(b"1111"))  # filtered out
-    await session.transact(root_signer, contract1.write.deposit(b"2222"))  # filtered out
-    await session.transact(another_signer, contract2.write.deposit(b"3333"))
+    await session.transact(root_signer, contract1.method.deposit(b"1111"))
+    await session.transact(root_signer, contract1.method.deposit2(b"1111"))  # filtered out
+    await session.transact(root_signer, contract1.method.deposit(b"2222"))  # filtered out
+    await session.transact(another_signer, contract2.method.deposit(b"3333"))
 
     entries = await session.eth_get_filter_changes(log_filter)
     assert len(entries) == 2
     assert entries[0].address == contract1.address
     assert (
         normalize_topics(entries[0].topics)
         == contract1.abi.event.Deposit(root_signer.address, b"1111").topics
@@ -548,20 +566,20 @@
 
 
 async def test_log_filter_by_block_num(session, compiled_contracts, root_signer, another_signer):
     basic_contract = compiled_contracts["BasicContract"]
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
 
-    await session.transact(root_signer, contract1.write.deposit(b"1111"))
+    await session.transact(root_signer, contract1.method.deposit(b"1111"))
     block_num = await session.eth_block_number()
-    await session.transact(root_signer, contract1.write.deposit(b"2222"))  # filter will start here
-    await session.transact(root_signer, contract1.write.deposit(b"3333"))
-    await session.transact(root_signer, contract1.write.deposit(b"4444"))  # filter will stop here
-    await session.transact(root_signer, contract1.write.deposit(b"5555"))
+    await session.transact(root_signer, contract1.method.deposit(b"2222"))  # filter will start here
+    await session.transact(root_signer, contract1.method.deposit(b"3333"))
+    await session.transact(root_signer, contract1.method.deposit(b"4444"))  # filter will stop here
+    await session.transact(root_signer, contract1.method.deposit(b"5555"))
 
     log_filter = await session.eth_new_filter(from_block=block_num + 1, to_block=block_num + 3)
     entries = await session.eth_get_filter_changes(log_filter)
 
     # The range in the filter is inclusive
     assert [entry.block_number for entry in entries] == list(range(block_num + 1, block_num + 4))
     assert [normalize_topics(entry.topics) for entry in entries] == [
@@ -648,26 +666,28 @@
                 break
 
     async with trio.open_nursery() as nursery:
         nursery.start_soon(observer)
         await trio.sleep(2)
 
         # filtered out, wrong event type
-        await session.transact(root_signer, contract1.write.deposit(b"1111"))
+        await session.transact(root_signer, contract1.method.deposit(b"1111"))
         # filtered out, wrong contract address
-        await session.transact(root_signer, contract1.write.deposit2(b"1111"))
+        await session.transact(root_signer, contract1.method.deposit2(b"1111"))
         # filtered out, wrong value
-        await session.transact(another_signer, contract2.write.deposit2(b"7890"))
+        await session.transact(another_signer, contract2.method.deposit2(b"7890"))
         # matches the filter
-        await session.transact(root_signer, contract2.write.deposit2(b"1111"), amount=Amount.wei(1))
         await session.transact(
-            another_signer, contract2.write.deposit2(b"1111"), amount=Amount.wei(2)
+            root_signer, contract2.method.deposit2(b"1111"), amount=Amount.wei(1)
+        )
+        await session.transact(
+            another_signer, contract2.method.deposit2(b"1111"), amount=Amount.wei(2)
         )
         await session.transact(
-            another_signer, contract2.write.deposit2(b"1111"), amount=Amount.wei(3)
+            another_signer, contract2.method.deposit2(b"1111"), amount=Amount.wei(3)
         )
 
     assert events[0] == {"from_": root_signer.address, "id": b"1111", "value": 1, "value2": 2}
     assert events[1] == {"from_": another_signer.address, "id": b"1111", "value": 2, "value2": 3}
     assert events[2] == {"from_": another_signer.address, "id": b"1111", "value": 3, "value2": 4}
 
 
@@ -701,88 +721,88 @@
 
     # `require(condition)`
     kwargs = dict(
         expected_code=ProviderError.Code.SERVER_ERROR,
         expected_message="execution reverted",
         expected_data=None,
     )
-    await check_rpc_error(session.eth_call(contract.read.viewError(0)), **kwargs)
+    await check_rpc_error(session.eth_call(contract.method.viewError(0)), **kwargs)
 
     # `require(condition, message)`
     kwargs = dict(
         expected_code=ProviderError.Code.EXECUTION_ERROR,
         expected_message="execution reverted: require(string)",
         expected_data=error_selector + encode_args((abi.string, "require(string)")),
     )
-    await check_rpc_error(session.eth_call(contract.read.viewError(1)), **kwargs)
+    await check_rpc_error(session.eth_call(contract.method.viewError(1)), **kwargs)
 
     # `revert()`
     kwargs = dict(
         expected_code=ProviderError.Code.SERVER_ERROR,
         expected_message="execution reverted",
         expected_data=None,
     )
-    await check_rpc_error(session.eth_call(contract.read.viewError(2)), **kwargs)
+    await check_rpc_error(session.eth_call(contract.method.viewError(2)), **kwargs)
 
     # `revert(message)`
     kwargs = dict(
         expected_code=ProviderError.Code.EXECUTION_ERROR,
         expected_message="execution reverted: revert(string)",
         expected_data=error_selector + encode_args((abi.string, "revert(string)")),
     )
-    await check_rpc_error(session.eth_call(contract.read.viewError(3)), **kwargs)
+    await check_rpc_error(session.eth_call(contract.method.viewError(3)), **kwargs)
 
     # `revert CustomError(...)`
     kwargs = dict(
         expected_code=ProviderError.Code.EXECUTION_ERROR,
         expected_message="execution reverted",
         expected_data=custom_error_selector + encode_args((abi.uint(256), 4)),
     )
-    await check_rpc_error(session.eth_call(contract.read.viewError(4)), **kwargs)
+    await check_rpc_error(session.eth_call(contract.method.viewError(4)), **kwargs)
 
 
 async def test_contract_panics(session, root_signer, compiled_contracts):
     compiled_contract = compiled_contracts["TestErrors"]
     contract = await session.deploy(root_signer, compiled_contract.constructor(999))
 
     panic_selector = keccak(b"Panic(uint256)")[:4]
 
     await check_rpc_error(
-        session.eth_call(contract.read.viewPanic(0)),
+        session.eth_call(contract.method.viewPanic(0)),
         expected_code=ProviderError.Code.EXECUTION_ERROR,
         expected_message="execution reverted",
         expected_data=panic_selector + encode_args((abi.uint(256), 0x01)),
     )
 
     await check_rpc_error(
-        session.eth_call(contract.read.viewPanic(1)),
+        session.eth_call(contract.method.viewPanic(1)),
         expected_code=ProviderError.Code.EXECUTION_ERROR,
         expected_message="execution reverted",
         expected_data=panic_selector + encode_args((abi.uint(256), 0x11)),
     )
 
 
 async def test_contract_exceptions_high_level(session, root_signer, compiled_contracts):
     compiled_contract = compiled_contracts["TestErrors"]
     contract = await session.deploy(root_signer, compiled_contract.constructor(999))
 
     with pytest.raises(ContractPanic) as exc:
-        await session.estimate_transact(contract.write.transactPanic(1))
+        await session.estimate_transact(contract.method.transactPanic(1))
     assert exc.value.reason == ContractPanic.Reason.OVERFLOW
 
     with pytest.raises(ContractLegacyError) as exc:
-        await session.estimate_transact(contract.write.transactError(0))
+        await session.estimate_transact(contract.method.transactError(0))
     assert exc.value.message == ""
 
     with pytest.raises(ContractLegacyError) as exc:
-        await session.estimate_transact(contract.write.transactError(1))
+        await session.estimate_transact(contract.method.transactError(1))
     assert exc.value.message == "require(string)"
 
     with pytest.raises(ContractError) as exc:
-        await session.estimate_transact(contract.write.transactError(4))
+        await session.estimate_transact(contract.method.transactError(4))
     assert exc.value.error == contract.error.CustomError
     assert exc.value.data == {"x": 4}
 
     # Check that the same works for deployment
 
     with pytest.raises(ContractError) as exc:
         await session.estimate_deploy(compiled_contract.constructor(4))
@@ -801,34 +821,34 @@
         data = PANIC_ERROR.selector + encode_args((abi.uint(256), 888))
         raise RPCError(
             ProviderError.Code.EXECUTION_ERROR, "execution reverted", rpc_encode_data(data)
         )
 
     with monkeypatched(test_provider, "eth_estimate_gas", eth_estimate_gas):
         with pytest.raises(ContractPanic, match=r"ContractPanicReason.UNKNOWN"):
-            await session.estimate_transact(contract.write.transactPanic(999))
+            await session.estimate_transact(contract.method.transactPanic(999))
 
     # Provider returns an unknown error (a selector not present in the ABI)
 
     def eth_estimate_gas(*args, **kwargs):
         # Invalid selector
         data = b"1234" + encode_args((abi.uint(256), 1))
         raise RPCError(
             ProviderError.Code.EXECUTION_ERROR, "execution reverted", rpc_encode_data(data)
         )
 
     with monkeypatched(test_provider, "eth_estimate_gas", eth_estimate_gas):
         with pytest.raises(
             ProviderError, match=r"Provider error \(EXECUTION_ERROR\): execution reverted"
         ):
-            await session.estimate_transact(contract.write.transactPanic(999))
+            await session.estimate_transact(contract.method.transactPanic(999))
 
     # Provider returns an error with an unknown RPC code
 
     def eth_estimate_gas(*args, **kwargs):
         # Invalid selector
         data = PANIC_ERROR.selector + encode_args((abi.uint(256), 0))
         raise RPCError(12345, "execution reverted", rpc_encode_data(data))
 
     with monkeypatched(test_provider, "eth_estimate_gas", eth_estimate_gas):
         with pytest.raises(ProviderError, match=r"Provider error \(12345\): execution reverted"):
-            await session.estimate_transact(contract.write.transactPanic(999))
+            await session.estimate_transact(contract.method.transactPanic(999))
```

### Comparing `pons-0.6.0/tests/test_contract.py` & `pons-0.7.0/tests/test_contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 import pytest
 
 from pons import (
     abi,
     Address,
     Constructor,
-    ReadMethod,
-    WriteMethod,
+    Method,
     Fallback,
     Receive,
     Event,
 )
 from pons._abi_types import keccak, encode_args
-from pons._contract import DeployedContract, BoundReadMethod, BoundWriteMethod
+from pons._contract import DeployedContract, BoundMethod
 from pons._entities import LogTopic
 
 from .compile import compile_file
 
 
 @pytest.fixture
 def compiled_contracts():
@@ -40,35 +39,35 @@
     assert cabi.constructor.payable
 
     assert isinstance(cabi.fallback, Fallback)
     assert cabi.fallback.payable
     assert isinstance(cabi.receive, Receive)
     assert cabi.receive.payable
 
-    assert isinstance(cabi.read.v1, ReadMethod)
-    assert str(cabi.read.v1.inputs) == "()"
-    assert str(cabi.read.v1.outputs) == "(uint256)"
-
-    assert isinstance(cabi.read.getState, ReadMethod)
-    assert str(cabi.read.getState.inputs) == "(uint256 _x)"
-    assert str(cabi.read.getState.outputs) == "(uint256)"
+    assert isinstance(cabi.method.v1, Method)
+    assert str(cabi.method.v1.inputs) == "()"
+    assert str(cabi.method.v1.outputs) == "(uint256)"
+
+    assert isinstance(cabi.method.getState, Method)
+    assert str(cabi.method.getState.inputs) == "(uint256 _x)"
+    assert str(cabi.method.getState.outputs) == "(uint256)"
 
-    assert isinstance(cabi.read.testStructs, ReadMethod)
+    assert isinstance(cabi.method.testStructs, Method)
     assert (
-        str(cabi.read.testStructs.inputs)
+        str(cabi.method.testStructs.inputs)
         == "((uint256,uint256) inner_in, ((uint256,uint256),uint256) outer_in)"
     )
     assert (
-        str(cabi.read.testStructs.outputs)
+        str(cabi.method.testStructs.outputs)
         == "((uint256,uint256) inner_out, ((uint256,uint256),uint256) outer_out)"
     )
 
-    assert isinstance(cabi.write.setState, WriteMethod)
-    assert str(cabi.write.setState.inputs) == "(uint256 _v1)"
-    assert cabi.write.setState.payable
+    assert isinstance(cabi.method.setState, Method)
+    assert str(cabi.method.setState.inputs) == "(uint256 _v1)"
+    assert cabi.method.setState.payable
 
     assert isinstance(cabi.event.Foo, Event)
     assert str(cabi.event.Foo.fields) == "(uint256 indexed x, bytes indexed y, bytes4 u, bytes v)"
     assert cabi.event.Foo.anonymous
     assert cabi.event.Foo.indexed == {"x", "y"}
 
 
@@ -80,38 +79,38 @@
     compiled_contract = compiled_contracts["JsonAbiTest"]
 
     address = Address(b"\xab" * 20)
     deployed_contract = DeployedContract(compiled_contract.abi, address)
 
     assert deployed_contract.address == address
     assert deployed_contract.abi == compiled_contract.abi
-    assert isinstance(deployed_contract.read.v1, BoundReadMethod)
-    assert isinstance(deployed_contract.read.getState, BoundReadMethod)
-    assert isinstance(deployed_contract.read.testStructs, BoundReadMethod)
-    assert isinstance(deployed_contract.write.setState, BoundWriteMethod)
+    assert isinstance(deployed_contract.method.v1, BoundMethod)
+    assert isinstance(deployed_contract.method.getState, BoundMethod)
+    assert isinstance(deployed_contract.method.testStructs, BoundMethod)
+    assert isinstance(deployed_contract.method.setState, BoundMethod)
 
     ctr_call = compiled_contract.constructor(1, 2)
     assert ctr_call.payable
     assert ctr_call.contract_abi == compiled_contract.abi
     assert ctr_call.data_bytes == (
         compiled_contract.bytecode + b"\x00" * 31 + b"\x01" + b"\x00" * 31 + b"\x02"
     )
 
-    read_call = deployed_contract.read.getState(3)
+    read_call = deployed_contract.method.getState(3)
     assert read_call.contract_address == address
     assert read_call.data_bytes == (
-        compiled_contract.abi.read.getState.selector + b"\x00" * 31 + b"\x03"
+        compiled_contract.abi.method.getState.selector + b"\x00" * 31 + b"\x03"
     )
     assert read_call.decode_output(b"\x00" * 31 + b"\x04") == (4,)
 
-    write_call = deployed_contract.write.setState(5)
+    write_call = deployed_contract.method.setState(5)
     assert write_call.contract_address == address
     assert write_call.payable
     assert write_call.data_bytes == (
-        compiled_contract.abi.write.setState.selector + b"\x00" * 31 + b"\x05"
+        compiled_contract.abi.method.setState.selector + b"\x00" * 31 + b"\x05"
     )
 
     event_filter = deployed_contract.event.Foo(1, b"1234")
     assert event_filter.contract_address == address
     assert event_filter.topics == (
         (LogTopic(abi.uint(256).encode(1)),),
         (LogTopic(keccak(b"1234")),),
```

### Comparing `pons-0.6.0/tests/test_contract_abi.py` & `pons-0.7.0/tests/test_contract_abi.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import re
 
 import pytest
 
 from pons import (
     abi,
     Constructor,
-    ReadMethod,
-    WriteMethod,
+    Method,
     Fallback,
     Receive,
     ContractABI,
     Event,
     Error,
     Either,
     ABIDecodingError,
+    Mutability,
 )
 from pons._abi_types import keccak, encode_args
 from pons._contract_abi import (
     Signature,
     EventSignature,
     PANIC_ERROR,
     LEGACY_ERROR,
@@ -143,36 +143,36 @@
     with pytest.raises(
         ValueError,
         match="Constructor's JSON entry state mutability must be `nonpayable` or `payable`",
     ):
         Constructor.from_json(dict(type="constructor", stateMutability="view"))
 
 
-def _check_read_method(read):
-    assert read.name == "someMethod"
-    assert read.inputs.canonical_form == "(uint8,bool)"
-    assert str(read.inputs) == "(uint8 a, bool b)"
-    assert read.outputs.canonical_form == "(uint8,bool)"
+def _check_method(method):
+    assert method.name == "someMethod"
+    assert method.inputs.canonical_form == "(uint8,bool)"
+    assert str(method.inputs) == "(uint8 a, bool b)"
+    assert method.outputs.canonical_form == "(uint8,bool)"
 
     encoded_bytes = b"\x00" * 31 + b"\x01" + b"\x00" * 31 + b"\x01"
 
-    rcall = read(1, True)
-    assert rcall.data_bytes == read.selector + encoded_bytes
+    call = method(1, True)
+    assert call.data_bytes == method.selector + encoded_bytes
 
-    vals = read.decode_output(encoded_bytes)
+    vals = method.decode_output(encoded_bytes)
     assert vals == (1, True)
 
     # A regression for a typo in argument passing.
     # Check that keyword arguments are processed correctly.
-    rcall = read(1, b=True)
-    assert rcall.data_bytes == read.selector + encoded_bytes
+    call = method(1, b=True)
+    assert call.data_bytes == method.selector + encoded_bytes
 
 
-def test_read_method_from_json_anonymous_outputs():
-    read = ReadMethod.from_json(
+def test_method_from_json_anonymous_outputs():
+    method = Method.from_json(
         dict(
             type="function",
             name="someMethod",
             stateMutability="view",
             inputs=[
                 dict(type="uint8", name="a"),
                 dict(type="bool", name="b"),
@@ -180,20 +180,20 @@
             outputs=[
                 dict(type="uint8", name=""),
                 dict(type="bool", name=""),
             ],
         )
     )
 
-    assert str(read.outputs) == "(uint8, bool)"
-    _check_read_method(read)
+    assert str(method.outputs) == "(uint8, bool)"
+    _check_method(method)
 
 
-def test_read_method_from_json_named_outputs():
-    read = ReadMethod.from_json(
+def test_method_from_json_named_outputs():
+    method = Method.from_json(
         dict(
             type="function",
             name="someMethod",
             stateMutability="view",
             inputs=[
                 dict(type="uint8", name="a"),
                 dict(type="bool", name="b"),
@@ -201,143 +201,63 @@
             outputs=[
                 dict(type="uint8", name="c"),
                 dict(type="bool", name="d"),
             ],
         )
     )
 
-    assert str(read.outputs) == "(uint8 c, bool d)"
-    _check_read_method(read)
+    assert str(method.outputs) == "(uint8 c, bool d)"
+    _check_method(method)
 
 
-def test_read_method_init():
-    read = ReadMethod(
+def test_method_init():
+    method = Method(
         name="someMethod",
+        mutability=Mutability.VIEW,
         inputs=dict(a=abi.uint(8), b=abi.bool),
         outputs=dict(c=abi.uint(8), d=abi.bool),
     )
 
-    assert str(read.outputs) == "(uint8 c, bool d)"
-    _check_read_method(read)
+    assert str(method.outputs) == "(uint8 c, bool d)"
+    _check_method(method)
 
 
-def test_read_method_single_output():
-    read = ReadMethod(
-        name="someMethod", inputs=dict(a=abi.uint(8), b=abi.bool), outputs=abi.uint(8)
+def test_method_single_output():
+    method = Method(
+        name="someMethod",
+        mutability=Mutability.VIEW,
+        inputs=dict(a=abi.uint(8), b=abi.bool),
+        outputs=abi.uint(8),
     )
 
-    assert read.outputs.canonical_form == "(uint8)"
-    assert str(read.outputs) == "(uint8)"
+    assert method.outputs.canonical_form == "(uint8)"
+    assert str(method.outputs) == "(uint8)"
 
     encoded_bytes = b"\x00" * 31 + b"\x01"
-    assert read.decode_output(encoded_bytes) == 1
+    assert method.decode_output(encoded_bytes) == 1
 
 
-def test_read_method_errors():
+def test_method_errors():
     with pytest.raises(
-        ValueError, match="ReadMethod object must be created from a JSON entry with type='function'"
+        ValueError, match="Method object must be created from a JSON entry with type='function'"
     ):
-        ReadMethod.from_json(dict(type="constructor"))
-
-    with pytest.raises(
-        ValueError,
-        match="Non-mutating method's JSON entry state mutability must be `pure` or `view`",
-    ):
-        ReadMethod.from_json(
-            dict(
-                type="function",
-                name="someMethod",
-                stateMutability="nonpayable",
-                inputs=[dict(type="uint8", name="a")],
-                outputs=[dict(type="uint8", name="")],
-            )
-        )
-
-
-def _check_write_method(write):
-    assert write.name == "someMethod"
-    assert write.inputs.canonical_form == "(uint8,bool)"
-    assert str(write.inputs) == "(uint8 a, bool b)"
-    assert write.payable
-
-    encoded_bytes = b"\x00" * 31 + b"\x01" + b"\x00" * 31 + b"\x01"
-
-    wcall = write(1, True)
-    assert wcall.data_bytes == write.selector + encoded_bytes
-
-    # A regression for a typo in argument passing.
-    # Check that keyword arguments are processed correctly.
-    wcall = write(1, b=True)
-    assert wcall.data_bytes == write.selector + encoded_bytes
-
+        Method.from_json(dict(type="constructor"))
 
-def test_write_method_from_json():
-    write = WriteMethod.from_json(
-        dict(
-            type="function",
-            name="someMethod",
-            stateMutability="payable",
-            inputs=[
-                dict(type="uint8", name="a"),
-                dict(type="bool", name="b"),
-            ],
-        )
-    )
-
-    _check_write_method(write)
-
-
-def test_write_method_with_output():
-    # Mutating methods can have outputs (in case they are called by other mutating methods),
-    # but we cannot get that output from the outside.
-    # So if we see those in a JSON ABI, we can just ignore them.
-    write = WriteMethod.from_json(
-        dict(
-            type="function",
-            name="someMethod",
-            stateMutability="payable",
-            inputs=[
-                dict(type="uint8", name="a"),
-                dict(type="bool", name="b"),
-            ],
-            outputs=[
-                dict(type="uint8", name="a"),
-                dict(type="bool", name="b"),
-            ],
-        )
+    json = dict(
+        type="function",
+        name="someMethod",
+        stateMutability="invalid",
+        inputs=[
+            dict(type="uint8", name="a"),
+            dict(type="bool", name="b"),
+        ],
     )
 
-    _check_write_method(write)
-
-
-def test_write_method_init():
-    write = WriteMethod(name="someMethod", inputs=dict(a=abi.uint(8), b=abi.bool), payable=True)
-
-    _check_write_method(write)
-
-
-def test_write_method_errors():
-    with pytest.raises(
-        ValueError,
-        match="WriteMethod object must be created from a JSON entry with type='function'",
-    ):
-        WriteMethod.from_json(dict(type="constructor"))
-
-    with pytest.raises(
-        ValueError,
-        match="Mutating method's JSON entry state mutability must be `nonpayable` or `payable`",
-    ):
-        WriteMethod.from_json(
-            dict(
-                type="function",
-                name="someMethod",
-                stateMutability="view",
-                inputs=[dict(type="uint8", name="a")],
-            )
-        )
+    with pytest.raises(ValueError, match="Unknown mutability identifier: invalid"):
+        Method.from_json(json)
 
 
 def test_fallback():
     fallback = Fallback.from_json(dict(type="fallback", stateMutability="payable"))
     assert fallback.payable
 
 
@@ -432,42 +352,45 @@
         [constructor_abi, read_abi, write_abi, fallback_abi, receive_abi, event_abi, error_abi]
     )
     assert str(cabi) == (
         "{\n"
         "    constructor(uint8 a, bool b) payable\n"
         "    fallback() payable\n"
         "    receive() payable\n"
-        "    function readMethod(uint8 a, bool b) returns (uint8, bool)\n"
+        "    function readMethod(uint8 a, bool b) view returns (uint8, bool)\n"
         "    function writeMethod(uint8 a, bool b) payable\n"
         "    event Deposit(address indexed from_, bytes indexed foo, uint8 bar) anonymous\n"
         "    error CustomError(address from_, bytes foo, uint8 bar)\n"
         "}"
     )
 
     assert isinstance(cabi.constructor, Constructor)
     assert isinstance(cabi.fallback, Fallback)
     assert isinstance(cabi.receive, Receive)
-    assert isinstance(cabi.read.readMethod, ReadMethod)
-    assert isinstance(cabi.write.writeMethod, WriteMethod)
+    assert isinstance(cabi.method.readMethod, Method)
+    assert isinstance(cabi.method.writeMethod, Method)
     assert isinstance(cabi.event.Deposit, Event)
     assert isinstance(cabi.error.CustomError, Error)
 
 
 def test_contract_abi_init():
     cabi = ContractABI(
         constructor=Constructor(inputs=dict(a=abi.uint(8), b=abi.bool), payable=True),
-        write=[
-            WriteMethod(name="writeMethod", inputs=dict(a=abi.uint(8), b=abi.bool), payable=True)
-        ],
-        read=[
-            ReadMethod(
+        methods=[
+            Method(
                 name="readMethod",
+                mutability=Mutability.VIEW,
                 inputs=dict(a=abi.uint(8), b=abi.bool),
                 outputs=[abi.uint(8), abi.bool],
-            )
+            ),
+            Method(
+                name="writeMethod",
+                mutability=Mutability.PAYABLE,
+                inputs=dict(a=abi.uint(8), b=abi.bool),
+            ),
         ],
         events=[
             Event(
                 name="Deposit",
                 fields=dict(from_=abi.address, foo=abi.bytes(), bar=abi.uint(8)),
                 indexed={"from_", "foo"},
                 anonymous=True,
@@ -484,26 +407,26 @@
     )
 
     assert str(cabi) == (
         "{\n"
         "    constructor(uint8 a, bool b) payable\n"
         "    fallback() payable\n"
         "    receive() payable\n"
-        "    function readMethod(uint8 a, bool b) returns (uint8, bool)\n"
+        "    function readMethod(uint8 a, bool b) view returns (uint8, bool)\n"
         "    function writeMethod(uint8 a, bool b) payable\n"
         "    event Deposit(address indexed from_, bytes indexed foo, uint8 bar) anonymous\n"
         "    error CustomError(address from_, bytes foo, uint8 bar)\n"
         "}"
     )
 
     assert isinstance(cabi.constructor, Constructor)
     assert isinstance(cabi.fallback, Fallback)
     assert isinstance(cabi.receive, Receive)
-    assert isinstance(cabi.read.readMethod, ReadMethod)
-    assert isinstance(cabi.write.writeMethod, WriteMethod)
+    assert isinstance(cabi.method.readMethod, Method)
+    assert isinstance(cabi.method.writeMethod, Method)
 
 
 def test_no_constructor():
     cabi = ContractABI()
     assert isinstance(cabi.constructor, Constructor)
     assert cabi.constructor.inputs.canonical_form == "()"
```

### Comparing `pons-0.6.0/tests/test_contract_functionality.py` & `pons-0.7.0/tests/test_contract_functionality.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 from pathlib import Path
 
 import pytest
 
-from pons import (
-    Amount,
-    ContractABI,
-    abi,
-    Constructor,
-    ReadMethod,
-    WriteMethod,
-    DeployedContract,
-)
+from pons import Amount, ContractABI, abi, Constructor, Method, DeployedContract, Mutability
 
 from .compile import compile_file
 
 
 @pytest.fixture
 def compiled_contracts():
     path = Path(__file__).resolve().parent / "TestContractFunctionality.sol"
@@ -26,84 +18,123 @@
     Checks that an empty constructor is created automatically if none is provided,
     and it can be used to deploy the contract.
     """
 
     compiled_contract = compiled_contracts["NoConstructor"]
 
     deployed_contract = await session.deploy(root_signer, compiled_contract.constructor())
-    call = deployed_contract.read.getState(123)
+    call = deployed_contract.method.getState(123)
     result = await session.eth_call(call)
     assert result == (1 + 123,)
 
 
 async def test_basics(session, root_signer, another_signer, compiled_contracts):
     compiled_contract = compiled_contracts["Test"]
 
     # Deploy the contract
     call = compiled_contract.constructor(12345, 56789)
     await session.transfer(root_signer, another_signer.address, Amount.ether(10))
     deployed_contract = await session.deploy(another_signer, call)
 
     # Check the state
-    assert await session.eth_call(deployed_contract.read.v1()) == (12345,)
-    assert await session.eth_call(deployed_contract.read.v2()) == (56789,)
+    assert await session.eth_call(deployed_contract.method.v1()) == (12345,)
+    assert await session.eth_call(deployed_contract.method.v2()) == (56789,)
 
     # Transact with the contract
-    await session.transact(another_signer, deployed_contract.write.setState(111))
-    assert await session.eth_call(deployed_contract.read.v1()) == (111,)
+    await session.transact(another_signer, deployed_contract.method.setState(111))
+    assert await session.eth_call(deployed_contract.method.v1()) == (111,)
 
     # Call the contract
 
-    result = await session.eth_call(deployed_contract.read.getState(123))
+    result = await session.eth_call(deployed_contract.method.getState(123))
     assert result == (111 + 123,)
 
     inner = dict(inner1=1, inner2=2)
     outer = dict(inner=inner, outer1=3)
-    result = await session.eth_call(deployed_contract.read.testStructs(inner, outer))
+    result = await session.eth_call(deployed_contract.method.testStructs(inner, outer))
     assert result == (inner, outer)
 
 
+async def test_read_only_mode(session, root_signer, compiled_contracts):
+    # Test that a "nonpayable" (that is, mutating) method can still be invoked
+    # via `eth_call`, and it will use the current state of the contract
+    # in a "copy-on-write" mode, where it will be able to make changes,
+    # but they will not be saved.
+
+    compiled_contract = compiled_contracts["Test"]
+
+    value = 12345
+    deployed_contract = await session.deploy(root_signer, compiled_contract.constructor(value, 0))
+
+    # check the state
+    result = await session.eth_call(deployed_contract.method.getState(0))
+    assert result == (value,)
+
+    # this method will not modify the state since it's invoked via `eth_call`,
+    # but it will return a value that reflects the ethereal "modified" state.
+    result = await session.eth_call(deployed_contract.method.setStateAndReturn(1))
+    assert result == (value + 1,)
+
+    result = await session.eth_call(deployed_contract.method.getState(0))
+    assert result == (value,)
+
+    # Now invoke it as a transaction, allowing it to modify the state
+    await session.transact(root_signer, deployed_contract.method.setStateAndReturn(1))
+
+    # The state is now modified
+    result = await session.eth_call(deployed_contract.method.getState(0))
+    assert result == (value + 1,)
+
+
 async def test_abi_declaration(session, root_signer, another_signer, compiled_contracts):
     compiled_contract = compiled_contracts["Test"]
 
     # Deploy the contract
     await session.transfer(root_signer, another_signer.address, Amount.ether(10))
     call = compiled_contract.constructor(12345, 56789)
     previously_deployed_contract = await session.deploy(another_signer, call)
 
     # The contract was deployed earlier, now all we have is this
     inner_struct = abi.struct(inner1=abi.uint(256), inner2=abi.uint(256))
     outer_struct = abi.struct(inner=inner_struct, outer1=abi.uint(256))
     declared_abi = ContractABI(
         constructor=Constructor(inputs=dict(_v1=abi.uint(256), _v2=abi.uint(256))),
-        write=[WriteMethod(name="setState", inputs=dict(_v1=abi.uint(256)))],
-        read=[
-            ReadMethod(name="getState", inputs=dict(_x=abi.uint(256)), outputs=abi.uint(256)),
-            ReadMethod(
+        methods=[
+            Method(
+                name="setState", mutability=Mutability.NONPAYABLE, inputs=dict(_v1=abi.uint(256))
+            ),
+            Method(
+                name="getState",
+                mutability=Mutability.VIEW,
+                inputs=dict(_x=abi.uint(256)),
+                outputs=abi.uint(256),
+            ),
+            Method(
                 name="testStructs",
+                mutability=Mutability.VIEW,
                 inputs=dict(inner_in=inner_struct, outer_in=outer_struct),
                 outputs=dict(inner_out=inner_struct, outer_out=outer_struct),
             ),
         ],
     )
 
     deployed_contract = DeployedContract(declared_abi, previously_deployed_contract.address)
 
     # Transact with the contract
     await session.transfer(root_signer, another_signer.address, Amount.ether(10))
-    await session.transact(another_signer, deployed_contract.write.setState(111))
+    await session.transact(another_signer, deployed_contract.method.setState(111))
 
     # Call the contract
 
-    result = await session.eth_call(deployed_contract.read.getState(123))
+    result = await session.eth_call(deployed_contract.method.getState(123))
     assert result == 111 + 123  # Note the lack of `[]` - we declared outputs as a single value
 
     inner = dict(inner1=1, inner2=2)
     outer = dict(inner=inner, outer1=3)
-    result = await session.eth_call(deployed_contract.read.testStructs(inner, outer))
+    result = await session.eth_call(deployed_contract.method.testStructs(inner, outer))
     assert result == (inner, outer)
 
 
 async def test_complicated_event(session, root_signer, compiled_contracts):
     # Smoke test for topic encoding, emitting an event with non-trivial topic structure.
     # The details of the encoding should be covered in ABI tests,
     # here we're just checking we got them right.
@@ -119,13 +150,13 @@
         b"aaaa", bytestring33len2, foo, [inner1, inner2]
     )
 
     contract = await session.deploy(root_signer, basic_contract.constructor(123, 456))
 
     log_filter1 = await session.eth_new_filter(event_filter=event_filter)  # filter by topics
     log_filter2 = await session.eth_new_filter()  # collect everything
-    await session.transact(root_signer, contract.write.emitComplicated())
+    await session.transact(root_signer, contract.method.emitComplicated())
     entries_filtered = await session.eth_get_filter_changes(log_filter1)
     entries_all = await session.eth_get_filter_changes(log_filter2)
 
     assert len(entries_all) == 1
     assert entries_filtered == entries_all
```

### Comparing `pons-0.6.0/tests/test_entities.py` & `pons-0.7.0/tests/test_entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,16 @@
         rpc_decode_data("0xefgh")
 
 
 def test_encode_decode_block():
     assert rpc_encode_block(Block.LATEST) == "latest"
     assert rpc_encode_block(Block.EARLIEST) == "earliest"
     assert rpc_encode_block(Block.PENDING) == "pending"
+    assert rpc_encode_block(Block.SAFE) == "safe"
+    assert rpc_encode_block(Block.FINALIZED) == "finalized"
     assert rpc_encode_block(123) == "0x7b"
     assert rpc_decode_block("latest") == "latest"
     assert rpc_decode_block("earliest") == "earliest"
     assert rpc_decode_block("pending") == "pending"
     assert rpc_decode_block("0x7b") == 123
```

### Comparing `pons-0.6.0/tests/test_provider.py` & `pons-0.7.0/tests/test_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from contextlib import asynccontextmanager
+
 import trio
 import pytest
 
 from pons import Client, Amount, HTTPProvider, Unreachable
 from pons._client import ProviderError, BadResponseFormat
-from pons._provider import ResponseDict, UnexpectedResponse, RPCError
+from pons._provider import ResponseDict, UnexpectedResponse, RPCError, Provider, ProviderSession
 
 from .provider_server import ServerHandle
 from . import provider_server  # For monkeypatching purposes
 
 
 @pytest.fixture
 async def test_server(nursery, test_provider):
@@ -178,7 +180,29 @@
     client = Client(bad_provider)
     async with client.session() as session:
         with trio.fail_after(1):  # Shouldn't be necessary, but just so that the test doesn't hang
             with pytest.raises(
                 Unreachable, match=r"all attempts to connect to 127\.0\.0\.1:8889 failed"
             ):
                 await session.net_version()
+
+
+async def test_default_implementations():
+    class MockProvider(Provider):
+        @asynccontextmanager
+        async def session(self):
+            yield MockSession()
+
+    class MockSession(ProviderSession):
+        async def rpc(self, method, *args):
+            return method
+
+    provider = MockProvider()
+    async with provider.session() as session:
+        result = await session.rpc_and_pin("1")
+        assert result == ("1", ())
+
+        result = await session.rpc_at_pin((), "2")
+        assert result == "2"
+
+        with pytest.raises(ValueError, match=r"Unexpected provider path: \(1,\)"):
+            await session.rpc_at_pin((1,), "3")
```

### Comparing `pons-0.6.0/tests/test_signer.py` & `pons-0.7.0/tests/test_signer.py`

 * *Files identical despite different names*

### Comparing `pons-0.6.0/PKG-INFO` & `pons-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pons
-Version: 0.6.0
+Version: 0.7.0
 Summary: Async RPC client for Ethereum
 License: MIT
 Author-email: Bogdan Opanchuk <bogdan@opanchuk.net>
 Requires-Python: >=3.8
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: tests
```

