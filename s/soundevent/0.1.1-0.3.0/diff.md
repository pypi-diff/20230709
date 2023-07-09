# Comparing `tmp/soundevent-0.1.1.tar.gz` & `tmp/soundevent-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundevent-0.1.1.tar", last modified: Wed Jul  5 17:43:26 2023, max compression
+gzip compressed data, was "soundevent-0.3.0.tar", last modified: Sun Jul  9 15:05:39 2023, max compression
```

## Comparing `soundevent-0.1.1.tar` & `soundevent-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,37 @@
--rw-r--r--   0        0        0     1084 2023-07-05 17:43:17.725381 soundevent-0.1.1/LICENSE
--rw-r--r--   0        0        0     3374 2023-07-05 17:43:17.725381 soundevent-0.1.1/README.md
--rw-r--r--   0        0        0     1152 2023-07-05 17:43:26.237410 soundevent-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1104 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/__init__.py
--rw-r--r--   0        0        0       60 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/__version__.py
--rw-r--r--   0        0        0     2974 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/__init__.py
--rw-r--r--   0        0        0     2523 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/annotation_projects.py
--rw-r--r--   0        0        0     3077 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/annotation_tasks.py
--rw-r--r--   0        0        0     3287 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/annotations.py
--rw-r--r--   0        0        0     2993 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/clips.py
--rw-r--r--   0        0        0     2854 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/dataset.py
--rw-r--r--   0        0        0     2424 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/features.py
--rw-r--r--   0        0        0    17278 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/geometries.py
--rw-r--r--   0        0        0     2102 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/matches.py
--rw-r--r--   0        0        0     2261 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/model_run.py
--rw-r--r--   0        0        0     3002 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/notes.py
--rw-r--r--   0        0        0     2638 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/predicted_sound_events.py
--rw-r--r--   0        0        0     1531 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/predicted_tags.py
--rw-r--r--   0        0        0     2590 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/processed_clip.py
--rw-r--r--   0        0        0     3765 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/recordings.py
--rw-r--r--   0        0        0     2574 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/sound_events.py
--rw-r--r--   0        0        0     2624 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/data/tags.py
--rw-r--r--   0        0        0        0 2023-07-05 17:43:17.729380 soundevent-0.1.1/src/soundevent/py.typed
--rw-r--r--   0        0        0        0 2023-07-05 17:43:17.729380 soundevent-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      183 2023-07-05 17:43:17.729380 soundevent-0.1.1/tests/test_soundevent.py
--rw-r--r--   0        0        0     3802 1970-01-01 00:00:00.000000 soundevent-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-09 15:05:30.648328 soundevent-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3164 2023-07-09 15:05:30.648328 soundevent-0.3.0/README.md
+-rw-r--r--   0        0        0     1328 2023-07-09 15:05:39.128515 soundevent-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1134 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/__init__.py
+-rw-r--r--   0        0        0       60 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/__version__.py
+-rw-r--r--   0        0        0      323 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/__init__.py
+-rw-r--r--   0        0        0     2939 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/chunks.py
+-rw-r--r--   0        0        0     3893 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/io.py
+-rw-r--r--   0        0        0     2461 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/media_info.py
+-rw-r--r--   0        0        0     2495 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/spectrograms.py
+-rw-r--r--   0        0        0     3037 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/__init__.py
+-rw-r--r--   0        0        0     2523 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/annotation_projects.py
+-rw-r--r--   0        0        0     3077 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/annotation_tasks.py
+-rw-r--r--   0        0        0     3287 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/annotations.py
+-rw-r--r--   0        0        0     2993 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/clips.py
+-rw-r--r--   0        0        0     2854 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/dataset.py
+-rw-r--r--   0        0        0     2424 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/features.py
+-rw-r--r--   0        0        0    17278 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/geometries.py
+-rw-r--r--   0        0        0     2102 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/matches.py
+-rw-r--r--   0        0        0     2261 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/model_run.py
+-rw-r--r--   0        0        0     3002 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/notes.py
+-rw-r--r--   0        0        0     2638 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/predicted_sound_events.py
+-rw-r--r--   0        0        0     1531 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/predicted_tags.py
+-rw-r--r--   0        0        0     2590 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/processed_clip.py
+-rw-r--r--   0        0        0     5531 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/recordings.py
+-rw-r--r--   0        0        0     2935 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/sequences.py
+-rw-r--r--   0        0        0     2574 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/sound_events.py
+-rw-r--r--   0        0        0     2624 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/tags.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/py.typed
+-rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/conftest.py
+-rw-r--r--   0        0        0     4678 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/test_audio.py
+-rw-r--r--   0        0        0     2691 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/test_spectrograms.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_soundevent.py
+-rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 soundevent-0.3.0/PKG-INFO
```

### Comparing `soundevent-0.1.1/LICENSE` & `soundevent-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/README.md` & `soundevent-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: soundevent
+Version: 0.3.0
+Summary: soundevent is an open-source Python package for the computational biocoustic community, providing standardized tools for sound event analysis and data management.
+Author-Email: Santiago Martinez <santiago.balvanera.20@ucl.ac.uk>
+License: MIT
+Requires-Python: >=3.8
+Requires-Dist: pydantic>=2.0
+Requires-Dist: shapely>=2.0.1
+Requires-Dist: scipy>=1.6.1
+Requires-Dist: xarray>=0.20.2
+Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: cython>=0.29.36
+Description-Content-Type: text/markdown
+
 # soundevent
 
 > **Warning**
 > This package is under active development use with caution. 
 > However, most of the data definitions are not expected to change. 
 > Will be adding data loading/exporting and prediction evaluation functions soon. 
 
