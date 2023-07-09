# Comparing `tmp/secretbox-2.7.0.tar.gz` & `tmp/secretbox-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretbox-2.7.0.tar", last modified: Fri Aug  5 00:46:45 2022, max compression
+gzip compressed data, was "secretbox-2.8.0.tar", last modified: Sun Jul  9 20:13:58 2023, max compression
```

## Comparing `secretbox-2.7.0.tar` & `secretbox-2.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-08-05 00:46:45.280000 secretbox-2.7.0/
--rw-r--r--   0 preocts   (1000) preocts   (1000)     1064 2022-08-05 00:44:40.000000 secretbox-2.7.0/LICENSE
--rw-r--r--   0 preocts   (1000) preocts   (1000)    13679 2022-08-05 00:46:45.280000 secretbox-2.7.0/PKG-INFO
--rw-r--r--   0 preocts   (1000) preocts   (1000)    11447 2022-08-05 00:44:40.000000 secretbox-2.7.0/README.md
--rw-r--r--   0 preocts   (1000) preocts   (1000)     3065 2022-08-05 00:44:40.000000 secretbox-2.7.0/pyproject.toml
--rw-r--r--   0 preocts   (1000) preocts   (1000)       38 2022-08-05 00:46:45.280000 secretbox-2.7.0/setup.cfg
--rw-r--r--   0 preocts   (1000) preocts   (1000)       74 2022-08-05 00:44:40.000000 secretbox-2.7.0/setup.py
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-08-05 00:46:45.270000 secretbox-2.7.0/src/
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-08-05 00:46:45.280000 secretbox-2.7.0/src/secretbox/
--rw-r--r--   0 preocts   (1000) preocts   (1000)      389 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/__init__.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     3564 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/aws_loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     4851 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/awsparameterstore_loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     4381 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/awssecret_loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     3042 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/envfile_loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     1094 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/environ_loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)      631 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)       64 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/py.typed
--rw-r--r--   0 preocts   (1000) preocts   (1000)     4807 2022-08-05 00:44:40.000000 secretbox-2.7.0/src/secretbox/secretbox.py
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-08-05 00:46:45.280000 secretbox-2.7.0/src/secretbox.egg-info/
--rw-r--r--   0 preocts   (1000) preocts   (1000)    13679 2022-08-05 00:46:45.000000 secretbox-2.7.0/src/secretbox.egg-info/PKG-INFO
--rw-r--r--   0 preocts   (1000) preocts   (1000)      493 2022-08-05 00:46:45.000000 secretbox-2.7.0/src/secretbox.egg-info/SOURCES.txt
--rw-r--r--   0 preocts   (1000) preocts   (1000)        1 2022-08-05 00:46:45.000000 secretbox-2.7.0/src/secretbox.egg-info/dependency_links.txt
--rw-r--r--   0 preocts   (1000) preocts   (1000)      181 2022-08-05 00:46:45.000000 secretbox-2.7.0/src/secretbox.egg-info/requires.txt
--rw-r--r--   0 preocts   (1000) preocts   (1000)       10 2022-08-05 00:46:45.000000 secretbox-2.7.0/src/secretbox.egg-info/top_level.txt
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-09 20:13:58.482142 secretbox-2.8.0/
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     1064 2023-07-09 17:54:22.000000 secretbox-2.8.0/LICENSE
+-rw-r--r--   0 preocts   (1000) preocts   (1000)    14053 2023-07-09 20:13:58.482142 secretbox-2.8.0/PKG-INFO
+-rw-r--r--   0 preocts   (1000) preocts   (1000)    12160 2023-07-09 17:54:22.000000 secretbox-2.8.0/README.md
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     1846 2023-07-09 20:07:25.000000 secretbox-2.8.0/pyproject.toml
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       38 2023-07-09 20:13:58.482142 secretbox-2.8.0/setup.cfg
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       74 2023-07-09 17:54:22.000000 secretbox-2.8.0/setup.py
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-09 20:13:58.482142 secretbox-2.8.0/src/
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-09 20:13:58.482142 secretbox-2.8.0/src/secretbox/
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      389 2023-07-09 17:54:22.000000 secretbox-2.8.0/src/secretbox/__init__.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     4902 2023-07-09 19:55:47.000000 secretbox-2.8.0/src/secretbox/aws_loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     4072 2023-07-09 19:56:11.000000 secretbox-2.8.0/src/secretbox/awsparameterstore_loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     3533 2023-07-09 19:56:11.000000 secretbox-2.8.0/src/secretbox/awssecret_loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     3042 2023-07-09 17:54:22.000000 secretbox-2.8.0/src/secretbox/envfile_loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     1094 2023-07-09 17:54:22.000000 secretbox-2.8.0/src/secretbox/environ_loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      230 2023-07-09 17:54:22.000000 secretbox-2.8.0/src/secretbox/exceptions.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      631 2023-07-09 17:54:22.000000 secretbox-2.8.0/src/secretbox/loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       64 2023-07-09 17:54:22.000000 secretbox-2.8.0/src/secretbox/py.typed
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     4953 2023-07-09 17:54:22.000000 secretbox-2.8.0/src/secretbox/secretbox.py
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-09 20:13:58.482142 secretbox-2.8.0/src/secretbox.egg-info/
+-rw-r--r--   0 preocts   (1000) preocts   (1000)    14053 2023-07-09 20:13:58.000000 secretbox-2.8.0/src/secretbox.egg-info/PKG-INFO
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      521 2023-07-09 20:13:58.000000 secretbox-2.8.0/src/secretbox.egg-info/SOURCES.txt
+-rw-r--r--   0 preocts   (1000) preocts   (1000)        1 2023-07-09 20:13:58.000000 secretbox-2.8.0/src/secretbox.egg-info/dependency_links.txt
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      195 2023-07-09 20:13:58.000000 secretbox-2.8.0/src/secretbox.egg-info/requires.txt
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       10 2023-07-09 20:13:58.000000 secretbox-2.8.0/src/secretbox.egg-info/top_level.txt
```

### Comparing `secretbox-2.7.0/LICENSE` & `secretbox-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secretbox-2.7.0/PKG-INFO` & `secretbox-2.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretbox
-Version: 2.7.0
+Version: 2.8.0
 Summary: A library that offers a simple method of loading and accessing environmental variables and `.env` file values.
 Author-email: Preocts <preocts@preocts.com>
 License: MIT License
         
         Copyright (c) 2021 Preocts
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,48 +22,48 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/Preocts/secretbox
-Project-URL: documentation, https://github.com/Preocts/secretbox/README.md
-Project-URL: repository, https://github.com/Preocts/secretbox
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: aws
 License-File: LICENSE
 
