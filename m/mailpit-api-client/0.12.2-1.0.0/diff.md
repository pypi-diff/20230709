# Comparing `tmp/mailpit-api-client-0.12.2.tar.gz` & `tmp/mailpit-api-client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailpit-api-client-0.12.2.tar", last modified: Sun Jul  9 14:22:45 2023, max compression
+gzip compressed data, was "mailpit-api-client-1.0.0.tar", last modified: Sun Jul  9 17:03:21 2023, max compression
```

## Comparing `mailpit-api-client-0.12.2.tar` & `mailpit-api-client-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit/client/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/mailpit/testing/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 14:22:45.000000 mailpit-api-client-0.12.2/mailpit_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-09 14:22:25.000000 mailpit-api-client-0.12.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:22:45.496074 mailpit-api-client-0.12.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:03:21.165603 mailpit-api-client-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-07-09 17:03:21.165603 mailpit-api-client-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:03:21.161603 mailpit-api-client-1.0.0/mailpit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/mailpit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:03:21.161603 mailpit-api-client-1.0.0/mailpit/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/mailpit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/mailpit/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/mailpit/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:03:21.165603 mailpit-api-client-1.0.0/mailpit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/mailpit/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/mailpit/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/mailpit/testing/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:03:21.165603 mailpit-api-client-1.0.0/mailpit_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-07-09 17:03:21.000000 mailpit-api-client-1.0.0/mailpit_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-09 17:03:21.000000 mailpit-api-client-1.0.0/mailpit_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:03:21.000000 mailpit-api-client-1.0.0/mailpit_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-09 17:03:21.000000 mailpit-api-client-1.0.0/mailpit_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 17:03:21.000000 mailpit-api-client-1.0.0/mailpit_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-09 17:02:57.000000 mailpit-api-client-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:03:21.165603 mailpit-api-client-1.0.0/setup.cfg
```

### Comparing `mailpit-api-client-0.12.2/LICENSE` & `mailpit-api-client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.12.2/PKG-INFO` & `mailpit-api-client-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.12.2
+Version: 1.0.0
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -198,15 +198,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.2
+    1.0.0
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.2/README.rst` & `mailpit-api-client-1.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.2
+    1.0.0
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.2/mailpit/client/api.py` & `mailpit-api-client-1.0.0/mailpit/client/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """module containing API related"""
-import logging as _logging
+import logging
 from typing import Optional, List, Any
 
-import httpx as _httpx
+import httpx
 
-import mailpit.client.models as _models
+import mailpit.client.models as models
 
-_log = _logging.getLogger("mailpit_client")
+_log = logging.getLogger("mailpit_client")
 
 
 class API:
     """
     class representing the different endpoints of the API
     """
 
@@ -18,45 +18,45 @@
 
     MESSAGES_ENDPOINT = "api/v1/messages"
     MESSAGE_ENDPOINT = "api/v1/message"
 
     def __init__(self, mailpit_url: str, timeout: Optional[int] = None):
         self.mailpit_url = mailpit_url
         self.timeout = timeout
-        self.last_response: Optional[_httpx.Response] = None
+        self.last_response: Optional[httpx.Response] = None
 
-    def get_messages(self, limit: int = 50, start: int = 0) -> _models.Messages:
+    def get_messages(self, limit: int = 50, start: int = 0) -> models.Messages:
         """
         send a GET request in order to retrieve messages
 
         :param limit: limit the returned number of messages
         :param start: start at an offset from the beginning
         :return: the messages returned by mailpit converted into models
         """
 
         # pylint: disable = no-member
 
