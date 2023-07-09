# Comparing `tmp/parrot-api-core-0.1.8.tar.gz` & `tmp/parrot-api-core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parrot-api-core-0.1.8.tar", last modified: Sun Jun  5 16:52:55 2022, max compression
+gzip compressed data, was "parrot-api-core-0.1.9.tar", last modified: Sun Jun  5 16:56:17 2022, max compression
```

## Comparing `parrot-api-core-0.1.8.tar` & `parrot-api-core-0.1.9.tar`

### file list

```diff
@@ -1,98 +1,48 @@
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.888836 parrot-api-core-0.1.8/
--rw-r--r--   0 perrystallings   (501) staff       (20)      158 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/AUTHORS.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)     3622 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)       89 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/HISTORY.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)     1074 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/LICENSE
--rw-r--r--   0 perrystallings   (501) staff       (20)      262 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/MANIFEST.in
--rw-r--r--   0 perrystallings   (501) staff       (20)     1962 2022-06-05 16:52:55.888922 parrot-api-core-0.1.8/PKG-INFO
--rw-r--r--   0 perrystallings   (501) staff       (20)     1115 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/README.rst
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.875761 parrot-api-core-0.1.8/docs/
--rw-r--r--   0 perrystallings   (501) staff       (20)      616 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/Makefile
--rw-r--r--   0 perrystallings   (501) staff       (20)       28 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/authors.rst
--rwxr-xr-x   0 perrystallings   (501) staff       (20)     4891 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/conf.py
--rw-r--r--   0 perrystallings   (501) staff       (20)       33 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/contributing.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)       28 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/history.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)      312 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/index.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)     1202 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/installation.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)      777 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/make.bat
--rw-r--r--   0 perrystallings   (501) staff       (20)       27 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/readme.rst
--rw-r--r--   0 perrystallings   (501) staff       (20)       85 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/docs/usage.rst
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.871855 parrot-api-core-0.1.8/parrot_api/
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.876465 parrot-api-core-0.1.8/parrot_api/core/
--rw-r--r--   0 perrystallings   (501) staff       (20)      277 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/__init__.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.876824 parrot-api-core-0.1.8/parrot_api/core/auth/
--rw-r--r--   0 perrystallings   (501) staff       (20)      321 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/auth/__init__.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     3749 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/auth/jwt.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     6732 2022-06-05 15:18:34.000000 parrot-api-core-0.1.8/parrot_api/core/auth/oauth.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.877245 parrot-api-core-0.1.8/parrot_api/core/auth/providers/
--rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/auth/providers/__init__.py
--rw-r--r--   0 perrystallings   (501) staff       (20)      403 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/auth/providers/auth0.py
--rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/auth/providers/okta.py
--rw-r--r--   0 perrystallings   (501) staff       (20)      750 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/common.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     1521 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/logging.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     1317 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/memos.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     1571 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/server.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     2058 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/parrot_api/core/settings.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.883454 parrot-api-core-0.1.8/parrot_api_core.egg-info/
--rw-r--r--   0 perrystallings   (501) staff       (20)     1962 2022-06-05 16:52:55.000000 parrot-api-core-0.1.8/parrot_api_core.egg-info/PKG-INFO
--rw-r--r--   0 perrystallings   (501) staff       (20)     1947 2022-06-05 16:52:55.000000 parrot-api-core-0.1.8/parrot_api_core.egg-info/SOURCES.txt
--rw-r--r--   0 perrystallings   (501) staff       (20)        1 2022-06-05 16:52:55.000000 parrot-api-core-0.1.8/parrot_api_core.egg-info/dependency_links.txt
--rw-r--r--   0 perrystallings   (501) staff       (20)        1 2022-06-01 13:04:26.000000 parrot-api-core-0.1.8/parrot_api_core.egg-info/not-zip-safe
--rw-r--r--   0 perrystallings   (501) staff       (20)      142 2022-06-05 16:52:55.000000 parrot-api-core-0.1.8/parrot_api_core.egg-info/requires.txt
--rw-r--r--   0 perrystallings   (501) staff       (20)       11 2022-06-05 16:52:55.000000 parrot-api-core-0.1.8/parrot_api_core.egg-info/top_level.txt
--rw-r--r--   0 perrystallings   (501) staff       (20)      387 2022-06-05 16:52:55.889306 parrot-api-core-0.1.8/setup.cfg
--rw-r--r--   0 perrystallings   (501) staff       (20)     1654 2022-06-05 16:52:47.000000 parrot-api-core-0.1.8/setup.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.885076 parrot-api-core-0.1.8/tests/
--rw-r--r--   0 perrystallings   (501) staff       (20)       45 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/__init__.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.885900 parrot-api-core-0.1.8/tests/auth/
--rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/auth/__init__.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     4579 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/auth/conftest.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.886375 parrot-api-core-0.1.8/tests/auth/mocks/
--rw-r--r--   0 perrystallings   (501) staff       (20)      521 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/auth/mocks/public_keys.json
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.886772 parrot-api-core-0.1.8/tests/auth/mocks/schemas/
--rw-r--r--   0 perrystallings   (501) staff       (20)      921 2022-06-05 15:10:06.000000 parrot-api-core-0.1.8/tests/auth/mocks/schemas/async.yaml
--rw-r--r--   0 perrystallings   (501) staff       (20)     1079 2022-06-05 15:12:19.000000 parrot-api-core-0.1.8/tests/auth/mocks/schemas/test.yaml
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.886972 parrot-api-core-0.1.8/tests/auth/mocks/settings/
--rw-r--r--   0 perrystallings   (501) staff       (20)      419 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/auth/mocks/settings/app.json
--rw-r--r--   0 perrystallings   (501) staff       (20)     1735 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/auth/mocks/signing_key.json
--rw-r--r--   0 perrystallings   (501) staff       (20)     3427 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/auth/test_jwt.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     5040 2022-06-05 14:59:14.000000 parrot-api-core-0.1.8/tests/auth/test_oauth.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     1886 2022-06-05 15:14:57.000000 parrot-api-core-0.1.8/tests/auth/test_oauth_async.py
--rw-r--r--   0 perrystallings   (501) staff       (20)      143 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/conftest.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.872975 parrot-api-core-0.1.8/tests/mocks/
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.887103 parrot-api-core-0.1.8/tests/mocks/async_app/
--rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/async_app/__init__.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.887184 parrot-api-core-0.1.8/tests/mocks/async_app/schemas/
--rw-r--r--   0 perrystallings   (501) staff       (20)      338 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/async_app/schemas/example.yaml
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.887395 parrot-api-core-0.1.8/tests/mocks/example_app/
--rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/example_app/__init__.py
--rw-r--r--   0 perrystallings   (501) staff       (20)       36 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/example_app/routes.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.887520 parrot-api-core-0.1.8/tests/mocks/example_app/schemas/
--rw-r--r--   0 perrystallings   (501) staff       (20)      336 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/example_app/schemas/example.yaml
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.887727 parrot-api-core-0.1.8/tests/mocks/example_package/
--rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/example_package/__init__.py
--rw-r--r--   0 perrystallings   (501) staff       (20)       40 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/example_package/example.py
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.887851 parrot-api-core-0.1.8/tests/mocks/example_package/schemas/
--rw-r--r--   0 perrystallings   (501) staff       (20)      494 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/example_package/schemas/test.yaml
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.872822 parrot-api-core-0.1.8/tests/mocks/invalid_settings/
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.887980 parrot-api-core-0.1.8/tests/mocks/invalid_settings/env/
--rw-r--r--   0 perrystallings   (501) staff       (20)       57 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/invalid_settings/env/app.json
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.888106 parrot-api-core-0.1.8/tests/mocks/invalid_settings/secrets/
--rw-r--r--   0 perrystallings   (501) staff       (20)        6 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/invalid_settings/secrets/app.json
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.872916 parrot-api-core-0.1.8/tests/mocks/stringified_settings/
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.888231 parrot-api-core-0.1.8/tests/mocks/stringified_settings/env/
--rw-r--r--   0 perrystallings   (501) staff       (20)      196 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/stringified_settings/env/app.json
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.873124 parrot-api-core-0.1.8/tests/mocks/test_settings/
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.888351 parrot-api-core-0.1.8/tests/mocks/test_settings/env/
--rw-r--r--   0 perrystallings   (501) staff       (20)       57 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/test_settings/env/app.json
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.888473 parrot-api-core-0.1.8/tests/mocks/test_settings/secrets/
--rw-r--r--   0 perrystallings   (501) staff       (20)        2 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/test_settings/secrets/app.json
-drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:52:55.888718 parrot-api-core-0.1.8/tests/mocks/test_settings/test/
--rw-r--r--   0 perrystallings   (501) staff       (20)       27 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/test_settings/test/app.json
--rw-r--r--   0 perrystallings   (501) staff       (20)       64 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/mocks/test_settings/test/celery.json
--rw-r--r--   0 perrystallings   (501) staff       (20)     3929 2022-06-05 16:37:40.000000 parrot-api-core-0.1.8/tests/test_async_requests.py
--rw-r--r--   0 perrystallings   (501) staff       (20)      789 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/test_common.py
--rw-r--r--   0 perrystallings   (501) staff       (20)      180 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/test_logs.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     3826 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/test_requests.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     2075 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/test_server.py
--rw-r--r--   0 perrystallings   (501) staff       (20)     2283 2022-06-01 13:03:01.000000 parrot-api-core-0.1.8/tests/test_settings.py
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.693489 parrot-api-core-0.1.9/
+-rw-r--r--   0 perrystallings   (501) staff       (20)      158 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/AUTHORS.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)     3622 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)       89 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/HISTORY.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1074 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/LICENSE
+-rw-r--r--   0 perrystallings   (501) staff       (20)      262 2022-06-05 16:56:16.000000 parrot-api-core-0.1.9/MANIFEST.in
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1962 2022-06-05 16:56:17.693625 parrot-api-core-0.1.9/PKG-INFO
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1115 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/README.rst
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.690299 parrot-api-core-0.1.9/docs/
+-rw-r--r--   0 perrystallings   (501) staff       (20)      616 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/Makefile
+-rw-r--r--   0 perrystallings   (501) staff       (20)       28 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/authors.rst
+-rwxr-xr-x   0 perrystallings   (501) staff       (20)     4891 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/conf.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)       33 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/contributing.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)       28 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/history.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)      312 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/index.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1202 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/installation.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)      777 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/make.bat
+-rw-r--r--   0 perrystallings   (501) staff       (20)       27 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/readme.rst
+-rw-r--r--   0 perrystallings   (501) staff       (20)       85 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/docs/usage.rst
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.687166 parrot-api-core-0.1.9/parrot_api/
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.691030 parrot-api-core-0.1.9/parrot_api/core/
+-rw-r--r--   0 perrystallings   (501) staff       (20)      277 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/__init__.py
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.691398 parrot-api-core-0.1.9/parrot_api/core/auth/
+-rw-r--r--   0 perrystallings   (501) staff       (20)      321 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/auth/__init__.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     3749 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/auth/jwt.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     6732 2022-06-05 15:18:34.000000 parrot-api-core-0.1.9/parrot_api/core/auth/oauth.py
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.691885 parrot-api-core-0.1.9/parrot_api/core/auth/providers/
+-rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/auth/providers/__init__.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)      403 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/auth/providers/auth0.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)        0 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/auth/providers/okta.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)      750 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/common.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1521 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/logging.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1317 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/memos.py
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.692431 parrot-api-core-0.1.9/parrot_api/core/requests/
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1183 2022-06-05 16:01:08.000000 parrot-api-core-0.1.9/parrot_api/core/requests/__init__.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     3025 2022-06-05 16:52:09.000000 parrot-api-core-0.1.9/parrot_api/core/requests/async_.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     2006 2022-06-05 16:01:08.000000 parrot-api-core-0.1.9/parrot_api/core/requests/sync.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1571 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/server.py
+-rw-r--r--   0 perrystallings   (501) staff       (20)     2058 2022-06-01 13:03:01.000000 parrot-api-core-0.1.9/parrot_api/core/settings.py
+drwxr-xr-x   0 perrystallings   (501) staff       (20)        0 2022-06-05 16:56:17.693381 parrot-api-core-0.1.9/parrot_api_core.egg-info/
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1962 2022-06-05 16:56:17.000000 parrot-api-core-0.1.9/parrot_api_core.egg-info/PKG-INFO
+-rw-r--r--   0 perrystallings   (501) staff       (20)      965 2022-06-05 16:56:17.000000 parrot-api-core-0.1.9/parrot_api_core.egg-info/SOURCES.txt
+-rw-r--r--   0 perrystallings   (501) staff       (20)        1 2022-06-05 16:56:17.000000 parrot-api-core-0.1.9/parrot_api_core.egg-info/dependency_links.txt
+-rw-r--r--   0 perrystallings   (501) staff       (20)        1 2022-06-01 13:04:26.000000 parrot-api-core-0.1.9/parrot_api_core.egg-info/not-zip-safe
+-rw-r--r--   0 perrystallings   (501) staff       (20)      142 2022-06-05 16:56:17.000000 parrot-api-core-0.1.9/parrot_api_core.egg-info/requires.txt
+-rw-r--r--   0 perrystallings   (501) staff       (20)       11 2022-06-05 16:56:17.000000 parrot-api-core-0.1.9/parrot_api_core.egg-info/top_level.txt
+-rw-r--r--   0 perrystallings   (501) staff       (20)      387 2022-06-05 16:56:17.694141 parrot-api-core-0.1.9/setup.cfg
+-rw-r--r--   0 perrystallings   (501) staff       (20)     1682 2022-06-05 16:55:46.000000 parrot-api-core-0.1.9/setup.py
```

### Comparing `parrot-api-core-0.1.8/CONTRIBUTING.rst` & `parrot-api-core-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/LICENSE` & `parrot-api-core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/PKG-INFO` & `parrot-api-core-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parrot-api-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python API Project Framework
 Home-page: https://github.com/perrystallings/parrot_api_core
 Author: Perry Stallings
 Author-email: astal01@gmail.com
 License: MIT license
 Keywords: parrot_api_core
 Platform: UNKNOWN
