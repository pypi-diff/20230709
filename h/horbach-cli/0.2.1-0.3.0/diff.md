# Comparing `tmp/horbach_cli-0.2.1.tar.gz` & `tmp/horbach_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horbach_cli-0.2.1.tar", max compression
+gzip compressed data, was "horbach_cli-0.3.0.tar", max compression
```

## Comparing `horbach_cli-0.2.1.tar` & `horbach_cli-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      129 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/README.md
--rw-r--r--   0        0        0     2047 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/README.md
--rw-r--r--   0        0        0       22 2023-07-05 08:24:52.491243 horbach_cli-0.2.1/horbach_cli/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/converter.py
--rw-r--r--   0        0        0      998 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/deduplicator.py
--rw-r--r--   0        0        0        0 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/libs/__init__.py
--rw-r--r--   0        0        0      309 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/libs/common.py
--rw-r--r--   0        0        0      687 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/libs/converter.py
--rw-r--r--   0        0        0     1295 2023-07-05 08:24:51.683225 horbach_cli-0.2.1/horbach_cli/main.py
--rw-r--r--   0        0        0      919 2023-07-05 08:24:52.499243 horbach_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 horbach_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      129 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/README.md
+-rw-r--r--   0        0        0     2354 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/README.md
+-rw-r--r--   0        0        0       70 2023-07-08 23:24:37.020210 horbach_cli-0.3.0/horbach_cli/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/converter.py
+-rw-r--r--   0        0        0      998 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/deduplicator.py
+-rw-r--r--   0        0        0        0 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/libs/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/libs/common.py
+-rw-r--r--   0        0        0      618 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/libs/common_xsh.xsh
+-rw-r--r--   0        0        0      687 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/libs/converter.py
+-rw-r--r--   0        0        0     1434 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/main.py
+-rw-r--r--   0        0        0     3434 2023-07-08 23:24:36.216156 horbach_cli-0.3.0/horbach_cli/warp.xsh
+-rw-r--r--   0        0        0      968 2023-07-08 23:24:37.032211 horbach_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 horbach_cli-0.3.0/PKG-INFO
```

### Comparing `horbach_cli-0.2.1/horbach_cli/README.md` & `horbach_cli-0.3.0/horbach_cli/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ```console
 $ h-cli [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `-v, --verbose TEXT`: :mag: `LOG_LEVEL` one of: DEBUG, INFO, WARNING, ERROR, CRITICAL  [default: INFO]
+* `--version`
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `converter`: :rocket: manipulates files and etc.
@@ -32,14 +33,15 @@
 
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `heic-to-jpg`: :camera: images from :green_apple: heic to...
 * `img-to-pdf`: :camera: images into :memo: pdf
+* `pdf-merge`: :camera: merge pdfs
 
 ### `h-cli converter heic-to-jpg`
 
 :camera: images from :green_apple: heic to jpg
 
 **Usage**:
 
@@ -70,14 +72,32 @@
 * `IMAGES_FOLDER`: Path to folder with images  [required]
 * `[PDF_FILE]`: Result file name  [default: result.pdf]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
+### `h-cli converter pdf-merge`
+
+:camera: merge pdfs
+
+**Usage**:
+
+```console
+$ h-cli converter pdf-merge [OPTIONS] PDFS_FOLDER
+```
+
+**Arguments**:
+
+* `PDFS_FOLDER`: Path to folder with pdfs  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
 ## `h-cli dedub`
 
 :two_men_holding_hands: dedublicates something.
 
 **Usage**:
 
 ```console
```

### Comparing `horbach_cli-0.2.1/horbach_cli/converter.py` & `horbach_cli-0.3.0/horbach_cli/converter.py`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.2.1/horbach_cli/deduplicator.py` & `horbach_cli-0.3.0/horbach_cli/deduplicator.py`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.2.1/horbach_cli/libs/converter.py` & `horbach_cli-0.3.0/horbach_cli/libs/converter.py`

 * *Files identical despite different names*

### Comparing `horbach_cli-0.2.1/horbach_cli/main.py` & `horbach_cli-0.3.0/horbach_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from rich.logging import RichHandler
 from rich import print
 import typer
 
 from horbach_cli import __version__
 from horbach_cli.libs.common import log_lvl_callback, LOG_LVL
-from horbach_cli import converter, deduplicator
+from horbach_cli import converter, deduplicator, warp
 
 app = typer.Typer(rich_markup_mode="markdown")
 
 
 def version_callback(value: bool):
     version = __version__
     if value:
@@ -47,9 +47,17 @@
 app.add_typer(
     deduplicator.app,
     name="dedub",
     help=":two_men_holding_hands: dedublicates something.",
     rich_help_panel="Hacks",
 )
 
+app.add_typer(
+    warp.app,
+    name="warp",
+    help=":computer: warp.dev workflows replacement",
+    rich_help_panel="Hacks",
+)
+
+
 if __name__ == "__main__":
     app(prog_name="h-cli")
```

### Comparing `horbach_cli-0.2.1/pyproject.toml` & `horbach_cli-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "horbach-cli"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["Andrew Horbach <andrewhorbach@gmail.com>"]
 readme = "README.md"
 packages = [{include = "horbach_cli"}]
 
 [tool.poetry.scripts]
 h-cli = "horbach_cli.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 pillow = "^9.5.0"
 difpy = "^3.0.10"
 typer = {extras = ["all"], version = "^0.7.0"}
 pymupdf = "^1.22.5"
+xonsh = {extras = ["full"], version = "^0.14.0"}
 
 [tool.poetry.group.dev.dependencies]
 typer-cli = "^0.0.13"
 python-semantic-release = "^7.33.2"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 yamllint = "^1.30.0"
```

### Comparing `horbach_cli-0.2.1/PKG-INFO` & `horbach_cli-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: horbach-cli
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: Andrew Horbach
 Author-email: andrewhorbach@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: difpy (>=3.0.10,<4.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pymupdf (>=1.22.5,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: xonsh[full] (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # h-cli
 
 - [cli-documentation](./horbach_cli/README.md)
 - run in docker `docker run ghcr.io/karma-git/h-cli/h-cli:latest --help`
```