-        response = _httpx.get(
+        response = httpx.get(
             f"{self.mailpit_url}/{API.MESSAGES_ENDPOINT}",
             params={"limit": limit, "start": start},
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
         _log.debug(response.text)
-        return _models.Messages.from_json(response.text)  # type: ignore
+        return models.Messages.from_json(response.text)  # type: ignore
 
     def delete_messages(self, ids: List[str]):
         """
         send a DELETE request to delete messages
 
         :param ids: the IDs of the messages to delete;
                     NOTE: passing an empty list will delete *all* messages
         """
-        response = _httpx.request(
+        response = httpx.request(
             method="DELETE",
             url=f"{self.mailpit_url}/{API.MESSAGES_ENDPOINT}",
             data={"ids": ids},
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
@@ -66,64 +66,64 @@
         update existing messages;
         for example pass "Read" as key and True as value to mark messages read
 
         :param ids: the IDs of the messages to update
         :param key: the message's attribute to update
         :param value: the value to update the attribute with
         """
-        response = _httpx.put(
+        response = httpx.put(
             f"{self.mailpit_url}/{API.MESSAGES_ENDPOINT}",
             data={"ids": ids, key: value},
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
 
-    def get_message(self, message_id: str) -> _models.Message:
+    def get_message(self, message_id: str) -> models.Message:
         """
         Send a GET request to get a certain Message by its Message-ID
 
         :param message_id: The Message-ID to get the message by
         """
 
         # pylint: disable = no-member
 
-        response = _httpx.get(
+        response = httpx.get(
             f"{self.mailpit_url}/{API.MESSAGE_ENDPOINT}/{message_id}",
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
         _log.debug(response.text)
-        message = _models.Message.from_json(response.text)
+        message = models.Message.from_json(response.text)
         return message
 
     def get_message_attachment(self, message_id: str, part_id: str) -> str:
         """
         Send a GET request to the message endpoint with querying for the part_id
         of an attachment
 
         :param message_id: the Message-ID the attachment belongs to
         :param part_id: the Part-ID of the attachment to receive
         :return the attachment's data
         """
-        response = _httpx.get(
+        response = httpx.get(
             f"{self.mailpit_url}/{API.MESSAGE_ENDPOINT}/{message_id}/part/{part_id}",
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
         return response.text
 
-    def get_message_headers(self, message_id: str) -> _models.Headers:
+    def get_message_headers(self, message_id: str) -> models.Headers:
         """
         Send a GET request to get a message's Headers
 
         :param message_id: The Message-ID to get the headers for
         """
-        response = _httpx.get(
+        response = httpx.get(
             f"{self.mailpit_url}/{API.MESSAGE_ENDPOINT}/{message_id}/headers",
             timeout=self.timeout,
         )
         self.last_response = response
         response.raise_for_status()
-        return _models.Headers.from_json(response.text)  # type: ignore
+        return models.Headers.from_json(response.text)  # type: ignore
```

### Comparing `mailpit-api-client-0.12.2/mailpit/client/models.py` & `mailpit-api-client-1.0.0/mailpit/client/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,73 @@
 """Definitions of model classes, that wrap Mailpit's API data-structures. Defined with 
 :py:mod:`dataclasses` and :py:mod:`dataclasses_json`, in order to use them as json over 
 the API and be used as objects in the Python domain."""
-import dataclasses as _dc
-import datetime as _dt
-import decimal as _d
-import email.utils as _email
+import dataclasses
+import datetime
+import decimal
+import email.utils as email
 import logging
-import re as _re
+import re
 from typing import Optional, Iterable
 
-import dataclasses_json as _dj
+import dataclasses_json
 import marshmallow.fields
 
 
 _log = logging.getLogger("mailpit_client")
 
 
-@_dj.dataclass_json
-@_dc.dataclass(init=True)
+@dataclasses_json.dataclass_json
+@dataclasses.dataclass(init=True)
 class Contact:
     """Represents a mail contact splitting 'Test User <test@example.com> into
     its name and address parts"""
 
     # pylint: disable=too-few-public-methods
 
-    name: str = _dc.field(init=True, metadata=_dj.config(field_name="Name"))
+    name: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Name")
+    )
     """Contact's Name"""
-    address: str = _dc.field(init=True, metadata=_dj.config(field_name="Address"))
+    address: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Address")
+    )
     """Contact's E-Mail address"""
 
     def __lt__(self, other):
         return f"{other.name} {other.address}".__lt__(f"{self.name} {self.address}")
 
     def __hash__(self):
         return f"{self.name} {self.address}".__hash__()
 
 
-@_dc.dataclass(init=True)
-class Attachment(_dj.DataClassJsonMixin):
+@dataclasses.dataclass(init=True)
+class Attachment(dataclasses_json.DataClassJsonMixin):
     """Represents an attachment of a :py:class:`Message`"""
 
     # pylint: disable=too-few-public-methods
 
-    part_id: str = _dc.field(init=True, metadata=_dj.config(field_name="PartID"))
+    part_id: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="PartID")
+    )
     """Attachment's part ID"""
-    file_name: str = _dc.field(init=True, metadata=_dj.config(field_name="FileName"))
+    file_name: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="FileName")
+    )
     """Attachment's file name"""
