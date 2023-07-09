# Comparing `tmp/qvsed-1.3.9.tar.gz` & `tmp/qvsed-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.3.9.tar", last modified: Sat Jul  8 22:22:45 2023, max compression
+gzip compressed data, was "qvsed-1.4.0.tar", last modified: Sun Jul  9 12:57:54 2023, max compression
```

## Comparing `qvsed-1.3.9.tar` & `qvsed-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 22:22:45.397108 qvsed-1.3.9/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.3.9/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-08 22:22:45.397108 qvsed-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     6130 2023-07-08 21:47:25.000000 qvsed-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 22:22:45.380665 qvsed-1.3.9/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.3.9/qvsed/__init__.py
--rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.3.9/qvsed/config_default.py
--rw-rw-rw-   0        0        0    15371 2023-07-08 22:20:49.000000 qvsed-1.3.9/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-08 21:34:43.000000 qvsed-1.3.9/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-08 22:22:45.395853 qvsed-1.3.9/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-08 22:22:45.000000 qvsed-1.3.9/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 22:22:45.000000 qvsed-1.3.9/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 22:22:45.000000 qvsed-1.3.9/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-08 22:22:45.000000 qvsed-1.3.9/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 22:22:45.000000 qvsed-1.3.9/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 22:22:45.000000 qvsed-1.3.9/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 22:22:45.398115 qvsed-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-08 22:21:43.000000 qvsed-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:54.169784 qvsed-1.4.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-09 12:57:54.169130 qvsed-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5834 2023-07-08 22:29:14.000000 qvsed-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:54.141771 qvsed-1.4.0/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.0/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.4.0/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    20861 2023-07-09 12:49:14.000000 qvsed-1.4.0/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.0/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-09 12:57:54.167130 qvsed-1.4.0/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-09 12:57:54.000000 qvsed-1.4.0/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 12:57:54.170310 qvsed-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-09 12:57:46.000000 qvsed-1.4.0/setup.py
```

### Comparing `qvsed-1.3.9/LICENSE.txt` & `qvsed-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.9/PKG-INFO` & `qvsed-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.9
+Version: 1.4.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.9/README.md` & `qvsed-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -88,30 +88,21 @@
 # The default QVSED config.
 
 # Font
 font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
 font_size = 11
 
 # Colours
-text_color = "white"
-background_color = "#282c34"
-button_background_color = "#393f4a"
-button_hover_background_color = "#31353f"
-button_pressed_background_color = background_color
-scrollbar_background_color = "#31353f"
-scrollbar_handle_background_color = "#393f4a"
-scrollbar_handle_hover_background_color = "#555B67"
+text_color = "#FFFFFF"
+background_color = "#282C34"
+button_color = "#393F4A"
+button_focus_color = "#31353F"
 ```
 
-Keep in mind that `font_family` *must* be a list. If you want only one font, specify:
-
-```python
-# Obviously replace "My Font" with the name of the font you want.
-font_family = ["My Font"]
-```
+Keep in mind that `font_family` *must* be a list. If you want only one font, specify `font_family = ["My Font"]`.
 
 ## Making Shortcuts
 
 ### Windows
 
 1. Locate the QVSED executable file, usually located at `C:\Users\<username>\AppData\Local\Programs\Python\Python3xx\Scripts\qvsed.exe`. Substitute `<username>` with your Windows username and `xx` with whatever Python version you use, for example `Python311`.
 2. Right-click on the executable file and select "Create Shortcut."
```

### Comparing `qvsed-1.3.9/qvsed/qvsed.py` & `qvsed-1.4.0/qvsed/qvsed.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 
 import os
 import sys
 import shutil
 import importlib.util
 import pkg_resources
 from PyQt5.QtWidgets import (
-    QApplication, QMainWindow, QPushButton, QWidget,
-    QFileDialog, QPlainTextEdit, QLineEdit,
+    QApplication, QMainWindow, QWidget, QFileDialog,
     QAction, QShortcut
 )
 from PyQt5.QtGui import (
-    QKeySequence, QFont, QDragEnterEvent, QDropEvent
+    QKeySequence, QFont, QDragEnterEvent, QDropEvent,
+    QTextCursor
+)
+from PyQt5.QtCore import (
+    Qt, QTextCodec, QEvent, QObject, QTimer
 )
-from PyQt5.QtCore import QTextCodec
 from PyQt5.uic import loadUi
 
 
 class QVSEDApp:
     """
     The main application class for QVSED.
     """
@@ -53,14 +55,15 @@
     def __init__(self):
         """
         Initialize the QVSED window.
         """
         super().__init__()
         self.load_ui_file()
         self.focus_text_area()
