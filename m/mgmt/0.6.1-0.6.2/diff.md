# Comparing `tmp/mgmt-0.6.1.tar.gz` & `tmp/mgmt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgmt-0.6.1.tar", max compression
+gzip compressed data, was "mgmt-0.6.2.tar", max compression
```

## Comparing `mgmt-0.6.1.tar` & `mgmt-0.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-03 05:37:03.674832 mgmt-0.6.1/LICENSE
--rw-r--r--   0        0        0     3511 2023-07-03 05:37:03.674832 mgmt-0.6.1/README.md
--rw-r--r--   0        0        0     1156 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/__init__.py
--rw-r--r--   0        0        0       44 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/__main__.py
--rw-r--r--   0        0        0     6721 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/app.py
--rw-r--r--   0        0        0     6652 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/aws.py
--rw-r--r--   0        0        0     1763 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/config.py
--rw-r--r--   0        0        0     2945 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/files.py
--rw-r--r--   0        0        0     1648 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/log.py
--rw-r--r--   0        0        0      656 2023-07-03 05:37:03.674832 mgmt-0.6.1/mgmt/utils.py
--rw-r--r--   0        0        0     2276 2023-07-03 05:37:03.674832 mgmt-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 mgmt-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-09 07:20:01.948364 mgmt-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4773 2023-07-09 07:20:01.948364 mgmt-0.6.2/README.md
+-rw-r--r--   0        0        0      553 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/__main__.py
+-rw-r--r--   0        0        0     6935 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/app.py
+-rw-r--r--   0        0        0     6653 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/aws.py
+-rw-r--r--   0        0        0     1762 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/config.py
+-rw-r--r--   0        0        0     4012 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/files.py
+-rw-r--r--   0        0        0     1744 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/log.py
+-rw-r--r--   0        0        0      338 2023-07-09 07:20:01.948364 mgmt-0.6.2/mgmt/utils.py
+-rw-r--r--   0        0        0     2304 2023-07-09 07:20:01.948364 mgmt-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 mgmt-0.6.2/PKG-INFO
```

### Comparing `mgmt-0.6.1/LICENSE` & `mgmt-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mgmt-0.6.1/mgmt/app.py` & `mgmt-0.6.2/mgmt/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 from typing import Optional
 from pathlib import Path
 
 import typer
+from rich import box
 from typer import echo
 from rich.table import Table
 from rich.console import Console
 
 from mgmt.aws import AwsStorageMgmt
 from mgmt.log import Log
 from mgmt.files import FileManager
