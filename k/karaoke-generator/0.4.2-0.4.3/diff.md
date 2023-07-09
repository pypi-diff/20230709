# Comparing `tmp/karaoke_generator-0.4.2.tar.gz` & `tmp/karaoke_generator-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karaoke_generator-0.4.2.tar", max compression
+gzip compressed data, was "karaoke_generator-0.4.3.tar", max compression
```

## Comparing `karaoke_generator-0.4.2.tar` & `karaoke_generator-0.4.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2372 2023-07-09 20:08:59.462959 karaoke_generator-0.4.2/README.md
--rw-r--r--   0        0        0       40 2023-07-09 20:08:59.462959 karaoke_generator-0.4.2/karaoke_generator/__init__.py
--rw-r--r--   0        0        0    15081 2023-07-09 20:08:59.462959 karaoke_generator-0.4.2/karaoke_generator/generator.py
--rw-r--r--   0        0        0        0 2023-07-09 20:08:59.462959 karaoke_generator-0.4.2/karaoke_generator/utils/__init__.py
--rwxr-xr-x   0        0        0     3471 2023-07-09 20:08:59.462959 karaoke_generator-0.4.2/karaoke_generator/utils/cli.py
--rw-r--r--   0        0        0     1312 2023-07-09 20:08:59.466959 karaoke_generator-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 karaoke_generator-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2360 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/README.md
+-rw-r--r--   0        0        0       40 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/__init__.py
+-rw-r--r--   0        0        0    15081 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/generator.py
+-rw-r--r--   0        0        0        0 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3471 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/utils/cli.py
+-rw-r--r--   0        0        0     1528 2023-07-09 20:12:18.915454 karaoke_generator-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 karaoke_generator-0.4.3/PKG-INFO
```

### Comparing `karaoke_generator-0.4.2/README.md` & `karaoke_generator-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # KaraokeHunt: Karaoke video generator
 Fully automated creation of _acceptable_ karaoke music videos from any music on YouTube, using open source tools and AI (e.g. Whisper and MDX-Net)
 
-[![PyPI version](https://badge.fury.io/py/karaoke-video-generator.svg)](https://badge.fury.io/py/karaoke-video-generator)
+[![PyPI version](https://badge.fury.io/py/karaoke-generator.svg)](https://badge.fury.io/py/karaoke-generator)
 
 ## Context
 This is one experimental tool as part of the journey towards implementing the [full vision](https://docs.google.com/document/d/19LS1aJI8YwSmkWmDdpCHpmTGiHL9l0VDJ1SxSl4l6Z8/edit#) for KaraokeHunt (https://karaokehunt.com).
 
 Some of the other components include:
 - [Lyrics from Genius](https://github.com/karaokenerds/lyrics-from-genius)
 - [Karaoke Song Finder (Spreadsheet generator)](https://github.com/karaokenerds/music-data-karaoke-song-sheets)
```

### Comparing `karaoke_generator-0.4.2/karaoke_generator/generator.py` & `karaoke_generator-0.4.3/karaoke_generator/generator.py`

 * *Files identical despite different names*

### Comparing `karaoke_generator-0.4.2/karaoke_generator/utils/cli.py` & `karaoke_generator-0.4.3/karaoke_generator/utils/cli.py`

 * *Files identical despite different names*

### Comparing `karaoke_generator-0.4.2/PKG-INFO` & `karaoke_generator-0.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: karaoke-generator
-Version: 0.4.2
+Version: 0.4.3
 Summary: Fully automated creation of _acceptable_ karaoke music videos from any music on YouTube, using open source tools and AI (e.g. Whisper and MDX-Net)
+Home-page: https://github.com/karaokenerds/karaoke-generator
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,20 +14,22 @@
 Requires-Dist: audio-separator (>=0.3,<0.4)
 Requires-Dist: lyrics-transcriber (>=0.6.3,<0.7.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: tldextract (>=3.4,<4.0)
 Requires-Dist: yt-dlp (>=2023.6.22,<2024.0.0)
+Project-URL: Documentation, https://github.com/karaokenerds/karaoke-generator/blob/main/README.md
+Project-URL: Repository, https://github.com/karaokenerds/karaoke-generator
 Description-Content-Type: text/markdown
 
 # KaraokeHunt: Karaoke video generator
 Fully automated creation of _acceptable_ karaoke music videos from any music on YouTube, using open source tools and AI (e.g. Whisper and MDX-Net)
 
-[![PyPI version](https://badge.fury.io/py/karaoke-video-generator.svg)](https://badge.fury.io/py/karaoke-video-generator)
+[![PyPI version](https://badge.fury.io/py/karaoke-generator.svg)](https://badge.fury.io/py/karaoke-generator)
 
 ## Context
 This is one experimental tool as part of the journey towards implementing the [full vision](https://docs.google.com/document/d/19LS1aJI8YwSmkWmDdpCHpmTGiHL9l0VDJ1SxSl4l6Z8/edit#) for KaraokeHunt (https://karaokehunt.com).
 
 Some of the other components include:
 - [Lyrics from Genius](https://github.com/karaokenerds/lyrics-from-genius)
 - [Karaoke Song Finder (Spreadsheet generator)](https://github.com/karaokenerds/music-data-karaoke-song-sheets)
```

