# Comparing `tmp/pymusiclooper-3.0.0.tar.gz` & `tmp/pymusiclooper-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymusiclooper-3.0.0.tar", max compression
+gzip compressed data, was "pymusiclooper-3.1.0.tar", max compression
```

## Comparing `pymusiclooper-3.0.0.tar` & `pymusiclooper-3.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1067 2023-07-07 15:55:51.972223 pymusiclooper-3.0.0/LICENSE
--rw-r--r--   0        0        0    10363 2023-07-07 15:55:51.972223 pymusiclooper-3.0.0/README.md
--rw-r--r--   0        0        0       22 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/__init__.py
--rw-r--r--   0        0        0      199 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/__main__.py
--rw-r--r--   0        0        0    23955 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/analysis.py
--rw-r--r--   0        0        0     3736 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/audio.py
--rw-r--r--   0        0        0    18617 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/cli.py
--rw-r--r--   0        0        0     1789 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/console.py
--rw-r--r--   0        0        0     6218 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/core.py
--rw-r--r--   0        0        0      205 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/exceptions.py
--rw-r--r--   0        0        0    13736 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/handler.py
--rw-r--r--   0        0        0     4637 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/playback.py
--rw-r--r--   0        0        0     2284 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pymusiclooper/youtube.py
--rw-r--r--   0        0        0     1511 2023-07-07 15:55:51.976223 pymusiclooper-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    11997 1970-01-01 00:00:00.000000 pymusiclooper-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-09 13:16:35.617369 pymusiclooper-3.1.0/LICENSE
+-rw-r--r--   0        0        0    10363 2023-07-09 13:16:35.617369 pymusiclooper-3.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/__main__.py
+-rw-r--r--   0        0        0    23955 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/analysis.py
+-rw-r--r--   0        0        0     3736 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/audio.py
+-rw-r--r--   0        0        0    18617 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/cli.py
+-rw-r--r--   0        0        0     1789 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/console.py
+-rw-r--r--   0        0        0     6218 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/core.py
+-rw-r--r--   0        0        0      205 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/exceptions.py
+-rw-r--r--   0        0        0    13736 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/handler.py
+-rw-r--r--   0        0        0     5914 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/playback.py
+-rw-r--r--   0        0        0     2284 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pymusiclooper/youtube.py
+-rw-r--r--   0        0        0     1511 2023-07-09 13:16:35.621369 pymusiclooper-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11997 1970-01-01 00:00:00.000000 pymusiclooper-3.1.0/PKG-INFO
```

### Comparing `pymusiclooper-3.0.0/LICENSE` & `pymusiclooper-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/README.md` & `pymusiclooper-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/pymusiclooper/analysis.py` & `pymusiclooper-3.1.0/pymusiclooper/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,15 @@
     test_offset = mlaudio.samples_to_frames(int(seconds_to_test * mlaudio.rate))
 
     # adjust offset for very short tracks to 25% of its length
     if test_offset > chroma.shape[-1]:
         test_offset = chroma.shape[-1] // 4
 
     # Prune candidates if there are too many
