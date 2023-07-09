# Comparing `tmp/rds-core-0.1.2.tar.gz` & `tmp/rds-core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-core-0.1.2.tar", last modified: Sun Jun 25 23:00:54 2023, max compression
+gzip compressed data, was "rds-core-0.2.0.tar", last modified: Sun Jul  9 21:32:58 2023, max compression
```

## Comparing `rds-core-0.1.2.tar` & `rds-core-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-25 23:00:35.000000 rds-core-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-25 23:00:54.301707 rds-core-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 23:00:35.000000 rds-core-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/helpers/cnes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/helpers/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/searchengine/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/searchengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/transformers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/transformers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/transformers/fields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/transformers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/transformers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-25 23:00:54.301707 rds-core-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-25 23:00:35.000000 rds-core-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.622728 rds-core-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-09 21:32:49.000000 rds-core-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-09 21:32:58.622728 rds-core-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-09 21:32:49.000000 rds-core-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-09 21:32:49.000000 rds-core-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/contrib/datasus/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/contrib/datasus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/contrib/datasus/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/contrib/datasus/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/contrib/datasus/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/contrib/datasus/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/cache/inmemory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/cache/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/cache/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.618728 rds-core-0.2.0/rds/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/helpers/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.622728 rds-core-0.2.0/rds/core/searchengine/
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/searchengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.622728 rds-core-0.2.0/rds/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.622728 rds-core-0.2.0/rds/core/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.622728 rds-core-0.2.0/rds/core/transformers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-09 21:32:49.000000 rds-core-0.2.0/rds/core/transformers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:32:58.622728 rds-core-0.2.0/rds_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-09 21:32:58.000000 rds-core-0.2.0/rds_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-09 21:32:58.000000 rds-core-0.2.0/rds_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:32:58.000000 rds-core-0.2.0/rds_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 21:32:58.000000 rds-core-0.2.0/rds_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 21:32:58.000000 rds-core-0.2.0/rds_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 21:32:58.622728 rds-core-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-09 21:32:49.000000 rds-core-0.2.0/setup.py
```

### Comparing `rds-core-0.1.2/PKG-INFO` & `rds-core-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.1.2
+Version: 0.2.0
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
```

### Comparing `rds-core-0.1.2/README.md` & `rds-core-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.2/rds_core/cache/base.py` & `rds-core-0.2.0/rds/core/cache/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,136 +1,130 @@
 """
 Documentar.
 """
 
 from typing import Any, Union, List, Dict
-
-
-DEFAULT_TTL = 300
-MISSING_KEY = object()
+from rds.core.cache import MISSING_KEY, DEFAULT_TTL
 
 
 class BaseCache:
-
     def __init__(self, **params: Dict[str, Any]) -> None:
         self.default_ttl = int(str(params.get("ttl", DEFAULT_TTL)))
 
     def get_ttl(self, ttl: Union[int, None] = None) -> int:
         return ttl if (isinstance(ttl, int) and ttl >= 0) or (ttl is not None) else self.default_ttl
 
     def key_exists(self, key: str) -> bool:
-        return self.get(key, MISSING_KEY) is not MISSING_KEY
+        return self.get(key) is not MISSING_KEY
 
     def add(self, key: str, value: Any, ttl: Union[int, None] = None) -> bool:
-        """ Define um valor no cache caso a chave ainda não exista.
+        """Define um valor no cache caso a chave ainda não exista.
 
-            Caso já exista, não define o valor no cache, preservando o TTL.
+        Caso já exista, não define o valor no cache, preservando o TTL.
 
-            Args:
-                key (_type_): A chave a ser usada para identificar o valor no cache.
-                value (_type_): O valor a ser posto em cache.
-                ttl (_type_, optional): O tempo máximo que o item pode existir no cache. O padrão é None.
+        Args:
+            key (_type_): A chave a ser usada para identificar o valor no cache.
+            value (_type_): O valor a ser posto em cache.
+            ttl (_type_, optional): O tempo máximo que o item pode existir no cache. O padrão é None.
 
-            Raises:
-                NotImplementedError: _description_
+        Raises:
+            NotImplementedError: _description_
 
