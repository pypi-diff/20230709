# Comparing `tmp/idownload-0.2.0-py3-none-any.whl.zip` & `tmp/idownload-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5092 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-07 22:09 idownload/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-07 22:09 idownload/__main__.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jul-07 22:09 idownload/cli.py
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-07 22:09 idownload/exceptions.py
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-07 22:09 idownload/sources/__init__.py
--rw-r--r--  2.0 unx     2907 b- defN 23-Jul-07 22:09 idownload/sources/pinterest.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1112 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-07 22:09 idownload-0.2.0.dist-info/RECORD
-12 files, 7180 bytes uncompressed, 3456 bytes compressed:  51.9%
+Zip file size: 5568 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-09 06:22 idownload/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 06:22 idownload/__main__.py
+-rw-r--r--  2.0 unx     1018 b- defN 23-Jul-09 06:22 idownload/cli.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-09 06:22 idownload/exceptions.py
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-09 06:22 idownload/sources/__init__.py
+-rw-r--r--  2.0 unx     3742 b- defN 23-Jul-09 06:22 idownload/sources/pinterest.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1351 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      968 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/RECORD
+12 files, 8659 bytes uncompressed, 3932 bytes compressed:  54.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: idownload/sources/__init__.py
 Comment: 
 
 Filename: idownload/sources/pinterest.py
 Comment: 
 
-Filename: idownload-0.2.0.dist-info/LICENSE
+Filename: idownload-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: idownload-0.2.0.dist-info/METADATA
+Filename: idownload-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: idownload-0.2.0.dist-info/WHEEL
+Filename: idownload-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: idownload-0.2.0.dist-info/entry_points.txt
+Filename: idownload-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: idownload-0.2.0.dist-info/top_level.txt
+Filename: idownload-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: idownload-0.2.0.dist-info/RECORD
+Filename: idownload-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## idownload/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0"
+__version__ = "1.0.0"
```

## idownload/cli.py

```diff
@@ -1,12 +1,12 @@
 import click
 
 from . import __version__
 from .sources import SOURCES