-    content_type: str = _dc.field(
-        init=True, metadata=_dj.config(field_name="ContentType")
+    content_type: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="ContentType")
     )
     """Attachment's MIME content-type"""
-    content_id: str = _dc.field(init=True, metadata=_dj.config(field_name="ContentID"))
-    size: int = _dc.field(init=True, metadata=_dj.config(field_name="Size"))
+    content_id: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="ContentID")
+    )
+    size: int = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Size")
+    )
     """Attachment's size in bytes"""
 
     def __lt__(self, other: "Attachment"):
         return (
             f"{other.part_id} {other.file_name} {other.content_type} "
             f"{other.content_id} {other.size}".__lt__(
                 f"{self.part_id} {self.file_name} {self.content_type} "
@@ -66,67 +78,83 @@
     def __hash__(self):
         return (
             f"{self.part_id} {self.file_name} {self.content_type} "
             f"{self.content_id} {self.size}"
         ).__hash__()
 
 
-@_dc.dataclass(init=True)
-class Message(_dj.DataClassJsonMixin):
+@dataclasses.dataclass(init=True)
+class Message(dataclasses_json.DataClassJsonMixin):
     """Represents a message returned by the message-endpoint"""
 
     # pylint: disable=too-many-instance-attributes
     # pylint: disable=too-few-public-methods
     # pylint: disable=invalid-name
 
-    id: str = _dc.field(init=True, metadata=_dj.config(field_name="ID"))
+    id: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="ID")
+    )
     """Message's database ID, of Mailpit's message-database"""
-    message_id: str = _dc.field(init=True, metadata=_dj.config(field_name="MessageID"))
+    message_id: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="MessageID")
+    )
     """Message's RFC-5322 message-id"""
-    read: bool = _dc.field(init=True, metadata=_dj.config(field_name="Read"))
+    read: bool = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Read")
+    )
     """Always true (message marked read on open)"""
-    from_: Optional[Contact] = _dc.field(
-        init=True, metadata=_dj.config(field_name="From")
+    from_: Optional[Contact] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="From")
     )
     """The :py:class`Contact`: the message is from"""
-    to: list[Contact] = _dc.field(init=True, metadata=_dj.config(field_name="To"))
+    to: list[Contact] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="To")
+    )
     """Message's To-Header, the list of :Contact: the message is addressed to"""
-    cc: Optional[list[Contact]] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Cc")
+    cc: Optional[list[Contact]] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Cc")
     )
     """Message's CC-Header, the list of :Contact: that the message is coal-copied to"""
-    bcc: Optional[list[Contact]] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Bcc")
+    bcc: Optional[list[Contact]] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Bcc")
     )
     """Message's BCC-Header, the list of :Contact:, that the message is blindly 
     coal-copied to"""
-    subject: str = _dc.field(init=True, metadata=_dj.config(field_name="Subject"))
+    subject: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Subject")
+    )
     """Message's subject"""
-    date: _dt.date = _dc.field(
+    date: datetime.date = dataclasses.field(
         init=True,
-        metadata=_dj.config(
+        metadata=dataclasses_json.config(
             field_name="Date",
-            encoder=_dt.datetime.isoformat,
-            decoder=_dt.datetime.fromisoformat,
+            encoder=datetime.datetime.isoformat,
+            decoder=datetime.datetime.fromisoformat,
             mm_field=marshmallow.fields.DateTime("iso"),
         ),
     )
     """Parsed email local date & time from headers"""
-    text: Optional[str] = _dc.field(init=True, metadata=_dj.config(field_name="Text"))
+    text: Optional[str] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Text")
+    )
     """Plain text MIME part of the email"""
-    html: Optional[str] = _dc.field(init=True, metadata=_dj.config(field_name="HTML"))
+    html: Optional[str] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="HTML")
+    )
     """HTML MIME part (if exists)"""
-    size: int = _dc.field(init=True, metadata=_dj.config(field_name="Size"))
+    size: int = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Size")
+    )
     """Total size of raw email in bytes"""
-    inline: list[Attachment] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Inline")
+    inline: list[Attachment] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Inline")
     )
     """Inline Attachments"""