-            Returns:
-                bool: True adicionou, ou seja, se ainda não existia. False se já existia.
+        Returns:
+            bool: True adicionou, ou seja, se ainda não existia. False se já existia.
         """
         raise NotImplementedError("subclasses of BaseCache must provide an add() method")
 
     def get(self, key: str, default: Any = None) -> Any:
-        """ Busca uma determinada chave no cache. Se a chave não existir, retorne o padrão, que por padrão é None.
-            Args:
-                key (_type_): A chave a ser usada para identificar o valor no cache.
-                default (_type_): O valor padrão, caso não seja encontrado no cache. O padrão é None.
-            Raises:
-                NotImplementedError: _description_
+        """Busca uma determinada chave no cache. Se a chave não existir, retorne o padrão, que por padrão é None.
+        Args:
+            key (_type_): A chave a ser usada para identificar o valor no cache.
+            default (_type_): O valor padrão, caso não seja encontrado no cache. O padrão é None.
+        Raises:
+            NotImplementedError: _description_
         """
         raise NotImplementedError("subclasses of BaseCache must provide a get() method")
 
     def set(self, key: str, value: Any, ttl: Union[int, None] = None) -> None:
-        """ Set a value in the cache. If ttl is given, use that ttl for the key; otherwise use the default cache ttl.
-        """
+        """Set a value in the cache. If ttl is given, use that ttl for the key; otherwise use the default cache ttl."""
         raise NotImplementedError("subclasses of BaseCache must provide a set() method")
 
     def get_or_set(self, key: str, default: Any, ttl: Union[int, None] = None) -> Any:
-        """ Fetch a given key from the cache. If the key does not exist,
-            set the key and set it to the default value. The default value can
-            also be any callable. If ttl is given, use that ttl for the
-            key; otherwise use the default cache ttl.
+        """Fetch a given key from the cache. If the key does not exist,
+        set the key and set it to the default value. The default value can
+        also be any callable. If ttl is given, use that ttl for the
+        key; otherwise use the default cache ttl.
 
-            Return the value of the key stored or retrieved.
+        Return the value of the key stored or retrieved.
         """
         val = self.get(key)
         if val is None:
             self.set(key, default, ttl=ttl)
             val = default
         return val
 
     def delete(self, key: str) -> None:
-        """ Delete a key from the cache and return whether it succeeded, failing silently.
-        """
+        """Delete a key from the cache and return whether it succeeded, failing silently."""
         raise NotImplementedError("subclasses of BaseCache must provide a delete() method")
 
     def touch(self, key: str, ttl: Union[int, None] = None) -> bool:
         """
-            Update the key's expiry time using ttl. Return True if successful or False if the key does not exist.
+        Update the key's expiry time using ttl. Return True if successful or False if the key does not exist.
         """
         raise NotImplementedError("subclasses of BaseCache must provide a touch() method")
 
     def get_many(self, keys: List[str]) -> Dict[str, Any]:
-        """ Fetch a bunch of keys from the cache. For certain backends (memcached, pgsql) this can be *much* faster
-            when fetching multiple values.
+        """Fetch a bunch of keys from the cache. For certain backends (memcached, pgsql) this can be *much* faster
+        when fetching multiple values.
 
-            Return a dict mapping each key in keys to its value. If the given key is missing, it will be missing from
-            the response dict.
+        Return a dict mapping each key in keys to its value. If the given key is missing, it will be missing from
+        the response dict.
         """
         d = {}
         for k in keys:
             val = self.get(k, MISSING_KEY)
             if val is not MISSING_KEY:
                 d[k] = val
         return d
 
     def set_many(self, data: Any, ttl: Union[int, None] = None) -> None:
-        """ Set a bunch of values in the cache at once from a dict of key/value
-            pairs.  For certain backends (memcached), this is much more efficient
-            than calling set() multiple times.
+        """Set a bunch of values in the cache at once from a dict of key/value
+        pairs.  For certain backends (memcached), this is much more efficient
+        than calling set() multiple times.
 
-            If ttl is given, use that ttl for the key; otherwise use the
-            default cache ttl.
+        If ttl is given, use that ttl for the key; otherwise use the
+        default cache ttl.
         """
         for key, value in data.items():
             self.set(key, value, ttl=ttl)
 
     def delete_many(self, keys: List[str]) -> None:
-        """ Delete a bunch of values in the cache at once. For certain backends
-            (memcached), this is much more efficient than calling delete() multiple times.
+        """Delete a bunch of values in the cache at once. For certain backends
+        (memcached), this is much more efficient than calling delete() multiple times.
         """
         for key in keys:
             self.delete(key)
 
     def incr(self, key: str, delta: Union[int, float] = 1) -> Union[int, float]:
