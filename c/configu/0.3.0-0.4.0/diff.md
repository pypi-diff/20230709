# Comparing `tmp/configu-0.3.0.tar.gz` & `tmp/configu-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configu-0.3.0.tar", max compression
+gzip compressed data, was "configu-0.4.0.tar", max compression
```

## Comparing `configu-0.3.0.tar` & `configu-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     1753 2023-06-29 07:04:01.013370 configu-0.3.0/README.md
--rw-r--r--   0        0        0      714 2023-06-29 07:04:01.013370 configu-0.3.0/configu/__init__.py
--rw-r--r--   0        0        0      182 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/__init__.py
--rw-r--r--   0        0        0    11921 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/eval_command.py
--rw-r--r--   0        0        0     1033 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/export_command.py
--rw-r--r--   0        0        0     3070 2023-06-29 07:04:01.013370 configu-0.3.0/configu/commands/upsert_command.py
--rw-r--r--   0        0        0      423 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/__init__.py
--rw-r--r--   0        0        0      524 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/command.py
--rw-r--r--   0        0        0     6880 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/config_schema.py
--rw-r--r--   0        0        0     1822 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/config_set.py
--rw-r--r--   0        0        0      995 2023-06-29 07:04:01.013370 configu-0.3.0/configu/core/config_store.py
--rw-r--r--   0        0        0    11311 2023-06-29 07:04:29.245509 configu-0.3.0/configu/core/generated.py
--rw-r--r--   0        0        0      342 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/__init__.py
--rw-r--r--   0        0        0      904 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/aws_secrets_manager_store.py
--rw-r--r--   0        0        0     2495 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/configu_store.py
--rw-r--r--   0        0        0     1373 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/in_memory_store.py
--rw-r--r--   0        0        0     2496 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/json_file_store.py
--rw-r--r--   0        0        0     3271 2023-06-29 07:04:01.013370 configu-0.3.0/configu/stores/key_value_store.py
--rw-r--r--   0        0        0     1239 2023-06-29 07:04:01.013370 configu-0.3.0/configu/utils.py
--rw-r--r--   0        0        0     1904 2023-06-29 07:05:02.477689 configu-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 configu-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1753 2023-07-09 11:49:30.182188 configu-0.4.0/README.md
+-rw-r--r--   0        0        0      976 2023-07-09 11:49:30.182188 configu-0.4.0/configu/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-09 11:49:30.182188 configu-0.4.0/configu/commands/__init__.py
+-rw-r--r--   0        0        0    11921 2023-07-09 11:49:30.182188 configu-0.4.0/configu/commands/eval_command.py
+-rw-r--r--   0        0        0     1033 2023-07-09 11:49:30.182188 configu-0.4.0/configu/commands/export_command.py
+-rw-r--r--   0        0        0     3070 2023-07-09 11:49:30.182188 configu-0.4.0/configu/commands/upsert_command.py
+-rw-r--r--   0        0        0      423 2023-07-09 11:49:30.182188 configu-0.4.0/configu/core/__init__.py
+-rw-r--r--   0        0        0      524 2023-07-09 11:49:30.182188 configu-0.4.0/configu/core/command.py
+-rw-r--r--   0        0        0     6880 2023-07-09 11:49:30.182188 configu-0.4.0/configu/core/config_schema.py
+-rw-r--r--   0        0        0     1822 2023-07-09 11:49:30.182188 configu-0.4.0/configu/core/config_set.py
+-rw-r--r--   0        0        0      995 2023-07-09 11:49:30.182188 configu-0.4.0/configu/core/config_store.py
+-rw-r--r--   0        0        0    11311 2023-07-09 11:49:58.884422 configu-0.4.0/configu/core/generated.py
+-rw-r--r--   0        0        0      723 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/__init__.py
+-rw-r--r--   0        0        0      904 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/aws_secrets_manager_store.py
+-rw-r--r--   0        0        0     1301 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/azure_key_vault_store.py
+-rw-r--r--   0        0        0     2495 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/configu_store.py
+-rw-r--r--   0        0        0     1544 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/gcp_secret_manager.py
+-rw-r--r--   0        0        0     1608 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/hashicorp_vault_store.py
+-rw-r--r--   0        0        0     1373 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/in_memory_store.py
+-rw-r--r--   0        0        0     2496 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/json_file_store.py
+-rw-r--r--   0        0        0     3413 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/key_value_store.py
+-rw-r--r--   0        0        0     1803 2023-07-09 11:49:30.182188 configu-0.4.0/configu/stores/kubernetes_secret_store.py
+-rw-r--r--   0        0        0     1239 2023-07-09 11:49:30.182188 configu-0.4.0/configu/utils.py
+-rw-r--r--   0        0        0     2028 2023-07-09 11:50:36.759389 configu-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 configu-0.4.0/PKG-INFO
```

### Comparing `configu-0.3.0/README.md` & `configu-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/__init__.py` & `configu-0.4.0/configu/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     ConfigStoreQuery,
 )
 from .stores import (
     ConfiguConfigStore,
     InMemoryConfigStore,
     JsonFileConfigStore,
     AWSSecretsManagerConfigStore,
+    HashicorpVaultConfigStore,
+    AzureKeyVaultConfigStore,
+    GCPSecretManagerConfigStore,
+    KubernetesSecretConfigStore,
 )
 
 __all__ = [
     "EvalCommand",
     "UpsertCommand",
     "ExportCommand",
     "Command",
@@ -30,8 +34,12 @@
     "Cfgu",
     "CfguType",
     "ConfigSchemaType",
     "InMemoryConfigStore",
     "ConfiguConfigStore",
     "JsonFileConfigStore",
     "AWSSecretsManagerConfigStore",
+    "HashicorpVaultConfigStore",
+    "AzureKeyVaultConfigStore",
+    "GCPSecretManagerConfigStore",
+    "KubernetesSecretConfigStore",
 ]
