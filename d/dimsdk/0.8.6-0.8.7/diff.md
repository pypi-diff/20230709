# Comparing `tmp/dimsdk-0.8.6.tar.gz` & `tmp/dimsdk-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimsdk-0.8.6.tar", last modified: Wed Jul  5 17:43:50 2023, max compression
+gzip compressed data, was "dist/dimsdk-0.8.7.tar", last modified: Sun Jul  9 09:57:48 2023, max compression
```

## Comparing `dimsdk-0.8.6.tar` & `dimsdk-0.8.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-07-05 17:43:50.000000 dimsdk-0.8.6/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      556 2022-12-11 05:05:26.000000 dimsdk-0.8.6/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk/
--rw-r--r--   0 moky       (501) staff       (20)     6206 2023-07-05 16:09:04.000000 dimsdk-0.8.6/dimsdk/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3727 2023-01-31 05:24:56.000000 dimsdk-0.8.6/dimsdk/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2669 2023-07-05 15:27:52.000000 dimsdk-0.8.6/dimsdk/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5610 2023-07-05 13:32:09.000000 dimsdk-0.8.6/dimsdk/cpu/base.py
--rw-r--r--   0 moky       (501) staff       (20)     7267 2023-07-05 15:12:46.000000 dimsdk-0.8.6/dimsdk/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     3404 2023-07-05 13:20:00.000000 dimsdk-0.8.6/dimsdk/cpu/contents.py
--rw-r--r--   0 moky       (501) staff       (20)     3808 2023-07-05 15:19:44.000000 dimsdk-0.8.6/dimsdk/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     4733 2023-07-05 15:10:37.000000 dimsdk-0.8.6/dimsdk/cpu/customized.py
--rw-r--r--   0 moky       (501) staff       (20)     4607 2023-07-05 15:15:25.000000 dimsdk-0.8.6/dimsdk/cpu/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     2415 2023-01-31 05:24:56.000000 dimsdk-0.8.6/dimsdk/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     8136 2023-07-05 15:40:56.000000 dimsdk-0.8.6/dimsdk/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8714 2023-07-05 11:09:04.000000 dimsdk-0.8.6/dimsdk/factories.py
--rw-r--r--   0 moky       (501) staff       (20)     6741 2023-07-05 15:44:11.000000 dimsdk-0.8.6/dimsdk/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     2263 2022-12-12 09:59:21.000000 dimsdk-0.8.6/dimsdk/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1965 2023-06-01 18:23:20.000000 dimsdk-0.8.6/dimsdk/mkm/robot.py
--rw-r--r--   0 moky       (501) staff       (20)     4672 2022-12-11 05:05:26.000000 dimsdk-0.8.6/dimsdk/mkm/roles.py
--rw-r--r--   0 moky       (501) staff       (20)     6579 2023-06-01 18:25:38.000000 dimsdk-0.8.6/dimsdk/mkm/station.py
--rw-r--r--   0 moky       (501) staff       (20)    10085 2023-07-05 15:52:28.000000 dimsdk-0.8.6/dimsdk/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     7188 2023-07-05 15:52:55.000000 dimsdk-0.8.6/dimsdk/processor.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1047 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      557 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       37 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        7 2023-07-05 17:43:50.000000 dimsdk-0.8.6/dimsdk.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-05 17:43:50.000000 dimsdk-0.8.6/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1256 2023-07-05 11:05:36.000000 dimsdk-0.8.6/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 09:57:48.000000 dimsdk-0.8.7/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2023-07-09 09:57:48.000000 dimsdk-0.8.7/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      556 2022-12-11 05:05:26.000000 dimsdk-0.8.7/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk/
+-rw-r--r--   0 moky       (501) staff       (20)     6209 2023-07-09 08:43:58.000000 dimsdk-0.8.7/dimsdk/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3727 2023-01-31 05:24:56.000000 dimsdk-0.8.7/dimsdk/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2669 2023-07-05 15:27:52.000000 dimsdk-0.8.7/dimsdk/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5689 2023-07-09 08:48:59.000000 dimsdk-0.8.7/dimsdk/cpu/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     7493 2023-07-09 08:51:56.000000 dimsdk-0.8.7/dimsdk/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     3404 2023-07-05 13:20:00.000000 dimsdk-0.8.7/dimsdk/cpu/contents.py
+-rw-r--r--   0 moky       (501) staff       (20)     3808 2023-07-05 15:19:44.000000 dimsdk-0.8.7/dimsdk/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     4757 2023-07-09 08:49:17.000000 dimsdk-0.8.7/dimsdk/cpu/customized.py
+-rw-r--r--   0 moky       (501) staff       (20)     4607 2023-07-05 15:15:25.000000 dimsdk-0.8.7/dimsdk/cpu/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     2415 2023-01-31 05:24:56.000000 dimsdk-0.8.7/dimsdk/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     8136 2023-07-05 15:40:56.000000 dimsdk-0.8.7/dimsdk/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8714 2023-07-05 11:09:04.000000 dimsdk-0.8.7/dimsdk/factories.py
+-rw-r--r--   0 moky       (501) staff       (20)     6741 2023-07-05 15:44:11.000000 dimsdk-0.8.7/dimsdk/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     2263 2022-12-12 09:59:21.000000 dimsdk-0.8.7/dimsdk/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1965 2023-06-01 18:23:20.000000 dimsdk-0.8.7/dimsdk/mkm/robot.py
+-rw-r--r--   0 moky       (501) staff       (20)     4672 2022-12-11 05:05:26.000000 dimsdk-0.8.7/dimsdk/mkm/roles.py
+-rw-r--r--   0 moky       (501) staff       (20)     6579 2023-06-01 18:25:38.000000 dimsdk-0.8.7/dimsdk/mkm/station.py
+-rw-r--r--   0 moky       (501) staff       (20)    10085 2023-07-05 15:52:28.000000 dimsdk-0.8.7/dimsdk/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7188 2023-07-05 15:52:55.000000 dimsdk-0.8.7/dimsdk/processor.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1047 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      557 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       37 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        7 2023-07-09 09:57:48.000000 dimsdk-0.8.7/dimsdk.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-09 09:57:48.000000 dimsdk-0.8.7/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1256 2023-07-09 08:43:58.000000 dimsdk-0.8.7/setup.py
```

### Comparing `dimsdk-0.8.6/PKG-INFO` & `dimsdk-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 0.8.6
+Version: 0.8.7
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-0.8.6/README.md` & `dimsdk-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/__init__.py` & `dimsdk-0.8.7/dimsdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     'BaseTextContent', 'SecretContent', 'ListContent',
     'BaseMoneyContent', 'TransferMoneyContent',
     'BaseFileContent', 'ImageFileContent', 'AudioFileContent', 'VideoFileContent',
     'WebPageContent', 'AppCustomizedContent',
 
     'BaseCommand',
     'BaseMetaCommand', 'BaseDocumentCommand',