-        """ NOT SAFE FOR CONCURRENCY. Add delta to value in the cache.
-            If the key does not exist, raise a ValueError exception.
+        """NOT SAFE FOR CONCURRENCY. Add delta to value in the cache.
+        If the key does not exist, raise a ValueError exception.
         """
         value = self.get(key, None)
         if value is None:
             raise ValueError("Key '%s' not found" % key)
         new_value = value + delta
         self.set(key, new_value)
         return new_value
 
     def decr(self, key: str, delta: Union[int, float] = 1) -> Union[int, float]:
-        """ NOT SAFE FOR CONCURRENCY. Subtract delta from value in the cache.
-            If the key does not exist, raise a ValueError exception.
+        """NOT SAFE FOR CONCURRENCY. Subtract delta from value in the cache.
+        If the key does not exist, raise a ValueError exception.
         """
         return self.incr(key, -delta)
 
     def clear(self) -> None:
-        """ Remove *all* values from the cache at once. """
+        """Remove *all* values from the cache at once."""
         raise NotImplementedError("subclasses of BaseCache must provide a clear() method")
 
     def close(self, **kwargs: Dict[str, Any]) -> None:
-        """ Close the cache connection """
+        """Close the cache connection"""
         pass
```

### Comparing `rds-core-0.1.2/rds_core/cache/nocache.py` & `rds-core-0.2.0/rds/core/cache/nocache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Documentar.
 """
 
 from typing import Any, List, Dict, Union
-from rds_core.cache.base import BaseCache
+from rds.core.cache.base import BaseCache
 
 
 class NoCache(BaseCache):
     def __init__(self, *args: List, **kwargs: Dict[str, Any]) -> None:
         super().__init__(*args, **kwargs)
 
     def add(self, key: str, value: Any, ttl: Union[int, None] = None) -> bool:
         return True
 
     def get(self, key: str, default: Any = None) -> Any:
         return default
 
     def set(self, key: str, value: Any, ttl: Union[int, None] = None) -> None:
-        pass
+        return
 
     def delete(self, key: str) -> None:
         return
 
     def clear(self) -> None:
         return
+
+    def key_exists(self, key: str) -> bool:
+        return False
```

### Comparing `rds-core-0.1.2/rds_core/cache/search_engine.py` & `rds-core-0.2.0/rds/core/cache/search_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 """
 Documentar.
 """
 
 from typing import Any, List, Dict, Union
 
-import opensearchpy
-import elasticsearch
-from rds_core.cache.base import BaseCache
-from rds_core.searchengine import search_engine as search_engine_func
+from rds.core.cache.base import BaseCache
+from rds.core.searchengine import search_engine as search_engine_func
 
 
 class SearchEngineCache(BaseCache):
-
     def __init__(self, **params: Dict[str, Any]) -> None:
         super(SearchEngineCache, self).__init__(**params)
-        self.search_engine_alias: str = str(params.get("search_engine_alias", 'default'))
-        self.index_name: str = str(params.get("index_name", 'cnes_establecimento_cache'))
-        self.refresh: str = str(params.get("refresh", 'wait_for'))
+        self.search_engine_alias: str = str(params.get("search_engine_alias", "default"))
+        self.index_name: str = str(params.get("index_name", "cnes_establecimento_cache"))
+        self.refresh: str = str(params.get("refresh", "wait_for"))
 
     @property
     def search_engine(self) -> Any:
         return search_engine_func(self.search_engine_alias)
 
     def key_exists(self, key: str) -> bool:
         return self.search_engine.exists(self.index_name, id=key)
 
     def add(self, key: str, value: Any, ttl: Union[int, None] = None) -> bool:
-        """ Define um valor no cache caso a chave ainda não exista.
+        """Define um valor no cache caso a chave ainda não exista.
 
-            Caso já exista, não define o valor no cache, preservando o TTL.
+        Caso já exista, não define o valor no cache, preservando o TTL.
 
-            Args:
-                key (_type_): A chave a ser usada para identificar o valor no cache.
-                value (_type_): O valor a ser posto em cache.
-                ttl (_type_, optional): O tempo máximo que o item pode existir no cache. O padrão é None.
+        Args:
+            key (_type_): A chave a ser usada para identificar o valor no cache.
+            value (_type_): O valor a ser posto em cache.
+            ttl (_type_, optional): O tempo máximo que o item pode existir no cache. O padrão é None.
 
-            Raises:
-                NotImplementedError: _description_
+        Raises:
+            NotImplementedError: _description_
 
-            Returns:
-                bool: True adicionou, ou seja, se ainda não existia. False se já existia.
+        Returns:
+            bool: True adicionou, ou seja, se ainda não existia. False se já existia.
         """
         if self.key_exists(key):
             return False