+        self.install_event_filter()
         self.set_text_area_encoding("UTF-8")
         self.set_up_text_area_handlers()
         self.set_up_action_deck()
         self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.load_config()
         self.set_up_fonts()
         if self.check_if_file_parameter():
@@ -138,79 +141,103 @@
         file_path = sys.argv[1]
         return os.path.isfile(file_path)
 
     def clear_text_area(self):
         """
         Clear the Text Area.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area = self.textArea
 
         if text_area.toPlainText() == "":
             self.echo_area_update("Text Area is already blank.")
             return
 
         text_area.clear()
 
         self.echo_area_update("Text Area has been cleared.")
 
     def connect_command_buttons(self):
         """
         Connect the Action Deck command buttons to their respective functions.
         """
-        self.findChild(QPushButton, "clearButton").clicked.connect(self.clear_text_area)
-        self.findChild(QPushButton, "saveButton").clicked.connect(self.save_text_contents)
-        self.findChild(QPushButton, "openButton").clicked.connect(self.load_from_file)
-        self.findChild(QPushButton, "helpButton").clicked.connect(self.show_help)
-        self.findChild(QPushButton, "quitButton").clicked.connect(self.quit_app)
-        self.findChild(QPushButton, "fullscreenButton").clicked.connect(self.toggle_fullscreen)
+        self.clearButton.clicked.connect(self.clear_text_area)
+        self.saveButton.clicked.connect(self.save_text_contents)
+        self.openButton.clicked.connect(self.load_from_file)
+        self.helpButton.clicked.connect(self.show_help)
+        self.quitButton.clicked.connect(self.quit_app)
+        self.fullscreenButton.clicked.connect(self.toggle_fullscreen)
 
     def connect_key_bindings(self):
         """
-        Connect the Action Deck keybindings to their respective functions.
+        Connect the QVSED keybindings to their respective functions.
         """
+        # Action Deck
         self.clear_shortcut.activated.connect(self.clear_text_area)
         self.save_shortcut.activated.connect(self.save_text_contents)
         self.open_shortcut.activated.connect(self.load_from_file)
         self.help_shortcut.activated.connect(self.show_help)
         self.quit_shortcut.activated.connect(self.quit_app)
         self.fullscreen_shortcut.activated.connect(self.toggle_fullscreen)
 
+        # Cursor movement
+        self.shortcut_up.activated.connect(lambda: self.move_cursor(QTextCursor.Up))
+        self.shortcut_down.activated.connect(lambda: self.move_cursor(QTextCursor.Down))
+        self.shortcut_left.activated.connect(lambda: self.move_cursor(QTextCursor.Left))
+        self.shortcut_right.activated.connect(lambda: self.move_cursor(QTextCursor.Right))
+        self.shortcut_home.activated.connect(lambda: self.move_cursor(QTextCursor.StartOfLine))
+        self.shortcut_end.activated.connect(lambda: self.move_cursor(QTextCursor.EndOfLine))
+        self.shortcut_fwrdword.activated.connect(lambda: self.move_cursor(QTextCursor.NextWord))
+        self.shortcut_backword.activated.connect(lambda: self.move_cursor(QTextCursor.PreviousWord))
+
+        # Page movement
+        self.shortcut_pgup.activated.connect(lambda: self.move_half_page(QTextCursor.Up))
+        self.shortcut_pgdn.activated.connect(lambda: self.move_half_page(QTextCursor.Down))
+
     def drag_enter_event(self, event: QDragEnterEvent):
         """
         Handle the drag enter event for the Text Area.
         """
         if event.mimeData().hasUrls():
             event.acceptProposedAction()
 
     def drop_event(self, event: QDropEvent):
         """
         Handle the drop event for the Text Area.
         """
         if event.mimeData().hasUrls():
             file_path = event.mimeData().urls()[0].toLocalFile()
             self.load_from_file(file_path)
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area = self.textArea
         text_area.repaint()
 
+    def echo_area_timeout_clear(self, interval):
+        """
+        Clear the Echo Area after a duration of time.
+        """
+        echo_area = self.echoArea
+        self.clear_timer = QTimer()
+        self.clear_timer.setSingleShot(True)
+        self.clear_timer.setInterval(interval)
+        self.clear_timer.timeout.connect(echo_area.clear)
+        self.clear_timer.start()
+
     def echo_area_update(self, message):
         """
         Update the Echo Area with the given message.
