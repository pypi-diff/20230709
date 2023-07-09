# Comparing `tmp/mailpit-api-client-0.12.0.tar.gz` & `tmp/mailpit-api-client-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailpit-api-client-0.12.0.tar", last modified: Sat Jul  8 17:00:49 2023, max compression
+gzip compressed data, was "mailpit-api-client-0.12.1.tar", last modified: Sun Jul  9 12:49:58 2023, max compression
```

## Comparing `mailpit-api-client-0.12.0.tar` & `mailpit-api-client-0.12.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.780160 mailpit-api-client-0.12.0/mailpit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.780160 mailpit-api-client-0.12.0/mailpit/client/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.780160 mailpit-api-client-0.12.0/mailpit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/mailpit/testing/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 17:00:49.000000 mailpit-api-client-0.12.0/mailpit_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-08 17:00:37.000000 mailpit-api-client-0.12.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:00:49.784160 mailpit-api-client-0.12.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.318992 mailpit-api-client-0.12.1/mailpit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.318992 mailpit-api-client-0.12.1/mailpit/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.318992 mailpit-api-client-0.12.1/mailpit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/mailpit/testing/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 12:49:58.000000 mailpit-api-client-0.12.1/mailpit_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-09 12:49:31.000000 mailpit-api-client-0.12.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 12:49:58.322992 mailpit-api-client-0.12.1/setup.cfg
```

### Comparing `mailpit-api-client-0.12.0/LICENSE` & `mailpit-api-client-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.0/PKG-INFO` & `mailpit-api-client-0.12.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.12.0
+Version: 0.12.1
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -165,15 +165,15 @@
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
-Project-URL: repository, https://github.com/Corvan/mailpit-api-client
+Project-URL: Repository, https://github.com/Corvan/mailpit-api-client
 Project-URL: Documentation, https://corvan.github.io/mailpit-api-client/
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -198,15 +198,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.0
+    0.12.1
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.0/README.rst` & `mailpit-api-client-0.12.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.0
+    0.12.1
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.0/mailpit/client/api.py` & `mailpit-api-client-0.12.1/mailpit/client/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import mailpit.client.models as _models
 
 _log = _logging.getLogger("mailpit_client")
 
 
 class API:
     """
-    class representing the message-endpoint of the API
+    class representing the different endpoints of the API
     """
 
     # pylint: disable=too-few-public-methods
 
     MESSAGES_ENDPOINT = "api/v1/messages"
     MESSAGE_ENDPOINT = "api/v1/message"
 
@@ -76,51 +76,53 @@
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
 
     def get_message(self, message_id: str) -> _models.Message:
         """
+        Send a GET request to get a certain Message by its Message-ID
 
-
-        :param message_id:
+        :param message_id: The Message-ID to get the message by
         """
 
         # pylint: disable = no-member
 
         response = _httpx.get(
             f"{self.mailpit_url}/{API.MESSAGE_ENDPOINT}/{message_id}",
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
         _log.debug(response.text)
         message = _models.Message.from_json(response.text)
         return message
 
-    def get_message_attachment(self, message_id: str, part_id: str):
+    def get_message_attachment(self, message_id: str, part_id: str) -> str:
         """
+        Send a GET request to the message endpoint with querying for the part_id
+        of an attachment
 
-
-        :param message_id:
-        :param part_id:
+        :param message_id: the Message-ID the attachment belongs to
+        :param part_id: the Part-ID of the attachment to receive
+        :return the attachment's data
         """
         response = _httpx.get(
             f"{self.mailpit_url}/{API.MESSAGE_ENDPOINT}/{message_id}/part/{part_id}",
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
         return response.text
 
-    def get_message_headers(self, message_id: str):
+    def get_message_headers(self, message_id: str) -> _models.Headers:
         """
+        Send a GET request to get a message's Headers
 
-
-        :param message_id:
+        :param message_id: The Message-ID to get the headers for
         """
         response = _httpx.get(
             f"{self.mailpit_url}/{API.MESSAGE_ENDPOINT}/{message_id}/headers",
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
```

### Comparing `mailpit-api-client-0.12.0/mailpit/client/models.py` & `mailpit-api-client-0.12.1/mailpit/client/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,15 +229,19 @@
 
 
 def millis_to_3_digit(isoformat: str) -> str:
     """replaces milliseconds with
     three-digits long value using zero padding before"""
     millis = _re.search(r"\.\d{0,3}", isoformat)
     if not millis:
-        raise ValueError("No milliseconds provided in isoformat string")
+        seconds = _re.search(r":\d+(:\d+)", isoformat)
+        _log.debug(f"seconds: {seconds}")
+        if seconds is None:
+            raise ValueError("seconds may not be None")
+        return isoformat.replace(seconds.group(0), f"{seconds.group(0)}.000")
     _log.debug(f"millis: {millis.group(0)}, {_d.Decimal(millis.group(0)):.03f}")
     return isoformat.replace(
         f"{millis.group(0)}", f".{int(_d.Decimal(millis.group(0)) * 1000):03}"
     )
 
 
 def zulu_to_utc_shift(isoformat: str) -> str:
```

### Comparing `mailpit-api-client-0.12.0/mailpit/testing/pytest.py` & `mailpit-api-client-0.12.1/mailpit/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.0/mailpit/testing/unittest.py` & `mailpit-api-client-0.12.1/mailpit/testing/unittest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.0/mailpit_api_client.egg-info/PKG-INFO` & `mailpit-api-client-0.12.1/mailpit_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.12.0
+Version: 0.12.1
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -165,15 +165,15 @@
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
-Project-URL: repository, https://github.com/Corvan/mailpit-api-client
+Project-URL: Repository, https://github.com/Corvan/mailpit-api-client
 Project-URL: Documentation, https://corvan.github.io/mailpit-api-client/
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -198,15 +198,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.0
+    0.12.1
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.0/pyproject.toml` & `mailpit-api-client-0.12.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailpit-api-client"
-version = "0.12.0"
+version = "0.12.1"
 description = "A Mailpit API Client"
 authors = [{name = "Lars Liedtke", email = "lars@familie-liedtke.net"}]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Framework :: Pytest",
@@ -35,31 +35,31 @@
     "Sphinx",
 ]
 test = [
     "black",
     "mypy>=1.1.1",
     "pylint",
     "respx",
-    "pytest>=7",
 ]
 pytest = [
+    "mailpit-api-client[test]",
     "pytest>=7",
 ]
 build = [
     "build",
     "twine",
 ]
 
 [project.urls]
-repository = "https://github.com/Corvan/mailpit-api-client"
+Repository = "https://github.com/Corvan/mailpit-api-client"
 Documentation = "https://corvan.github.io/mailpit-api-client/"
 
 [tool.poetry]
 name = "mailpit-api-client"
-version = "0.12.0"
+version = "0.12.1"
 description = ""
 authors = ["Lars Liedtke <lars@familie-liedtke.net>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dataclasses_json = "*"
 httpx = "*"
@@ -73,17 +73,20 @@
 sphinx = "*"
 
 [tool.poetry.group.test.dependencies]
 black = "*"
 mypy = "^1.4.1"
 pylint = "*"
 respx = "*"
-pytest = "^7"
 
 [tool.poetry.group.pytest.dependencies]
+black = "*"
+mypy = "^1.4.1"
+pylint = "*"
+respx = "*"
 pytest = "^7"
 
 [tool.poetry.group.build.dependencies]
 build = "*"
 twine = "*"
 
 [tool.invoke.test]
```

