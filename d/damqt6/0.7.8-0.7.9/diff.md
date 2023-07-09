# Comparing `tmp/damqt6-0.7.8.tar.gz` & `tmp/damqt6-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damqt6-0.7.8.tar", last modified: Fri Jan  6 10:24:15 2023, max compression
+gzip compressed data, was "damqt6-0.7.9.tar", last modified: Sun Jul  9 11:25:42 2023, max compression
```

## Comparing `damqt6-0.7.8.tar` & `damqt6-0.7.9.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrws---   0 michel    (1000) michel    (1000)        0 2023-01-06 10:24:15.247900 damqt6-0.7.8/
--rw-rw----   0 michel    (1000) michel    (1000)     1060 2022-06-26 12:25:51.000000 damqt6-0.7.8/LICENSE
--rw-rw----   0 michel    (1000) michel    (1000)      462 2023-01-06 10:24:15.247900 damqt6-0.7.8/PKG-INFO
--rw-rw----   0 michel    (1000) michel    (1000)      101 2022-06-27 17:26:58.000000 damqt6-0.7.8/README.rst
--rw-rw----   0 michel    (1000) michel    (1000)      685 2023-01-06 10:23:55.000000 damqt6-0.7.8/pyproject.toml
--rw-rw----   0 michel    (1000) michel    (1000)       38 2023-01-06 10:24:15.247900 damqt6-0.7.8/setup.cfg
-drwxrws---   0 michel    (1000) michel    (1000)        0 2023-01-06 10:24:15.243900 damqt6-0.7.8/src/
-drwxrws---   0 michel    (1000) michel    (1000)        0 2023-01-06 10:24:15.247900 damqt6-0.7.8/src/damqt6/
--rw-rw----   0 michel    (1000) michel    (1000)      343 2022-12-23 10:36:15.000000 damqt6-0.7.8/src/damqt6/__init__.py
--rwxrwx---   0 michel    (1000) michel    (1000)     4918 2023-01-06 10:23:03.000000 damqt6-0.7.8/src/damqt6/_common.py
--rw-rw----   0 michel    (1000) michel    (1000)      964 2022-12-18 09:09:19.000000 damqt6-0.7.8/src/damqt6/_qapplication.py
--rw-rw----   0 michel    (1000) michel    (1000)     1163 2022-06-26 12:25:51.000000 damqt6-0.7.8/src/damqt6/_qbuttons.py
--rw-rw----   0 michel    (1000) michel    (1000)     6683 2022-06-26 17:54:27.000000 damqt6-0.7.8/src/damqt6/_qcomboboxes.py
--rw-rw----   0 michel    (1000) michel    (1000)     2888 2022-06-26 12:25:51.000000 damqt6-0.7.8/src/damqt6/_qdialogs.py
--rw-rw----   0 michel    (1000) michel    (1000)     1112 2022-06-26 12:25:51.000000 damqt6-0.7.8/src/damqt6/_qlabels.py
--rw-rw----   0 michel    (1000) michel    (1000)     3171 2022-12-18 12:35:47.000000 damqt6-0.7.8/src/damqt6/_qlineedits.py
--rw-rw----   0 michel    (1000) michel    (1000)     2244 2022-06-26 17:54:38.000000 damqt6-0.7.8/src/damqt6/_qlistwidgets.py
--rwxrwx---   0 michel    (1000) michel    (1000)     3029 2022-12-25 18:54:21.000000 damqt6-0.7.8/src/damqt6/_qsignals.py
--rw-rw----   0 michel    (1000) michel    (1000)     1564 2022-12-19 13:51:05.000000 damqt6-0.7.8/src/damqt6/_qtablewidgets.py
--rw-rw----   0 michel    (1000) michel    (1000)      727 2022-06-26 12:25:51.000000 damqt6-0.7.8/src/damqt6/_qvalidators.py
--rw-rw----   0 michel    (1000) michel    (1000)      263 2022-06-26 12:25:51.000000 damqt6-0.7.8/src/damqt6/_qwindows.py
--rwxrwx---   0 michel    (1000) michel    (1000)     1619 2022-06-26 12:25:51.000000 damqt6-0.7.8/src/damqt6/_settings.py
--rwxrwx---   0 michel    (1000) michel    (1000)      511 2022-12-23 10:37:04.000000 damqt6-0.7.8/src/damqt6/debug.py
-drwxrws---   0 michel    (1000) michel    (1000)        0 2023-01-06 10:24:15.247900 damqt6-0.7.8/src/damqt6.egg-info/
--rw-rw----   0 michel    (1000) michel    (1000)      462 2023-01-06 10:24:15.000000 damqt6-0.7.8/src/damqt6.egg-info/PKG-INFO
--rw-rw----   0 michel    (1000) michel    (1000)      575 2023-01-06 10:24:15.000000 damqt6-0.7.8/src/damqt6.egg-info/SOURCES.txt
--rw-rw----   0 michel    (1000) michel    (1000)        1 2023-01-06 10:24:15.000000 damqt6-0.7.8/src/damqt6.egg-info/dependency_links.txt
--rw-rw----   0 michel    (1000) michel    (1000)       66 2023-01-06 10:24:15.000000 damqt6-0.7.8/src/damqt6.egg-info/requires.txt
--rw-rw----   0 michel    (1000) michel    (1000)        7 2023-01-06 10:24:15.000000 damqt6-0.7.8/src/damqt6.egg-info/top_level.txt
+drwxrws---   0 michel    (1000) michel    (1000)        0 2023-07-09 11:25:42.372447 damqt6-0.7.9/
+-rw-rw----   0 michel    (1000) michel    (1000)     1060 2022-06-26 12:25:51.000000 damqt6-0.7.9/LICENSE
+-rw-rw----   0 michel    (1000) michel    (1000)      462 2023-07-09 11:25:42.372447 damqt6-0.7.9/PKG-INFO
+-rw-rw----   0 michel    (1000) michel    (1000)      101 2022-06-27 17:26:58.000000 damqt6-0.7.9/README.rst
+-rw-rw----   0 michel    (1000) michel    (1000)      685 2023-07-09 11:22:58.000000 damqt6-0.7.9/pyproject.toml
+-rw-rw----   0 michel    (1000) michel    (1000)       38 2023-07-09 11:25:42.372447 damqt6-0.7.9/setup.cfg
+drwxrws---   0 michel    (1000) michel    (1000)        0 2023-07-09 11:25:42.368447 damqt6-0.7.9/src/
+drwxrws---   0 michel    (1000) michel    (1000)        0 2023-07-09 11:25:42.368447 damqt6-0.7.9/src/damqt6/
+-rw-rw----   0 michel    (1000) michel    (1000)      343 2022-12-23 10:36:15.000000 damqt6-0.7.9/src/damqt6/__init__.py
+-rwxrwx---   0 michel    (1000) michel    (1000)     4973 2023-01-06 15:04:25.000000 damqt6-0.7.9/src/damqt6/_common.py
+-rw-rw----   0 michel    (1000) michel    (1000)     1237 2023-07-09 10:49:53.000000 damqt6-0.7.9/src/damqt6/_qapplication.py
+-rw-rw----   0 michel    (1000) michel    (1000)     1163 2022-06-26 12:25:51.000000 damqt6-0.7.9/src/damqt6/_qbuttons.py
+-rw-rw----   0 michel    (1000) michel    (1000)     6683 2022-06-26 17:54:27.000000 damqt6-0.7.9/src/damqt6/_qcomboboxes.py
+-rw-rw----   0 michel    (1000) michel    (1000)     2888 2022-06-26 12:25:51.000000 damqt6-0.7.9/src/damqt6/_qdialogs.py
+-rw-rw----   0 michel    (1000) michel    (1000)     1112 2022-06-26 12:25:51.000000 damqt6-0.7.9/src/damqt6/_qlabels.py
+-rw-rw----   0 michel    (1000) michel    (1000)     3171 2022-12-18 12:35:47.000000 damqt6-0.7.9/src/damqt6/_qlineedits.py
+-rw-rw----   0 michel    (1000) michel    (1000)     2244 2022-06-26 17:54:38.000000 damqt6-0.7.9/src/damqt6/_qlistwidgets.py
+-rwxrwx---   0 michel    (1000) michel    (1000)     3029 2022-12-25 18:54:21.000000 damqt6-0.7.9/src/damqt6/_qsignals.py
+-rw-rw----   0 michel    (1000) michel    (1000)     1564 2022-12-19 13:51:05.000000 damqt6-0.7.9/src/damqt6/_qtablewidgets.py
+-rw-rw----   0 michel    (1000) michel    (1000)      727 2022-06-26 12:25:51.000000 damqt6-0.7.9/src/damqt6/_qvalidators.py
+-rw-rw----   0 michel    (1000) michel    (1000)      263 2022-06-26 12:25:51.000000 damqt6-0.7.9/src/damqt6/_qwindows.py
+-rwxrwx---   0 michel    (1000) michel    (1000)     1619 2022-06-26 12:25:51.000000 damqt6-0.7.9/src/damqt6/_settings.py
+-rwxrwx---   0 michel    (1000) michel    (1000)      511 2022-12-23 10:37:04.000000 damqt6-0.7.9/src/damqt6/debug.py
+drwxrws---   0 michel    (1000) michel    (1000)        0 2023-07-09 11:25:42.372447 damqt6-0.7.9/src/damqt6.egg-info/
+-rw-rw----   0 michel    (1000) michel    (1000)      462 2023-07-09 11:25:42.000000 damqt6-0.7.9/src/damqt6.egg-info/PKG-INFO
+-rw-rw----   0 michel    (1000) michel    (1000)      590 2023-07-09 11:25:42.000000 damqt6-0.7.9/src/damqt6.egg-info/SOURCES.txt
+-rw-rw----   0 michel    (1000) michel    (1000)        1 2023-07-09 11:25:42.000000 damqt6-0.7.9/src/damqt6.egg-info/dependency_links.txt
+-rw-rw----   0 michel    (1000) michel    (1000)       66 2023-07-09 11:25:42.000000 damqt6-0.7.9/src/damqt6.egg-info/requires.txt
+-rw-rw----   0 michel    (1000) michel    (1000)        7 2023-07-09 11:25:42.000000 damqt6-0.7.9/src/damqt6.egg-info/top_level.txt
+drwxrws---   0 michel    (1000) michel    (1000)        0 2023-07-09 11:25:42.372447 damqt6-0.7.9/tests/
+-rw-rw----   0 michel    (1000) michel    (1000)     1491 2023-07-09 11:16:23.000000 damqt6-0.7.9/tests/tests.py
```

### Comparing `damqt6-0.7.8/LICENSE` & `damqt6-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/pyproject.toml` & `damqt6-0.7.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "damqt6"
-version = "0.7.8"
+version = "0.7.9"
 authors = [
   { name="Dahmaloch", email="dahmaloch@gmail.com" },
 ]
 description = "Dahmaloch's PyQt6 controls"
 readme = "README.rst"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'PyQt6>=6.4.0',