```

### Comparing `parrot-api-core-0.1.8/README.rst` & `parrot-api-core-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/docs/Makefile` & `parrot-api-core-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/docs/conf.py` & `parrot-api-core-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/docs/installation.rst` & `parrot-api-core-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/docs/make.bat` & `parrot-api-core-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api/core/auth/jwt.py` & `parrot-api-core-0.1.9/parrot_api/core/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api/core/auth/oauth.py` & `parrot-api-core-0.1.9/parrot_api/core/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api/core/common.py` & `parrot-api-core-0.1.9/parrot_api/core/common.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api/core/logging.py` & `parrot-api-core-0.1.9/parrot_api/core/logging.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api/core/memos.py` & `parrot-api-core-0.1.9/parrot_api/core/memos.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api/core/server.py` & `parrot-api-core-0.1.9/parrot_api/core/server.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api/core/settings.py` & `parrot-api-core-0.1.9/parrot_api/core/settings.py`

 * *Files identical despite different names*

### Comparing `parrot-api-core-0.1.8/parrot_api_core.egg-info/PKG-INFO` & `parrot-api-core-0.1.9/parrot_api_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parrot-api-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python API Project Framework
 Home-page: https://github.com/perrystallings/parrot_api_core
 Author: Perry Stallings
 Author-email: astal01@gmail.com
 License: MIT license
 Keywords: parrot_api_core
 Platform: UNKNOWN
```

### Comparing `parrot-api-core-0.1.8/setup.py` & `parrot-api-core-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     description="Python API Project Framework",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='parrot_api_core',
     name='parrot-api-core',
-    packages=['parrot_api.core', 'parrot_api.core.auth', 'parrot_api.core.auth.providers'],
+    packages=['parrot_api.core', 'parrot_api.core.auth', 'parrot_api.core.auth.providers', 'parrot_api.core.requests'],
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/perrystallings/parrot_api_core',
-    version='0.1.8',
+    version='0.1.9',
     zip_safe=False,
     extras_require={
         'async': [
             'aiohttp>=3.6.2',
             'aiohttp_jinja2>=1.2.0',
             'orjson',
             'aioresponses'
```