-    attachments: list[Attachment] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Attachments")
+    attachments: list[Attachment] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Attachments")
     )
     """Attachments"""
 
     def __eq__(self, other):
         """check if a message is equal to another message. Fields not included are
         Mailpit's Database-ID because it might not be known and the size in bytes,
         because it might be differently depending on the way messages are saved
@@ -191,130 +219,146 @@
         if set(sorted(other.attachments)).difference(sorted(self.attachments)) or set(
             sorted(self.attachments)
         ).difference(sorted(other.attachments)):
             return False
         return True
 
 
-def _datelist_encoder(encodes: Iterable[_dt.datetime]) -> list[str]:
-    return list(map(lambda encode: _email.format_datetime(encode), encodes))
+def datelist_encoder(encodes: Iterable[datetime.datetime]) -> list[str]:
+    return list(map(lambda encode: email.format_datetime(encode), encodes))
 
 
-def _datelist_decoder(decodes: Iterable[str]) -> list[_dt.datetime]:
-    return list(map(lambda decode: _email.parsedate_to_datetime(decode), decodes))
+def datelist_decoder(decodes: Iterable[str]) -> list[datetime.datetime]:
+    return list(map(lambda decode: email.parsedate_to_datetime(decode), decodes))
 
 
-@_dj.dataclass_json(undefined=_dj.Undefined.INCLUDE)
-@_dc.dataclass(init=True)
+@dataclasses_json.dataclass_json(undefined=dataclasses_json.Undefined.INCLUDE)
+@dataclasses.dataclass(init=True)
 class Headers:
-    content_type: list[str] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Content-Type")
+    content_type: list[str] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Content-Type")
     )
-    date: list[_dt.date] = _dc.field(
+    date: list[datetime.date] = dataclasses.field(
         init=True,
-        metadata=_dj.config(
+        metadata=dataclasses_json.config(
             field_name="Date",
-            encoder=_datelist_encoder,
-            decoder=_datelist_decoder,
+            encoder=datelist_encoder,
+            decoder=datelist_decoder,
             mm_field=marshmallow.fields.List(marshmallow.fields.DateTime("iso")),
         ),
     )
-    delivered_to: list[str] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Delivered-To")
+    delivered_to: list[str] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Delivered-To")
     )
-    from_: list[str] = _dc.field(init=True, metadata=_dj.config(field_name="From"))
-    message_id: list[str] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Message-Id")
+    from_: list[str] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="From")
     )
-    additional: _dj.CatchAll = _dc.field(init=True)
+    message_id: list[str] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Message-Id")
+    )
+    additional: dataclasses_json.CatchAll = dataclasses.field(init=True)
 
 
 def millis_to_3_digit(isoformat: str) -> str:
     """replaces milliseconds with
     three-digits long value using zero padding before"""
-    millis = _re.search(r"\.\d{0,3}", isoformat)
+    millis = re.search(r"\.\d{0,3}", isoformat)
     if not millis:
-        seconds = _re.search(r":\d+(:\d+)", isoformat)
+        seconds = re.search(r":\d+(:\d+)", isoformat)
         _log.debug(f"seconds: {seconds}")
         if seconds is None:
             raise ValueError("seconds may not be None")
         return isoformat.replace(seconds.group(0), f"{seconds.group(0)}.000")
-    _log.debug(f"millis: {millis.group(0)}, {_d.Decimal(millis.group(0)):.03f}")
+    _log.debug(f"millis: {millis.group(0)}, {decimal.Decimal(millis.group(0)):.03f}")
     return isoformat.replace(
-        f"{millis.group(0)}", f".{int(_d.Decimal(millis.group(0)) * 1000):03}"
+        f"{millis.group(0)}", f".{int(decimal.Decimal(millis.group(0)) * 1000):03}"
     )
 
 
 def zulu_to_utc_shift(isoformat: str) -> str:
     """replaces 'Z' with '+00:00' for UTC"""
     return isoformat.replace("Z", "+00:00")
 
 
-def datetime_decoder(isoformat: str) -> _dt.datetime:
+def datetime_decoder(isoformat: str) -> datetime.datetime:
     """replaces golang isoformat with Python parsable isoformat
     and decodes it to `datetime.datetime`"""
     _log.debug(f"old isdoformat: {isoformat}")
 
     result = zulu_to_utc_shift(millis_to_3_digit(isoformat))
     _log.debug(f"new isoformat: {result}")
-    return _dt.datetime.fromisoformat(result)
+    return datetime.datetime.fromisoformat(result)
 
 
-@_dc.dataclass(init=True)
-class MessageSummary(_dj.DataClassJsonMixin):
+@dataclasses.dataclass(init=True)
+class MessageSummary(dataclasses_json.DataClassJsonMixin):
     """class representing a single message that has been returned by the messages
     endpoint"""
 
     # pylint: disable=too-many-instance-attributes
     # pylint: disable=too-few-public-methods
     # pylint: disable=invalid-name
 
-    id: str = _dc.field(init=True, metadata=_dj.config(field_name="ID"))
-    message_id: str = _dc.field(init=True, metadata=_dj.config(field_name="MessageID"))
-    read: bool = _dc.field(init=True, metadata=_dj.config(field_name="Read"))
+    id: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="ID")
+    )
+    message_id: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="MessageID")
+    )
+    read: bool = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Read")
+    )
     """always true (message marked read on open)"""
-    from_: Optional[Contact] = _dc.field(
-        init=True, metadata=_dj.config(field_name="From")
+    from_: Optional[Contact] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="From")
+    )
+    to: list[Contact] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="To")
+    )
+    cc: Optional[list[Contact]] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Cc")
     )
-    to: list[Contact] = _dc.field(init=True, metadata=_dj.config(field_name="To"))
-    cc: Optional[list[Contact]] = _dc.field(
-        init=True, metadata=_dj.config(field_name="Cc")
+    bcc: list[Contact] = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Bcc")
+    )
+    subject: str = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Subject")
     )
-    bcc: list[Contact] = _dc.field(init=True, metadata=_dj.config(field_name="Bcc"))
-    subject: str = _dc.field(init=True, metadata=_dj.config(field_name="Subject"))
     """Message subject"""
-    created: _dt.date = _dc.field(
+    created: datetime.date = dataclasses.field(
         init=True,
-        metadata=_dj.config(
+        metadata=dataclasses_json.config(
             field_name="Created",
-            encoder=_dt.datetime.isoformat,
+            encoder=datetime.datetime.isoformat,
             decoder=datetime_decoder,
             mm_field=marshmallow.fields.DateTime("iso"),
         ),
     )
     """Parsed email local date & time from headers"""
-    size: int = _dc.field(init=True, metadata=_dj.config(field_name="Size"))
+    size: int = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Size")
+    )
     """Total size of raw email"""
-    attachments: int = _dc.field(
-        init=True, metadata=_dj.config(field_name="Attachments")
+    attachments: int = dataclasses.field(
+        init=True, metadata=dataclasses_json.config(field_name="Attachments")
     )
 
 
-@_dc.dataclass(init=True)
-class Messages(_dj.DataClassJsonMixin):
+@dataclasses.dataclass(init=True)
+class Messages(dataclasses_json.DataClassJsonMixin):
     # pylint: disable=too-few-public-methods
     """class representing the returns of the messages endpoint"""
 
-    total: int = _dc.field(init=True)
+    total: int = dataclasses.field(init=True)
     """Total messages in mailbox"""
-    unread: int = _dc.field(init=True)
+    unread: int = dataclasses.field(init=True)
     """Total unread messages in mailbox"""
-    count: int = _dc.field(init=True)
+    count: int = dataclasses.field(init=True)
     """Number of messages returned in request"""
-    start: int = _dc.field(init=True)
+    start: int = dataclasses.field(init=True)
     """The offset (default=0) for pagination"""
     messages: list[MessageSummary]
 
     def __post_init__(self):
         if self.total < 0:
             raise ValueError("field 'total' may not be negative")
         if self.unread < 0:
```

### Comparing `mailpit-api-client-0.12.2/mailpit/testing/pytest.py` & `mailpit-api-client-1.0.0/mailpit/testing/pytest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Module providing helpers for :py:mod:`unittest` kind of testing against the
 Mailpit-API"""
 
 try:
-    import pytest as _pytest
+    import pytest
 except ImportError:
-    _pytest = None
+    pytest = None
 
-if _pytest:
+if pytest:
     import pathlib as _pathlib
     import os as _os
     import mailpit.client.api as _api
 
-    @_pytest.fixture(scope="session")
+    @pytest.fixture(scope="session")
     def mailpit_api(request):
         """:py:func:`pytest.fixture` creating a connection to the mailpit API.
         This fixture has got a default of ``http://localhost:8025`` but it is possible
         to be called `parametrized <https://docs.pytest.org/en/stable/example/
         parametrize.html #indirect-parametrization>`_ with the parameter
         ``indirect`` set to ``True``, in order to pass the url for which an
         :py:class:`mailpit.client.api.API` instance is created and yielded.
```

### Comparing `mailpit-api-client-0.12.2/mailpit/testing/unittest.py` & `mailpit-api-client-1.0.0/mailpit/testing/unittest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 """Provides helpers for :py:mod:`unittest` kind of testing against the
 Mailpit-API"""
 from typing import Optional
-import unittest as _unittest
+import unittest
 
-import mailpit.client.models as _models
-import mailpit.client.api as _api
+import mailpit.client.models as models
+import mailpit.client.api as api
 
 
-class EMailTestCase(_unittest.TestCase):
+class EMailTestCase(unittest.TestCase):
     """:py:class:`unittest.TestCase`-derived class with added test-helper methods and
     attributes, in order to test against the Mailpit-API. Simply derive from this class,
     as you would from :py:class:`unittest.TestCase` and write your tests as you are used
     to.
 
 
     e.g.::
 
         class ExampleTestCase(EMailTestCase):
 
