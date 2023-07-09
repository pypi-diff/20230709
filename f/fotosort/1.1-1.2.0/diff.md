# Comparing `tmp/fotosort-1.1-py3-none-any.whl.zip` & `tmp/fotosort-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27804 bytes, number of entries: 12
+Zip file size: 28041 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     1038 b- defN 19-Jun-23 08:15 fotosort/__init__.py
--rw-r--r--  2.0 unx     3377 b- defN 19-Jun-22 13:15 fotosort/controller.py
+-rw-r--r--  2.0 unx     3702 b- defN 23-Jul-09 10:28 fotosort/controller.py
 -rw-r--r--  2.0 unx     1064 b- defN 19-Jun-22 13:16 fotosort/imgutils.py
--rw-r--r--  2.0 unx     5651 b- defN 19-Jun-23 09:00 fotosort/ui.py
+-rw-r--r--  2.0 unx     6195 b- defN 23-Jul-09 10:28 fotosort/ui.py
 -rw-r--r--  2.0 unx     6121 b- defN 19-Mar-17 16:29 fotosort/images/noimage.png
--rw-r--r--  2.0 unx     8561 b- defN 19-Jun-23 09:00 fotosort/qml/main.qml
--rwxr-xr-x  2.0 unx       40 b- defN 19-Jun-23 09:04 fotosort-1.1.data/scripts/fotosort
--rw-r--r--  2.0 unx    35149 b- defN 19-Jun-23 09:04 fotosort-1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     8861 b- defN 19-Jun-23 09:04 fotosort-1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Jun-23 09:04 fotosort-1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 19-Jun-23 09:04 fotosort-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      936 b- defN 19-Jun-23 09:04 fotosort-1.1.dist-info/RECORD
-12 files, 70899 bytes uncompressed, 26246 bytes compressed:  63.0%
+-rw-r--r--  2.0 unx     8737 b- defN 23-Jul-09 10:28 fotosort/qml/main.qml
+-rwxr-xr-x  2.0 unx       40 b- defN 23-Jul-09 10:45 fotosort-1.2.0.data/scripts/fotosort
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8866 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      948 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/RECORD
+12 files, 71961 bytes uncompressed, 26459 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: fotosort/images/noimage.png
 Comment: 
 
 Filename: fotosort/qml/main.qml
 Comment: 
 
-Filename: fotosort-1.1.data/scripts/fotosort
+Filename: fotosort-1.2.0.data/scripts/fotosort
 Comment: 
 
-Filename: fotosort-1.1.dist-info/LICENSE
+Filename: fotosort-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: fotosort-1.1.dist-info/METADATA
+Filename: fotosort-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: fotosort-1.1.dist-info/WHEEL
+Filename: fotosort-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: fotosort-1.1.dist-info/top_level.txt
+Filename: fotosort-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fotosort-1.1.dist-info/RECORD
+Filename: fotosort-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fotosort/controller.py

```diff
@@ -19,26 +19,38 @@
                 self.file_list = sorted(self.file_list)
 
     def current(self):
         if not self.file_list:
             return None
         return self.file_list[self.curr_index]
 
+    def first(self):
+        if not self.file_list:
+            return None
+        self.curr_index = 0
+        return self.file_list[self.curr_index]
+
     def prev(self):
         if not self.file_list:
             return None
         self.curr_index = max(0, self.curr_index - 1)
         return self.file_list[self.curr_index]
 
     def next(self):
         if not self.file_list:
             return None
         self.curr_index = min(len(self.file_list) - 1, self.curr_index + 1)
         return self.file_list[self.curr_index]
 
+    def last(self):
+        if not self.file_list:
+            return None
+        self.curr_index = len(self.file_list) - 1
+        return self.file_list[self.curr_index]
+
     def copyCurrentFile(self, target_dir):
         if not self.file_list:
             return None
         source_file = self.file_list[self.curr_index]
         target_file = self.__collision_free_filename(source_file, target_dir)
         self.history.append(["Copy", source_file, target_file, self.curr_index])
         shutil.copy(source_file, target_file)
```

## fotosort/ui.py