-
-        Args:
-            message (str): The message to display in the Echo Area.
         """
-        echo_area = self.findChild(QLineEdit, "echoArea")
+        echo_area = self.echoArea
         echo_area.setText(message)
         echo_area.setCursorPosition(0)
+        self.echo_area_timeout_clear(3000)
 
     def focus_text_area(self):
         """
         Set the Text Area to have focus.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area = self.textArea
         text_area.setFocus()
 
     def generate_config(self):
         """
         Generate the config file for QVSED.
         """
         current_dir = os.path.dirname(os.path.abspath(__file__))
@@ -243,14 +270,24 @@
         Return the QVSED version specified in setup.py.
         """
         try:
             return pkg_resources.get_distribution('qvsed').version
         except pkg_resources.DistributionNotFound:
             return "?.?.?"
 
+    def install_event_filter(self):
+        """
+        Install the `keyPressFilter` to the Text Area.
+
+        Used to handle incorrect key combinations.
+        """
+        text_area = self.textArea
+        self.keyPressFilter = KeyPressFilter(self)
+        text_area.installEventFilter(self.keyPressFilter)
+
     def load_config(self):
         """
         Load the configuration for QVSED.
         """
         if os.name == "nt":  # Windows
             user_config_dir = os.path.join(os.environ["APPDATA"], "QVSED")
         else:  # *nix
@@ -279,15 +316,15 @@
         except AttributeError as error:
             self.echo_area_update(f"Check config.py: {str(error)}")
 
     def load_from_file(self, file_path = None):
         """
         Open a file dialog, and load the contents of a file into the Text Area.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area = self.textArea
 
         if not file_path:
             file_path, _ = QFileDialog.getOpenFileName(self, "Open File")
 
         if file_path:
             try:
                 with open(file_path, "r", encoding="utf-8") as file:
@@ -301,25 +338,57 @@
         """
         Load the UI file for the QVSED window.
         """
         current_dir = os.path.dirname(os.path.abspath(__file__))
         ui_file = os.path.join(current_dir, "qvsed.ui")
         loadUi(ui_file, self)
 
+    def move_cursor(self, direction):
+        """
+        Move the cursor in the Text Area.
+
+        Used for the Vim-style A-h, A-j, A-k and A-l commands.
+        """
+        text_area = self.textArea
+        cursor = text_area.textCursor()
+        cursor.movePosition(direction)
+        text_area.setTextCursor(cursor)
+
+    def move_half_page(self, direction):
+        """
+        Move the page up or down in the Text Area.
+
+        Used for the Vim-style A-u and A-d commands.
+        """
+        text_area = self.textArea
+        scroll_bar = text_area.verticalScrollBar()
+        scroll_value = scroll_bar.value()
+        scroll_maximum = scroll_bar.maximum()
+        scroll_step = scroll_bar.singleStep()
+
+        half_page_steps = int(scroll_bar.pageStep() / 2)
+
+        if direction == QTextCursor.Up:
+            scroll_bar.setValue(max(scroll_value - half_page_steps * scroll_step, 0))
+        elif direction == QTextCursor.Down:
+            scroll_bar.setValue(min(scroll_value + half_page_steps * scroll_step, scroll_maximum))
+
+        text_area.verticalScrollBar().valueChanged.emit(scroll_bar.value())
+
     def quit_app(self):
         """
         Quit QVSED.
         """
         QApplication.quit()
 
     def save_text_contents(self):
         """
         Open a file dialog, and save the contents of the Text Area to a file.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area = self.textArea
 
         if text_area.toPlainText() == "":
             self.echo_area_update("Text Area is blank, will not save.")
             return
 
         file_path, _ = QFileDialog.getSaveFileName(self, "Save File")
 
@@ -369,46 +438,65 @@
         self.connect_command_buttons()
         self.connect_key_bindings()
 
     def set_up_text_area_handlers(self):
         """
         Set up the event handlers for the Text Area.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area = self.textArea
 
         text_area.dragEnterEvent = self.drag_enter_event
         text_area.dragMoveEvent = self.drag_enter_event
         text_area.dropEvent = self.drop_event
 
     def set_up_fonts(self):
         """
         Set up the fonts for the QVSED window.
         """
+        text_area = self.textArea
         font = QFont()
         font.setFamilies(self.font_family)
         font.setPointSize(self.font_size)
+        text_area.setTabStopWidth(4 * text_area.fontMetrics().width(' '))
         QApplication.instance().setFont(font)
         self.update_widget_fonts(self)
 
     def set_up_shortcuts(self):
         """
-        Set up the key bindings for the Action Deck commands.
+        Set up the key bindings for QVSED.
         """