-    'BaseReceiptCommand', 'TextReceiptCommand',
+    'BaseReceiptCommand',  # 'TextReceiptCommand',
 
     'BaseHistoryCommand', 'BaseGroupCommand',
     'InviteGroupCommand', 'ExpelGroupCommand', 'JoinGroupCommand',
     'QuitGroupCommand', 'QueryGroupCommand', 'ResetGroupCommand',
 
     # 'MessageEnvelope', 'MessageEnvelopeFactory',
     # 'BaseMessage',
```

### Comparing `dimsdk-0.8.6/dimsdk/ans.py` & `dimsdk-0.8.7/dimsdk/ans.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/cpu/__init__.py` & `dimsdk-0.8.7/dimsdk/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/cpu/base.py` & `dimsdk-0.8.7/dimsdk/cpu/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import weakref
 from abc import ABC, abstractmethod
 from typing import Optional, Union, List, Dict
 
 from dimp import ID
 from dimp import ReliableMessage
 from dimp import ContentType, Content, Command
-from dimp import TextReceiptCommand
+from dimp import ReceiptCommand
 
 
 class ContentProcessor(ABC):
     """
         CPU: Content Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     """
@@ -151,24 +151,25 @@
         Content Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~
     """
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         # override to process this content
-        return self._respond_text(text='Content not support.', group=content.group, extra={
+        return self._respond_receipt(text='Content not support.', msg=msg, group=content.group, extra={
             'template': 'Content (type: ${type}) not support yet!',
             'replacements': {
                 'type': content.type,
             }
         })
 
     # noinspection PyMethodMayBeStatic
-    def _respond_text(self, text: str, group: Optional[ID] = None, extra: Dict = None) -> List[Content]:
-        res = TextReceiptCommand.from_text(text=text)
+    def _respond_receipt(self, text: str, msg: ReliableMessage = None,
+                         group: Optional[ID] = None, extra: Dict = None) -> List[Content]:
+        res = ReceiptCommand.create(text=text, msg=msg)
         if group is not None:
             res.group = group
         if extra is not None:
             for key in extra:
                 res[key] = extra[key]
         return [res]
 
@@ -178,13 +179,13 @@
         Command Processing Unit
         ~~~~~~~~~~~~~~~~~~~~~~~
     """
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, Command), 'command error: %s' % content
-        return self._respond_text(text='Command not support.', group=content.group, extra={
+        return self._respond_receipt(text='Command not support.', msg=msg, group=content.group, extra={
             'template': 'Command (name: ${command}) not support yet!',
             'replacements': {
                 'command': content.cmd,
             }
         })
```

### Comparing `dimsdk-0.8.6/dimsdk/cpu/commands.py` & `dimsdk-0.8.7/dimsdk/cpu/commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,44 +56,44 @@
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, MetaCommand), 'meta command error: %s' % content
         identifier = content.identifier
         meta = content.meta
         if meta is None:
             # query meta for ID
-            return self._get_meta(identifier=identifier)
+            return self._get_meta(identifier=identifier, msg=msg)
         else:
             # received a meta for ID
-            return self._put_meta(identifier=identifier, meta=meta)
+            return self._put_meta(identifier=identifier, meta=meta, msg=msg)
 
-    def _get_meta(self, identifier: ID) -> List[Content]:
+    def _get_meta(self, identifier: ID, msg: ReliableMessage) -> List[Content]:
         facebook = get_facebook(cpu=self)
         meta = facebook.meta(identifier=identifier)
         if meta is None:
-            return self._respond_text(text='Meta not found.', extra={
+            return self._respond_receipt(text='Meta not found.', msg=msg, extra={
                 'template': 'Meta not found: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         else:
             res = MetaCommand.response(identifier=identifier, meta=meta)
             return [res]
 
-    def _put_meta(self, identifier: ID, meta: Meta) -> List[Content]:
+    def _put_meta(self, identifier: ID, meta: Meta, msg: ReliableMessage) -> List[Content]:
         facebook = get_facebook(cpu=self)
         if facebook.save_meta(meta=meta, identifier=identifier):
-            return self._respond_text(text='Meta received.', extra={
+            return self._respond_receipt(text='Meta received.', msg=msg, extra={
                 'template': 'Meta received: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         else:
-            return self._respond_text(text='Meta not accepted.', extra={
+            return self._respond_receipt(text='Meta not accepted.', msg=msg, extra={
                 'template': 'Meta not accepted: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
 
 
@@ -108,74 +108,74 @@
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, DocumentCommand), 'document command error: %s' % content
         identifier = content.identifier
         doc = content.document
         if doc is None:
             # query entity document for ID
             doc_type = content.get_str(key='doc_type', default='*')
-            return self._get_doc(identifier=identifier, doc_type=doc_type)
+            return self._get_doc(identifier=identifier, doc_type=doc_type, msg=msg)
         else:
             # received a new document for ID
-            return self._put_doc(identifier=identifier, meta=content.meta, document=doc)
+            return self._put_doc(identifier=identifier, meta=content.meta, document=doc, msg=msg)
 
-    def _get_doc(self, identifier: ID, doc_type: str = '*') -> List[Content]:
+    def _get_doc(self, identifier: ID, doc_type: str, msg: ReliableMessage) -> List[Content]:
         facebook = get_facebook(cpu=self)
         doc = facebook.document(identifier=identifier, doc_type=doc_type)
         if doc is None:
-            return self._respond_text(text='Document not found.', extra={
+            return self._respond_receipt(text='Document not found.', msg=msg, extra={
                 'template': 'Document not found: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         else:
             meta = facebook.meta(identifier=identifier)
             res = DocumentCommand.response(document=doc, meta=meta, identifier=identifier)
             return [res]
 
-    def _put_doc(self, identifier: ID, meta: Optional[Meta], document: Document) -> List[Content]:
+    def _put_doc(self, identifier: ID, meta: Optional[Meta], document: Document, msg: ReliableMessage) -> List[Content]:
         facebook = get_facebook(cpu=self)
         # check meta
         if meta is None:
             meta = facebook.meta(identifier=identifier)
             if meta is None:
-                return self._respond_text(text='Meta not found.', extra={
+                return self._respond_receipt(text='Meta not found.', msg=msg, extra={
                     'template': 'Meta not found: ${ID}.',
                     'replacements': {
                         'ID': str(identifier),
                     }
                 })
         elif not facebook.save_meta(meta=meta, identifier=identifier):
-            return self._respond_text(text='Meta not accepted.', extra={
+            return self._respond_receipt(text='Meta not accepted.', msg=msg, extra={
                 'template': 'Meta not accepted: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         # check document
         valid = document.valid or document.verify(public_key=meta.key)
         # TODO: check for group document
         if not valid:
             # document error
-            return self._respond_text(text='Document not accepted.', extra={
+            return self._respond_receipt(text='Document not accepted.', msg=msg, extra={
                 'template': 'Document not accepted: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         elif facebook.save_document(document=document):
             # document saved
-            return self._respond_text(text='Document received.', extra={
+            return self._respond_receipt(text='Document received.', msg=msg, extra={
                 'template': 'Document received: ${ID}.',
                 'replacements': {
                     'ID': str(identifier),
                 }
             })
         # document expired
-        return self._respond_text(text='Document not changed.', extra={
+        return self._respond_receipt(text='Document not changed.', msg=msg, extra={
             'template': 'Document not changed: ${ID}.',
             'replacements': {
                 'ID': str(identifier),
             }
         })
```

### Comparing `dimsdk-0.8.6/dimsdk/cpu/contents.py` & `dimsdk-0.8.7/dimsdk/cpu/contents.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/cpu/creator.py` & `dimsdk-0.8.7/dimsdk/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/cpu/customized.py` & `dimsdk-0.8.7/dimsdk/cpu/customized.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         Check for application
 
         :param app:     app ID
         :param content: customized content
         :param msg:     received message
         :return: None on app ID matched
         """
-        return self._respond_text(text='Content not support.', group=content.group, extra={
+        return self._respond_receipt(text='Content not support.', msg=msg, group=content.group, extra={
             'template': 'Customized content (app: ${app}) not support yet!',
             'replacements': {
                 'app': app,
             }
         })
 
     # noinspection PyUnusedLocal
@@ -110,15 +110,15 @@
         return self
 
     # Override
     def handle_action(self, act: str, sender: ID, content: CustomizedContent, msg: ReliableMessage) -> List[Content]:
         """ Override for customized actions """
         app = content.application
         mod = content.module
-        return self._respond_text(text='Content not support.', group=content.group, extra={
+        return self._respond_receipt(text='Content not support.', msg=msg, group=content.group, extra={
             'template': 'Customized content (app: ${app}, mod: ${mod}, act: ${act}) not support yet!',
             'replacements': {
                 'app': app,
                 'mod': mod,
                 'act': act,
             }
         })
```

### Comparing `dimsdk-0.8.6/dimsdk/cpu/factory.py` & `dimsdk-0.8.7/dimsdk/cpu/factory.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/delegate.py` & `dimsdk-0.8.7/dimsdk/delegate.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/facebook.py` & `dimsdk-0.8.7/dimsdk/facebook.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/factories.py` & `dimsdk-0.8.7/dimsdk/factories.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/messenger.py` & `dimsdk-0.8.7/dimsdk/messenger.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/mkm/__init__.py` & `dimsdk-0.8.7/dimsdk/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/mkm/robot.py` & `dimsdk-0.8.7/dimsdk/mkm/robot.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/mkm/roles.py` & `dimsdk-0.8.7/dimsdk/mkm/roles.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/mkm/station.py` & `dimsdk-0.8.7/dimsdk/mkm/station.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/packer.py` & `dimsdk-0.8.7/dimsdk/packer.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk/processor.py` & `dimsdk-0.8.7/dimsdk/processor.py`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/dimsdk.egg-info/PKG-INFO` & `dimsdk-0.8.7/dimsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimsdk
-Version: 0.8.6
+Version: 0.8.7
 Summary: Decentralized Instant Messaging SDK
 Home-page: https://github.com/dimchat/sdk-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging (Python SDK)
```

### Comparing `dimsdk-0.8.6/dimsdk.egg-info/SOURCES.txt` & `dimsdk-0.8.7/dimsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimsdk-0.8.6/setup.py` & `dimsdk-0.8.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.8.6'
+__version__ = '0.8.7'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