```

### Comparing `configu-0.3.0/configu/commands/eval_command.py` & `configu-0.4.0/configu/commands/eval_command.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/commands/export_command.py` & `configu-0.4.0/configu/commands/export_command.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/commands/upsert_command.py` & `configu-0.4.0/configu/commands/upsert_command.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/core/command.py` & `configu-0.4.0/configu/core/command.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/core/config_schema.py` & `configu-0.4.0/configu/core/config_schema.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/core/config_set.py` & `configu-0.4.0/configu/core/config_set.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/core/config_store.py` & `configu-0.4.0/configu/core/config_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/core/generated.py` & `configu-0.4.0/configu/core/generated.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/stores/aws_secrets_manager_store.py` & `configu-0.4.0/configu/stores/aws_secrets_manager_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/stores/configu_store.py` & `configu-0.4.0/configu/stores/configu_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/stores/in_memory_store.py` & `configu-0.4.0/configu/stores/in_memory_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/stores/json_file_store.py` & `configu-0.4.0/configu/stores/json_file_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/configu/stores/key_value_store.py` & `configu-0.4.0/configu/stores/key_value_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,8 +99,13 @@
                 config.key: config.value,
             }
 
         for key, value in key_value_dict.items():
             if value == "" or value is None:
                 self.delete(key)
             else:
-                self.upsert(key, json.dumps(value))
+                self.upsert(
+                    key,
+                    json.dumps(value)
+                    if isinstance(value, dict)
+                    else str(value),
+                )
```

### Comparing `configu-0.3.0/configu/utils.py` & `configu-0.4.0/configu/utils.py`

 * *Files identical despite different names*

### Comparing `configu-0.3.0/pyproject.toml` & `configu-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configu"
-version = "0.3.0"
+version = "0.4.0"
 description = "Configu Python SDK"
 authors = ["Configu <info@configu.com>"]
 maintainers = [
   "Ron Roditi <ron@configu.com>",
   "Or Levi <orlevi128@gmail.com>"
 ]
 license = "Apache-2.0"
@@ -32,14 +32,18 @@
 python = ">=3.9,<3.12"
 requests = "^2.28.1"
 py-validator = "^0.17.0"
 pydantic = "^1.10.6"
 chevron = "^0.14.0"
 boto3 = "^1.26.155"
 boto3-stubs = { extras = ["secretsmanager"], version = "^1.26.155" }
+azure-keyvault-secrets = "^4.7.0"
+azure-identity = "^1.13.0"
+google-cloud-secret-manager = "^2.16.1"
+kubernetes = "^26.1.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0" # configs at .flake8
 black = { extras = ["d"], version = "^23.1.0" }
 pdoc = "^13.1.0" # https://pdoc.dev/docs/pdoc.html
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `configu-0.3.0/PKG-INFO` & `configu-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configu
-Version: 0.3.0
+Version: 0.4.0
 Summary: Configu Python SDK
 Home-page: https://configu.com/
 License: Apache-2.0
 Keywords: cfgu,configu,configu-sdk,configu-python-sdk
 Author: Configu
 Author-email: info@configu.com
 Maintainer: Ron Roditi
@@ -16,17 +16,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
+Requires-Dist: azure-identity (>=1.13.0,<2.0.0)
+Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
 Requires-Dist: boto3 (>=1.26.155,<2.0.0)
 Requires-Dist: boto3-stubs[secretsmanager] (>=1.26.155,<2.0.0)
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
+Requires-Dist: google-cloud-secret-manager (>=2.16.1,<3.0.0)
+Requires-Dist: kubernetes (>=26.1.0,<27.0.0)
 Requires-Dist: py-validator (>=0.17.0,<0.18.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://configu.com/docs/
 Project-URL: Repository, https://github.com/configu/configu
 Description-Content-Type: text/markdown
```