+        # Action Deck
         self.clear_shortcut = QShortcut(QKeySequence("Ctrl+N"), self)
         self.save_shortcut = QShortcut(QKeySequence("Ctrl+S"), self)
         self.open_shortcut = QShortcut(QKeySequence("Ctrl+F"), self)
         self.help_shortcut = QShortcut(QKeySequence("Ctrl+H"), self)
         self.quit_shortcut = QShortcut(QKeySequence("Alt+Q"), self)
         self.fullscreen_shortcut = QShortcut(QKeySequence("Alt+F"), self)
 
+        # Vim-style movement with Alt/Option key
+        self.shortcut_left = QShortcut(QKeySequence("Alt+H"), self)
+        self.shortcut_down = QShortcut(QKeySequence("Alt+J"), self)
+        self.shortcut_up = QShortcut(QKeySequence("Alt+K"), self)
+        self.shortcut_right = QShortcut(QKeySequence("Alt+L"), self)
+
+        self.shortcut_pgup = QShortcut(QKeySequence("Alt+U"), self)
+        self.shortcut_pgdn = QShortcut(QKeySequence("Alt+D"), self)
+
+        self.shortcut_fwrdword = QShortcut(QKeySequence("Alt+W"), self)
+        self.shortcut_backword = QShortcut(QKeySequence("Alt+B"), self)
+
+        # Emacs-style C-a and C-e, but with Alt instead
+        self.shortcut_home = QShortcut(QKeySequence("Alt+A"), self)
+        self.shortcut_end = QShortcut(QKeySequence("Alt+E"), self)
+
     def show_help(self):
         """
         Display the help message in the Text Area.
         """
-        text_area = self.findChild(QPlainTextEdit, "textArea")
+        text_area = self.textArea
 
         help_message = """QVSED - Qt-based Volatile Small Editor
 ========================================
 QVSED is a stateless, volatile text editor with a minimalist approach, focusing solely on text editing without file metadata or prompts for potentially destructive actions.
 
 This is the Text Area, where the actual editing takes place. Type anything you want into here, and edit as you please.
 Down there, at the bottom of the window, is the Echo Area, where messages and errors will be displayed.
@@ -444,14 +532,56 @@
             return
 
         widget.setFont(QApplication.instance().font())
 
         for child_widget in widget.findChildren(QWidget):
             self.update_widget_fonts(child_widget)
 
+class KeyPressFilter(QObject):
+    """
+    Subclasses QObject.
+    """
+    def __init__(self, window):
+        super().__init__()
+        self.window = window
+
+    def eventFilter(self, obj, event):
+        # yes, Pylint, I know it's not snake_case, wanna fight about it?
+        """
+        Override the eventFilter and use QEvent.KeyPress to handle invalid key bindings.
+        """
+        if event.type() == QEvent.KeyPress:
+            if (event.modifiers() & (Qt.ControlModifier | Qt.AltModifier)) and event.key() not in [Qt.Key_Control, Qt.Key_Alt, Qt.Key_Shift]:
+                keys = []
+                if event.modifiers() & Qt.ControlModifier:
+                    keys.append("C")
+                if event.modifiers() & Qt.AltModifier:
+                    keys.append("A")
+                if event.modifiers() & Qt.ShiftModifier:
+                    keys.append("S")
+                if event.key() != Qt.Key_No:
+                    is_os_shortcut = any(event.matches(shortcut) for shortcut in [
+                        QKeySequence.Copy, QKeySequence.Cut, QKeySequence.Paste,
+                        QKeySequence.Undo, QKeySequence.Redo, QKeySequence.SelectAll,
+                        QKeySequence.MoveToPreviousWord, QKeySequence.MoveToNextWord,
+                        QKeySequence.SelectPreviousWord, QKeySequence.SelectNextWord,
+                        QKeySequence.SelectStartOfDocument, QKeySequence.SelectEndOfDocument,
+                        QKeySequence.DeleteStartOfWord, QKeySequence.DeleteEndOfWord
+                    ])
+                    if is_os_shortcut:
+                        return super().eventFilter(obj, event)
+
+                    key_name = QKeySequence(event.key()).toString().lower()
+                    keys.append(key_name)
+
+                key_combination = "-".join(keys)
+                undefined_message = f"<{key_combination}> is undefined."
+                self.window.echo_area_update(undefined_message)
+                return True
+        return super().eventFilter(obj, event)
 
 def main():
     """
     The entry point for the QVSED application.
     """
     app = QVSEDApp()
     app.run()
```

### Comparing `qvsed-1.3.9/qvsed/qvsed.ui` & `qvsed-1.4.0/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.3.9/qvsed.egg-info/PKG-INFO` & `qvsed-1.4.0/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.3.9
+Version: 1.4.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.3.9/setup.py` & `qvsed-1.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.3.9',
+    version='1.4.0',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