-    'PyQt6-Qt6>=6.4.1',
-    'PyQt6-sip>=13.4.0',
+    'PyQt6==6.4.2',
+    'PyQt6-Qt6==6.4.2',
+    'PyQt6-sip==13.5.1',
     'damstrings>=0.7.2',
 ]
 
 #[project.urls]
 #"Homepage" = "https://github.com/pypa/sampleproject"
 #"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `damqt6-0.7.8/src/damqt6/_common.py` & `damqt6-0.7.9/src/damqt6/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         _read_window_pos(self)
 
     def show(self) -> None:
         if self.isVisible():
             self.activateWindow()
         else:
             super().show()
+        # Sometimes focus widget is not really focused
         if self.focusWidget():
             self.focusWidget().setFocus()
 
     def showNormal(self) -> None:
         self.show()
         self.setWindowState(self.windowState() & ~Qt.WindowState.WindowMinimized & ~Qt.WindowState.WindowMaximized)
```

### Comparing `damqt6-0.7.8/src/damqt6/_qapplication.py` & `damqt6-0.7.9/src/damqt6/_qapplication.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from PyQt6.QtCore import QObject, QEvent
+from PyQt6.QtCore import QObject, QEvent, QByteArray, QBuffer
 from PyQt6.QtWidgets import QApplication as PyQt6_QApplication, QLineEdit, QComboBox
 
 
 class QApplication(PyQt6_QApplication):
     _prev_focus = QObject()
     _prev_selection = QObject()
 
