# Comparing `tmp/qvsed-1.4.0.tar.gz` & `tmp/qvsed-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.4.0.tar", last modified: Sun Jul  9 12:57:54 2023, max compression
+gzip compressed data, was "qvsed-1.4.1.tar", last modified: Sun Jul  9 16:32:53 2023, max compression
```

## Comparing `qvsed-1.4.0.tar` & `qvsed-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 12:57:54.169784 qvsed-1.4.0/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-09 12:57:54.169130 qvsed-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5834 2023-07-08 22:29:14.000000 qvsed-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 12:57:54.141771 qvsed-1.4.0/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.0/qvsed/__init__.py
--rw-rw-rw-   0        0        0      383 2023-07-08 21:13:12.000000 qvsed-1.4.0/qvsed/config_default.py
--rw-rw-rw-   0        0        0    20861 2023-07-09 12:49:14.000000 qvsed-1.4.0/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.0/qvsed/qvsed.ui
-drwxrwxrwx   0        0        0        0 2023-07-09 12:57:54.167130 qvsed-1.4.0/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-09 12:57:54.000000 qvsed-1.4.0/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 12:57:53.000000 qvsed-1.4.0/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 12:57:54.170310 qvsed-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-09 12:57:46.000000 qvsed-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:32:53.068050 qvsed-1.4.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-08 21:12:53.000000 qvsed-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-09 16:32:53.068050 qvsed-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7077 2023-07-09 16:31:54.000000 qvsed-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 16:32:53.029254 qvsed-1.4.1/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.4.1/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      477 2023-07-09 16:20:45.000000 qvsed-1.4.1/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    21540 2023-07-09 16:29:20.000000 qvsed-1.4.1/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.4.1/qvsed/qvsed.ui
+drwxrwxrwx   0        0        0        0 2023-07-09 16:32:53.066260 qvsed-1.4.1/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-09 16:32:52.000000 qvsed-1.4.1/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 16:32:53.068050 qvsed-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-09 16:32:34.000000 qvsed-1.4.1/setup.py
```

### Comparing `qvsed-1.4.0/LICENSE.txt` & `qvsed-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.0/PKG-INFO` & `qvsed-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.0
+Version: 1.4.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.0/README.md` & `qvsed-1.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 QVSED follows the philosophy of ultra-minimalism, with its heavy emphasis on just editing text and nothing more. QVSED's editing style is text-based, not file-based like basically every other editor out there. Text goes in, from a file, and then text later comes out, into another or perhaps the same file.
 
 QVSED can be used as a simple scratchpad or throwaway editor, as well as a general editing software application, since it won't prompt you if you do anything destructive, It stays out of your way on many occasions. Whether or not that's a good thing is up to you.
 
 QVSED is a PyQt5 rewrite of my older project, [ASMED (Another SMol EDitor)](https://github.com/That1M8Head/ASMED), which was written using Windows Forms, and was quite obviously only for Windows.
 
-QVSED aims to replace ASMED by offering cross-platform support and the advantages of a lightweight editor without the overhead of .NET.
+QVSED aims to replace ASMED by offering cross-platform support and the advantages of a lightweight editor without the overhead of .NET, as well as provide features that I never thought to add to ASMED because it was .NET only.
 
 ## Installing
 
 QVSED [is available on PyPI](https://pypi.org/project/QVSED/). You can install it using the following command:
 
 ```bash
 pip install --upgrade qvsed
@@ -30,38 +30,64 @@
 
 ## Usage
 
 QVSED is broken up into three parts - the Action Deck, the Text Area and the Echo Area.
 
 The Action Deck contains editing commands, the Text Area is a text area, and the Echo Area is where messages will be printed.
 
-## Action Deck
+## Keyboard Shortcuts
 
-The Action Deck, positioned on the left side of the QVSED window, containing commands to clear the Text Area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
-
-The Action Deck is on the left rather than on the top like a traditional menu bar, so that the buttons can be bigger while still providing enough screen real estate for the Text Area.
+QVSED contains a mix of bindings from the original ASMED, Vim-style bindings and Emacs-style bindings.
 
 ### Key Prefixes
 
 + `C-` - `Ctrl` (Windows, Linux), `⌘` (macOS)
 + `A-` - `Alt` (Windows, Linux), `⌥` (macOS)
 
 When you see `<C-n>`, for instance, that means pressing `Ctrl+N` on Windows/Linux, or `⌘N` on macOS.
 
+`Ctrl` being `⌘` and `Alt` being `⌥` is a Qt thing, not a QVSED thing, and there isn't much of a reason to change it.
+
 This kind of notation was inspired by Emacs (though, QVSED uses `A-` instead of `M-` to be clearer).
 
-### Commands
+### Action Deck bindings
+
+These bindings are evolutions of the original ASMED key bindings.
 
 + **Clear Text** - `<C-n>` - Clear the Text Area. Think of it like New File.
 + **Open File** - `<C-f>` - Launch a file picker and load the chosen file's contents into the Text Area.
 + **Save File** - `<C-s>` - Launch a file picker and save the contents of the Text Area to the chosen file name.
 + **Full Screen** - `<A-f>` - Toggle full screen mode.
 + **Get Help** - `<C-h>` - Show a help message in the Text Area. This will overwrite your current work.
 + **Quit QVSED**  - `<A-q>` - Quit QVSED on the spot with no confirmation dialog.
 
+### Motion bindings
+
+These bindings are for the most part inspired by Vim, if not Emacs.
+
++ `<A-h>` - Move left a character. Inspired by Vim's `h`.
++ `<A-j>` - Move down a character. Inspired by Vim's `j`.
++ `<A-k>` - Move up a character. Inspired by Vim's `k`.
++ `<A-l>` - Move right a character. Inspired by Vim's `l`.
+
++ `<A-u>` - Move up half a page. Inspired by Vim's `<C-u>`.
++ `<A-d>` - Move up half a page. Inspired by Vim's `<C-d>`.
+
++ `<A-w>` - Move forward a word. Inspired by Vim's `w`.
++ `<A-b>` - Move back a word. Inspired by Vim's `b`.
+
++ `<A-a>` - Move to the start of the line. Inspired by Emacs' `<C-a>`.
++ `<A-e>` - Move to the end of the line. Inspired by Emacs' `<C-e>`.
+
+## Action Deck
+
+The Action Deck, positioned on the left side of the QVSED window, containing commands to clear the Text Area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
+
+The Action Deck is on the left rather than on the top like a traditional menu bar, so that the buttons can be bigger while still providing enough screen real estate for the Text Area.
+
 ## Text Area
 
 The Text Area is where the actual text editing takes place.
 
 You can enter and delete text, scroll down and up, cut, copy, paste, all that standard Notepad stuff.
 
 QVSED is intentionally simplistic, and so there's not much to the Text Area.
@@ -78,28 +104,31 @@
 
 When QVSED is started, it looks for a configuration file. If it can't find one, it creates one and populates it with defaults.
 
 On Windows, the configuration file will be stored at `C:\Users\<username>\AppData\Roaming\QVSED\config.py`, where `<username>` is your Windows username.
 
 On *nix systems, the configuration file will be stored at `~/.config/QVSED/config.py`, where `~` is your home directory (`/home/<username>`).
 
-As of QVSED 1.3.0, you can customise the font and the colour scheme. For a list of sample colour schemes, [go here](COLOURS.md).
+As of QVSED 1.3.0, you can customise the colour scheme in addition to the font. For a list of sample colour schemes, [go here](COLOURS.md).
 
 ```python
 # The default QVSED config.
 
 # Font
 font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
 font_size = 11
 
 # Colours
 text_color = "#FFFFFF"
 background_color = "#282C34"
 button_color = "#393F4A"
 button_focus_color = "#31353F"
+button_pressed_color = "#282C34"
+text_area_color = "#31353F"
+echo_area_color = "#31353F"
 ```
 
 Keep in mind that `font_family` *must* be a list. If you want only one font, specify `font_family = ["My Font"]`.
 
 ## Making Shortcuts
 
 ### Windows
```

### Comparing `qvsed-1.4.0/qvsed/qvsed.py` & `qvsed-1.4.1/qvsed/qvsed.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,62 +54,70 @@
 
     def __init__(self):
         """
         Initialize the QVSED window.
         """
         super().__init__()
         self.load_ui_file()
-        self.focus_text_area()
+        self.hover_text_area()
         self.install_event_filter()
         self.set_text_area_encoding("UTF-8")
         self.set_up_text_area_handlers()
         self.set_up_action_deck()
         self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.load_config()
         self.set_up_fonts()
         if self.check_if_file_parameter():
             self.load_from_file(sys.argv[1])
 
-    def apply_style_sheet(self, text_color, background_color, button_color, button_focus_color):
+    def apply_style_sheet(self, text_color, background_color, button_color, button_hover_color, button_pressed_color, text_area_color, echo_area_color):
         """
         Generate and apply a style sheet based on the config.py file.
         """
 
         stylesheet = f"""
 QMainWindow {{
     color: {text_color};
     background: {background_color};
 }}
 
 QPlainTextEdit, QLineEdit {{
-    color: {text_color};
-    background: {button_focus_color};
     padding: 8px;
     border: none;
 }}
 
+QPlainTextEdit {{
+    color: {text_color};
+    background: {text_area_color};
+}}
+
+QLineEdit {{
+    color: {text_color};
+    background: {echo_area_color};
+}}
+
 QPushButton {{
     color: {text_color};
-    border: 2px solid {button_focus_color};
+    border: 2px solid {button_hover_color};
     background: {button_color};
     padding: 2px;
 }}
 
 QPushButton:hover {{
     color: {text_color};
-    background: {button_focus_color};
+    background: {button_hover_color};
 }}
 
 QPushButton:pressed {{
     color: {text_color};
-    background: {background_color};
+    background: {button_pressed_color};
 }}
 
 QScrollBar:vertical {{
-    background-color: {button_focus_color};
+    background-color: {button_hover_color};
     width: 16px;
     margin: 16px 0 16px 0;
 }}
 
 QScrollBar::handle:vertical {{
     background-color: {button_color};
     min-height: 20px;
@@ -225,17 +233,17 @@
         Update the Echo Area with the given message.
         """
         echo_area = self.echoArea
         echo_area.setText(message)
         echo_area.setCursorPosition(0)
         self.echo_area_timeout_clear(3000)
 
-    def focus_text_area(self):
+    def hover_text_area(self):
         """
-        Set the Text Area to have focus.
+        Set the Text Area to have hover.
         """
         text_area = self.textArea
         text_area.setFocus()
 
     def generate_config(self):
         """
         Generate the config file for QVSED.
@@ -303,22 +311,25 @@
         spec.loader.exec_module(qvsed_config)
 
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
 
         # Load the colour scheme settings from the config file
         # We use the shorter American spellings because it's standard, I guess
-        try:
-            text_color = qvsed_config.text_color
-            background_color = qvsed_config.background_color
-            button_color = qvsed_config.button_color
-            button_focus_color = qvsed_config.button_focus_color
-            self.apply_style_sheet(text_color, background_color, button_color, button_focus_color)
-        except AttributeError as error:
-            self.echo_area_update(f"Check config.py: {str(error)}")
+        text_color = getattr(qvsed_config, 'text_color', None)
+        background_color = getattr(qvsed_config, 'background_color', None)
+        button_color = getattr(qvsed_config, 'button_color', None)
+        button_hover_color = getattr(qvsed_config, 'button_hover_color', getattr(qvsed_config, 'button_focus_color', None))
+        button_pressed_color = getattr(qvsed_config, 'button_pressed_color', background_color)
+        text_area_color = getattr(qvsed_config, 'text_area_color', button_hover_color)
+        echo_area_color = getattr(qvsed_config, 'echo_area_color', button_hover_color)
+        self.apply_style_sheet(text_color, background_color, button_color, button_hover_color, button_pressed_color, text_area_color, echo_area_color)
+        if None in (text_color, background_color, button_color, button_hover_color):
+            self.echo_area_update("config.py appears to be broken, generating a new one.")
+            self.generate_config()
 
     def load_from_file(self, file_path = None):
         """
         Open a file dialog, and load the contents of a file into the Text Area.
         """
         text_area = self.textArea
 
@@ -492,15 +503,15 @@
         """
         Display the help message in the Text Area.
         """
         text_area = self.textArea
 
         help_message = """QVSED - Qt-based Volatile Small Editor
 ========================================
-QVSED is a stateless, volatile text editor with a minimalist approach, focusing solely on text editing without file metadata or prompts for potentially destructive actions.
+QVSED is a stateless, volatile text editor with a minimalist approach, hovering solely on text editing without file metadata or prompts for potentially destructive actions.
 
 This is the Text Area, where the actual editing takes place. Type anything you want into here, and edit as you please.
 Down there, at the bottom of the window, is the Echo Area, where messages and errors will be displayed.
 On the left of the QVSED window is the Action Deck, containing commands to clear the Text Area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
 
 I hope you enjoy using QVSED! I enjoyed writing it, and it's a nice little venture into my first Qt project.
```

### Comparing `qvsed-1.4.0/qvsed/qvsed.ui` & `qvsed-1.4.1/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.4.0/qvsed.egg-info/PKG-INFO` & `qvsed-1.4.1/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.4.0
+Version: 1.4.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.4.0/setup.py` & `qvsed-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.4.0',
+    version='1.4.1',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