@@ -12,15 +27,15 @@
 is in a computational sense, along with a set of tools to easily work with this
 definition. The package comprises three key components:
 
 ## Main features
 
 ### 1. Data Classes for Bioacoustic Analysis
 
-The `soundevent` package defines several data classes that conceptualize and
+The `soundevent` package defines several [data classes](https://mbsantiago.github.io/soundevent/data/) that conceptualize and
 standardize different recurrent objects in bioacoustic analysis. These data
 classes establish the relationships between various concepts and specify the
 attributes each object possesses. They are designed to be flexible enough to
 cover a wide range of use cases in bioacoustic analysis. The package also
 includes data validation mechanisms to ensure that the information stored is
 valid and meaningful. Specifically, it defines objects related to sound events,
 such as user annotations and model predictions.
@@ -51,32 +66,20 @@
 ```{shell}
 pip install soundevent
 ```
 
 ## Documentation
 
 For detailed information on how to use the package, please refer to the
-[documentation](https://github.com/mbsantiago/soundevent/settings/pages).
+[documentation](https://mbsantiago.github.io/soundevent/).
 
 ## Example Usage
 
-Here's a brief example demonstrating the usage of `soundevent` package:
-
-``` py
-import soundevent
-
-dataset = soundevent.load_dataset("example_dataset.json", audio_dir="audio")
-print(f"Dataset {dataset.name} has {len(dataset.recordings)} Recordings")
-
-recording = dataset.recordings[0]
-print(f"Recording {recording.id}:  duration={recording.duration}, samplerate={recording.samplerate}")
-
-wav = soundevent.load_recording_audio(recording)
-
-```
+To see practical examples of how to use soundevent, you can explore the collection of examples provided in the
+[documentation's gallery](https://mbsantiago.github.io/soundevent/generated/gallery/).
 
 ## Contributing
 
 We welcome contributions from the community to make `soundevent` even better. If
 you would like to contribute, please refer to the [contribution guidelines](CONTRIBUTING.md).
 
 ## License
```

### Comparing `soundevent-0.1.1/pyproject.toml` & `soundevent-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     "mkdocs>=1.2.4",
     "importlib-metadata>=4.3",
     "ruff>=0.0.276",
     "mkdocs-material>=9.1.18",
     "isort>=5.11.5",
     "mkdocstrings[python]>=0.22.0",
     "tox>=4.6.3",
+    "hypothesis>=6.79.4",
+    "mkdocs-gallery>=0.7.8",
+    "memory-profiler>=0.61.0",
 ]
 
 [tool.black]
 line-length = 79
 
 [tool.pyright]
 venvPath = "."
@@ -34,24 +37,28 @@
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [project]
 name = "soundevent"
-version = "0.1.1"
+version = "0.3.0"
 description = "soundevent is an open-source Python package for the computational biocoustic community, providing standardized tools for sound event analysis and data management."
 authors = [
     { name = "Santiago Martinez", email = "santiago.balvanera.20@ucl.ac.uk" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "shapely>=2.0.1",
+    "scipy>=1.6.1",
+    "xarray>=0.20.2",
+    "matplotlib>=3.5.3",
+    "cython>=0.29.36",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `soundevent-0.1.1/src/soundevent/__init__.py` & `soundevent-0.3.0/src/soundevent/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Geometry,
     GeometryType,
     LineString,
     Match,
     ModelRun,
     MultiLineString,
     MultiPoint,
+    Sequence,
     MultiPolygon,
     Note,
     Point,
     Polygon,
     PredictedSoundEvent,
     PredictedTag,
     ProcessedClip,
@@ -30,38 +31,39 @@
     Tag,
     Time,
     TimeInterval,
     TimeStamp,
 )
 
 __all__ = [
-    "__version__",
     "Annotation",
     "AnnotationProject",
     "AnnotationTask",
+    "BoundingBox",
     "Clip",
     "Dataset",
     "Feature",
+    "Frequency",
+    "Geometry",
+    "GeometryType",
+    "LineString",
+    "MAX_FREQUENCY",
     "Match",
     "ModelRun",
+    "MultiLineString",
+    "MultiPoint",
+    "MultiPolygon",
     "Note",
+    "Point",
+    "Polygon",
     "PredictedSoundEvent",
     "PredictedTag",
     "ProcessedClip",
     "Recording",
+    "Sequence",
     "SoundEvent",
     "Tag",
     "Time",
-    "Frequency",
-    "GeometryType",
-    "MAX_FREQUENCY",
-    "Geometry",
-    "TimeStamp",
     "TimeInterval",
-    "BoundingBox",
-    "Point",
-    "LineString",
-    "Polygon",
-    "MultiPoint",
-    "MultiLineString",
-    "MultiPolygon",
+    "TimeStamp",
+    "__version__",
 ]
```

### Comparing `soundevent-0.1.1/src/soundevent/data/__init__.py` & `soundevent-0.3.0/src/soundevent/data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 from soundevent.data.annotation_projects import AnnotationProject
 from soundevent.data.annotation_tasks import AnnotationTask
 from soundevent.data.annotations import Annotation
 from soundevent.data.clips import Clip
 from soundevent.data.dataset import Dataset
 from soundevent.data.features import Feature
+from soundevent.data.sequences import Sequence
 from soundevent.data.geometries import (
     MAX_FREQUENCY,
     BoundingBox,
     Frequency,
     Geometry,
     GeometryType,
     LineString,
@@ -62,34 +63,35 @@
 from soundevent.data.sound_events import SoundEvent
 from soundevent.data.tags import Tag
 
 __all__ = [
     "Annotation",
     "AnnotationProject",
     "AnnotationTask",
+    "BoundingBox",
     "Clip",
     "Dataset",
     "Feature",
+    "Frequency",
+    "Geometry",
+    "GeometryType",
+    "LineString",
+    "MAX_FREQUENCY",
     "Match",
     "ModelRun",
+    "MultiLineString",
+    "MultiPoint",
+    "MultiPolygon",
     "Note",
+    "Point",
+    "Polygon",
     "PredictedSoundEvent",
     "PredictedTag",
     "ProcessedClip",
     "Recording",
+    "Sequence",
     "SoundEvent",
     "Tag",
     "Time",
-    "Frequency",
-    "GeometryType",
-    "MAX_FREQUENCY",
-    "Geometry",
-    "TimeStamp",
     "TimeInterval",
-    "BoundingBox",
-    "Point",
-    "LineString",
-    "Polygon",
-    "MultiPoint",
-    "MultiLineString",
-    "MultiPolygon",
+    "TimeStamp",
 ]
```

### Comparing `soundevent-0.1.1/src/soundevent/data/annotation_projects.py` & `soundevent-0.3.0/src/soundevent/data/annotation_projects.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/annotation_tasks.py` & `soundevent-0.3.0/src/soundevent/data/annotation_tasks.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/annotations.py` & `soundevent-0.3.0/src/soundevent/data/annotations.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/clips.py` & `soundevent-0.3.0/src/soundevent/data/clips.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/dataset.py` & `soundevent-0.3.0/src/soundevent/data/dataset.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/features.py` & `soundevent-0.3.0/src/soundevent/data/features.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/geometries.py` & `soundevent-0.3.0/src/soundevent/data/geometries.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/matches.py` & `soundevent-0.3.0/src/soundevent/data/matches.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/model_run.py` & `soundevent-0.3.0/src/soundevent/data/model_run.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/notes.py` & `soundevent-0.3.0/src/soundevent/data/notes.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/predicted_sound_events.py` & `soundevent-0.3.0/src/soundevent/data/predicted_sound_events.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/predicted_tags.py` & `soundevent-0.3.0/src/soundevent/data/predicted_tags.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/processed_clip.py` & `soundevent-0.3.0/src/soundevent/data/processed_clip.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/sound_events.py` & `soundevent-0.3.0/src/soundevent/data/sound_events.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.1.1/src/soundevent/data/tags.py` & `soundevent-0.3.0/src/soundevent/data/tags.py`

 * *Files identical despite different names*