-# secretbox
-
+[![Python 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Preocts/python-template/main.svg)](https://results.pre-commit.ci/latest/github/Preocts/python-template/main)
 [![Python Tests](https://github.com/Preocts/secretbox/actions/workflows/python-tests.yml/badge.svg)](https://github.com/Preocts/secretbox/actions/workflows/python-tests.yml)
-[![codecov](https://codecov.io/gh/Preocts/secretbox/branch/main/graph/badge.svg?token=7QFJGMD3JI)](https://codecov.io/gh/Preocts/secretbox)
+
+# secretbox
 
 A library that offers a simple method of loading and accessing environmental
 variables, `.env` file values, and other sources of secrets. The class stores
 values to state when load methods are called.
 
 Loaded values are also injected into the local environ. This is to assist with
 adjacent libraries that reference `os.environ` values by default. Required
 values can be kept in a `.env` file instead of managing a script to load them
 into the environment.
 
+**Note**: The default behavior of `secretbox` is to hide exceptions during
+loading. This places the detection of missing values on the caller. This
+behavior can be altered by passing `capture_exceptions=False` to any loader.
+Exceptions will be raised from their source as `LoaderException`.
+
 ---
 
 ### Requirements
 
 - Python >=3.7
 
 ### Optional Dependencies
@@ -94,25 +94,25 @@
 
 # Documentation:
 
 ## Example use with `auto_load=True`
 
 This loads the system environ and the `.env` from the current working directory
 into the class state for quick reference. Loaded secrets can be accessed from
-the `.values` property or from other methods such as `os.getenviron()`.
+the `.get()` method or from other methods such as `os.getenviron()`.
 
 ```python
 from secretbox import SecretBox
 
 secrets = SecretBox(auto_load=True)
 
 
 def main() -> int:
     """Main function"""
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -124,29 +124,30 @@
 loaded values then `.use_loaders()` is the solution. Each loader is executed in
 turn and the results compiled with the `SecretBox` object.
 
 This loads the system environment variables, an AWS secret store, and then a
 specific `.env` file if it exists. Secrets are loaded in the order of loaders,
 replacing any matching keys from the prior loader.
 
+
 ```python
 from secretbox import SecretBox
 
 secrets = SecretBox()
 
 
 def main() -> int:
     """Main function"""
     secrets.use_loaders(
         secrets.EnvironLoader(),
         secrets.AWSSecretLoader("mySecrets", "us-east-1"),
         secrets.EnvFileLoader("sandbox/.override_env"),
     )
 
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -163,15 +164,15 @@
 
 secrets = AWSParameterStoreLoader("mystore/params/", "us-west-2")
 secrets.run()
 
 
 def main() -> int:
     """Main function"""
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -188,14 +189,17 @@
   directory if found.
 
 **load_debug**
 
 - When true, internal logger level is set to DEBUG. Secret values are truncated,
   however it is not recommended to leave this on for production deployments.
 
+
+  *note:* Does not enable debug output for aws loaders.
+
 ### SecretBox API:
 
 **.values**
 
 - *Property*: A copy of the `dict[str, str]` key:value pairs loaded
 
 **.use_loaders(\*loaders: Loader) -> None**
@@ -243,25 +247,47 @@
 
 - Args:
   - aws_sstore: [str] Name of the secret store (not the arn)
     - Can be provided through environ `AWS_SSTORE_NAME`
   - aws_region: [str] Regional location of secret store
     - Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
 
+- Keyword Args:
+  - hide_boto_debug: [bool, default = `True`]
+    - Hides debug logging output from botocore clients to prevent exposing
+      plain-text secrets
+  - capture_exceptions: [bool, default = `True`]
+    - All internal exceptions are captured, logged, and ignored.
+
+- Raises:
+  - `LoaderException` if `capture_exceptions` is `False`. All exceptions are
+    raised from their source.
+
 **AWSParameterStoreLoader**
 
 Load secrets from AWS parameter store.
 
 - Args:
   - aws_sstore: [str] Name of parameter or path of parameters if endings with
     `/`
     - Can be provided through environ `AWS_SSTORE_NAME`
   - aws_region: [str] Regional Location of parameter(s)
     - Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
 
+- Keyword Args:
+  - hide_boto_debug: [bool, default = `True`]
+    - Hides debug logging output from botocore clients to prevent exposing
+      plain-text secrets
+  - capture_exceptions: [bool, default = `True`]
+    - All internal exceptions are captured, logged, and ignored.
+
+- Raises:
+  - `LoaderException` if `capture_exceptions` is `False`. All exceptions are
+    raised from their source.
+
 ---
 
 ## A note about logging output
 
 This library restricts any `DEBUG` logging output during the use of a `boto3`
 client or the methods of that client. This is to prevent the logging of your
 secrets as well as the bearer tokens used within AWS. You can disable this at
@@ -399,15 +425,15 @@
 ```console
 $ pre-commit run --all-files
 ```
 
 Run tests:
 
 ```console
-$ tox [-r] [-e py3x]
+$ tox
 ```
 
 Build dist:
 
 ```console
 $ python -m pip install --upgrade build
 
@@ -450,18 +476,14 @@
 
 ## Makefile
 
 This repo has a Makefile with some quality of life scripts if the system
 supports `make`.  Please note there are no checks for an active `venv` in the
 Makefile.
 
-| PHONY             | Description                                                           |
-| ----------------- | --------------------------------------------------------------------- |
-| `init`            | Update pip to newest version                                          |
-| `install`         | install the project                                                   |
-| `install-test`    | install test requirements and project as editable install             |
-| `install-dev`     | install development/test requirements and project as editable install |
-| `build-dist`      | Build source distribution and wheel distribution                      |
-| `clean-artifacts` | Deletes python/mypy artifacts, cache, and pyc files                   |
-| `clean-tests`     | Deletes tox, coverage, and pytest artifacts                           |
-| `clean-build`     | Deletes build artifacts                                               |
-| `clean-all`       | Runs all clean scripts                                                |
+| PHONY         | Description                                                           |
+| ------------- | --------------------------------------------------------------------- |
+| `install-dev` | install development/test requirements and project as editable install |
+| `coverage`    | Run tests with coverage, generate console report                      |
+| `docker-test' | Run coverage and tests in a docker container.                         |
+| `build-dist`  | Build source distribution and wheel distribution                      |
+| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts  |
```

### Comparing `secretbox-2.7.0/README.md` & `secretbox-2.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-# secretbox
-
+[![Python 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Preocts/python-template/main.svg)](https://results.pre-commit.ci/latest/github/Preocts/python-template/main)
 [![Python Tests](https://github.com/Preocts/secretbox/actions/workflows/python-tests.yml/badge.svg)](https://github.com/Preocts/secretbox/actions/workflows/python-tests.yml)
-[![codecov](https://codecov.io/gh/Preocts/secretbox/branch/main/graph/badge.svg?token=7QFJGMD3JI)](https://codecov.io/gh/Preocts/secretbox)
+
+# secretbox
 
 A library that offers a simple method of loading and accessing environmental
 variables, `.env` file values, and other sources of secrets. The class stores
 values to state when load methods are called.
 
 Loaded values are also injected into the local environ. This is to assist with
 adjacent libraries that reference `os.environ` values by default. Required
 values can be kept in a `.env` file instead of managing a script to load them
 into the environment.
 
+**Note**: The default behavior of `secretbox` is to hide exceptions during
+loading. This places the detection of missing values on the caller. This
+behavior can be altered by passing `capture_exceptions=False` to any loader.
+Exceptions will be raised from their source as `LoaderException`.
+
 ---
 
 ### Requirements
 
 - Python >=3.7
 
 ### Optional Dependencies
@@ -49,25 +55,25 @@
 
 # Documentation:
 
 ## Example use with `auto_load=True`
 
 This loads the system environ and the `.env` from the current working directory
 into the class state for quick reference. Loaded secrets can be accessed from
-the `.values` property or from other methods such as `os.getenviron()`.
+the `.get()` method or from other methods such as `os.getenviron()`.
 
 ```python
 from secretbox import SecretBox
 
 secrets = SecretBox(auto_load=True)
 
 
 def main() -> int:
     """Main function"""
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -79,29 +85,30 @@
 loaded values then `.use_loaders()` is the solution. Each loader is executed in
 turn and the results compiled with the `SecretBox` object.
 
 This loads the system environment variables, an AWS secret store, and then a
 specific `.env` file if it exists. Secrets are loaded in the order of loaders,
 replacing any matching keys from the prior loader.
 
+
 ```python
 from secretbox import SecretBox
 
 secrets = SecretBox()
 
 
 def main() -> int:
     """Main function"""
     secrets.use_loaders(
         secrets.EnvironLoader(),
         secrets.AWSSecretLoader("mySecrets", "us-east-1"),
         secrets.EnvFileLoader("sandbox/.override_env"),
     )
 
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -118,15 +125,15 @@
 
 secrets = AWSParameterStoreLoader("mystore/params/", "us-west-2")
 secrets.run()
 
 
 def main() -> int:
     """Main function"""
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -143,14 +150,17 @@
   directory if found.
 
 **load_debug**
 
 - When true, internal logger level is set to DEBUG. Secret values are truncated,
   however it is not recommended to leave this on for production deployments.
 
+
+  *note:* Does not enable debug output for aws loaders.
+
 ### SecretBox API:
 
 **.values**
 
 - *Property*: A copy of the `dict[str, str]` key:value pairs loaded
 
 **.use_loaders(\*loaders: Loader) -> None**
@@ -198,25 +208,47 @@
 
 - Args:
   - aws_sstore: [str] Name of the secret store (not the arn)
     - Can be provided through environ `AWS_SSTORE_NAME`
   - aws_region: [str] Regional location of secret store
     - Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
 
+- Keyword Args:
+  - hide_boto_debug: [bool, default = `True`]
+    - Hides debug logging output from botocore clients to prevent exposing
+      plain-text secrets
+  - capture_exceptions: [bool, default = `True`]
+    - All internal exceptions are captured, logged, and ignored.
+
+- Raises:
+  - `LoaderException` if `capture_exceptions` is `False`. All exceptions are
+    raised from their source.
+
 **AWSParameterStoreLoader**
 
 Load secrets from AWS parameter store.
 
 - Args:
   - aws_sstore: [str] Name of parameter or path of parameters if endings with
     `/`
     - Can be provided through environ `AWS_SSTORE_NAME`
   - aws_region: [str] Regional Location of parameter(s)
     - Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
 
+- Keyword Args:
+  - hide_boto_debug: [bool, default = `True`]
+    - Hides debug logging output from botocore clients to prevent exposing
+      plain-text secrets
+  - capture_exceptions: [bool, default = `True`]
+    - All internal exceptions are captured, logged, and ignored.
+
+- Raises:
+  - `LoaderException` if `capture_exceptions` is `False`. All exceptions are
+    raised from their source.
+
 ---
 
 ## A note about logging output
 
 This library restricts any `DEBUG` logging output during the use of a `boto3`
 client or the methods of that client. This is to prevent the logging of your
 secrets as well as the bearer tokens used within AWS. You can disable this at
@@ -354,15 +386,15 @@
 ```console
 $ pre-commit run --all-files
 ```
 
 Run tests:
 
 ```console
-$ tox [-r] [-e py3x]
+$ tox
 ```
 
 Build dist:
 
 ```console
 $ python -m pip install --upgrade build
 
@@ -405,18 +437,14 @@
 
 ## Makefile
 
 This repo has a Makefile with some quality of life scripts if the system
 supports `make`.  Please note there are no checks for an active `venv` in the
 Makefile.
 
-| PHONY             | Description                                                           |
-| ----------------- | --------------------------------------------------------------------- |
-| `init`            | Update pip to newest version                                          |
-| `install`         | install the project                                                   |
-| `install-test`    | install test requirements and project as editable install             |
-| `install-dev`     | install development/test requirements and project as editable install |
-| `build-dist`      | Build source distribution and wheel distribution                      |
-| `clean-artifacts` | Deletes python/mypy artifacts, cache, and pyc files                   |
-| `clean-tests`     | Deletes tox, coverage, and pytest artifacts                           |
-| `clean-build`     | Deletes build artifacts                                               |
-| `clean-all`       | Runs all clean scripts                                                |
+| PHONY         | Description                                                           |
+| ------------- | --------------------------------------------------------------------- |
+| `install-dev` | install development/test requirements and project as editable install |
+| `coverage`    | Run tests with coverage, generate console report                      |
+| `docker-test' | Run coverage and tests in a docker container.                         |
+| `build-dist`  | Build source distribution and wheel distribution                      |
+| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts  |
```

### Comparing `secretbox-2.7.0/src/secretbox/aws_loader.py` & `secretbox-2.8.0/src/secretbox/awsparameterstore_loader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,131 @@
 """
-Super class for AWS secrets manager and parameter store loaders
-
-Author  : Preocts <preocts#8196>
-Git Repo: https://github.com/Preocts/secretbox
+Author      : James McKain (@jjmckain)
+Created     : 2021-12-10
+SCM Repo    : https://github.com/Preocts/secretbox
 """
 from __future__ import annotations
 
-import logging
-import os
-from contextlib import contextmanager
 from typing import Any
-from typing import Generator
+from typing import TYPE_CHECKING
+
+from secretbox.aws_loader import AWSLoader
 
 try:
-    from botocore.awsrequest import HeadersDict
+    import boto3
 except ImportError:
-    HeadersDict = dict  # type: ignore
-
-from secretbox.loader import Loader
-
-
-class AWSLoader(Loader):
-    """Super class with mutual methods of AWS loaders, inherits Loader"""
+    if not TYPE_CHECKING:
+        boto3 = None
 
-    logger = logging.getLogger(__name__)
+try:
+    from mypy_boto3_ssm.client import SSMClient
+except ImportError:
+    if not TYPE_CHECKING:
+        SSMClient = None
 
-    # Override hide_boto_debug to False to allow full debug logging of boto3 libraries
-    # NOTE: This exposes sensitive data and should never be in production
-    hide_boto_debug = True
 
-    def _load_values(self, **kwargs: Any) -> bool:
-        """To be overrided in child classes"""
-        raise NotImplementedError()
+class AWSParameterStoreLoader(AWSLoader):
+    """Load secrets from an AWS Parameter Store"""
 
     @property
     def values(self) -> dict[str, str]:
-        """To be overrided in child classes"""
-        raise NotImplementedError()
+        """Copy of loaded values"""
+        return self._loaded_values.copy()
+
+    def _run(self) -> bool:
+        """Load secrets from given AWS parameter store."""
+        has_loaded = self._load_values()
+
+        for key, value in self._loaded_values.items():
+            self.logger.debug("Found, %s : ***%s", key, value[-(len(value) // 4) :])
 
-    def run(self) -> bool:
-        """To be overrided in child classes"""
-        raise NotImplementedError()
-
-    def get_aws_client(self) -> Any:
-        """Returns correct AWS client for low-level API requests"""
-        # NOTE: Override in client specific implementation
-        raise NotImplementedError
+        return has_loaded
 
-    def populate_region_store_names(
+    def _load_values(
         self,
-        sstore: str | None = None,
-        region: str | None = None,
-        **kwargs: str,
-    ) -> None:
-        """Populate store/region values."""
-        kw_sstore = sstore or kwargs.get("aws_sstore_name")
-        kw_region = region or kwargs.get("aws_region_name")
-        os_sstore = os.getenv("AWS_SSTORE_NAME")
-        os_region = os.getenv("AWS_REGION_NAME", os.getenv("AWS_REGION"))  # Lambda's
-
-        # Use the keyword over the os, default to None
-        self.aws_sstore = kw_sstore if kw_sstore is not None else os_sstore
-        self.aws_region = kw_region if kw_region is not None else os_region
-        self.logger.debug("Using store name '%s'", self.aws_sstore)
-        self.logger.debug("Using region name '%s'", self.aws_region)
-
-    def log_aws_error(self, err: Any) -> None:
-        """Verbose AWS error log output. If not an AWS error, generic repl of err"""
-        if (
-            hasattr(err, "response")  # assert attribute exists or fail early
-            and "Error" in err.response
-            and "ResponseMetadata" in err.response
-        ):
-            self.logger.error(
-                "%s - %s (%s)",
-                err.response["Error"]["Code"],
-                err.response["Error"]["Message"],
-                err.response["ResponseMetadata"],
+        aws_sstore_name: str | None = None,
+        aws_region_name: str | None = None,
+        **kwargs: Any,
+    ) -> bool:
+        """
+        Load all secrets from AWS parameter store.
+
+        Parameter values set at class instantiation are used if values
+        are not provided here.
+
+        Args:
+            aws_sstore: Name of parameter or path of parameters if endings with `/`
+                Can be provided through environ `AWS_SSTORE_NAME`
+            aws_region: Regional Location of parameter(s)
+                Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
+
+        Keyword Args:
+            Deprecated.
+        """
+        if boto3 is None:
+            self.logger.debug("Skipping AWS loader, boto3 is not available.")
+            return False
+
+        aws_sstore = aws_sstore_name or self.aws_sstore
+        aws_region = aws_region_name or self.aws_region
+
+        self.populate_region_store_names(aws_sstore, aws_region, **kwargs)
+        if self.aws_sstore is None:
+            self.logger.warning("Missing parameter name")
+            return True  # this isn't a failure on our part
+
+        aws_client = self.get_aws_client()
+        if aws_client is None:
+            self.logger.error("Invalid SSM client")
+            return False
+
+        # if the prefix contains forward slashes treat the last token as the key name
+        do_split = "/" in self.aws_sstore
+
+        args: dict[str, Any] = {
+            "Path": self.aws_sstore,
+            "Recursive": True,
+            "MaxResults": 10,
+            "WithDecryption": True,
+        }
+
+        # ensure that boto3 doesn't write sensitive payload to the logger
+        with self.disable_debug_logging():
+            # loop through next page tokens, page size caps at 10
+            while True:
+                resp = aws_client.get_parameters_by_path(**args)
+
+                # Process results, break if finished
+                for param in resp["Parameters"] or []:
+                    # remove the prefix
+                    # we want /path/to/DB_PASSWORD to populate os.env.DB_PASSWORD
+                    key = param["Name"].split("/")[-1] if do_split else param["Name"]
+                    self._loaded_values[key] = param["Value"]
+
+                args["NextToken"] = resp.get("NextToken")
+
+                if not args["NextToken"]:
+                    break
+
+                self.logger.debug("fetching next page: %s", args["NextToken"])
+
+        self.logger.info(
+            "loaded %d parameters matching %s",
+            len(self._loaded_values),
+            self.aws_sstore,
+        )
+        return True
+
+    def get_aws_client(self) -> SSMClient | None:
+        """Make the connection"""
+
+        if self.aws_region is None:
+            self.logger.debug("Missing AWS region, cannot create client")
+            return None
+
+        with self.disable_debug_logging():
+            client = boto3.client(
+                service_name="ssm",
+                region_name=self.aws_region,
             )
-        else:
-            self.logger.error("Unexpected error occurred: '%s'", str(err))
 
-    @contextmanager
-    def disable_debug_logging(self) -> Generator[None, None, None]:
-        """Context manager to enforce level 20 (INFO) logging minimum at root logger."""
-        # This should prevent boto and botocore loggers from outputting
-        # client secrets in plaintext if debug logging is on.
-        prior_root_level = logging.getLogger().level
-
-        if self.hide_boto_debug:
-            self.logger.info("Forcing all loggers to > DEBUG level.")
-            logging.getLogger().setLevel(logging.INFO)
-
-        try:
-            yield None
-
-        finally:
-            if self.hide_boto_debug:
-                self.logger.info("Restoring previous loggers settings.")
-                logging.getLogger().setLevel(prior_root_level)
+        return client
```

### Comparing `secretbox-2.7.0/src/secretbox/awssecret_loader.py` & `secretbox-2.8.0/src/secretbox/awssecret_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,56 +4,40 @@
 Author  : Preocts <Preocts#8196>
 Git Repo: https://github.com/Preocts/secretbox
 """
 from __future__ import annotations
 
 import json
 from typing import Any
+from typing import TYPE_CHECKING
 
 try:
     import boto3
-    from botocore.exceptions import ClientError
-    from botocore.exceptions import NoCredentialsError
 except ImportError:
-    boto3 = None  # type: ignore
+    if not TYPE_CHECKING:
+        boto3 = None
 
 try:
     from mypy_boto3_secretsmanager.client import SecretsManagerClient
 except ImportError:
-    SecretsManagerClient = None  # type: ignore
+    if not TYPE_CHECKING:
+        SecretsManagerClient = None
 
 from secretbox.aws_loader import AWSLoader
 
 
 class AWSSecretLoader(AWSLoader):
-    def __init__(
-        self,
-        aws_sstore_name: str | None = None,
-        aws_region_name: str | None = None,
-    ) -> None:
-        """
-        Load secrets from an AWS secret manager.
-
-        Args:
-            aws_sstore: Name of the secret store (not the arn)
-                Can be provided through environ `AWS_SSTORE_NAME`
-            aws_region: Regional location of secret store
-                Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
-        """
-        self.aws_sstore = aws_sstore_name
-        self.aws_region = aws_region_name
-
-        self._loaded_values: dict[str, str] = {}
+    """Load secrets from an AWS Secret Store"""
 
     @property
     def values(self) -> dict[str, str]:
         """Copy of loaded values"""
         return self._loaded_values.copy()
 
-    def run(self) -> bool:
+    def _run(self) -> bool:
         """Load all secrets from given AWS secret store."""
         has_loaded = self._load_values()
 
         for key, value in self._loaded_values.items():
             self.logger.debug("Found, %s : ***%s", key, value[-(len(value) // 4) :])
 
         return has_loaded
@@ -93,28 +77,21 @@
 
         aws_client = self.get_aws_client()
         if aws_client is None:
             self.logger.error("Invalid secrets manager client")
             return False
 
         secrets: dict[str, str] = {}
-        try:
-            # ensure that boto3 doesn't write sensitive payload to the logger
-            with self.disable_debug_logging():
-                response = aws_client.get_secret_value(SecretId=self.aws_sstore)
-
-        except NoCredentialsError as err:
-            self.logger.error("Missing AWS credentials (%s)", err)
-
-        except ClientError as err:
-            self.log_aws_error(err)
-
-        else:
-            secrets = self._resolve_response(response)
-            self._loaded_values.update(secrets)
+
+        # ensure that boto3 doesn't write sensitive payload to the logger
+        with self.disable_debug_logging():
+            response = aws_client.get_secret_value(SecretId=self.aws_sstore)
+
+        secrets = self._resolve_response(response)
+        self._loaded_values.update(secrets)
 
         return bool(secrets)
 
     def _resolve_response(self, response: Any) -> dict[str, str]:
         """Resolve response body to json."""
         try:
             secrets = json.loads(response.get("SecretString", "{}"))
@@ -132,9 +109,8 @@
             return None
 
         with self.disable_debug_logging():
             client = boto3.client(
                 service_name="secretsmanager",
                 region_name=self.aws_region,
             )
-
         return client
```

### Comparing `secretbox-2.7.0/src/secretbox/envfile_loader.py` & `secretbox-2.8.0/src/secretbox/envfile_loader.py`

 * *Files identical despite different names*

### Comparing `secretbox-2.7.0/src/secretbox/environ_loader.py` & `secretbox-2.8.0/src/secretbox/environ_loader.py`

 * *Files identical despite different names*

### Comparing `secretbox-2.7.0/src/secretbox/loader.py` & `secretbox-2.8.0/src/secretbox/loader.py`

 * *Files identical despite different names*

### Comparing `secretbox-2.7.0/src/secretbox/secretbox.py` & `secretbox-2.8.0/src/secretbox/secretbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,7 +128,11 @@
         return self._loaded_values.get(key, default)
 
     def set(self, key: str, value: str) -> None:  # noqa: A003
         """Set a value by key. Will be converted to string and pushed to environment."""
         value = str(value)
         self._loaded_values[key] = value
         self._push_to_environment()
+
+    def is_set(self, key: str) -> bool:
+        """Returns true if key is set in the loaded values."""
+        return key in self._loaded_values
```

### Comparing `secretbox-2.7.0/src/secretbox.egg-info/PKG-INFO` & `secretbox-2.8.0/src/secretbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretbox
-Version: 2.7.0
+Version: 2.8.0
 Summary: A library that offers a simple method of loading and accessing environmental variables and `.env` file values.
 Author-email: Preocts <preocts@preocts.com>
 License: MIT License
         
         Copyright (c) 2021 Preocts
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,48 +22,48 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/Preocts/secretbox
-Project-URL: documentation, https://github.com/Preocts/secretbox/README.md
-Project-URL: repository, https://github.com/Preocts/secretbox
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: aws
 License-File: LICENSE
 
-# secretbox
-
+[![Python 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Preocts/python-template/main.svg)](https://results.pre-commit.ci/latest/github/Preocts/python-template/main)
 [![Python Tests](https://github.com/Preocts/secretbox/actions/workflows/python-tests.yml/badge.svg)](https://github.com/Preocts/secretbox/actions/workflows/python-tests.yml)
-[![codecov](https://codecov.io/gh/Preocts/secretbox/branch/main/graph/badge.svg?token=7QFJGMD3JI)](https://codecov.io/gh/Preocts/secretbox)
+
+# secretbox
 
 A library that offers a simple method of loading and accessing environmental
 variables, `.env` file values, and other sources of secrets. The class stores
 values to state when load methods are called.
 
 Loaded values are also injected into the local environ. This is to assist with
 adjacent libraries that reference `os.environ` values by default. Required
 values can be kept in a `.env` file instead of managing a script to load them
 into the environment.
 
+**Note**: The default behavior of `secretbox` is to hide exceptions during
+loading. This places the detection of missing values on the caller. This
+behavior can be altered by passing `capture_exceptions=False` to any loader.
+Exceptions will be raised from their source as `LoaderException`.
+
 ---
 
 ### Requirements
 
 - Python >=3.7
 
 ### Optional Dependencies
@@ -94,25 +94,25 @@
 
 # Documentation:
 
 ## Example use with `auto_load=True`
 
 This loads the system environ and the `.env` from the current working directory
 into the class state for quick reference. Loaded secrets can be accessed from
-the `.values` property or from other methods such as `os.getenviron()`.
+the `.get()` method or from other methods such as `os.getenviron()`.
 
 ```python
 from secretbox import SecretBox
 
 secrets = SecretBox(auto_load=True)
 
 
 def main() -> int:
     """Main function"""
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -124,29 +124,30 @@
 loaded values then `.use_loaders()` is the solution. Each loader is executed in
 turn and the results compiled with the `SecretBox` object.
 
 This loads the system environment variables, an AWS secret store, and then a
 specific `.env` file if it exists. Secrets are loaded in the order of loaders,
 replacing any matching keys from the prior loader.
 
+
 ```python
 from secretbox import SecretBox
 
 secrets = SecretBox()
 
 
 def main() -> int:
     """Main function"""
     secrets.use_loaders(
         secrets.EnvironLoader(),
         secrets.AWSSecretLoader("mySecrets", "us-east-1"),
         secrets.EnvFileLoader("sandbox/.override_env"),
     )
 
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -163,15 +164,15 @@
 
 secrets = AWSParameterStoreLoader("mystore/params/", "us-west-2")
 secrets.run()
 
 
 def main() -> int:
     """Main function"""
-    my_sevice_password = secrets.values.get("SERVICE_PW")
+    my_sevice_password = secrets.get("SERVICE_PW")
     # More code
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 ```
@@ -188,14 +189,17 @@
   directory if found.
 
 **load_debug**
 
 - When true, internal logger level is set to DEBUG. Secret values are truncated,
   however it is not recommended to leave this on for production deployments.
 
+
+  *note:* Does not enable debug output for aws loaders.
+
 ### SecretBox API:
 
 **.values**
 
 - *Property*: A copy of the `dict[str, str]` key:value pairs loaded
 
 **.use_loaders(\*loaders: Loader) -> None**
@@ -243,25 +247,47 @@
 
 - Args:
   - aws_sstore: [str] Name of the secret store (not the arn)
     - Can be provided through environ `AWS_SSTORE_NAME`
   - aws_region: [str] Regional location of secret store
     - Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
 
+- Keyword Args:
+  - hide_boto_debug: [bool, default = `True`]
+    - Hides debug logging output from botocore clients to prevent exposing
+      plain-text secrets
+  - capture_exceptions: [bool, default = `True`]
+    - All internal exceptions are captured, logged, and ignored.
+
+- Raises:
+  - `LoaderException` if `capture_exceptions` is `False`. All exceptions are
+    raised from their source.
+
 **AWSParameterStoreLoader**
 
 Load secrets from AWS parameter store.
 
 - Args:
   - aws_sstore: [str] Name of parameter or path of parameters if endings with
     `/`
     - Can be provided through environ `AWS_SSTORE_NAME`
   - aws_region: [str] Regional Location of parameter(s)
     - Can be provided through environ `AWS_REGION_NAME` or `AWS_REGION`
 
+- Keyword Args:
+  - hide_boto_debug: [bool, default = `True`]
+    - Hides debug logging output from botocore clients to prevent exposing
+      plain-text secrets
+  - capture_exceptions: [bool, default = `True`]
+    - All internal exceptions are captured, logged, and ignored.
+
+- Raises:
+  - `LoaderException` if `capture_exceptions` is `False`. All exceptions are
+    raised from their source.
+
 ---
 
 ## A note about logging output
 
 This library restricts any `DEBUG` logging output during the use of a `boto3`
 client or the methods of that client. This is to prevent the logging of your
 secrets as well as the bearer tokens used within AWS. You can disable this at
@@ -399,15 +425,15 @@
 ```console
 $ pre-commit run --all-files
 ```
 
 Run tests:
 
 ```console
-$ tox [-r] [-e py3x]
+$ tox
 ```
 
 Build dist:
 
 ```console
 $ python -m pip install --upgrade build
 
@@ -450,18 +476,14 @@
 
 ## Makefile
 
 This repo has a Makefile with some quality of life scripts if the system
 supports `make`.  Please note there are no checks for an active `venv` in the
 Makefile.
 
-| PHONY             | Description                                                           |
-| ----------------- | --------------------------------------------------------------------- |
-| `init`            | Update pip to newest version                                          |
-| `install`         | install the project                                                   |
-| `install-test`    | install test requirements and project as editable install             |
-| `install-dev`     | install development/test requirements and project as editable install |
-| `build-dist`      | Build source distribution and wheel distribution                      |
-| `clean-artifacts` | Deletes python/mypy artifacts, cache, and pyc files                   |
-| `clean-tests`     | Deletes tox, coverage, and pytest artifacts                           |
-| `clean-build`     | Deletes build artifacts                                               |
-| `clean-all`       | Runs all clean scripts                                                |
+| PHONY         | Description                                                           |
+| ------------- | --------------------------------------------------------------------- |
+| `install-dev` | install development/test requirements and project as editable install |
+| `coverage`    | Run tests with coverage, generate console report                      |
+| `docker-test' | Run coverage and tests in a docker container.                         |
+| `build-dist`  | Build source distribution and wheel distribution                      |
+| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts  |
```

