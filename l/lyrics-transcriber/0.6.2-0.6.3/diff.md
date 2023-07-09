# Comparing `tmp/lyrics_transcriber-0.6.2.tar.gz` & `tmp/lyrics_transcriber-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.6.2.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.6.3.tar", max compression
```

## Comparing `lyrics_transcriber-0.6.2.tar` & `lyrics_transcriber-0.6.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-07 23:36:37.237837 lyrics_transcriber-0.6.2/LICENSE
--rw-r--r--   0        0        0     3513 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/README.md
--rw-r--r--   0        0        0       94 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0    13091 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     4176 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1427 2023-07-07 23:36:37.241837 lyrics_transcriber-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 lyrics_transcriber-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-09 20:00:22.954882 lyrics_transcriber-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3626 2023-07-09 20:00:22.954882 lyrics_transcriber-0.6.3/README.md
+-rw-r--r--   0        0        0       94 2023-07-09 20:00:22.954882 lyrics_transcriber-0.6.3/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    13166 2023-07-09 20:00:22.954882 lyrics_transcriber-0.6.3/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-07-09 20:00:22.954882 lyrics_transcriber-0.6.3/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     4176 2023-07-09 20:00:22.954882 lyrics_transcriber-0.6.3/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1427 2023-07-09 20:00:22.958882 lyrics_transcriber-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 lyrics_transcriber-0.6.3/PKG-INFO
```

### Comparing `lyrics_transcriber-0.6.2/LICENSE` & `lyrics_transcriber-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.2/README.md` & `lyrics_transcriber-0.6.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Lyrics Transcriber 🎶
 
+[![PyPI version](https://badge.fury.io/py/lyrics-transcriber.svg)](https://badge.fury.io/py/lyrics-transcriber)
+
 Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using OpenAI Whisper and lyrics from Genius and Spotify, for convenience in use cases such as karaoke video production.
 
 ## Features 🌟
 
 - Automatically transcribe lyrics with word-level timestamps.
 - Outputs lyrics in ASS and MidiCo LRC formats.
 - Can fetch lyrics from with Genius and Spotify.
```

### Comparing `lyrics_transcriber-0.6.2/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.6.3/lyrics_transcriber/transcriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     def write_spotify_lyrics_file(self):
         if self.spotify_cookie and self.song_known:
             self.logger.debug(f"attempting spotify fetch as spotify_cookie and song name was set")
         else:
             self.logger.warning(f"skipping spotify fetch as not all spotify params were set")
             return
 
-        spotify_lyrics_cache_filepath = os.path.join(self.cache_dir, self.get_song_slug() + "-spotify.json")
+        spotify_lyrics_cache_filepath = os.path.join(self.cache_dir, "lyrics-" + self.get_song_slug() + "-spotify.json")
 
         if os.path.isfile(spotify_lyrics_cache_filepath):
             self.logger.debug(f"found existing file at spotify_lyrics_cache_filepath, reading: {spotify_lyrics_cache_filepath}")
 
             with open(spotify_lyrics_cache_filepath, "r") as cached_lyrics:
                 self.result_metadata["spotify_lyrics_filepath"] = spotify_lyrics_cache_filepath
                 self.result_metadata["spotify_lyrics"] = cached_lyrics
@@ -153,15 +153,15 @@
     def write_genius_lyrics_file(self):
         if self.genius_api_token and self.song_known:
             self.logger.debug(f"attempting genius fetch as genius_api_token and song name was set")
         else:
             self.logger.warning(f"skipping genius fetch as not all genius params were set")
             return
 
-        genius_lyrics_cache_filepath = os.path.join(self.cache_dir, self.get_song_slug() + "-genius.txt")
+        genius_lyrics_cache_filepath = os.path.join(self.cache_dir, "lyrics-" + self.get_song_slug() + "-genius.txt")
 
         if os.path.isfile(genius_lyrics_cache_filepath):
             self.logger.debug(f"found existing file at genius_lyrics_cache_filepath, reading: {genius_lyrics_cache_filepath}")
 
             with open(genius_lyrics_cache_filepath, "r") as cached_lyrics:
                 self.result_metadata["genius_lyrics_filepath"] = genius_lyrics_cache_filepath
                 self.result_metadata["genius_lyrics"] = cached_lyrics
@@ -265,24 +265,24 @@
         with open(whisper_cache_filepath, "w") as cache_file:
             json.dump(result, cache_file, indent=4)
 
         return result
 
     def get_cache_filepath(self, extension):
         filename = os.path.split(self.audio_filepath)[1]
-        filename_slug = slugify.slugify(filename)
+        filename_slug = slugify.slugify(filename, lowercase=False)
         hash_value = self.get_file_hash(self.audio_filepath)
         cache_filepath = os.path.join(self.cache_dir, filename_slug + "_" + hash_value + extension)
         self.logger.debug(f"get_cache_filepath returning cache_filepath: {cache_filepath}")
         return cache_filepath
 
     def get_song_slug(self):
-        artist_slug = slugify.slugify(self.artist)
-        title_slug = slugify.slugify(self.title)
-        return artist_slug + "_" + title_slug
+        artist_slug = slugify.slugify(self.artist, lowercase=False)
+        title_slug = slugify.slugify(self.title, lowercase=False)
+        return artist_slug + "-" + title_slug
 
     def get_file_hash(self, filepath):
         return hashlib.md5(open(filepath, "rb").read()).hexdigest()
 
     def create_folders(self):
         if self.cache_dir is not None:
             os.makedirs(self.cache_dir, exist_ok=True)
```

### Comparing `lyrics_transcriber-0.6.2/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.6.3/lyrics_transcriber/utils/cli.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.2/pyproject.toml` & `lyrics_transcriber-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.6.2"
+version = "0.6.3"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lyrics_transcriber" }]
 
 [tool.poetry.dependencies]
```

### Comparing `lyrics_transcriber-0.6.2/PKG-INFO` & `lyrics_transcriber-0.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.6.2
+Version: 0.6.3
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,14 +24,16 @@
 Requires-Dist: torch (>=1,<2)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: whisper-timestamped (>=1,<2)
 Description-Content-Type: text/markdown
 
 # Lyrics Transcriber 🎶
 
+[![PyPI version](https://badge.fury.io/py/lyrics-transcriber.svg)](https://badge.fury.io/py/lyrics-transcriber)
+
 Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using OpenAI Whisper and lyrics from Genius and Spotify, for convenience in use cases such as karaoke video production.
 
 ## Features 🌟
 
 - Automatically transcribe lyrics with word-level timestamps.
 - Outputs lyrics in ASS and MidiCo LRC formats.
 - Can fetch lyrics from with Genius and Spotify.
```

