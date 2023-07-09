# Comparing `tmp/simple-rsa-1.0.0.tar.gz` & `tmp/simple-rsa-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simple-rsa-1.0.0.tar", last modified: Mon Mar 18 21:48:55 2019, max compression
+gzip compressed data, was "simple-rsa-1.1.0.tar", last modified: Sun Jul  9 17:59:11 2023, max compression
```

## Comparing `simple-rsa-1.0.0.tar` & `simple-rsa-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/
--rw-r--r--   0 xtof       (501) staff       (20)     4058 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/simple_rsa/
--rw-r--r--   0 xtof       (501) staff       (20)     1790 2019-03-18 21:21:34.000000 simple-rsa-1.0.0/simple_rsa/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      783 2019-03-18 21:00:11.000000 simple-rsa-1.0.0/Makefile
--rw-r--r--   0 xtof       (501) staff       (20)      107 2019-03-18 21:00:11.000000 simple-rsa-1.0.0/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1626 2019-03-18 21:22:28.000000 simple-rsa-1.0.0/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     2929 2019-03-18 21:43:11.000000 simple-rsa-1.0.0/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)       38 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/setup.cfg
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/simple_rsa.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     4058 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/simple_rsa.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      239 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/simple_rsa.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)       13 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/simple_rsa.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       11 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/simple_rsa.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2019-03-18 21:48:55.000000 simple-rsa-1.0.0/simple_rsa.egg-info/dependency_links.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-09 17:59:11.577037 simple-rsa-1.1.0/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-09 17:59:11.576077 simple-rsa-1.1.0/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     3035 2023-07-09 17:54:33.000000 simple-rsa-1.1.0/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1067 2023-07-09 17:40:18.000000 simple-rsa-1.1.0/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      107 2023-07-09 17:40:18.000000 simple-rsa-1.1.0/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)      262 2023-07-09 17:58:22.000000 simple-rsa-1.1.0/Makefile
+-rw-r--r--   0 xtof       (501) staff       (20)     4202 2023-07-09 17:59:11.576938 simple-rsa-1.1.0/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-07-09 17:59:11.577072 simple-rsa-1.1.0/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1583 2023-07-09 17:53:35.000000 simple-rsa-1.1.0/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-09 17:59:11.576185 simple-rsa-1.1.0/simple_rsa/
+-rw-r--r--   0 xtof       (501) staff       (20)     1790 2023-07-09 17:53:26.000000 simple-rsa-1.1.0/simple_rsa/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-09 17:59:11.576684 simple-rsa-1.1.0/simple_rsa.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     4202 2023-07-09 17:59:11.000000 simple-rsa-1.1.0/simple_rsa.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      292 2023-07-09 17:59:11.000000 simple-rsa-1.1.0/simple_rsa.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-07-09 17:59:11.000000 simple-rsa-1.1.0/simple_rsa.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       13 2023-07-09 17:59:11.000000 simple-rsa-1.1.0/simple_rsa.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       11 2023-07-09 17:59:11.000000 simple-rsa-1.1.0/simple_rsa.egg-info/top_level.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-07-09 17:59:11.576788 simple-rsa-1.1.0/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)      583 2023-07-09 17:40:18.000000 simple-rsa-1.1.0/tests/test_basic_encoding_and_signing.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `simple-rsa-1.0.0/PKG-INFO` & `simple-rsa-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 Metadata-Version: 2.1
 Name: simple-rsa
-Version: 1.0.0
+Version: 1.1.0
 Summary: A straightforward API to perform basic RSA-based operations..
 Home-page: https://github.com/christophevg/py-simple-rsa
 Author: Christophe VG
 License: MIT
 Description: # Simple RSA
         
         > A straightforward API to perform basic RSA-based operations.
         
         [![Latest Version on PyPI](https://img.shields.io/pypi/v/simple-rsa.svg)](https://pypi.python.org/pypi/simple-rsa/)
         [![Supported Implementations](https://img.shields.io/pypi/pyversions/simple-rsa.svg)](https://pypi.python.org/pypi/simple-rsa/)
-        [![Build Status](https://secure.travis-ci.org/christophevg/py-simple-rsa.svg?branch=master)](http://travis-ci.org/christophevg/py-simple-rsa)
         [![Coverage Status](https://coveralls.io/repos/github/christophevg/py-simple-rsa/badge.svg?branch=master)](https://coveralls.io/github/christophevg/py-simple-rsa?branch=master)
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.0.6-blue.svg)](https://github.com/christophevg/pypi-template)
         
         ## Rationale
         
         Any cryptographic library exposes all possibilities, and it should. But sometimes you just want a simple `sign` and `validate` API. That is what this wrapper module around the Cryptography module is. Nothing more, nothing less.
         
+        ## Minimal Survival Commands
+        
+        ```console
+        % pip install simple-rsa
+        ```
+        
+        When running from the repo (probably in some virtualenv) install cryptography and optionally `tox` is you want to run the tests:
+        
+        ```console
+        % pip install cryptography tox
+        ```
+        
         ## Getting Started
         
         The module basically exposes the following functions:
         
         - `generate_key_pair()` returning a tuple of private and public keys
         - `encode(key)` returning an encoded key
         - `decode(pem)` returning a key
@@ -60,10 +71,9 @@
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `simple-rsa-1.0.0/simple_rsa/__init__.py` & `simple-rsa-1.1.0/simple_rsa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ A straightforward API to perform basic RSA-based operations.
 
 .. moduleauthor:: Christophe VG <contact@christophe.vg>
 
 """
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 from cryptography.hazmat.backends import default_backend
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 
 from cryptography.hazmat.primitives.asymmetric import rsa
```

### Comparing `simple-rsa-1.0.0/setup.py` & `simple-rsa-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
   "Environment :: Console",
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "Topic :: Software Development",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 2.7",
   "Programming Language :: Python :: 3.7",
 ]
 INSTALL_REQUIRES = [
   "cryptography"
 ]
 ENTRY_POINTS     = {}
 SCRIPTS          = []
```

### Comparing `simple-rsa-1.0.0/.github/README.md` & `simple-rsa-1.1.0/.github/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # Simple RSA
 
 > A straightforward API to perform basic RSA-based operations.
 
 [![Latest Version on PyPI](https://img.shields.io/pypi/v/simple-rsa.svg)](https://pypi.python.org/pypi/simple-rsa/)
 [![Supported Implementations](https://img.shields.io/pypi/pyversions/simple-rsa.svg)](https://pypi.python.org/pypi/simple-rsa/)
-[![Build Status](https://secure.travis-ci.org/christophevg/py-simple-rsa.svg?branch=master)](http://travis-ci.org/christophevg/py-simple-rsa)
 [![Coverage Status](https://coveralls.io/repos/github/christophevg/py-simple-rsa/badge.svg?branch=master)](https://coveralls.io/github/christophevg/py-simple-rsa?branch=master)
 [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.0.6-blue.svg)](https://github.com/christophevg/pypi-template)
 
 ## Rationale
 
 Any cryptographic library exposes all possibilities, and it should. But sometimes you just want a simple `sign` and `validate` API. That is what this wrapper module around the Cryptography module is. Nothing more, nothing less.
 
+## Minimal Survival Commands
+
+```console
+% pip install simple-rsa
+```
+
+When running from the repo (probably in some virtualenv) install cryptography and optionally `tox` is you want to run the tests:
+
+```console
+% pip install cryptography tox
+```
+
 ## Getting Started
 
 The module basically exposes the following functions:
 
 - `generate_key_pair()` returning a tuple of private and public keys
 - `encode(key)` returning an encoded key
 - `decode(pem)` returning a key
```

### Comparing `simple-rsa-1.0.0/simple_rsa.egg-info/PKG-INFO` & `simple-rsa-1.1.0/simple_rsa.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 Metadata-Version: 2.1
 Name: simple-rsa
-Version: 1.0.0
+Version: 1.1.0
 Summary: A straightforward API to perform basic RSA-based operations..
 Home-page: https://github.com/christophevg/py-simple-rsa
 Author: Christophe VG
 License: MIT
 Description: # Simple RSA
         
         > A straightforward API to perform basic RSA-based operations.
         
         [![Latest Version on PyPI](https://img.shields.io/pypi/v/simple-rsa.svg)](https://pypi.python.org/pypi/simple-rsa/)
         [![Supported Implementations](https://img.shields.io/pypi/pyversions/simple-rsa.svg)](https://pypi.python.org/pypi/simple-rsa/)
-        [![Build Status](https://secure.travis-ci.org/christophevg/py-simple-rsa.svg?branch=master)](http://travis-ci.org/christophevg/py-simple-rsa)
         [![Coverage Status](https://coveralls.io/repos/github/christophevg/py-simple-rsa/badge.svg?branch=master)](https://coveralls.io/github/christophevg/py-simple-rsa?branch=master)
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.0.6-blue.svg)](https://github.com/christophevg/pypi-template)
         
         ## Rationale
         
         Any cryptographic library exposes all possibilities, and it should. But sometimes you just want a simple `sign` and `validate` API. That is what this wrapper module around the Cryptography module is. Nothing more, nothing less.
         
+        ## Minimal Survival Commands
+        
+        ```console
+        % pip install simple-rsa
+        ```
+        
+        When running from the repo (probably in some virtualenv) install cryptography and optionally `tox` is you want to run the tests:
+        
+        ```console
+        % pip install cryptography tox
+        ```
+        
         ## Getting Started
         
         The module basically exposes the following functions:
         
         - `generate_key_pair()` returning a tuple of private and public keys
         - `encode(key)` returning an encoded key
         - `decode(pem)` returning a key
@@ -60,10 +71,9 @@
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