-            def test_api_object(self):
+            def testapi_object(self):
                 messages: mailpit.client.models.Messages = self.api.get_messages()
                 self.assertEqual(0, len(messages.messages))
     """
 
     api_url: str = "http://localhost:8025"
     """URL pointing to the Mailpit-API to test, if you need to use another url,
     override this attribute in your derived class"""
-    api: Optional[_api.API] = None
+    mailpit_api: Optional[api.API] = None
     """API object created on class setup for testing against Mailpit's API, access this
     object if you need to communicate directly with the API in your tests. """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.addTypeEqualityFunc(_models.Message, self.assertMessageEqual)
+        self.addTypeEqualityFunc(models.Message, self.assertMessageEqual)
 
     @classmethod
     def setUpClass(cls) -> None:
         """Creates the class attribute object for the API, on creation of this class and
         classes derived from it. Remember to call :py:func:`super().setUpClass()` while
         subclassing and overriding this method"""
         super().setUpClass()
-        cls.api = _api.API(cls.api_url)
+        cls.mailpit_api = api.API(cls.api_url)
 
     def assertMessageEqual(
-        self, first: _models.Message, second: _models.Message, msg: Optional[str] = None
+        self, first: models.Message, second: models.Message, msg: Optional[str] = None
     ):
         """Fail if two instances of :py:class:`Message` are not equal as determined
         by the '==' operator
 
         e.g.::
 
             import mailpit.client.models
@@ -66,18 +66,18 @@
 
     def assertMessageReceived(
         self,
         message_id: str,
         msg: Optional[str] = None,
     ):
         """Fail if the passed message has not been sent to Mailpit"""
-        if self.api is None:
+        if self.mailpit_api is None:
             raise self.failureException(
                 self._formatMessage(msg, "self.api may not be None")
             )
-        messages: _models.Messages = self.api.get_messages()
+        messages: models.Messages = self.mailpit_api.get_messages()
         if message_id not in [message.message_id for message in messages.messages]:
             raise self.failureException(
                 self._formatMessage(
                     msg, "Message not found, so it has not been received"
                 )
             )
```

### Comparing `mailpit-api-client-0.12.2/mailpit_api_client.egg-info/PKG-INFO` & `mailpit-api-client-1.0.0/mailpit_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.12.2
+Version: 1.0.0
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -198,15 +198,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.12.2
+    1.0.0
 
 Go to the `documentation <https://corvan.github.io/mailpit-api-client/>`_
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
```

### Comparing `mailpit-api-client-0.12.2/pyproject.toml` & `mailpit-api-client-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailpit-api-client"
-version = "0.12.2"
+version = "1.0.0"
 description = "A Mailpit API Client"
 authors = [{name = "Lars Liedtke", email = "lars@familie-liedtke.net"}]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Framework :: Pytest",
@@ -51,15 +51,15 @@
 
 [project.urls]
 Repository = "https://github.com/Corvan/mailpit-api-client"
 Documentation = "https://corvan.github.io/mailpit-api-client/"
 
 [tool.poetry]
 name = "mailpit-api-client"
-version = "0.12.1"
+version = "1.0.0"
 description = ""
 authors = ["Lars Liedtke <lars@familie-liedtke.net>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dataclasses_json = "*"
 httpx = "*"
```