-    if len(candidate_pairs) >= 250 and not disable_pruning:
+    if len(candidate_pairs) >= 100 and not disable_pruning:
         pruned_candidate_pairs = _prune_candidates(candidate_pairs)
     else:
         pruned_candidate_pairs = candidate_pairs
 
     weights = _weights(test_offset, start=max(2, test_offset // num_test_beats), stop=1)
 
     pair_score_list = [
@@ -374,37 +374,37 @@
     )
     return pruned_candidate_pairs
 
 
 def _prune_candidates(
     candidate_pairs: List[LoopPair],
     keep_top_notes: float = 75,
-    keep_top_loudness: float = 90,
+    keep_top_loudness: float = 50,
     acceptable_loudness=0.25,
 ) -> List[LoopPair]:
     db_diff_array = np.array([pair.loudness_difference for pair in candidate_pairs])
     note_dist_array = np.array([pair.note_distance for pair in candidate_pairs])
 
     # Minimum value used to avoid issues with tracks with lots of silence
     epsilon = 1e-3
     min_adjusted_db_diff_array = db_diff_array[db_diff_array > epsilon]
     min_adjusted_note_dist_array = note_dist_array[note_dist_array > epsilon]
 
     # Avoid index errors by having at least 3 elements when performing percentile-based pruning
     # Otherwise, skip by setting the value to the highest available
     if min_adjusted_db_diff_array.size > 3:
         db_threshold = np.percentile(
-            min_adjusted_db_diff_array, keep_top_notes
+            min_adjusted_db_diff_array, keep_top_loudness
         )
     else:
         db_threshold = np.max(db_diff_array)
 
     if min_adjusted_note_dist_array.size > 3:
         note_dist_threshold = np.percentile(
-            min_adjusted_note_dist_array, keep_top_loudness
+            min_adjusted_note_dist_array, keep_top_notes
         )
     else:
         note_dist_threshold = np.max(note_dist_array)
 
     # Lower values are better
     indices_that_meet_cond = np.flatnonzero(
         (db_diff_array <= max(acceptable_loudness, db_threshold)) & (note_dist_array <= note_dist_threshold)
```

### Comparing `pymusiclooper-3.0.0/pymusiclooper/audio.py` & `pymusiclooper-3.1.0/pymusiclooper/audio.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/pymusiclooper/cli.py` & `pymusiclooper-3.1.0/pymusiclooper/cli.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/pymusiclooper/console.py` & `pymusiclooper-3.1.0/pymusiclooper/console.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/pymusiclooper/core.py` & `pymusiclooper-3.1.0/pymusiclooper/core.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/pymusiclooper/handler.py` & `pymusiclooper-3.1.0/pymusiclooper/handler.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/pymusiclooper/playback.py` & `pymusiclooper-3.1.0/pymusiclooper/playback.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import logging
 import signal
 import threading
 
 import numpy as np
 import sounddevice as sd
+from rich.progress import BarColumn, Progress, TextColumn
 
 from .console import rich_console
 
 
 class PlaybackHandler:
     def __init__(self) -> None:
         self.event = threading.Event()
+        self.progressbar = Progress(
+            TextColumn("{task.description}"),
+            BarColumn(),
+            TextColumn("{task.fields[time_field]}"),
+            TextColumn("{task.fields[loop_field]}"),
+            console=rich_console,
+            transient=True,
+            refresh_per_second=1,
+        )
 
     def play_looping(
         self,
         playback_data: np.ndarray,
         samplerate: int,
         n_channels: int,
         loop_start: int,
@@ -84,22 +94,44 @@
             self.stream = sd.OutputStream(
                 samplerate=samplerate,
                 channels=n_channels,
                 callback=callback,
                 finished_callback=self.event.set,
             )
 
-            with self.stream:
+            with self.stream, self.progressbar:
+                # Initialize playback progress bar
+                pbar = self.progressbar.add_task(
+                    "Now Playing...",
+                    total=total_samples,
+                    loop_field="",
+                    time_field="",
+                )
+
                 # Override SIGINT/KeyboardInterrupt handler with custom logic for loop handling
                 signal.signal(signal.SIGINT, self._loop_interrupt_handler)
+
                 # Workaround for python issue on Windows
                 # (threading.Event().wait() not interruptable with Ctrl-C on Windows): https://bugs.python.org/issue35935
                 # Set a 0.5 second timeout to handle interrupts in-between
                 while not self.event.wait(0.5):
-                    pass
+                    # Update playback progress bar between wait timeouts
+                    time_sec = self.current_frame / samplerate
+                    ftime = f"{time_sec // 60:02.0f}:{time_sec % 60:02.0f}"
+                    self.progressbar.update(
+                        pbar,
+                        completed=self.current_frame,
+                        time_field=ftime,
+                        loop_field=(
+                            f"[dim] | Currently on Loop #{self.loop_counter}[/]"
+                            if self.loop_counter
+                            else ""
+                        ),
+                    )
+
                 # Restore default SIGINT handler after playback is stopped
                 signal.signal(signal.SIGINT, signal.default_int_handler)
         except Exception as e:
             logging.error(e)
 
     def _loop_interrupt_handler(self, *args):
         if self.looping:
```

### Comparing `pymusiclooper-3.0.0/pymusiclooper/youtube.py` & `pymusiclooper-3.1.0/pymusiclooper/youtube.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.0.0/pyproject.toml` & `pymusiclooper-3.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymusiclooper"
-version = "3.0.0"
+version = "3.1.0"
 description = "Automatically find the loop points of any music file and export into intro/loop/outro sections or loop points, with support for playback and preview through the terminal."
 license = "MIT"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `pymusiclooper-3.0.0/PKG-INFO` & `pymusiclooper-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymusiclooper
-Version: 3.0.0
+Version: 3.1.0
 Summary: Automatically find the loop points of any music file and export into intro/loop/outro sections or loop points, with support for playback and preview through the terminal.
 Home-page: https://github.com/arkrow/PyMusicLooper
 License: MIT
 Author: arkrow
 Author-email: arkrow@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

