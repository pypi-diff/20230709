# Comparing `tmp/voicemeeter_api-2.1.2.tar.gz` & `tmp/voicemeeter_api-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.1.2.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.1.3.tar", max compression
```

## Comparing `voicemeeter_api-2.1.2.tar` & `voicemeeter_api-2.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.1.2/LICENSE
--rw-r--r--   0        0        0     1111 2023-07-08 06:49:33.599926 voicemeeter_api-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    17394 2023-07-01 19:24:29.927689 voicemeeter_api-2.1.2/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.1.2/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.1.2/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter_api-2.1.2/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.1.2/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.1.2/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.1.2/voicemeeterlib/device.py
--rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter_api-2.1.2/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.1.2/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.1.2/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.1.2/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.1.2/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.1.2/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.1.2/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.1.2/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-01 18:51:25.725768 voicemeeter_api-2.1.2/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.1.2/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    11145 2023-07-08 06:48:45.639873 voicemeeter_api-2.1.2/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.1.2/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.1.2/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2978 2023-06-25 02:33:59.383974 voicemeeter_api-2.1.2/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.1.2/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.1.2/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    17226 1970-01-01 00:00:00.000000 voicemeeter_api-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.1.3/LICENSE
+-rw-r--r--   0        0        0     1111 2023-07-09 00:45:16.686090 voicemeeter_api-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0    17394 2023-07-01 19:24:29.927689 voicemeeter_api-2.1.3/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.1.3/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.1.3/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter_api-2.1.3/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.1.3/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.1.3/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.1.3/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter_api-2.1.3/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.1.3/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.1.3/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.1.3/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.1.3/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.1.3/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.1.3/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.1.3/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-01 18:51:25.725768 voicemeeter_api-2.1.3/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.1.3/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    11192 2023-07-09 00:42:36.890657 voicemeeter_api-2.1.3/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.1.3/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.1.3/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2978 2023-06-25 02:33:59.383974 voicemeeter_api-2.1.3/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.1.3/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.1.3/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    17226 1970-01-01 00:00:00.000000 voicemeeter_api-2.1.3/PKG-INFO
```

### Comparing `voicemeeter_api-2.1.2/LICENSE` & `voicemeeter_api-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/pyproject.toml` & `voicemeeter_api-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.1.2"
+version = "2.1.3"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [
```

### Comparing `voicemeeter_api-2.1.2/README.md` & `voicemeeter_api-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/bus.py` & `voicemeeter_api-2.1.3/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.1.3/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/command.py` & `voicemeeter_api-2.1.3/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/config.py` & `voicemeeter_api-2.1.3/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/device.py` & `voicemeeter_api-2.1.3/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/event.py` & `voicemeeter_api-2.1.3/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/factory.py` & `voicemeeter_api-2.1.3/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/inst.py` & `voicemeeter_api-2.1.3/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/iremote.py` & `voicemeeter_api-2.1.3/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/kinds.py` & `voicemeeter_api-2.1.3/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.1.3/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/meta.py` & `voicemeeter_api-2.1.3/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/misc.py` & `voicemeeter_api-2.1.3/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/recorder.py` & `voicemeeter_api-2.1.3/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/remote.py` & `voicemeeter_api-2.1.3/voicemeeterlib/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,17 @@
         """Login to the API, initialize dirty parameters"""
         self.gui.launched = self.call(self.vm_login, ok=(0, 1)) == 0
         if not self.gui.launched:
             self.logger.info(
                 "Voicemeeter engine running but GUI not launched. Launching the GUI now."
             )
             self.run_voicemeeter(self.kind.name)
-        self.logger.info(f"{type(self).__name__}: Successfully logged into {self}")
+        self.logger.info(
+            f"{type(self).__name__}: Successfully logged into {self} version {self.version}"
+        )
         self.clear_dirty()
 
     def run_voicemeeter(self, kind_id: str) -> NoReturn:
         if kind_id not in (kind.name.lower() for kind in KindId):
             raise VMError(f"Unexpected Voicemeeter type: '{kind_id}'")
         if kind_id == "potato" and bits == 8:
             value = KindId[kind_id.upper()].value + 3
```

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/strip.py` & `voicemeeter_api-2.1.3/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/subject.py` & `voicemeeter_api-2.1.3/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/updater.py` & `voicemeeter_api-2.1.3/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/util.py` & `voicemeeter_api-2.1.3/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/voicemeeterlib/vban.py` & `voicemeeter_api-2.1.3/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.1.2/PKG-INFO` & `voicemeeter_api-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.1.2
+Version: 2.1.3
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