-        body = {'value': value, 'ttl': self.get_ttl(ttl)}
+        body = {"value": value, "ttl": self.get_ttl(ttl)}
         self.search_engine.create(self.index_name, body=body, id=key, refresh=self.refresh)
         return True
 
     def get(self, key: str, default: Any = None) -> Any:
         try:
             response = self.search_engine.get(self.index_name, key)
-            doc = response['_source']
+            doc = response["_source"]
             # ttl = doc['ttl']
-            return doc['value'] if doc['value'] is not None else default
-        except opensearchpy.exceptions.NotFoundError:
-            return default
-        except elasticsearch.exceptions.NotFoundError:
-            return default
+            return doc["value"] if doc["value"] is not None else default
+        except Exception as e:
+            if str(type(e))[-15:-2] == "NotFoundError":
+                return default
+            raise e
 
     def set(self, key: str, value: Any, ttl: Union[int, None] = None) -> None:
         if type(value) == bytes:
             raise ValueError("Não suporta salvar bytes")
-        body = {'value': value, 'ttl': self.get_ttl(ttl)}
+        body = {"value": value, "ttl": self.get_ttl(ttl)}
         self.search_engine.index(self.index_name, body=body, id=key, refresh=self.refresh)
 
     def touch(self, key: str, ttl: Union[int, None] = None) -> bool:
         if self.key_exists(key):
-            self.search_engine.index(self.index_name, body={'ttl': self.get_ttl(ttl)}, id=key, refresh=self.refresh)
+            self.search_engine.index(self.index_name, body={"ttl": self.get_ttl(ttl)}, id=key, refresh=self.refresh)
             return True
         return False
 
     def delete(self, key: str) -> None:
         try:
             self.search_engine.delete(self.index_name, id=key, refresh=self.refresh)
-        except opensearchpy.exceptions.NotFoundError:
-            return None
-        except elasticsearch.exceptions.NotFoundError:
-            return None
+        except Exception as e:
+            if str(type(e))[-15:-2] == "NotFoundError":
+                return None
+            raise e
 
     def clear(self) -> None:
         raise NotImplementedError("subclasses of BaseCache must provide a clear() method")
 
     def get_many(self, keys: List[str]) -> Dict[str, Any]:
-        """ Fetch a bunch of keys from the cache. For certain backends (memcached, pgsql) this can be *much* faster
-            when fetching multiple values.
+        """Fetch a bunch of keys from the cache. For certain backends (memcached, pgsql) this can be *much* faster
+        when fetching multiple values.
 
-            Return a dict mapping each key in keys to its value. If the given key is missing, it will be missing from
-            the response dict.
+        Return a dict mapping each key in keys to its value. If the given key is missing, it will be missing from
+        the response dict.
         """
-        response = self.search_engine.mget({'ids': [k for k in keys]}, index=self.index_name)
-        return {x['_id']: x['_source']['value'] for x in response['docs'] if x['found']}
+        response = self.search_engine.mget({"ids": [k for k in keys]}, index=self.index_name)
+        return {x["_id"]: x["_source"]["value"] for x in response["docs"] if x["found"]}
```

### Comparing `rds-core-0.1.2/rds_core/helpers/__init__.py` & `rds-core-0.2.0/rds/core/helpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     ref = tmp.replace(".XX", "[0]")
     if tmp != ref:
         logger.warning("Warning: replaced '.XX' with [0]-th index")
     for key in ref.split("."):
         idstart = key.find("[")
         embedslist = 1 if idstart > 0 else 0
         if embedslist:
-            idx = int(key[idstart + 1: key.find("]")])
+            idx = int(key[idstart + 1 : key.find("]")])
             kyx = key[:idstart]
             try:
                 val = val[kyx][idx]
             except IndexError:
                 logger.warning(f"Index: x['{kyx}'][{idx}] does not exist.")
                 raise
         else:
```

### Comparing `rds-core-0.1.2/rds_core/helpers/http_client.py` & `rds-core-0.2.0/rds/core/helpers/http_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,45 +3,50 @@
 """
 
 from typing import Dict, List, Any, Union
 import json
 from http.client import HTTPException as OriginalHTTPException
 import requests
 from requests.structures import CaseInsensitiveDict