@@ -29,23 +30,25 @@
         filename (str): The name of the file or directory to upload. Use 'all' to upload all files in the directory.
         compression (Optional[str]): The compression algorithm to use. Defaults to 'gzip'.
     """
     target = filename
     cwd = Path(".").resolve()
     target_path = cwd / target
     files_created = []
+    skip_files = [".DS_Store"]
 
     try:
         if target == "all":
             echo("uploading all media objects to S3")
             for _file_or_dir in cwd.iterdir():
-                echo()
-                echo("compressing...")
-                echo(str(_file_or_dir))
-                files_created.append(aws.upload_target(_file_or_dir, compression))
+                if str(_file_or_dir) not in skip_files:
+                    echo()
+                    echo("compressing...")
+                    echo(str(_file_or_dir))
+                    files_created.append(aws.upload_target(_file_or_dir, compression))
         elif target in os.listdir(cwd):
             echo()
             echo("file found, compressing...")
             echo(str(target))
             files_created.append(aws.upload_target(target_path, compression))
         else:
             echo("invalid file or directory")
@@ -76,30 +79,30 @@
 
     if len(local_matches + s3_matches) >= 1:
         echo("at least one match found\n")
         echo("Local File Matches")
         echo("\n".join(local_matches))
 
         console = Console()
-        table = Table(title="AWS S3 Search Matches")
-        table.add_column("Option #")
-        table.add_column("Storage Tier")
+        table = Table(title="AWS S3 Search Matches", box=box.SIMPLE)
+        table.add_column("Option #", style="cyan", no_wrap=True)
+        table.add_column("Storage Tier", style="green")
         table.add_column("Last Modified")
-        table.add_column("Object Key")
+        table.add_column("Object Key", style="magenta")
         table.add_column("Restored Status")
         doptions = {}
         for i, file_name in enumerate(s3_matches):
             try:
                 resp = aws.get_obj_head(file_name)
                 storage_class = resp.get("StorageClass", "STANDARD")
                 last_modified = resp.get("LastModified", "")
                 restored_status = resp.get("Restore")
                 if restored_status:
                     restored_status = str(restored_status).split("expiry-date=")[-1].replace('"', "")
-                table.add_row(str(i), storage_class, str(last_modified), file_name, str(restored_status))
+                table.add_row(str(i), storage_class, str(last_modified).split(" ")[0], file_name, str(restored_status))
                 doptions[i] = file_name
             except Exception as e:
                 logger.error(f"An error occurred while getting metadata: {e}")
 
         console.print(table)
         if not typer.confirm("Download?", default=False):
             echo("Aborted.")
```

### Comparing `mgmt-0.6.1/mgmt/aws.py` & `mgmt-0.6.2/mgmt/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class AwsStorageMgmt:
     def __init__(self):
         self.s3_resource = boto3.resource("s3")
         self.s3_client = boto3.client("s3")
         self.config = Config()
+        self.logger = Log(debug=False)
         self.load_config_file()
-        self.logger = Log(debug=True)
 
     def load_config_file(self):
         if self.config.check_exists():
             self.configs = self.config.get_configs()
             self.bucket = self.configs.get("BUCKET")
             self.object_prefix = self.configs.get("OBJECT_PREFIX")
             self.local_dir = self.configs.get("LOCAL_DIR")
```

### Comparing `mgmt-0.6.1/mgmt/config.py` & `mgmt-0.6.2/mgmt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dotenv
 
 from mgmt.log import Log
 
 
 class Config:
     def __init__(self):
-        self.path = Path("~/.config/mmgmt").expanduser()
+        self.path = Path("~/.config/mgmt").expanduser()
         self.path.mkdir(parents=True, exist_ok=True)
         self.dotenv_path = self.path / "config"
         self.logger = Log(debug=False)
         if not self.check_exists():
             self.logger.error("config file not found")
             self.logger.info(f"check config file exists: {str(self.check_exists())}")
             self.logger.info(f"dotenv_path: {str(self.dotenv_path)}")
```

### Comparing `mgmt-0.6.1/mgmt/files.py` & `mgmt-0.6.2/mgmt/files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import os
 import gzip
 import shutil
-import pathlib
 import tarfile
 from typing import List
+from pathlib import Path
 from zipfile import ZipFile
 
+import rarfile
+
 from mgmt.log import Log
 
 
 class FileManager:
     def __init__(self, base_path=None):
         self.logger = Log(debug=False)
         if base_path:
-            self.base_path = pathlib.Path(base_path)
+            self.base_path = Path(base_path)
         else:
-            self.base_path = pathlib.Path.home() / "media"
+            self.base_path = Path.home() / "media"
             self.base_path = self.base_path.resolve()
+        if not self.base_path.exists():
+            raise ValueError(f"Path {str(self.base_path)} does not exist")
 
     def zip_single_file(self, filename: str) -> str:
         zip_file = filename.split(".")[0] + ".zip"
         with ZipFile(zip_file, "w") as zipf:
             zipf.write(os.path.join(self.base_path, filename), arcname=filename)
         return zip_file
 
@@ -28,25 +32,25 @@
         gzip_file = f"{filename}.gz"
         with open(os.path.join(self.base_path, filename), "rb") as f_in, gzip.open(
             os.path.join(self.base_path, gzip_file), "wb"
         ) as f_out:
             shutil.copyfileobj(f_in, f_out)
         return gzip_file
 
-    def zip_process(self, target_path: pathlib.Path) -> str:
+    def zip_process(self, target_path: Path) -> str:
         try:
             # dir_name = str(self.base_path / target_path)
             dir_name = str(target_path)
             zip_path = shutil.make_archive(dir_name, "zip", dir_name)
             return zip_path.split("/")[-1]
         except NotADirectoryError as e:
             self.logger.error(e)
             return self.zip_single_file(target_path)
 
-    def gzip_process(self, target_path: pathlib.Path) -> str:
+    def gzip_process(self, target_path: Path) -> str:
         self.logger.debug("gzip_process")
         try:
             # dir_path = str(self.base_path / target_path)
             dir_path = str(target_path)
             self.logger.debug(dir_path)
             gzip_file = f"{target_path}.tar.gz"
             self.logger.debug("tarfile open")
@@ -65,21 +69,51 @@
             os.listdir(os.path.join(self.base_path, folder))
             if os.path.isdir(os.path.join(self.base_path, folder))
             else [folder]
             for folder in tmp
         ]
         return [item for sublist in tmp for item in sublist]
 
+    def list_all_files(self):
+        for file in self.base_path.glob("**/*"):
+            self.logger.info(file)
+
+    def list_all_dirs(self):
+        for directory in self.base_path.glob("**/"):
+            self.logger.info(directory)
+
     @staticmethod
     def clean_string(string: str) -> str:
         string = "".join(e for e in string if e.isalnum() or e == " " or e == "/")
         string = string.replace("  ", " ").replace("  ", " ").replace(" ", "_")
         return string
 
     @staticmethod
     def keyword_in_string(keyword, file):
         return file.lower().find(keyword.lower()) != -1
 
     @staticmethod
     def abort_if_false(ctx, param, value):
         if not value:
             ctx.abort()
+
+
+class RarHandler:
+    def __init__(self, path):
+        self.path = Path(path)
+        if not self.path.exists():
+            raise ValueError(f"Path {path} does not exist")
+
+    def extract_all(self, destination):
+        destination = Path(destination)
+        if not destination.exists():
+            destination.mkdir(parents=True)
+
+        for rar_file in self.path.glob("**/*.rar"):
+            with rarfile.RarFile(rar_file) as rf:
+                rf.extractall(destination)
+
+    def list_all(self):
+        for rar_file in self.path.glob("**/*.rar"):
+            with rarfile.RarFile(rar_file) as rf:
+                self.logger.info(f"Contents of {rar_file}:")
+                self.logger.info(rf.namelist())
```

### Comparing `mgmt-0.6.1/mgmt/log.py` & `mgmt-0.6.2/mgmt/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 import inspect
 import logging
 
 
 class Log:
     def __init__(self, debug=False):
         self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(logging.DEBUG if debug else logging.INFO)
-        formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-        # Create a StreamHandler to stream log messages to stdout
-        stream_handler = logging.StreamHandler(sys.stdout)
-        stream_handler.setLevel(logging.DEBUG)
-        stream_handler.setFormatter(formatter)
-        self.logger.addHandler(stream_handler)
+        if not self.logger.handlers:
+            self.logger.setLevel(logging.DEBUG if debug else logging.INFO)
+            formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+            stream_handler = logging.StreamHandler(sys.stdout)
+            stream_handler.setLevel(logging.DEBUG)
+            stream_handler.setFormatter(formatter)
+            self.logger.addHandler(stream_handler)
+        else:
+            self.logger.handlers[0].setLevel(logging.DEBUG if debug else logging.INFO)
 
     def set_debug(self, debug):
         log_level = logging.DEBUG if debug else logging.INFO
         self.logger.setLevel(log_level)
 
     def debug(self, message):
         frame = inspect.currentframe().f_back
```

### Comparing `mgmt-0.6.1/pyproject.toml` & `mgmt-0.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "mgmt"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 readme = "README.md"
 authors = ["Will Wright <willwright@example.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/will-wright-eng/media-mgmt-cli"
 homepage = "https://github.com/will-wright-eng/media-mgmt-cli"
 
@@ -23,25 +23,26 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.26.54"
 botocore = "^1.29.54"
-certifi = "^2022.12.7"
+certifi = ">=2022.12.7,<2024.0.0"
 click = "^8.1.3"
 jmespath = "^1.0.1"
 python-dateutil = "^2.8.2"
 s3transfer = "^0.6.0"
 six = "^1.16.0"
 urllib3 = "^1.26.14"
 pytest = "^7.2.1"
 typer = "^0.9.0"
 rich = "^13.3.5"
 python-dotenv = "^1.0.0"
+rarfile = "^4.0"
 
 [package.optional-dependencies]
 test = [
     "pytest >= 7.2.2, < 8.0.0",
     "requests-mock[fixture] >= 1.10.0, < 2.0.0",
     "isort >= 5.12.0, < 6.0.0",
     "black == 23.1.0",
```

