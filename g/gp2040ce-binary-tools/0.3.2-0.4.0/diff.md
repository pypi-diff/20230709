# Comparing `tmp/gp2040ce-binary-tools-0.3.2.tar.gz` & `tmp/gp2040ce-binary-tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2040ce-binary-tools-0.3.2.tar", last modified: Thu Jul  6 05:00:09 2023, max compression
+gzip compressed data, was "gp2040ce-binary-tools-0.4.0.tar", last modified: Sun Jul  9 16:10:35 2023, max compression
```

## Comparing `gp2040ce-binary-tools-0.3.2.tar` & `gp2040ce-binary-tools-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.605764 gp2040ce-binary-tools-0.3.2/
--rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 17:52:07.000000 gp2040ce-binary-tools-0.3.2/.gitattributes
--rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-21 04:55:18.000000 gp2040ce-binary-tools-0.3.2/.gitignore
--rw-r--r--   0 bss       (1026) bss       (1000)     1077 2023-06-20 04:25:43.000000 gp2040ce-binary-tools-0.3.2/LICENSE
--rw-r--r--   0 bss       (1026) bss       (1000)     6073 2023-07-06 05:00:09.604764 gp2040ce-binary-tools-0.3.2/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     5373 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/README.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.592764 gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/
--rw-r--r--   0 bss       (1026) bss       (1000)     6073 2023-07-06 05:00:09.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     1096 2023-07-06 05:00:09.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 bss       (1026) bss       (1000)        1 2023-07-06 05:00:09.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      174 2023-07-06 05:00:09.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/entry_points.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      271 2023-07-06 05:00:09.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/requires.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       18 2023-07-06 05:00:09.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/top_level.txt
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.593764 gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/
--rw-r--r--   0 bss       (1026) bss       (1000)     2093 2023-06-21 04:55:18.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)      160 2023-07-06 05:00:09.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/_version.py
--rw-r--r--   0 bss       (1026) bss       (1000)     5702 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)      712 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/config_tree.css
--rw-r--r--   0 bss       (1026) bss       (1000)    16333 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7082 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2286 2023-07-06 04:36:13.000000 gp2040ce-binary-tools-0.3.2/pyproject.toml
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.593764 gp2040ce-binary-tools-0.3.2/requirements/
--rw-r--r--   0 bss       (1026) bss       (1000)     3911 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/requirements/requirements-dev.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      929 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/requirements/requirements.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       38 2023-07-06 05:00:09.605764 gp2040ce-binary-tools-0.3.2/setup.cfg
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.593764 gp2040ce-binary-tools-0.3.2/tests/
--rw-r--r--   0 bss       (1026) bss       (1000)     1222 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/conftest.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.594764 gp2040ce-binary-tools-0.3.2/tests/test-files/
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.604764 gp2040ce-binary-tools-0.3.2/tests/test-files/pb2-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    22122 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/pb2-files/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7378 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/pb2-files/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2023-06-21 04:55:18.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/pb2-files/nanopb_pb2.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-06 05:00:09.604764 gp2040ce-binary-tools-0.3.2/tests/test-files/proto-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    12702 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/proto-files/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     4135 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/proto-files/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2023-06-21 04:55:18.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/proto-files/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     2046 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/test-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)   727084 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/test-firmware.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     8192 2023-06-21 04:55:18.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/test-storage-area.bin
--rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-06-21 22:14:29.000000 gp2040ce-binary-tools-0.3.2/tests/test-files/test-whole-board.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     5334 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test_builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2354 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test_commands.py
--rw-r--r--   0 bss       (1026) bss       (1000)     6687 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test_gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1321 2023-06-21 04:55:18.000000 gp2040ce-binary-tools-0.3.2/tests/test_package.py
--rw-r--r--   0 bss       (1026) bss       (1000)     5799 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tests/test_storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1604 2023-07-03 03:56:02.000000 gp2040ce-binary-tools-0.3.2/tox.ini
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/
+-rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce-binary-tools-0.4.0/.gitattributes
+-rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce-binary-tools-0.4.0/.gitignore
+-rw-r--r--   0 bss       (1026) bss       (1000)     1077 2023-06-20 17:56:42.000000 gp2040ce-binary-tools-0.4.0/LICENSE
+-rw-r--r--   0 bss       (1026) bss       (1000)     6593 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     5893 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/README.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.632900 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/
+-rw-r--r--   0 bss       (1026) bss       (1000)     6593 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     1141 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)        1 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      226 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      277 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/requires.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       18 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/top_level.txt
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.633900 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2093 2023-06-26 20:39:01.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      160 2023-07-09 16:10:35.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/_version.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     6666 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      712 2023-06-30 07:04:59.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/config_tree.css
+-rw-r--r--   0 bss       (1026) bss       (1000)    17641 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     8426 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/pico.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     8893 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2349 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/pyproject.toml
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.633900 gp2040ce-binary-tools-0.4.0/requirements/
+-rw-r--r--   0 bss       (1026) bss       (1000)     3991 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/requirements/requirements-dev.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      991 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/requirements/requirements.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       38 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/setup.cfg
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.633900 gp2040ce-binary-tools-0.4.0/tests/
+-rw-r--r--   0 bss       (1026) bss       (1000)     1222 2023-06-28 19:59:12.000000 gp2040ce-binary-tools-0.4.0/tests/conftest.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.634900 gp2040ce-binary-tools-0.4.0/tests/test-files/
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    22122 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     7378 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2023-07-01 19:13:13.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/nanopb_pb2.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2023-07-09 16:10:35.642900 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    12702 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     4135 2023-07-01 19:47:01.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2023-06-21 00:57:38.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     2046 2023-06-30 06:50:33.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)   727084 2023-06-26 19:51:10.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-firmware.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     8192 2023-07-01 21:47:58.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-storage-area.bin
+-rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-06-29 19:56:04.000000 gp2040ce-binary-tools-0.4.0/tests/test-files/test-whole-board.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     6039 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2798 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_commands.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     6687 2023-07-01 22:06:16.000000 gp2040ce-binary-tools-0.4.0/tests/test_gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1321 2023-06-21 00:57:38.000000 gp2040ce-binary-tools-0.4.0/tests/test_package.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9649 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_pico.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     6590 2023-07-09 16:07:25.000000 gp2040ce-binary-tools-0.4.0/tests/test_storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1604 2023-06-28 19:59:12.000000 gp2040ce-binary-tools-0.4.0/tox.ini
```

### Comparing `gp2040ce-binary-tools-0.3.2/.gitignore` & `gp2040ce-binary-tools-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/LICENSE` & `gp2040ce-binary-tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/PKG-INFO` & `gp2040ce-binary-tools-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.3.2
+Version: 0.4.0
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: MIT
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -24,33 +24,39 @@
 
 Interacting with your board (e.g. getting dumps, etc.) requires [picotool](https://github.com/raspberrypi/picotool), and
 currently the expectation is that you can run it yourself before invoking these tools. That may change one day.
 
 ## Installation
 
 ```
+% pip install gp2040ce-binary-tools
+```
+
+### Development Installation
+
+```
 % git clone [URL to this repository]
 % cd gp2040ce-binary-tools
 % python -m venv venv
 % source ./venv/bin/activate
 % pip install -e .
+% pip install -Ur requirements/requirements-dev.txt
 ```
 
-At some point we may publish packages to e.g. pypi.
-
-### Development Installation
+## Tools
 
-As above, plus also `pip install -Ur requirements/requirements-dev.txt` to get linters and whatnot.
+In all cases, online help can be retrieved by providing the `-h` or ``--help`` flags to the below programs.
 
-## Config Editor
+### Config Editor
 
 [![asciicast](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo.svg)](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo)
 
 A terminal UI config editor, capable of viewing and editing existing configurations, can be launched via
-**edit-config**. It supports navigation both via the keyboard or the mouse.
+`edit-config`. It supports navigation both via the keyboard or the mouse, and can view and edit either a binary file
+made via `picotool` or configuration directly on the board in BOOTSEL mode over USB.
 
 Simple usage:
 
 | Key(s)                | Action                                                 |
 |-----------------------|--------------------------------------------------------|
 | Up, Down              | Move up and down the config tree                       |
 | Left, Right           | Scroll the tree left and right (when content is long)  |
@@ -59,54 +65,61 @@
 | Tab (in edit popup)   | Cycle highlight between input field and buttons        |
 | Enter (in edit popup) | Choose dropdown option or activate button              |
 | S                     | Save the config to the opened file                     |
 | Q                     | Quit without saving                                    |
 
 A quick demonstration of the editor is available [on asciinema.org](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo).
 
-## Tools
-
-In all cases, online help can be retrieved by providing the `-h` or ``--help`` flags to the below programs.
-
 ### concatenate
 
-**concatenate** combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
+`concatenate` combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
 section .bin or config (with footer) .bin, and produces a properly-offset .bin file suitable for flashing to a board.
 This may be useful to ensure the board is flashed with a particular configuration, for instances such as producing a
 binary to flash many boards with a particular configuration (specific customizations, etc.), or keeping documented
 backups of what you're testing with during development.
 
 Sample usage:
 
 ```
 % concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin new-firmware-with-config.bin
 ```
 
+### dump-config
+
+`dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
+This could be used with the other tools, or just to keep a backup.
+
+Sample usage:
+
+```
+% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename `date +%Y%m%d`-config-backup.bin
+```
+
 ### visualize-storage
 
-**visualize-storage** reads a dump of a GP2040-CE board's flash storage section, where the configuration lives, and
-prints it out for visual inspection or diffing with other tools. It can also find the storage section from a GP2040-CE
-whole board dump, if you have that instead. Usage is simple; just pass the tool your binary file to analyze along with
-the path to the Protobuf files.
+`visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
+storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
+section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
+mode or pass the tool your binary file to analyze along with the path to the Protobuf files.
 
 Because Protobuf relies on .proto files to convey the serialized structure, you must supply them from the main GP2040-CE
 project, e.g. pointing this tool at your clone of the core project. Something like this would suffice for a working
 invocation (note: you do not need to compile the files yourself):
 
 ```
-% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto memory.bin
+% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename memory.bin
 ```
 
 (In the future we will look into publishing complete packages that include the compiled `_pb2.py` files, so that you
 don't need to provide them yourself.)
 
 Sample output:
 
 ```
-% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto ~/proj/GP2040-CE/demo-memory.bin
+% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --usb
 boardVersion: "v0.7.2"
 gamepadOptions {
   inputMode: INPUT_MODE_HID
   dpadMode: DPAD_MODE_DIGITAL
   socdMode: SOCD_MODE_SECOND_INPUT_PRIORITY
   invertXAxis: false
   invertYAxis: false
@@ -163,18 +176,21 @@
   ...[and so on]...
 }
 forcedSetupOptions {
   mode: FORCED_SETUP_MODE_OFF
 }
 ```
 
-### Dumping the GP2040-CE board
+## Miscellaneous
+
+### Dumping the GP2040-CE board with picotool
 
-These tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on the
-context. The storage section of a GP2040-CE board is a reserved 8 KB starting at `0x101FE000`. To dump your board's storage:
+Some of these tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on
+the context. The storage section of a GP2040-CE board is a reserved 8 KB starting at `0x101FE000`. To dump your board's
+storage with picotool:
 
 ```
 % picotool save -r 101FE000 10200000 memory.bin
 ```
 
 And to dump your whole board:
```

### Comparing `gp2040ce-binary-tools-0.3.2/README.md` & `gp2040ce-binary-tools-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,39 @@
 
 Interacting with your board (e.g. getting dumps, etc.) requires [picotool](https://github.com/raspberrypi/picotool), and
 currently the expectation is that you can run it yourself before invoking these tools. That may change one day.
 
 ## Installation
 
 ```
+% pip install gp2040ce-binary-tools
+```
+
+### Development Installation
+
+```
 % git clone [URL to this repository]
 % cd gp2040ce-binary-tools
 % python -m venv venv
 % source ./venv/bin/activate
 % pip install -e .
+% pip install -Ur requirements/requirements-dev.txt
 ```
 
-At some point we may publish packages to e.g. pypi.
-
-### Development Installation
+## Tools
 
-As above, plus also `pip install -Ur requirements/requirements-dev.txt` to get linters and whatnot.
+In all cases, online help can be retrieved by providing the `-h` or ``--help`` flags to the below programs.
 
-## Config Editor
+### Config Editor
 
 [![asciicast](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo.svg)](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo)
 
 A terminal UI config editor, capable of viewing and editing existing configurations, can be launched via
-**edit-config**. It supports navigation both via the keyboard or the mouse.
+`edit-config`. It supports navigation both via the keyboard or the mouse, and can view and edit either a binary file
+made via `picotool` or configuration directly on the board in BOOTSEL mode over USB.
 
 Simple usage:
 
 | Key(s)                | Action                                                 |
 |-----------------------|--------------------------------------------------------|
 | Up, Down              | Move up and down the config tree                       |
 | Left, Right           | Scroll the tree left and right (when content is long)  |
@@ -41,54 +47,61 @@
 | Tab (in edit popup)   | Cycle highlight between input field and buttons        |
 | Enter (in edit popup) | Choose dropdown option or activate button              |
 | S                     | Save the config to the opened file                     |
 | Q                     | Quit without saving                                    |
 
 A quick demonstration of the editor is available [on asciinema.org](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo).
 
-## Tools
-
-In all cases, online help can be retrieved by providing the `-h` or ``--help`` flags to the below programs.
-
 ### concatenate
 
-**concatenate** combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
+`concatenate` combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
 section .bin or config (with footer) .bin, and produces a properly-offset .bin file suitable for flashing to a board.
 This may be useful to ensure the board is flashed with a particular configuration, for instances such as producing a
 binary to flash many boards with a particular configuration (specific customizations, etc.), or keeping documented
 backups of what you're testing with during development.
 
 Sample usage:
 
 ```
 % concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin new-firmware-with-config.bin
 ```
 
+### dump-config
+
+`dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
+This could be used with the other tools, or just to keep a backup.
+
+Sample usage:
+
+```
+% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename `date +%Y%m%d`-config-backup.bin
+```
+
 ### visualize-storage
 
-**visualize-storage** reads a dump of a GP2040-CE board's flash storage section, where the configuration lives, and
-prints it out for visual inspection or diffing with other tools. It can also find the storage section from a GP2040-CE
-whole board dump, if you have that instead. Usage is simple; just pass the tool your binary file to analyze along with
-the path to the Protobuf files.
+`visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
+storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
+section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
+mode or pass the tool your binary file to analyze along with the path to the Protobuf files.
 
 Because Protobuf relies on .proto files to convey the serialized structure, you must supply them from the main GP2040-CE
 project, e.g. pointing this tool at your clone of the core project. Something like this would suffice for a working
 invocation (note: you do not need to compile the files yourself):
 
 ```
-% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto memory.bin
+% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename memory.bin
 ```
 
 (In the future we will look into publishing complete packages that include the compiled `_pb2.py` files, so that you
 don't need to provide them yourself.)
 
 Sample output:
 
 ```
-% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto ~/proj/GP2040-CE/demo-memory.bin
+% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --usb
 boardVersion: "v0.7.2"
 gamepadOptions {
   inputMode: INPUT_MODE_HID
   dpadMode: DPAD_MODE_DIGITAL
   socdMode: SOCD_MODE_SECOND_INPUT_PRIORITY
   invertXAxis: false
   invertYAxis: false
@@ -145,18 +158,21 @@
   ...[and so on]...
 }
 forcedSetupOptions {
   mode: FORCED_SETUP_MODE_OFF
 }
 ```
 
-### Dumping the GP2040-CE board
+## Miscellaneous
+
+### Dumping the GP2040-CE board with picotool
 
-These tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on the
-context. The storage section of a GP2040-CE board is a reserved 8 KB starting at `0x101FE000`. To dump your board's storage:
+Some of these tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on
+the context. The storage section of a GP2040-CE board is a reserved 8 KB starting at `0x101FE000`. To dump your board's
+storage with picotool:
 
 ```
 % picotool save -r 101FE000 10200000 memory.bin
 ```
 
 And to dump your whole board:
```

### Comparing `gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/PKG-INFO` & `gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2040ce-binary-tools
-Version: 0.3.2
+Version: 0.4.0
 Summary: Tools for working with GP2040-CE firmware and storage binaries.
 Author-email: "Brian S. Stephan" <bss@incorporeal.org>
 License: MIT
 Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
 Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
@@ -24,33 +24,39 @@
 
 Interacting with your board (e.g. getting dumps, etc.) requires [picotool](https://github.com/raspberrypi/picotool), and
 currently the expectation is that you can run it yourself before invoking these tools. That may change one day.
 
 ## Installation
 
 ```
+% pip install gp2040ce-binary-tools
+```
+
+### Development Installation
+
+```
 % git clone [URL to this repository]
 % cd gp2040ce-binary-tools
 % python -m venv venv
 % source ./venv/bin/activate
 % pip install -e .
+% pip install -Ur requirements/requirements-dev.txt
 ```
 
-At some point we may publish packages to e.g. pypi.
-
-### Development Installation
+## Tools
 
-As above, plus also `pip install -Ur requirements/requirements-dev.txt` to get linters and whatnot.
+In all cases, online help can be retrieved by providing the `-h` or ``--help`` flags to the below programs.
 
-## Config Editor
+### Config Editor
 
 [![asciicast](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo.svg)](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo)
 
 A terminal UI config editor, capable of viewing and editing existing configurations, can be launched via
-**edit-config**. It supports navigation both via the keyboard or the mouse.
+`edit-config`. It supports navigation both via the keyboard or the mouse, and can view and edit either a binary file
+made via `picotool` or configuration directly on the board in BOOTSEL mode over USB.
 
 Simple usage:
 
 | Key(s)                | Action                                                 |
 |-----------------------|--------------------------------------------------------|
 | Up, Down              | Move up and down the config tree                       |
 | Left, Right           | Scroll the tree left and right (when content is long)  |
@@ -59,54 +65,61 @@
 | Tab (in edit popup)   | Cycle highlight between input field and buttons        |
 | Enter (in edit popup) | Choose dropdown option or activate button              |
 | S                     | Save the config to the opened file                     |
 | Q                     | Quit without saving                                    |
 
 A quick demonstration of the editor is available [on asciinema.org](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo).
 
-## Tools
-
-In all cases, online help can be retrieved by providing the `-h` or ``--help`` flags to the below programs.
-
 ### concatenate
 
-**concatenate** combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
+`concatenate` combines a GP2040-CE firmware .bin file (such as from a fresh build) and a GP2040-CE board's storage
 section .bin or config (with footer) .bin, and produces a properly-offset .bin file suitable for flashing to a board.
 This may be useful to ensure the board is flashed with a particular configuration, for instances such as producing a
 binary to flash many boards with a particular configuration (specific customizations, etc.), or keeping documented
 backups of what you're testing with during development.
 
 Sample usage:
 
 ```
 % concatenate build/GP2040-CE_foo_bar.bin storage-dump.bin new-firmware-with-config.bin
 ```
 
+### dump-config
+
+`dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
+This could be used with the other tools, or just to keep a backup.
+
+Sample usage:
+
+```
+% dump-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename `date +%Y%m%d`-config-backup.bin
+```
+
 ### visualize-storage
 
-**visualize-storage** reads a dump of a GP2040-CE board's flash storage section, where the configuration lives, and
-prints it out for visual inspection or diffing with other tools. It can also find the storage section from a GP2040-CE
-whole board dump, if you have that instead. Usage is simple; just pass the tool your binary file to analyze along with
-the path to the Protobuf files.
+`visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
+storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
+section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
+mode or pass the tool your binary file to analyze along with the path to the Protobuf files.
 
 Because Protobuf relies on .proto files to convey the serialized structure, you must supply them from the main GP2040-CE
 project, e.g. pointing this tool at your clone of the core project. Something like this would suffice for a working
 invocation (note: you do not need to compile the files yourself):
 
 ```
-% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto memory.bin
+% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename memory.bin
 ```
 
 (In the future we will look into publishing complete packages that include the compiled `_pb2.py` files, so that you
 don't need to provide them yourself.)
 
 Sample output:
 
 ```
-% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto ~/proj/GP2040-CE/demo-memory.bin
+% visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --usb
 boardVersion: "v0.7.2"
 gamepadOptions {
   inputMode: INPUT_MODE_HID
   dpadMode: DPAD_MODE_DIGITAL
   socdMode: SOCD_MODE_SECOND_INPUT_PRIORITY
   invertXAxis: false
   invertYAxis: false
@@ -163,18 +176,21 @@
   ...[and so on]...
 }
 forcedSetupOptions {
   mode: FORCED_SETUP_MODE_OFF
 }
 ```
 
-### Dumping the GP2040-CE board
+## Miscellaneous
+
+### Dumping the GP2040-CE board with picotool
 
-These tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on the
-context. The storage section of a GP2040-CE board is a reserved 8 KB starting at `0x101FE000`. To dump your board's storage:
+Some of these tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on
+the context. The storage section of a GP2040-CE board is a reserved 8 KB starting at `0x101FE000`. To dump your board's
+storage with picotool:
 
 ```
 % picotool save -r 101FE000 10200000 memory.bin
 ```
 
 And to dump your whole board:
```

### Comparing `gp2040ce-binary-tools-0.3.2/gp2040ce_binary_tools.egg-info/SOURCES.txt` & `gp2040ce-binary-tools-0.4.0/gp2040ce_binary_tools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 gp2040ce_binary_tools.egg-info/requires.txt
 gp2040ce_binary_tools.egg-info/top_level.txt
 gp2040ce_bintools/__init__.py
 gp2040ce_bintools/_version.py
 gp2040ce_bintools/builder.py
 gp2040ce_bintools/config_tree.css
 gp2040ce_bintools/gui.py
+gp2040ce_bintools/pico.py
 gp2040ce_bintools/storage.py
 requirements/requirements-dev.txt
 requirements/requirements.txt
 tests/conftest.py
 tests/test_builder.py
 tests/test_commands.py
 tests/test_gui.py
 tests/test_package.py
+tests/test_pico.py
 tests/test_storage.py
 tests/test-files/test-config.bin
 tests/test-files/test-firmware.bin
 tests/test-files/test-storage-area.bin
 tests/test-files/test-whole-board.bin
 tests/test-files/pb2-files/config_pb2.py
 tests/test-files/pb2-files/enums_pb2.py
```

### Comparing `gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/__init__.py` & `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/builder.py` & `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import argparse
 import copy
 import logging
 
 from google.protobuf.message import Message
 
 from gp2040ce_bintools import core_parser
-from gp2040ce_bintools.storage import (STORAGE_LOCATION, STORAGE_SIZE, pad_config_to_storage_size,
-                                       serialize_config_with_footer)
+from gp2040ce_bintools.pico import write
+from gp2040ce_bintools.storage import (STORAGE_BINARY_LOCATION, STORAGE_MEMORY_ADDRESS, STORAGE_SIZE,
+                                       pad_config_to_storage_size, serialize_config_with_footer)
 
 logger = logging.getLogger(__name__)
 
 
 #################
 # LIBRARY ITEMS #
 #################
@@ -53,19 +54,19 @@
     Args:
         firmware: the firmware binary to process
     Returns:
         the resulting padded binary as a bytearray
     Raises:
         FirmwareLengthError: if the firmware is larger than the storage location
     """
-    bytes_to_pad = STORAGE_LOCATION - len(firmware)
+    bytes_to_pad = STORAGE_BINARY_LOCATION - len(firmware)
     logger.debug("firmware is length %s, padding %s bytes", len(firmware), bytes_to_pad)
     if bytes_to_pad < 0:
         raise FirmwareLengthError(f"provided firmware binary is larger than the start of "
-                                  f"storage at {STORAGE_LOCATION}!")
+                                  f"storage at {STORAGE_BINARY_LOCATION}!")
 
     return bytearray(firmware) + bytearray(b'\x00' * bytes_to_pad)
 
 
 def replace_config_in_binary(board_binary: bytearray, config_binary: bytearray) -> bytearray:
     """Given (presumed) whole board and config binaries, combine the two to one, with proper offsets for GP2040-CE.
 
@@ -75,20 +76,21 @@
 
     Args:
         board_binary: binary data of a whole board dump from a GP2040-CE board
         config_binary: binary data of board config + footer, possibly padded to be a full storage section
     Returns:
         the resulting correctly-offset binary suitable for a GP2040-CE board
     """
-    if len(board_binary) < STORAGE_LOCATION + STORAGE_SIZE:
+    if len(board_binary) < STORAGE_BINARY_LOCATION + STORAGE_SIZE:
         # this is functionally the same, since this doesn't sanity check the firmware
         return combine_firmware_and_config(board_binary, config_binary)
     else:
         new_binary = bytearray(copy.copy(board_binary))
-        new_binary[STORAGE_LOCATION:(STORAGE_LOCATION + STORAGE_SIZE)] = pad_config_to_storage_size(config_binary)
+        new_config = pad_config_to_storage_size(config_binary)
+        new_binary[STORAGE_BINARY_LOCATION:(STORAGE_BINARY_LOCATION + STORAGE_SIZE)] = new_config
         return new_binary
 
 
 def write_new_config_to_filename(config: Message, filename: str, inject: bool = False) -> None:
     """Serialize the provided config to the specified file.
 
     The file may be replaced, creating a configuration section-only binary, or appended to
@@ -108,18 +110,35 @@
     else:
         binary = serialize_config_with_footer(config)
 
     with open(filename, 'wb') as file:
         file.write(binary)
 
 
+def write_new_config_to_usb(config: Message, endpoint_out: object, endpoint_in: object):
+    """Serialize the provided config to a device over USB, in the proper location for a GP2040-CE board.
+
+    Args:
+        config: the Protobuf configuration to write to a Pico board in BOOTSEL mode
+        endpoint_out: the USB endpoint to write to
+        endpoint_in: the USB endpoint to read from
+    """
+    serialized = serialize_config_with_footer(config)
+    # we don't write the whole area, just the minimum from the end of the storage section
+    # nevertheless, the USB device needs writes to start at 256 byte boundaries
+    padding = 256 - (len(serialized) % 256)
+    binary = bytearray(b'\x00' * padding) + serialized
+    write(endpoint_out, endpoint_in, STORAGE_MEMORY_ADDRESS + (STORAGE_SIZE - len(binary)), binary)
+
+
 ############
 # COMMANDS #
 ############
 
+
 def concatenate():
     """Combine a built firmware .bin and a storage .bin."""
     parser = argparse.ArgumentParser(
         description="Combine a compiled GP2040-CE firmware-only .bin and an existing storage area or config .bin "
                     "into one file suitable for flashing onto a board.",
         parents=[core_parser],
     )
```

### Comparing `gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/config_tree.css` & `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/config_tree.css`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/gui.py` & `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from textual.logging import TextualHandler
 from textual.screen import ModalScreen
 from textual.validation import Number
 from textual.widgets import Button, Footer, Header, Input, Label, Pretty, Select, Tree
 from textual.widgets.tree import TreeNode
 
 from gp2040ce_bintools import core_parser, handler
-from gp2040ce_bintools.builder import write_new_config_to_filename
-from gp2040ce_bintools.storage import get_config_from_file
+from gp2040ce_bintools.builder import write_new_config_to_filename, write_new_config_to_usb
+from gp2040ce_bintools.storage import get_config_from_file, get_config_from_usb
 
 logger = logging.getLogger(__name__)
 
 
 class EditScreen(ModalScreen):
     """Do an input prompt by way of an overlaid screen."""
 
@@ -126,16 +126,26 @@
         ('q', 'quit', "Quit"),
     ]
     CSS_PATH = "config_tree.css"
     TITLE = "GP2040-CE Configuration Editor"
 
     def __init__(self, *args, **kwargs):
         """Initialize config."""
-        self.config_filename = kwargs.pop('config_filename')
+        self.config_filename = kwargs.pop('config_filename', None)
         self.whole_board = kwargs.pop('whole_board', False)
+        self.usb = kwargs.pop('usb', False)
+        # load the config
+        if self.usb:
+            self.config, self.endpoint_out, self.endpoint_in = get_config_from_usb()
+            self.source_name = (f"DEVICE ID {hex(self.endpoint_out.device.idVendor)}:"
+                                f"{hex(self.endpoint_out.device.idProduct)} "
+                                f"on bus {self.endpoint_out.device.bus} address {self.endpoint_out.device.address}")
+        else:
+            self.config = get_config_from_file(self.config_filename, whole_board=self.whole_board)
+            self.source_name = self.config_filename
         super().__init__(*args, **kwargs)
 
         # disable normal logging and enable console logging if we're not headless
         logger.debug("reconfiguring logging...")
         root = logging.getLogger()
         root.setLevel(logging.DEBUG)
         root.removeHandler(handler)
@@ -145,19 +155,18 @@
         """Compose the UI."""
         yield Header()
         yield Footer()
         yield Tree("Root")
 
     def on_mount(self) -> None:
         """Load the configuration object into the tree view."""
-        self.config = get_config_from_file(self.config_filename, whole_board=self.whole_board)
         tree = self.query_one(Tree)
 
         tree.root.data = (None, self.config.DESCRIPTOR, self.config)
-        tree.root.set_label(self.config_filename)
+        tree.root.set_label(self.source_name)
         missing_fields = [f for f in self.config.DESCRIPTOR.fields
                           if f not in [fp for fp, vp in self.config.ListFields()]]
         for field_descriptor, field_value in sorted(self.config.ListFields(), key=lambda f: f[0].name):
             child_is_message = ConfigEditor._descriptor_is_message(field_descriptor)
             ConfigEditor._add_node(tree.root, self.config, field_descriptor, field_value,
                                    value_is_config=child_is_message)
         for child_field_descriptor in sorted(missing_fields, key=lambda f: f.name):
@@ -196,16 +205,22 @@
             logger.debug("adding new node %s", field_value.DESCRIPTOR.name)
             ConfigEditor._add_node(current_node, config, actual_field_descriptor, field_value,
                                    value_is_config=True)
             current_node.expand()
 
     def action_save(self) -> None:
         """Save the configuration."""
-        write_new_config_to_filename(self.config, self.config_filename, inject=self.whole_board)
-        self.push_screen(MessageScreen(f"Configuration saved to {self.config_filename}."))
+        if self.usb:
+            write_new_config_to_usb(self.config, self.endpoint_out, self.endpoint_in)
+            self.push_screen(MessageScreen(f"Configuration saved to "
+                                           f"{hex(self.endpoint_out.device.idVendor)}:"
+                                           f"{hex(self.endpoint_out.device.idProduct)}."))
+        elif self.config_filename:
+            write_new_config_to_filename(self.config, self.config_filename, inject=self.whole_board)
+            self.push_screen(MessageScreen(f"Configuration saved to {self.config_filename}."))
 
     def action_quit(self) -> None:
         """Quit the application."""
         self.exit()
 
     @staticmethod
     def _add_node(parent_node: TreeNode, parent_config: Message,
@@ -335,13 +350,20 @@
 
 def edit_config():
     """Edit the configuration in an interactive fashion."""
     parser = argparse.ArgumentParser(
         description="Utilize a GUI to view and alter the contents of a GP2040-CE configuration.",
         parents=[core_parser],
     )
+    group = parser.add_mutually_exclusive_group(required=True)
+    group.add_argument('--usb', action='store_true', help="retrieve the config from a Pico board connected over USB "
+                                                          "and in BOOTSEL mode")
+    group.add_argument('--filename', help=".bin file of a GP2040-CE board's config + footer or entire storage section, "
+                                          "or of a GP2040-CE's whole board dump if --whole-board is specified")
     parser.add_argument('--whole-board', action='store_true', help="indicate the binary file is a whole board dump")
-    parser.add_argument('filename', help=".bin file of a GP2040-CE board's config + footer or entire storage section, "
-                                         "or of a GP2040-CE's whole board dump if --whole-board is specified")
     args, _ = parser.parse_known_args()
-    app = ConfigEditor(config_filename=args.filename, whole_board=args.whole_board)
+
+    if args.usb:
+        app = ConfigEditor(usb=True)
+    else:
+        app = ConfigEditor(config_filename=args.filename, whole_board=args.whole_board)
     app.run()
```

### Comparing `gp2040ce-binary-tools-0.3.2/gp2040ce_bintools/storage.py` & `gp2040ce-binary-tools-0.4.0/gp2040ce_bintools/storage.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import binascii
 import logging
 
 from google.protobuf.json_format import MessageToJson
 from google.protobuf.message import Message
 
 from gp2040ce_bintools import core_parser, get_config_pb2
+from gp2040ce_bintools.pico import get_bootsel_endpoints, read
 
 logger = logging.getLogger(__name__)
 
-STORAGE_LOCATION = 0x1FE000
+STORAGE_BINARY_LOCATION = 0x1FE000
+STORAGE_MEMORY_ADDRESS = 0x101FE000
 STORAGE_SIZE = 8192
 
 FOOTER_SIZE = 12
 FOOTER_MAGIC = b'\x65\xe3\xf1\xd2'
 
 
 #################
@@ -110,31 +112,46 @@
 
     if whole_board:
         return get_config(get_storage_section(content))
     else:
         return get_config(content)
 
 
+def get_config_from_usb() -> tuple[Message, object, object]:
+    """Read the config section from a USB device and get back its config section.
+
+    Returns:
+        the parsed configuration, along with the USB out and in endpoints for reference
+    """
+    # open the USB device and get the config
+    endpoint_out, endpoint_in = get_bootsel_endpoints()
+    logger.debug("reading DEVICE ID %s:%s, bus %s, address %s", hex(endpoint_out.device.idVendor),
+                 hex(endpoint_out.device.idProduct), endpoint_out.device.bus, endpoint_out.device.address)
+    storage = read(endpoint_out, endpoint_in, STORAGE_MEMORY_ADDRESS, STORAGE_SIZE)
+    return get_config(bytes(storage)), endpoint_out, endpoint_in
+
+
 def get_storage_section(content: bytes) -> bytes:
     """Pull out what should be the GP2040-CE storage section from a whole board dump.
 
     Args:
         content: bytes of a GP2040-CE whole board dump
     Returns:
         the presumed storage section from the binary
     Raises:
         ConfigLengthError: if the provided bytes don't appear to have a storage section
     """
     # a whole board must be at least as big as the known fences
     logger.debug("length of content to look for storage in: %s", len(content))
-    if len(content) < STORAGE_LOCATION + STORAGE_SIZE:
+    if len(content) < STORAGE_BINARY_LOCATION + STORAGE_SIZE:
         raise ConfigLengthError("provided content is not large enough to have a storage section!")
 
-    logger.debug("returning bytes from %s to %s", hex(STORAGE_LOCATION), hex(STORAGE_LOCATION + STORAGE_SIZE))
-    return content[STORAGE_LOCATION:(STORAGE_LOCATION + STORAGE_SIZE)]
+    logger.debug("returning bytes from %s to %s", hex(STORAGE_BINARY_LOCATION),
+                 hex(STORAGE_BINARY_LOCATION + STORAGE_SIZE))
+    return content[STORAGE_BINARY_LOCATION:(STORAGE_BINARY_LOCATION + STORAGE_SIZE)]
 
 
 def pad_config_to_storage_size(config: bytes) -> bytearray:
     """Provide a copy of the config (with footer) padded with zero bytes to be the proper storage section size.
 
     Args:
         firmware: the config section binary to process
@@ -163,24 +180,46 @@
 
 
 ############
 # COMMANDS #
 ############
 
 
+def dump_config():
+    """Save the GP2040-CE's configuration to a binary file."""
+    parser = argparse.ArgumentParser(
+        description="Read the configuration section from a USB device and save it to a binary file.",
+        parents=[core_parser],
+    )
+    parser.add_argument('--filename', help=".bin file to save the GP2040-CE board's config section to")
+    args, _ = parser.parse_known_args()
+    config, _, _ = get_config_from_usb()
+    with open(args.filename, 'wb') as out_file:
+        out_file.write(serialize_config_with_footer(config))
+
+
 def visualize():
     """Print the contents of GP2040-CE's storage."""
     parser = argparse.ArgumentParser(
         description="Read the configuration section from a dump of a GP2040-CE board's storage section and print out "
                     "its contents.",
         parents=[core_parser],
     )
+    group = parser.add_mutually_exclusive_group(required=True)
+    group.add_argument('--usb', action='store_true', help="retrieve the config from a Pico board connected over USB "
+                                                          "and in BOOTSEL mode")
+    group.add_argument('--filename', help=".bin file of a GP2040-CE board's storage section, bytes "
+                                          "101FE000-10200000, or of a GP2040-CE's whole board dump "
+                                          "if --whole-board is specified")
     parser.add_argument('--whole-board', action='store_true', help="indicate the binary file is a whole board dump")
     parser.add_argument('--json', action='store_true', help="print the config out as a JSON document")
-    parser.add_argument('filename', help=".bin file of a GP2040-CE board's storage section, bytes 101FE000-10200000, "
-                                         "or of a GP2040-CE's whole board dump if --whole-board is specified")
     args, _ = parser.parse_known_args()
-    config = get_config_from_file(args.filename, whole_board=args.whole_board)
+
+    if args.usb:
+        config, _, _ = get_config_from_usb()
+    else:
+        config = get_config_from_file(args.filename, whole_board=args.whole_board)
+
     if args.json:
         print(MessageToJson(config))
     else:
         print(config)
```

### Comparing `gp2040ce-binary-tools-0.3.2/pyproject.toml` & `gp2040ce-binary-tools-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "Tools for working with GP2040-CE firmware and storage binaries."
 readme = "README.md"
 license = {text = "MIT"}
 authors = [
     {name = "Brian S. Stephan", email = "bss@incorporeal.org"},
 ]
 requires-python = ">=3.9"
-dependencies = ["grpcio-tools", "textual"]
+dependencies = ["grpcio-tools", "pyusb", "textual"]
 dynamic = ["version"]
 classifiers = [
     "Environment :: Console",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
@@ -30,14 +30,15 @@
 dev = ["bandit", "decorator", "flake8", "flake8-blind-except", "flake8-builtins", "flake8-docstrings",
        "flake8-executable", "flake8-fixme", "flake8-isort", "flake8-logging-format", "flake8-mutable",
        "flake8-pyproject", "mypy", "pip-tools", "pytest", "pytest-asyncio", "pytest-cov", "setuptools-scm",
        "tox"]
 
 [project.scripts]
 concatenate = "gp2040ce_bintools.builder:concatenate"
+dump-config = "gp2040ce_bintools.storage:dump_config"
 edit-config = "gp2040ce_bintools.gui:edit_config"
 visualize-storage = "gp2040ce_bintools.storage:visualize"
 
 [tool.flake8]
 enable-extensions = "G,M"
 exclude = [".tox/", "venv/", "_version.py", "tests/test-files/"]
 extend-ignore = "T101"
```

### Comparing `gp2040ce-binary-tools-0.3.2/requirements/requirements-dev.txt` & `gp2040ce-binary-tools-0.4.0/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # via tox
 coverage[toml]==7.2.7
     # via pytest-cov
 decorator==5.1.1
     # via gp2040ce-binary-tools (pyproject.toml)
 distlib==0.3.6
     # via virtualenv
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via
@@ -67,15 +67,15 @@
     # via textual
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via flake8-isort
 linkify-it-py==2.0.2
     # via markdown-it-py
-markdown-it-py[linkify,plugins]==2.2.0
+markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 mccabe==0.7.0
     # via flake8
 mdit-py-plugins==0.4.0
@@ -91,15 +91,15 @@
     #   build
     #   pyproject-api
     #   pytest
     #   setuptools-scm
     #   tox
 pbr==5.11.1
     # via stevedore
-pip-tools==6.13.0
+pip-tools==6.14.0
     # via gp2040ce-binary-tools (pyproject.toml)
 platformdirs==3.8.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.2.0
     # via
@@ -124,44 +124,47 @@
     #   gp2040ce-binary-tools (pyproject.toml)
     #   pytest-asyncio
     #   pytest-cov
 pytest-asyncio==0.21.0
     # via gp2040ce-binary-tools (pyproject.toml)
 pytest-cov==4.1.0
     # via gp2040ce-binary-tools (pyproject.toml)
+pyusb==1.2.1
+    # via gp2040ce-binary-tools (pyproject.toml)
 pyyaml==6.0
     # via bandit
 rich==13.4.2
     # via
     #   bandit
     #   textual
 setuptools-scm==7.1.0
     # via gp2040ce-binary-tools (pyproject.toml)
 smmap==5.0.0
     # via gitdb
 snowballstemmer==2.2.0
     # via pydocstyle
 stevedore==5.1.0
     # via bandit
-textual==0.28.1
+textual==0.29.0
     # via gp2040ce-binary-tools (pyproject.toml)
 tomli==2.0.1
     # via
     #   build
     #   coverage
     #   flake8-pyproject
     #   mypy
+    #   pip-tools
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   setuptools-scm
     #   tox
 tox==4.6.3
     # via gp2040ce-binary-tools (pyproject.toml)
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   mypy
     #   setuptools-scm
     #   textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 virtualenv==20.23.1
```

### Comparing `gp2040ce-binary-tools-0.3.2/requirements/requirements.txt` & `gp2040ce-binary-tools-0.4.0/requirements/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,34 @@
     # via grpcio-tools
 grpcio-tools==1.56.0
     # via gp2040ce-binary-tools (pyproject.toml)
 importlib-metadata==6.7.0
     # via textual
 linkify-it-py==2.0.2
     # via markdown-it-py
-markdown-it-py[linkify,plugins]==2.2.0
+markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
 mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 protobuf==4.23.3
     # via grpcio-tools
 pygments==2.15.1
     # via rich
+pyusb==1.2.1
+    # via gp2040ce-binary-tools (pyproject.toml)
 rich==13.4.2
     # via textual
-textual==0.28.1
+textual==0.29.0
     # via gp2040ce-binary-tools (pyproject.toml)
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via textual
 uc-micro-py==1.0.2
     # via linkify-it-py
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `gp2040ce-binary-tools-0.3.2/tests/conftest.py` & `gp2040ce-binary-tools-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/pb2-files/config_pb2.py` & `gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/pb2-files/enums_pb2.py` & `gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/pb2-files/nanopb_pb2.py` & `gp2040ce-binary-tools-0.4.0/tests/test-files/pb2-files/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/proto-files/config.proto` & `gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/proto-files/enums.proto` & `gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/proto-files/nanopb.proto` & `gp2040ce-binary-tools-0.4.0/tests/test-files/proto-files/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/test-config.bin` & `gp2040ce-binary-tools-0.4.0/tests/test-files/test-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/test-firmware.bin` & `gp2040ce-binary-tools-0.4.0/tests/test-files/test-firmware.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/test-storage-area.bin` & `gp2040ce-binary-tools-0.4.0/tests/test-files/test-storage-area.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test-files/test-whole-board.bin` & `gp2040ce-binary-tools-0.4.0/tests/test-files/test-whole-board.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test_builder.py` & `gp2040ce-binary-tools-0.4.0/tests/test_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Tests for the image builder module."""
 import os
 import sys
+import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
 from gp2040ce_bintools import get_config_pb2
 from gp2040ce_bintools.builder import (FirmwareLengthError, combine_firmware_and_config, pad_firmware_up_to_storage,
-                                       replace_config_in_binary, write_new_config_to_filename)
-from gp2040ce_bintools.storage import get_config, get_config_footer, get_storage_section
+                                       replace_config_in_binary, write_new_config_to_filename, write_new_config_to_usb)
+from gp2040ce_bintools.storage import get_config, get_config_footer, get_storage_section, serialize_config_with_footer
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 @decorator
 def with_pb2s(test, *args, **kwargs):
     """Wrap a test with precompiled pb2 files on the path."""
@@ -130,7 +131,22 @@
     # read new file
     with open(tmp_file, 'rb') as file:
         config_dump = file.read()
     config = get_config(config_dump)
     config_size, _, _ = get_config_footer(config_dump)
     assert config.boardVersion == 'v0.7.2-COOL'
     assert len(config_dump) == config_size + 12
+
+
+@with_pb2s
+def test_write_new_config_to_usb(config_binary):
+    """Test that the config can be written to USB at the proper alignment."""
+    config = get_config(config_binary)
+    serialized = serialize_config_with_footer(config)
+    end_out, end_in = mock.MagicMock(), mock.MagicMock()
+    with mock.patch('gp2040ce_bintools.builder.write') as mock_write:
+        write_new_config_to_usb(config, end_out, end_in)
+
+    # check that it got padded
+    padded_serialized = bytearray(b'\x00' * 4) + serialized
+    assert mock_write.call_args.args[2] % 256 == 0
+    assert mock_write.call_args.args[3] == padded_serialized
```

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test_commands.py` & `gp2040ce-binary-tools-0.4.0/tests/test_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 """Test our tools themselves to make sure they adhere to certain flags."""
 import json
 import os
+import sys
 from subprocess import run
 
+from decorator import decorator
+
 from gp2040ce_bintools import __version__
 
+HERE = os.path.dirname(os.path.abspath(__file__))
+
+
+@decorator
+def with_pb2s(test, *args, **kwargs):
+    """Wrap a test with precompiled pb2 files on the path."""
+    proto_path = os.path.join(HERE, 'test-files', 'pb2-files')
+    sys.path.append(proto_path)
+
+    test(*args, **kwargs)
+
+    sys.path.pop()
+    del sys.modules['config_pb2']
+
 
 def test_version_flag():
     """Test that tools report the version."""
     result = run(['visualize-storage', '-v'], capture_output=True, encoding='utf8')
     assert __version__ in result.stdout
 
 
@@ -28,28 +45,29 @@
         out = out_file.read()
         storage = storage_file.read()
     assert out[2088960:2097152] == storage
 
 
 def test_storage_dump_invocation():
     """Test that a normal invocation against a dump works."""
-    result = run(['visualize-storage', '-P', 'tests/test-files/proto-files', 'tests/test-files/test-storage-area.bin'],
+    result = run(['visualize-storage', '-P', 'tests/test-files/proto-files',
+                  '--filename', 'tests/test-files/test-storage-area.bin'],
                  capture_output=True, encoding='utf8')
     assert 'boardVersion: "v0.7.2"' in result.stdout
 
 
 def test_debug_storage_dump_invocation():
     """Test that a normal invocation against a dump works."""
     result = run(['visualize-storage', '-d', '-P', 'tests/test-files/proto-files',
-                  'tests/test-files/test-storage-area.bin'],
+                  '--filename', 'tests/test-files/test-storage-area.bin'],
                  capture_output=True, encoding='utf8')
     assert 'boardVersion: "v0.7.2"' in result.stdout
     assert 'length of content to look for footer in: 8192' in result.stderr
 
 
 def test_storage_dump_json_invocation():
     """Test that a normal invocation against a dump works."""
     result = run(['visualize-storage', '-P', 'tests/test-files/proto-files', '--json',
-                  'tests/test-files/test-storage-area.bin'],
+                  '--filename', 'tests/test-files/test-storage-area.bin'],
                  capture_output=True, encoding='utf8')
     to_dict = json.loads(result.stdout)
     assert to_dict['boardVersion'] == 'v0.7.2'
```

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test_gui.py` & `gp2040ce-binary-tools-0.4.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test_package.py` & `gp2040ce-binary-tools-0.4.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.3.2/tests/test_storage.py` & `gp2040ce-binary-tools-0.4.0/tests/test_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Unit tests for the storage module."""
 import os
 import sys
+import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
 import gp2040ce_bintools.storage as storage
 
 HERE = os.path.dirname(os.path.abspath(__file__))
@@ -146,7 +147,25 @@
     assert len(storage_section) == 8192
 
 
 def test_pad_config_to_storage_raises(config_binary):
     """Test that we raise an exception if the config is bigger than the storage section."""
     with pytest.raises(storage.ConfigLengthError):
         _ = storage.pad_config_to_storage_size(config_binary * 5)
+
+
+@with_pb2s
+def test_get_config_from_usb(config_binary):
+    """Test we attempt to read from the proper location over USB."""
+    mock_out = mock.MagicMock()
+    mock_out.device.idVendor = 0xbeef
+    mock_out.device.idProduct = 0xcafe
+    mock_out.device.bus = 1
+    mock_out.device.address = 2
+    mock_in = mock.MagicMock()
+    with mock.patch('gp2040ce_bintools.storage.get_bootsel_endpoints', return_value=(mock_out, mock_in)) as mock_get:
+        with mock.patch('gp2040ce_bintools.storage.read', return_value=config_binary) as mock_read:
+            config, _, _ = storage.get_config_from_usb()
+
+    mock_get.assert_called_once()
+    mock_read.assert_called_with(mock_out, mock_in, 0x101FE000, 8192)
+    assert config == storage.get_config(config_binary)
```

### Comparing `gp2040ce-binary-tools-0.3.2/tox.ini` & `gp2040ce-binary-tools-0.4.0/tox.ini`

 * *Files identical despite different names*