-from rds_core.config import settings
+from rds.core.config import settings
 
-DEFAULT_HEADERS: Dict[str, Any] = settings.get('DEFAULT_HEADERS', {})
+DEFAULT_HEADERS: Dict[str, Any] = settings.get("DEFAULT_HEADERS", {})
 
 
 class HTTPException(OriginalHTTPException):
-    def __init__(self,
-                 message: str,
-                 url: str,
-                 status_code: Union[str, None] = None,
-                 reason: Union[str, None] = None,
-                 request_headers: Union[Dict[Any, Any], None] = None,
-                 response_headers: Union[CaseInsensitiveDict, None] = None) -> None:
+    def __init__(
+        self,
+        message: str,
+        url: str,
+        status_code: Union[str, None] = None,
+        reason: Union[str, None] = None,
+        request_headers: Union[Dict[Any, Any], None] = None,
+        response_headers: Union[CaseInsensitiveDict, None] = None,
+    ) -> None:
         super().__init__(message)
         self.url = url
         self.status_code = status_code
         self.reason = reason
         self.request_headers = request_headers
         self.response_headers = response_headers
 
 
-def get(url: str, headers: Dict[str, str] = {}, encoding: str = 'utf-8', decode: bool = True, **kwargs) -> Any:
-
+def get(url: str, headers: Dict[str, str] = {}, encoding: str = "utf-8", decode: bool = True, **kwargs) -> Any:
     _headers = {**DEFAULT_HEADERS, **headers}
-    response = requests.get(url, headers=_headers, **kwargs)
+    try:
+        response = requests.get(url, headers=_headers, **kwargs)
+    except Exception as e:
+        raise e
 
     if response.ok:
-        byte_array_content = response.content
-        return byte_array_content.decode(encoding) if decode and encoding is not None else byte_array_content
+        result = response.content.decode(encoding) if decode and encoding is not None else response.content
+        return result
     else:
-        message = f'{response.status_code} - {response.reason}'
+        message = f"{response.status_code} - {response.reason}"
         raise HTTPException(message, url, str(response.status_code), response.reason, _headers, response.headers)
 
 
-def get_json(url: str, headers: Dict[str, str] = {}, encoding: str = 'utf-8',
-             json_kwargs: Dict[str, Any] = {}, **kwargs) -> Union[List[Any], Dict[str, Any]]:
+def get_json(
+    url: str, headers: Dict[str, str] = {}, encoding: str = "utf-8", json_kwargs: Dict[str, Any] = {}, **kwargs
+) -> Union[List[Any], Dict[str, Any]]:
     content = get(url, headers=headers, encoding=encoding, **kwargs)
     return json.loads(content, **json_kwargs)
```

### Comparing `rds-core-0.1.2/rds_core/searchengine/__init__.py` & `rds-core-0.2.0/rds/core/searchengine/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,42 @@
 """
 Documentar.
 """
 
 import datetime
 from typing import Dict, Union, Any, List
-import opensearchpy
-import elasticsearch
 from dynaconf.utils.boxing import DynaBox
-from rds_core.config import settings
-from rds_core.helpers import instantiate_class
+from rds.core.config import settings
+from rds.core.helpers import instantiate_class
 
 
 __search_engine_cache: Dict[str, Any] = {}
 
 
 def get_search_engine_config(alias: str = "default") -> DynaBox:
     return settings.SEARCH_ENGINES[alias]
 
 
 def search_engine(
     alias: str = "default",
     username: Union[str, None] = None,
     password: Union[str, None] = None,
-) -> Union[opensearchpy.OpenSearch, elasticsearch.Elasticsearch]:
+):
     se_config = get_search_engine_config(alias)
 
     engine = se_config["engine"]
-    params = {
-        k: v
-        for k, v in se_config.items()
-        if k not in ("username", "password", "engine", "dsl_engine", "hosts")
-    }
+    params = {k: v for k, v in se_config.items() if k not in ("username", "password", "engine", "dsl_engine", "hosts")}
     username = username if username else se_config["username"]
     password = password if password else se_config["password"]
     params["http_auth"] = (username, password)
     client = instantiate_class(engine, se_config["hosts"].split(","), **params)
     __search_engine_cache[alias] = client
     return client
 
 