-from .exceptions import ImageDownloadException
+from .exceptions import SourceAccessException
 
 
 @click.group(
     help="Downloads images and stores metadata about them in a JSON file.",
     context_settings={
         "help_option_names": ["-h", "--help"],
     },
@@ -16,13 +16,27 @@
     pass
 
 
 for source in SOURCES:
 
     def command(**kwargs):
         kwargs["progressbar"] = click.progressbar
-        source.download(**kwargs)
+        try:
+            source.download(**kwargs)
+        except SourceAccessException as e:
+            click.echo(str(e), err=True)
 
     command.__name__ = source.COMMAND
     for arg in reversed(source.ARGS):
         command = click.argument(arg, nargs=1)(command)
     command = cli.command()(command)
+
+    command = click.option(
+        "--with-attr/--no-with-attr",
+        default=False,
+        help="""
+Attempt to attribute to the image to a person or organization and use that name for source_name.
+        """,
+    )(command)
+
+
+__all__ = ("cli",)
```

## idownload/exceptions.py

```diff
@@ -1,4 +1,8 @@
+class SourceAccessException(Exception):
+    pass
+
+
 class ImageDownloadException(Exception):
     def __init__(self, url, cause):
         super().__init__(f"Failure of image download at {url} caused by {cause}")
         self.__cause__ = cause
```

## idownload/sources/pinterest.py

```diff
@@ -1,43 +1,71 @@
 import re
 import urllib.request
 import urllib.error
+import io
+import sys
 from datetime import datetime
 from pathlib import Path
-from contextlib import contextmanager
+from contextlib import contextmanager, redirect_stdout, redirect_stderr
+from os import devnull
 import feedparser
 from imeta import ImageMetadata
 from fnum import FnumMetadata
 
-from ..exceptions import ImageDownloadException
+from ..exceptions import SourceAccessException, ImageDownloadException
+
+
+stdout = io.StringIO()
+stderr = io.StringIO()
+try:
+    with redirect_stdout(stdout), redirect_stderr(stderr):
+        import nameattr
+except ImportError:
+    pass
+nameattr_out = stdout.getvalue()
+nameattr_err = stderr.getvalue()
 
 
 class PinterestSource:
     COMMAND = "pinterest"
     ARGS = ("username", "board", "dirpath")
 
     @classmethod
-    def download(cls, username, board, dirpath, progressbar=None):
+    def download(cls, username, board, dirpath, progressbar=None, with_attr=False):
         url = f"https://www.pinterest.com/{username}/{board}.rss"
         feed = feedparser.parse(url)
+        if feed.status < 200 or feed.status > 299:
+            raise SourceAccessException(
+                f"HTTP status {feed.status} while requesting feed {url}"
+            )
+
         if not progressbar:
 
             @contextmanager
             def noop_progressbar(*args, **kwargs):
                 yield args[0]
 
             progressbar = noop_progressbar
 
         with progressbar(feed["items"], label="Downloading images") as bar:
             for item in bar:
                 source_name = item["title"]
+                if with_attr:
+                    try:
+                        source_name = nameattr.from_text(source_name)
+                    except:
+                        print(nameattr_err, end="")
+                        print(nameattr_err, file=sys.stderr, end="")
+                        raise
+
                 source_id = re.match(
                     "^https:\\/\\/www\\.pinterest\\.com\\/pin\\/(\\d+)\\/$",
                     item["guid"],
                 ).groups()[0]
+
                 metadata = {
                     "$version": "1.0",
                     "source_url": item["link"],
                     "source_id": source_id,
                     "source_name": source_name,
                     "access_date": int(datetime.now().timestamp()),
                     "tags": ["source:pinterest"],
```

## Comparing `idownload-0.2.0.dist-info/LICENSE` & `idownload-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `idownload-0.2.0.dist-info/METADATA` & `idownload-1.0.0.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idownload
-Version: 0.2.0
+Version: 1.0.0
 Summary: Downloads images and stores metadata about them in a JSON file
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/idownload
 Keywords: idownload,cli,utility,image,download,backup,archive,pinterest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,8 +21,14 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8.0
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: feedparser (~=6.0)
 Requires-Dist: imeta (~=1.1)
 Requires-Dist: fnum (~=1.2)
+Provides-Extra: nameattr
+Requires-Dist: nameattr (~=1.0) ; extra == 'nameattr'
+Provides-Extra: tests
+Requires-Dist: pytest ; extra == 'tests'
+Requires-Dist: networktest ; extra == 'tests'
+Requires-Dist: nameattr (~=1.0) ; extra == 'tests'
```

## Comparing `idownload-0.2.0.dist-info/RECORD` & `idownload-1.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-idownload/__init__.py,sha256=Zn1KFblwuFHiDRdRAiRnDBRkbPttWh44jKa5zG2ov0E,22
+idownload/__init__.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
 idownload/__main__.py,sha256=VNXCcgJ6hm4LbZBeOMBPCzuFTICAcX2m_2ThvsGiB2M,29
-idownload/cli.py,sha256=d89ym3S173uoeXqG5NUeUhCqZ6JQJyboy384IckvhZU,665
-idownload/exceptions.py,sha256=shnyTKfLDO6AvqSrStn-HUU8sUxtIZeK7OkI74yi-Yo,190
+idownload/cli.py,sha256=4-baQmuaZhKB2xICp9YOvfedyzbz9xKMLam0ejdzTmo,1018
+idownload/exceptions.py,sha256=HCMziNWDLs85kKmyAd8KRKqLNttBtw38SMBrFzYzxCw,241
 idownload/sources/__init__.py,sha256=ueX9ofgR0hNk6kP1hOazFZc4V6alNJlzO2iSAwGmfNw,69
-idownload/sources/pinterest.py,sha256=WmvyxdtUKqp8MCMvnYQo9TnhkNeTLyH4mc7nNlD3dLc,2907
-idownload-0.2.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
-idownload-0.2.0.dist-info/METADATA,sha256=6KaYBwBXXx4wnrZI2Hx66LuU31q0M3WVJj-yHA6mIQs,1112
-idownload-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-idownload-0.2.0.dist-info/entry_points.txt,sha256=KDq6QIybIzNOcikhtmF1AGljdRtpft5G1MmZOQwBAXk,48
-idownload-0.2.0.dist-info/top_level.txt,sha256=naaqaO3WgkP36-DF4qyxiZEZZyeNrtlrG68XGO_kOAw,10
-idownload-0.2.0.dist-info/RECORD,,
+idownload/sources/pinterest.py,sha256=8d-D5E1IKdRqcwYuANkA8RgbXjBdA7mPiTsSeh7Vq-0,3742
+idownload-1.0.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
+idownload-1.0.0.dist-info/METADATA,sha256=nshOLi8zMRjo3tvNEM9K7SvAeD_g9_TaBFMtOyqRyOg,1351
+idownload-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+idownload-1.0.0.dist-info/entry_points.txt,sha256=KDq6QIybIzNOcikhtmF1AGljdRtpft5G1MmZOQwBAXk,48
+idownload-1.0.0.dist-info/top_level.txt,sha256=naaqaO3WgkP36-DF4qyxiZEZZyeNrtlrG68XGO_kOAw,10
+idownload-1.0.0.dist-info/RECORD,,
```