```diff
@@ -60,30 +60,42 @@
 
     @Slot(result=str)
     def getCurrentImageTimestamp(self):
         return imgutils.get_timestamp(self.currentImage)
 
     def setCurrentImage(self, new_image):
         self.currentImage = new_image
-        self.imageChangedSignal.emit()
+        w, h = self.root.width(), self.root.height()  # Save previous window geometry
+        self.imageChangedSignal.emit()  # This loads the picture and displays it, unfortunately resizing the window
+        self.root.resize(w,h)  # Programatically restore the window geometry prior to the load to avoid huge window
         # Adjust undo button
         if self.root.setUndoEnabled(len(self.controller.history) > 0):
             self.root.setUndoText("Undo {}".format(self.controller.history[-1][0]))
 
     @Slot()
+    def first(self):
+        self.setCurrentImage(self.controller.first())
+        self.root.showStatus("[<-", "black")
+
+    @Slot()
     def prev(self):
         self.setCurrentImage(self.controller.prev())
         self.root.showStatus("<-", "black")
 
     @Slot()
     def next(self):
         self.setCurrentImage(self.controller.next())
         self.root.showStatus("->", "black")
 
     @Slot()
+    def last(self):
+        self.setCurrentImage(self.controller.last())
+        self.root.showStatus("->]", "black")
+
+    @Slot()
     def reload(self):
         self.setCurrentImage(self.controller.current())
 
     @Slot(str)
     def moveOrCopyCurrentFile(self, targetdir):
         if self.conf.copy_pictures:
             self.controller.copyCurrentFile(targetdir)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## fotosort/qml/main.qml

```diff
@@ -204,16 +204,18 @@
             MenuItem { text: "Manage settings"; shortcut: "Ctrl+,"; onTriggered: ui.openSettingsDialog() }
             MenuItem { text: "Manage target locations"; shortcut: "Ctrl+Shift+T"; onTriggered: ui.openTargetsDialog() }
             MenuItem { text: "Add temporary target location"; shortcut: "Ctrl+T"; onTriggered: ui.openAddTempTargetDialog() }
             MenuItem { text: "Quit"; shortcut: "Ctrl+Q"; onTriggered: Qt.quit() }
         }
         Menu {
             title: "Navigate"
+            MenuItem { text: "First"; shortcut: "Ctrl+Shift+Tab"; onTriggered: ui.first() }
             MenuItem { text: "Prev"; shortcut: "Shift+Tab"; onTriggered: ui.prev() }
             MenuItem { text: "Next"; shortcut: "Tab"; onTriggered: ui.next() }
+            MenuItem { text: "Last"; shortcut: "Ctrl+Tab"; onTriggered: ui.last() }
         }
         Menu {
             title: "Actions"
             MenuItem { text: "Undo"; shortcut: "Ctrl+Z"; onTriggered: { ui.undo(); ui.reload(); } id: undoMenuItem; enabled: false }
             MenuItem { text: "Trash"; shortcut: "Ctrl+D"; onTriggered: { ui.trashCurrentFile(); ui.reload(); } }
         }
     }
```

## Comparing `fotosort-1.1.dist-info/LICENSE` & `fotosort-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fotosort-1.1.dist-info/METADATA` & `fotosort-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fotosort
-Version: 1.1
+Version: 1.2.0
 Summary: Fotosort is a program for quickly copying or moving pictures from different events into different folders.
 Home-page: https://github.com/kalsan/fotosort
 Author: Sandro Kalbermatter
 Author-email: 
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: pyyaml
 Requires-Dist: pyside2
 Requires-Dist: appdirs
 
 # Fotosort
 
@@ -76,8 +76,7 @@
 ## Quickly creating a temporary target directory
 
 In order to quickly create a temporary target directory as described in scenario 2, press Ctrl+T. The suggested target directory name is generated from the prefix you specified in the config file as well as the capture date found in the current picture. However, this is just a suggestion and you may enter an arbitrary path. Once done, hit Enter and the folder is created (unless it exists already), added to the temporary target directories, and activated in the combobox. When you hit Enter again, the current picture is moved to that folder.
 
 # Contributing
 
 I wrote this program for my own convenience, but there isn't really a reason why you shouldn't be able to adjust it for you own needs. After all, this is FOSS! :-) I'm happy to accept your pull requests.
-
```