-# def dsl_connection(alias: str = 'default') -> Union[opensearchpy.OpenSearch, elasticsearch.Elasticsearch]:
-#     se_config = get_search_engine_config(alias)
-#
-#     dsl_connections = get_variable_by_pathname(se_config['dsl_engine'])
-#     if alias not in dsl_connections.connections:
-#         dsl_connections.add_connection(alias, search_engine(alias))
-#     # dsl_connections.create_connection(
-#     #     alias=alias,
-#     #     http_auth=(se_config['user'], se_config['password']),
-#     #     **{k:v for k,v in se_config.items() if k not in ('user', 'password', 'engine', 'dsl_engine')},
-#     # )
-#     return dsl_connections.get_connection(alias)
-
-
 def create_index_if_not_exists(
     index: str,
     body: Union[dict, None] = None,
     params: Union[Dict[str, Any], None] = None,
     headers: Union[Dict[str, Any], None] = None,
     alias: str = "default",
 ) -> bool:
@@ -159,9 +139,8 @@
 
 
 def search_engine_healthy(
     params: Union[Dict[str, Any], None] = None,
     headers: Union[Dict[str, Any], None] = None,
     alias: str = "default",
 ) -> bool:
-    print(search_engine(alias).ping)
     return search_engine(alias).ping(params=params, headers=headers)
```

### Comparing `rds-core-0.1.2/rds_core/transformers/fields/__init__.py` & `rds-core-0.2.0/rds/core/transformers/fields/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 import logging
 from typing import Union, Dict, Any, List
 from datetime import datetime
-from rds_core.helpers import get_dict_by_pathname
+from rds.core.helpers import get_dict_by_pathname
 
 strptime = datetime.strptime
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 class Field:
     def __init__(self, source_field: Union[str, object, None]):
         self.source_field = source_field
 
-    def transform_to_dict(
-        self,
-        source_dict: Dict[str, Any],
-        dest_dict: Dict[str, Any],
-        dest_fieldname: str,
-    ):
+    def transform_to_dict(self, source_dict: Dict[str, Any], dest_dict: Dict[str, Any], dest_fieldname: str):
         if self.source_field is None:
             dest_dict[dest_fieldname] = None
         else:
-            dest_dict[dest_fieldname] = self.cast_source_value(
-                get_dict_by_pathname(source_dict, self.source_field)
-            )
+            dest_dict[dest_fieldname] = self.cast_source_value(get_dict_by_pathname(source_dict, self.source_field))
 
     def cast_source_value(self, source_value: Union[str, int, bool, float]):
         return source_value
 
 
 class CharField(Field):
     pass
 
 
 class DateField(Field):
     def __init__(self, source_field: str, format: str = "%d/%m/%Y"):
         super().__init__(source_field)
         self.format = format
 
-    def cast_source_value(
-        self, source_value: Union[None, str, int, bool, float]
-    ) -> datetime.date:
+    def cast_source_value(self, source_value: Union[None, str, int, bool, float]) -> datetime.date:
         return strptime(source_value, self.format) if source_value is not None else None
 
 
 class DateTimeField(Field):
     def __init__(self, source_field: str, format: str = "%d/%m/%Y %H:%M:%S"):
         super().__init__(source_field)
         self.format = format
@@ -57,30 +48,29 @@
 
 class SimpleConcatField(Field):
     def __init__(self, fields: Union[List[str], None] = None, separator: str = ""):
         super().__init__(None)
         self.fields = fields
         self.separator = separator
 
-    def transform_to_dict(
-        self,
-        source_dict: Dict[str, Any],
-        dest_dict: Dict[str, Any],
-        dest_fieldname: str,
-    ) -> str:
+    def transform_to_dict(self, source_dict: Dict[str, Any], dest_dict: Dict[str, Any], dest_fieldname: str) -> str:
         if self.fields is not None:
             dest_dict[dest_fieldname] = self.separator.join(
-                [
-                    self.cast_source_value(get_dict_by_pathname(source_dict, f))
-                    for f in self.fields
-                ]
+                [self.cast_source_value(get_dict_by_pathname(source_dict, f)) for f in self.fields]
             )
 
 
 class SubModelField(Field):