@@ -26,7 +26,16 @@
     @classmethod
     def prev_focus(cls) -> QObject:
         return cls._prev_focus
 
     @classmethod
     def prev_selection(cls) -> QObject:
         return cls._prev_selection
+
+    @classmethod
+    def get_clipboard_image(cls) -> QByteArray:
+        img = cls.clipboard().image()
+        ba = QByteArray()
+        buf = QBuffer(ba)
+        buf.open(QBuffer.OpenModeFlag.ReadWrite)
+        img.save(buf, 'PNG')
+        return ba
```

### Comparing `damqt6-0.7.8/src/damqt6/_qbuttons.py` & `damqt6-0.7.9/src/damqt6/_qbuttons.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qcomboboxes.py` & `damqt6-0.7.9/src/damqt6/_qcomboboxes.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qdialogs.py` & `damqt6-0.7.9/src/damqt6/_qdialogs.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qlabels.py` & `damqt6-0.7.9/src/damqt6/_qlabels.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qlineedits.py` & `damqt6-0.7.9/src/damqt6/_qlineedits.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qlistwidgets.py` & `damqt6-0.7.9/src/damqt6/_qlistwidgets.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qsignals.py` & `damqt6-0.7.9/src/damqt6/_qsignals.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qtablewidgets.py` & `damqt6-0.7.9/src/damqt6/_qtablewidgets.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_qvalidators.py` & `damqt6-0.7.9/src/damqt6/_qvalidators.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6/_settings.py` & `damqt6-0.7.9/src/damqt6/_settings.py`

 * *Files identical despite different names*

### Comparing `damqt6-0.7.8/src/damqt6.egg-info/SOURCES.txt` & `damqt6-0.7.9/src/damqt6.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 src/damqt6/_qwindows.py
 src/damqt6/_settings.py
 src/damqt6/debug.py
 src/damqt6.egg-info/PKG-INFO
 src/damqt6.egg-info/SOURCES.txt
 src/damqt6.egg-info/dependency_links.txt
 src/damqt6.egg-info/requires.txt
-src/damqt6.egg-info/top_level.txt
+src/damqt6.egg-info/top_level.txt
+tests/tests.py
```