-    def transform_to_dict(
-        self,
-        source_dict: Dict[str, Any],
-        dest_dict: Dict[str, Any],
-        dest_fieldname: str,
-    ):
+    def transform_to_dict(self, source_dict: Dict[str, Any], dest_dict: Dict[str, Any], dest_fieldname: str):
         dest_dict[dest_fieldname] = self.source_field.transform_to_dict(source_dict)
+
+
+class FixedField(Field):
+    def __init__(self, fixed_value: str):
+        super().__init__(None)
+        self.fixed_value = fixed_value
+
+    def transform_to_dict(self, source_dict: Dict[str, Any], dest_dict: Dict[str, Any], dest_fieldname: str):
+        dest_dict[dest_fieldname] = self.cast_source_value(self.fixed_value)
+
+    def cast_source_value(self, source_value: Union[None, str, int, bool, float]) -> datetime.date:
+        return self.fixed_value
```

### Comparing `rds-core-0.1.2/rds_core/transformers/models/__init__.py` & `rds-core-0.2.0/rds/core/transformers/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from typing import Union, Dict, Any
 import inspect
-from rds_core.transformers.fields import Field
+import datetime
+from rds.core.transformers.fields import Field
 
 
 class ModelTransformer:
     __fields = None
 
     @classmethod
-    def transform_to_dict(
-        cls, source_dict: Union[Dict, None]
-    ) -> Union[Dict[str, Any], None]:
+    def transform_to_dict(cls, source_dict: Union[Dict, None]) -> Union[Dict[str, Any], None]:
         destination_dict = {}
+
         for destination_fieldname, transformer_field in cls.get_fields().items():
-            transformer_field.transform_to_dict(
-                source_dict, destination_dict, destination_fieldname
-            )
+            transformer_field.transform_to_dict(source_dict, destination_dict, destination_fieldname)
+
+        if hasattr(cls, "Meta") and hasattr(cls.Meta, "auto_timestamp") and cls.Meta.auto_timestamp:
+            timestamp_field = cls.Meta.timestamp_field if hasattr(cls.Meta, "timestamp_field") else "@timestamp"
+            destination_dict[timestamp_field] = datetime.datetime.now()
+
         return destination_dict
 
     @classmethod
     def get_fields(cls) -> dict:
         if cls.__fields is None:
-            cls.__fields = {}
-            for k, v in inspect.getmembers(cls):
-                if isinstance(v, Field):
-                    cls.__fields[k] = v
+            cls.__fields = {k: v for k, v in inspect.getmembers(cls) if isinstance(v, Field)}
+            # for k, v in inspect.getmembers(cls):
+            #     if isinstance(v, Field):
+            #         cls.__fields[k] = v
         return cls.__fields
```

### Comparing `rds-core-0.1.2/rds_core.egg-info/PKG-INFO` & `rds-core-0.2.0/rds_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.1.2
+Version: 0.2.0
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
```

### Comparing `rds-core-0.1.2/rds_core.egg-info/SOURCES.txt` & `rds-core-0.2.0/rds_core.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 LICENSE.md
 README.md
+pyproject.toml
 setup.cfg
 setup.py
-rds_core/__init__.py
+rds/contrib/__init__.py
+rds/contrib/datasus/__init__.py
+rds/contrib/datasus/transformers/__init__.py
+rds/contrib/datasus/transformers/fields/__init__.py
+rds/core/__init__.py
+rds/core/cache/__init__.py
+rds/core/cache/base.py
+rds/core/cache/inmemory.py
+rds/core/cache/nocache.py
+rds/core/cache/search_engine.py
+rds/core/config/__init__.py
+rds/core/helpers/__init__.py
+rds/core/helpers/http_client.py
+rds/core/searchengine/__init__.py
+rds/core/transformers/__init__.py
+rds/core/transformers/fields/__init__.py
+rds/core/transformers/models/__init__.py
 rds_core.egg-info/PKG-INFO
 rds_core.egg-info/SOURCES.txt
 rds_core.egg-info/dependency_links.txt
 rds_core.egg-info/requires.txt
-rds_core.egg-info/top_level.txt
-rds_core/cache/__init__.py
-rds_core/cache/base.py
-rds_core/cache/nocache.py
-rds_core/cache/search_engine.py
-rds_core/config/__init__.py
-rds_core/helpers/__init__.py
-rds_core/helpers/cnes.py
-rds_core/helpers/http_client.py
-rds_core/searchengine/__init__.py
-rds_core/transformers/fields/__init__.py
-rds_core/transformers/models/__init__.py
+rds_core.egg-info/top_level.txt
```

