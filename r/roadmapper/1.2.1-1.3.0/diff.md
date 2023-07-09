# Comparing `tmp/roadmapper-1.2.1.tar.gz` & `tmp/roadmapper-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadmapper-1.2.1.tar", last modified: Sat May 27 09:13:47 2023, max compression
+gzip compressed data, was "roadmapper-1.3.0.tar", last modified: Sun Jul  9 09:28:08 2023, max compression
```

## Comparing `roadmapper-1.2.1.tar` & `roadmapper-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.670058 roadmapper-1.2.1/
--rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.2.1/LICENSE.md
--rw-rw-rw-   0        0        0     4337 2023-05-27 09:13:47.670058 roadmapper-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3781 2023-05-27 09:08:32.000000 roadmapper-1.2.1/README.md
--rw-rw-rw-   0        0        0     1314 2023-05-27 09:13:34.000000 roadmapper-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 09:13:47.671059 roadmapper-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.624504 roadmapper-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.642562 roadmapper-1.2.1/src/roadmapper/
--rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.2.1/src/roadmapper/__init__.py
--rw-rw-rw-   0        0        0    17086 2023-04-23 20:15:33.000000 roadmapper-1.2.1/src/roadmapper/colourtheme.py
--rw-rw-rw-   0        0        0     2888 2023-04-23 20:31:54.000000 roadmapper-1.2.1/src/roadmapper/footer.py
--rw-rw-rw-   0        0        0     6722 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/group.py
--rw-rw-rw-   0        0        0     4376 2023-04-23 20:32:17.000000 roadmapper-1.2.1/src/roadmapper/logo.py
--rw-rw-rw-   0        0        0     4833 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/marker.py
--rw-rw-rw-   0        0        0     2732 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/milestone.py
--rw-rw-rw-   0        0        0    20304 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/painter.py
--rw-rw-rw-   0        0        0    17420 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/roadmap.py
--rw-rw-rw-   0        0        0     2767 2023-04-23 20:32:35.000000 roadmapper-1.2.1/src/roadmapper/subtitle.py
--rw-rw-rw-   0        0        0    20860 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/task.py
--rw-rw-rw-   0        0        0    22043 2023-04-23 20:32:42.000000 roadmapper-1.2.1/src/roadmapper/timeline.py
--rw-rw-rw-   0        0        0    13397 2023-04-23 20:32:46.000000 roadmapper-1.2.1/src/roadmapper/timelineitem.py
--rw-rw-rw-   0        0        0     3846 2023-04-23 20:32:50.000000 roadmapper-1.2.1/src/roadmapper/timelineitemyear.py
--rw-rw-rw-   0        0        0     4655 2023-04-09 00:51:50.000000 roadmapper-1.2.1/src/roadmapper/timelinelocale.py
--rw-rw-rw-   0        0        0     1330 2023-04-09 00:51:50.000000 roadmapper-1.2.1/src/roadmapper/timelinemode.py
--rw-rw-rw-   0        0        0     2978 2023-04-23 20:33:00.000000 roadmapper-1.2.1/src/roadmapper/title.py
--rw-rw-rw-   0        0        0       24 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/roadmapper/version.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.658056 roadmapper-1.2.1/src/roadmapper.egg-info/
--rw-rw-rw-   0        0        0     4337 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1139 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-05-27 09:13:47.000000 roadmapper-1.2.1/src/roadmapper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.665057 roadmapper-1.2.1/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 00:51:50.000000 roadmapper-1.2.1/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2643 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/compare_generated_roadmaps_test.py
--rw-rw-rw-   0        0        0      141 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/conftest.py
--rw-rw-rw-   0        0        0     1056 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_draw_test.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:13:47.669058 roadmapper-1.2.1/src/tests/roadmap_generators/
--rw-rw-rw-   0        0        0        0 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_generators/__init__.py
--rw-rw-rw-   0        0        0     7122 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_generators/colour_theme_extensive.py
--rw-rw-rw-   0        0        0      233 2023-05-26 11:05:58.000000 roadmapper-1.2.1/src/tests/roadmap_generators/roadmap_abc.py
--rw-rw-rw-   0        0        0     1990 2023-05-27 08:40:54.000000 roadmapper-1.2.1/src/tests/roadmap_generators/roadmap_generator.py
--rw-rw-rw-   0        0        0    43031 2023-05-27 08:49:41.000000 roadmapper-1.2.1/src/tests/test_cases.py
--rw-rw-rw-   0        0        0      320 2023-05-26 11:31:22.000000 roadmapper-1.2.1/src/tests/test_generate_roadmap.py
--rw-rw-rw-   0        0        0     3044 2023-04-23 20:15:33.000000 roadmapper-1.2.1/src/tests/test_painter.py
--rw-rw-rw-   0        0        0    13290 2023-05-27 08:54:11.000000 roadmapper-1.2.1/src/tests/test_roadmapper.py
+drwxrwxrwx   0        0        0        0 2023-07-09 09:28:08.220716 roadmapper-1.3.0/
+-rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0     4573 2023-07-09 09:28:08.220716 roadmapper-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4017 2023-07-09 09:20:05.000000 roadmapper-1.3.0/README.md
+-rw-rw-rw-   0        0        0     1393 2023-07-09 09:27:52.000000 roadmapper-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 09:28:08.221716 roadmapper-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 09:28:08.180709 roadmapper-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 09:28:08.196715 roadmapper-1.3.0/src/roadmapper/
+-rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.3.0/src/roadmapper/__init__.py
+-rw-rw-rw-   0        0        0    17086 2023-04-23 20:15:33.000000 roadmapper-1.3.0/src/roadmapper/colourtheme.py
+-rw-rw-rw-   0        0        0     2888 2023-04-23 20:31:54.000000 roadmapper-1.3.0/src/roadmapper/footer.py
+-rw-rw-rw-   0        0        0     6722 2023-05-26 11:05:58.000000 roadmapper-1.3.0/src/roadmapper/group.py
+-rw-rw-rw-   0        0        0     4376 2023-04-23 20:32:17.000000 roadmapper-1.3.0/src/roadmapper/logo.py
+-rw-rw-rw-   0        0        0     4833 2023-05-26 11:05:58.000000 roadmapper-1.3.0/src/roadmapper/marker.py
+-rw-rw-rw-   0        0        0     2732 2023-05-26 11:05:58.000000 roadmapper-1.3.0/src/roadmapper/milestone.py
+-rw-rw-rw-   0        0        0    35094 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/roadmapper/painter.py
+-rw-rw-rw-   0        0        0    17771 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/roadmapper/roadmap.py
+-rw-rw-rw-   0        0        0     2769 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/roadmapper/subtitle.py
+-rw-rw-rw-   0        0        0    20858 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/roadmapper/task.py
+-rw-rw-rw-   0        0        0    22043 2023-04-23 20:32:42.000000 roadmapper-1.3.0/src/roadmapper/timeline.py
+-rw-rw-rw-   0        0        0    13397 2023-04-23 20:32:46.000000 roadmapper-1.3.0/src/roadmapper/timelineitem.py
+-rw-rw-rw-   0        0        0     3846 2023-04-23 20:32:50.000000 roadmapper-1.3.0/src/roadmapper/timelineitemyear.py
+-rw-rw-rw-   0        0        0     4655 2023-04-09 00:51:50.000000 roadmapper-1.3.0/src/roadmapper/timelinelocale.py
+-rw-rw-rw-   0        0        0     1330 2023-04-09 00:51:50.000000 roadmapper-1.3.0/src/roadmapper/timelinemode.py
+-rw-rw-rw-   0        0        0     2978 2023-04-23 20:33:00.000000 roadmapper-1.3.0/src/roadmapper/title.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 09:18:09.000000 roadmapper-1.3.0/src/roadmapper/version.py
+drwxrwxrwx   0        0        0        0 2023-07-09 09:28:08.209714 roadmapper-1.3.0/src/roadmapper.egg-info/
+-rw-rw-rw-   0        0        0     4573 2023-07-09 09:28:08.000000 roadmapper-1.3.0/src/roadmapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-07-09 09:28:08.000000 roadmapper-1.3.0/src/roadmapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 09:28:08.000000 roadmapper-1.3.0/src/roadmapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-09 09:28:08.000000 roadmapper-1.3.0/src/roadmapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-09 09:28:08.000000 roadmapper-1.3.0/src/roadmapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 09:28:08.216715 roadmapper-1.3.0/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 00:51:50.000000 roadmapper-1.3.0/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     3868 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/compare_generated_roadmaps_test.py
+-rw-rw-rw-   0        0        0      671 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/conftest.py
+-rw-rw-rw-   0        0        0     1056 2023-05-26 11:05:58.000000 roadmapper-1.3.0/src/tests/roadmap_draw_test.py
+drwxrwxrwx   0        0        0        0 2023-07-09 09:28:08.219715 roadmapper-1.3.0/src/tests/roadmap_generators/
+-rw-rw-rw-   0        0        0        0 2023-05-26 11:05:58.000000 roadmapper-1.3.0/src/tests/roadmap_generators/__init__.py
+-rw-rw-rw-   0        0        0     2452 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/roadmap_generators/colour_theme.py
+-rw-rw-rw-   0        0        0     7122 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/roadmap_generators/colour_theme_extensive.py
+-rw-rw-rw-   0        0        0      233 2023-05-26 11:05:58.000000 roadmapper-1.3.0/src/tests/roadmap_generators/roadmap_abc.py
+-rw-rw-rw-   0        0        0     2471 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/roadmap_generators/roadmap_generator.py
+-rw-rw-rw-   0        0        0    45151 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/test_cases.py
+-rw-rw-rw-   0        0        0    45990 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/test_cases_svg.py
+-rw-rw-rw-   0        0        0     3041 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/test_painter.py
+-rw-rw-rw-   0        0        0    13617 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/test_roadmapper.py
+-rw-rw-rw-   0        0        0    14002 2023-07-09 09:15:03.000000 roadmapper-1.3.0/src/tests/test_roadmapper_svg.py
```

### Comparing `roadmapper-1.2.1/LICENSE.md` & `roadmapper-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/PKG-INFO` & `roadmapper-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadmapper
-Version: 1.2.1
+Version: 1.3.0
 Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/roadmapper
 Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,16 +40,18 @@
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
-* Pillow 9.5.0
-* python-dateutil 2.8.2
+* python-dateutil >= 2.8.2
+* Pillow >= 10.0.0
+* drawsvg >= 2.2.0
+
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
@@ -68,14 +70,15 @@
 ## Documentation
 Please refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki) for more information on how to use this RaC library.
 
 <br/>
 <hr>
 
 ## Code Example
+:point_right: Note: In order for the following code to work, you will need to download the `matariki-tech-logo.png` file to your local storage. The png file can be downloaded in the `\images\logo\` folder.
 
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
```

### Comparing `roadmapper-1.2.1/README.md` & `roadmapper-1.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
-* Pillow 9.5.0
-* python-dateutil 2.8.2
+* python-dateutil >= 2.8.2
+* Pillow >= 10.0.0
+* drawsvg >= 2.2.0
+
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
@@ -54,14 +56,15 @@
 ## Documentation
 Please refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki) for more information on how to use this RaC library.
 
 <br/>
 <hr>
 
 ## Code Example
+:point_right: Note: In order for the following code to work, you will need to download the `matariki-tech-logo.png` file to your local storage. The png file can be downloaded in the `\images\logo\` folder.
 
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
```

### Comparing `roadmapper-1.2.1/pyproject.toml` & `roadmapper-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ['Pillow>=9.5.0', 'python-dateutil>=2.8.2']
+dependencies = ['Pillow>=10.0.0', 'python-dateutil>=2.8.2', 'drawsvg>=2.2.0']
 
 [project.urls]
 "Homepage" = "https://github.com/csgoh/roadmapper"
 "Bug Tracker" = "https://github.com/csgoh/roadmapper/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"] # list of folders that contain the packages (["."] by default)
@@ -33,10 +33,11 @@
 version = { attr = "roadmapper.version.__version__" }
 readme = { file = ["README.md"] }
 
 [tool.pytest.ini_options]
 addopts = "-v"
 markers = [
     "unit: Unit tests which are not dependent on environment",
-    "ubuntu: Test which only apply to Ubuntu environment",
+    "ubuntu: Tests which only apply to Ubuntu environment",
+    "macos: Tests which only apply to macOS environment",
     "genimage: To generate test image",
 ]
```

### Comparing `roadmapper-1.2.1/src/roadmapper/colourtheme.py` & `roadmapper-1.3.0/src/roadmapper/colourtheme.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/footer.py` & `roadmapper-1.3.0/src/roadmapper/footer.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/group.py` & `roadmapper-1.3.0/src/roadmapper/group.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/logo.py` & `roadmapper-1.3.0/src/roadmapper/logo.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/marker.py` & `roadmapper-1.3.0/src/roadmapper/marker.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/milestone.py` & `roadmapper-1.3.0/src/roadmapper/milestone.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/painter.py` & `roadmapper-1.3.0/src/roadmapper/painter.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,20 +21,24 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import sys
 from .colourtheme import ColourTheme
 from PIL import Image, ImageDraw, ImageFont, ImageColor
+import drawsvg as dw
+
 import textwrap
 
 
-class Painter:
-    """A wrapper class for Pillow library"""
+class UnsupportedOSException(Exception):
+    pass
+
 
+class Painter:
     width = 0
     height = 0
     next_y_pos = 0
 
     top_margin = 30
     bottom_margin = 30
     left_margin = 30
@@ -98,36 +102,25 @@
     current_colour: str
     line_width: int
     transparency_level: int
     dash = None
     font: str
     font_size: int
 
-    # initialise code
     def __init__(self, width: int, height: int):
         """__init__ method
 
         Args:
             width (int): Width of the surface
             height (int): Height of the surface
         """
         self.width = width
         self.height = height
         self.next_y_pos = 0
 
-        # Default file format
-        self.output_type = "PNG"
-
-        self.__surface = Image.new("RGBA", (width, height), (0, 0, 0, 0))
-
-        self.__cr = ImageDraw.Draw(self.__surface)
-
-        self.__new_cr = None
-        self.__new_surface = None
-
     def set_colour_theme(self, colour_theme: str) -> None:
         """Set colour palette
 
         Args:
             colour_palette (str): Name of the colour palette. Eg. OrangePeel
         """
         self.colour_theme = ColourTheme(colour_theme)
@@ -190,129 +183,325 @@
         if sys.platform.startswith("win"):  # Windows
             return os.path.join("C:\\", "Windows", "Fonts", f"{font_name}.ttf")
         elif sys.platform.startswith("darwin"):  # macOS
             return os.path.join(
                 "/", "System", "Library", "Fonts", "Supplemental", f"{font_name}.ttf"
             )
         elif sys.platform.startswith("linux"):  # Linux
-            font_dir = f"/usr/share/fonts/truetype/msttcorefonts"
+            font_dir = "/usr/share/fonts/truetype/msttcorefonts"
 
             if os.path.exists(os.path.join(font_dir, f"{font_name}.ttf")):
                 return os.path.join(font_dir, f"{font_name}.ttf")
-            else:
-                ### This is cater for cases where msttcorefonts is not installed
-                linux_font_name = "DejaVuSans"  # Default font for Linux
-                return os.path.join(
-                    "/",
-                    "usr",
-                    "share",
-                    "fonts",
-                    "truetype",
-                    "dejavu",  # Use the DejaVu font directory instead of msttcorefonts
-                    f"{linux_font_name}.ttf",
-                )
+            ### This is cater for cases where msttcorefonts is not installed
+            linux_font_name = "DejaVuSans"  # Default font for Linux
+            return os.path.join(
+                "/",
+                "usr",
+                "share",
+                "fonts",
+                "truetype",
+                "dejavu",  # Use the DejaVu font directory instead of msttcorefonts
+                f"{linux_font_name}.ttf",
+            )
         else:
-            raise Exception("Unsupported operating system")
+            raise UnsupportedOSException("Unsupported operating system")
+
+    def get_display_text_position(
+        self,
+        x: int,
+        y: int,
+        width: int,
+        height: int,
+        text: str,
+        alignment: str,
+        text_font: str,
+        text_font_size: int,
+    ) -> tuple:
+        """Get text position relative to the rectangle box
+
+        Args:
+            x (int): Rectangle X coordinate
+            y (int): Rectangle Y coordinate
+            width (int): Rectangle width
+            height (int): Rectangle height
+            text (str): Text used to calculate position
+            alignment (str): Text alignment. Eg. left, center, right
+
+        Returns:
+            (text_x (int), text_y (int)): Text x and y coordinates
+        """
+        text_width, text_height = self.get_text_dimension(
+            text, text_font, text_font_size
+        )
+
+        if alignment == "centre":
+            text_x_pos = (width / 2) - (text_width / 2)
+        elif alignment == "right":
+            text_x_pos = width - text_width - 5
+        elif alignment == "left":
+            text_x_pos = 0 + 5
+
+        text_y_pos = (height / 2) + (text_height / 2)
+
+        return x + text_x_pos, y + text_y_pos
+
+    def get_text_dimension(self, text: str, font: str, font_size: int) -> tuple:
+        raise NotImplementedError
+
+    def set_line_style(self, style: str = "solid") -> None:
+        """Set line style
+
+        Args:
+            style (str, optional): Line style. Defaults to "solid". Options: "solid", "dashed"
+        """
+        self.dash = (10.0, 5.0) if style == "dashed" else None
 
     def draw_box(
         self, x: int, y: int, width: int, height: int, box_fill_colour: str
-    ) -> None:
+    ) -> list:
         """Draw a rectagle
 
         Args:
             x (int): X coordinate
             y (int): Y coordinate
             width (int): Rectangle width
             height (int): Rectangle height
             box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
         """
-        shape = [(x, y), (x + width, y + height)]
-        self.__cr.rectangle(shape, fill=box_fill_colour)
+        return [(x, y), (x + width, y + height)]
 
     def draw_rounded_box(
         self, x: int, y: int, width: int, height: int, box_fill_colour: str
-    ) -> None:
+    ) -> list:
         """Draw a rounded rectagle
 
         Args:
             x (int): X coordinate
             y (int): Y coordinate
             width (int): Rectangle width
             height (int): Rectangle height
             box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
         """
-        shape = [(x, y), (x + width, y + height)]
-        radius = 20
-        self.__cr.rounded_rectangle(shape, radius, fill=box_fill_colour)
+        return [(x, y), (x + width, y + height)]
 
     def draw_arrowhead_box(
         self, x: int, y: int, width: int, height: int, box_fill_colour: str
-    ) -> None:
+    ) -> list:
         """Draw a rounded rectagle
 
         Args:
             x (int): X coordinate
             y (int): Y coordinate
             width (int): Rectangle width
             height (int): Rectangle height
             box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
         """
         arrowhead_width = 10
-        width = width - arrowhead_width
-        shape = [(x, y), (x + width, y + height)]
-
-        # Draw the rectangle
-        self.__cr.rectangle(shape, fill=box_fill_colour)
+        width -= arrowhead_width
+        box_shape = [(x, y), (x + width, y + height)]
 
         # Set the coordinates of the arrowhead
         vertical_midpoint = (height / 2) + y
         arrowhead_endpoint = x + width + arrowhead_width
-        arrowhead = [
+        arrowhead_shape = [
             (x + width, y),
             (arrowhead_endpoint, vertical_midpoint),
             (x + width, y + height),
         ]
 
-        # Draw the arrowhead
-        self.__cr.polygon(arrowhead, fill=box_fill_colour)
+        return box_shape, arrowhead_shape
 
     def draw_box_with_text(
         self,
         box_x: int,
         box_y: int,
         box_width: int,
         box_height: int,
         box_fill_colour: int,
         text: str,
         text_alignment: str,
         text_font: str,
         text_font_size: int,
         text_font_colour: str,
         style: str = "rectangle",
+    ) -> tuple:
+        return (
+            box_x,
+            box_y,
+            box_x + box_width,
+            box_y + box_height,
+        )
+
+    def draw_diamond(
+        self, x: int, y: int, width: int, height: int, fill_colour: str
+    ) -> list:
+        """Draw a diamond
+
+        Args:
+            x (int): X coordinate
+            y (int): Y coordinate
+            width (int): Diamond width
+            height (int): Diamond height
+            fill_colour (str): Diamond fill colour in HTML colour name or hex code. Eg. #FFFFFF or LightGreen
+        """
+
+        # Calculate the coordinates of the four points of the diamond.
+        return [
+            (x + width / 2, y),
+            (x + width, y + height / 2),
+            (x + width / 2, y + height),
+            (x, y + height / 2),
+        ]
+
+    def draw_text(
+        self, x: int, y: int, text: str, font: str, font_size: int, font_colour: str
     ) -> None:
-        font = ImageFont.truetype(self.get_font_path(text_font), size=text_font_size)
+        raise NotImplementedError
 
-        multi_lines = []
-        wrap_lines = []
+    def draw_line(
+        self,
+        x1: int,
+        y1: int,
+        x2: int,
+        y2: int,
+        line_colour: str,
+        line_transparency: int,
+        line_width: int,
+        line_style: str = "dashed",
+    ) -> None:
+        raise NotImplementedError
 
-        ### Make '\n' work
-        multi_lines = text.splitlines()
+    def draw_cross_on_box(
+        self, x1: int, y1: int, x2: int, y2: int, colour: str
+    ) -> None:
+        raise NotImplementedError
 
-        left, _, right, bottom = font.getbbox("a")
-        single_char_width = right - left
+    def draw_logo(self, image: str, x: int, y: int, width: int, height: int) -> None:
+        raise NotImplementedError
 
-        ### wrap text
-        for line in multi_lines:
-            wrap_lines.extend(textwrap.wrap(line, int(box_width / single_char_width)))
+    def get_text_dimension(self, text: str, font: str, font_size: int) -> tuple:
+        raise NotImplementedError
+
+    def set_background_colour(self) -> None:
+        raise NotImplementedError
 
-        box_x1, box_y1, box_x2, box_y2 = (
+    def set_surface_size(self, width: int, height: int) -> tuple:
+        """Set surface size
+
+        Args:
+            width (int): Surface width
+            height (int): Surface height
+        """
+        height += self.bottom_margin
+        return 0, 0, width, height
+
+    def get_image_size(self, image: str) -> tuple:
+        raise NotImplementedError
+
+    def save_surface(self, filename: str) -> None:
+        raise NotImplementedError
+
+
+class PNGPainter(Painter):
+    """A wrapper class for Pillow library"""
+
+    # initialise code
+    def __init__(self, width: int, height: int):
+        """__init__ method
+
+        Args:
+            width (int): Width of the surface
+            height (int): Height of the surface
+        """
+        super().__init__(width, height)
+
+        self.__surface = Image.new("RGBA", (width, height), (0, 0, 0, 0))
+
+        self.__cr = ImageDraw.Draw(self.__surface)
+
+    def draw_box(
+        self, x: int, y: int, width: int, height: int, box_fill_colour: str
+    ) -> None:
+        """Draw a rectagle
+
+        Args:
+            x (int): X coordinate
+            y (int): Y coordinate
+            width (int): Rectangle width
+            height (int): Rectangle height
+            box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
+        """
+
+        shape = super().draw_box(x, y, width, height, box_fill_colour)
+        self.__cr.rectangle(shape, fill=box_fill_colour)
+
+    def draw_rounded_box(
+        self, x: int, y: int, width: int, height: int, box_fill_colour: str
+    ) -> None:
+        """Draw a rounded rectagle
+
+        Args:
+            x (int): X coordinate
+            y (int): Y coordinate
+            width (int): Rectangle width
+            height (int): Rectangle height
+            box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
+        """
+        shape = super().draw_rounded_box(x, y, width, height, box_fill_colour)
+        radius = 20
+        self.__cr.rounded_rectangle(shape, radius, fill=box_fill_colour)
+
+    def draw_arrowhead_box(
+        self, x: int, y: int, width: int, height: int, box_fill_colour: str
+    ) -> None:
+        """Draw a rounded rectagle
+
+        Args:
+            x (int): X coordinate
+            y (int): Y coordinate
+            width (int): Rectangle width
+            height (int): Rectangle height
+            box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
+        """
+        box_shape, arrowhead_shape = super().draw_arrowhead_box(
+            x, y, width, height, box_fill_colour
+        )
+
+        # Draw the rectangle
+        self.__cr.rectangle(box_shape, fill=box_fill_colour)
+
+        # Draw the arrowhead
+        self.__cr.polygon(arrowhead_shape, fill=box_fill_colour)
+
+    def draw_box_with_text(
+        self,
+        box_x: int,
+        box_y: int,
+        box_width: int,
+        box_height: int,
+        box_fill_colour: int,
+        text: str,
+        text_alignment: str,
+        text_font: str,
+        text_font_size: int,
+        text_font_colour: str,
+        style: str = "rectangle",
+    ) -> None:
+        box_x1, box_y1, box_x2, box_y2 = super().draw_box_with_text(
             box_x,
             box_y,
-            box_x + box_width,
-            box_y + box_height,
+            box_width,
+            box_height,
+            box_fill_colour,
+            text,
+            text_alignment,
+            text_font,
+            text_font_size,
+            text_font_colour,
+            style,
         )
         match style:
             case "rectangle":
                 self.draw_box(
                     box_x1,
                     box_y1,
                     box_width,
@@ -326,14 +515,29 @@
             case "arrowhead":
                 self.draw_arrowhead_box(
                     box_x1, box_y1, box_width, box_height, box_fill_colour
                 )
             case _:
                 raise ValueError("Invalid style")
 
+        font = ImageFont.truetype(self.get_font_path(text_font), size=text_font_size)
+
+        multi_lines = []
+        wrap_lines = []
+
+        ### Make '\n' work
+        multi_lines = text.splitlines()
+
+        left, _, right, _ = font.getbbox("a")
+        single_char_width = right - left
+
+        ### wrap text
+        for line in multi_lines:
+            wrap_lines.extend(textwrap.wrap(line, int(box_width / single_char_width)))
+
         pad = 4
         line_count = len(wrap_lines)
 
         for i, line in enumerate(wrap_lines):
             font_width, font_height = self.get_text_dimension(
                 line, text_font, text_font_size
             )
@@ -370,20 +574,15 @@
             y (int): Y coordinate
             width (int): Diamond width
             height (int): Diamond height
             fill_colour (str): Diamond fill colour in HTML colour name or hex code. Eg. #FFFFFF or LightGreen
         """
 
         # Calculate the coordinates of the four points of the diamond.
-        points = [
-            (x + width / 2, y),
-            (x + width, y + height / 2),
-            (x + width / 2, y + height),
-            (x, y + height / 2),
-        ]
+        points = super().draw_diamond(x, y, width, height, fill_colour)
 
         # Use Pillow's ImageDraw module to draw a polygon with the given points and fill color.
         self.__cr.polygon(points, fill=fill_colour)
 
     def draw_text(
         self, x: int, y: int, text: str, font: str, font_size: int, font_colour: str
     ) -> None:
@@ -398,27 +597,14 @@
             (x, y),
             text,
             font=ImageFont.truetype(self.get_font_path(font), font_size),
             anchor="la",
             fill=(font_colour),
         )
 
-    def set_line_style(self, style: str = "solid") -> None:
-        """Set line style
-
-        Args:
-            style (str, optional): Line style. Defaults to "solid". Options: "solid", "dashed"
-        """
-        if style == "solid":
-            self.dash = None
-        elif style == "dashed":
-            self.dash = (10.0, 5.0)
-        else:
-            self.dash = None
-
     def draw_line(
         self,
         x1: int,
         y1: int,
         x2: int,
         y2: int,
         line_colour: str,
@@ -524,76 +710,38 @@
 
         Returns:
             (text_width (int), text_height (int)): Text dimension (width, height)
         """
         # Use Pillow's ImageFont module to get the dimensions of the text.
         image_font = ImageFont.truetype(self.get_font_path(font), font_size)
 
-        ascent, descent = image_font.getmetrics()
-
         left, _, right, bottom = image_font.getbbox(text)
         font_width = right
         font_height = bottom
 
         return font_width, font_height
 
     def set_background_colour(self) -> None:
         """Set surface background colour"""
-        self.__cr.rectangle(
-            (0, 0, self.width, self.height), fill=self.background_colour
-        )
-
-    def get_display_text_position(
-        self,
-        x: int,
-        y: int,
-        width: int,
-        height: int,
-        text: str,
-        alignment: str,
-        text_font: str,
-        text_font_size: int,
-    ) -> tuple:
-        """Get text position relative to the rectangle box
-
-        Args:
-            x (int): Rectangle X coordinate
-            y (int): Rectangle Y coordinate
-            width (int): Rectangle width
-            height (int): Rectangle height
-            text (str): Text used to calculate position
-            alignment (str): Text alignment. Eg. left, center, right
-
-        Returns:
-            (text_x (int), text_y (int)): Text x and y coordinates
-        """
-        text_width, text_height = self.get_text_dimension(
-            text, text_font, text_font_size
-        )
-
-        if alignment == "centre":
-            text_x_pos = (width / 2) - (text_width / 2)
-        elif alignment == "right":
-            text_x_pos = width - text_width - 5
-        elif alignment == "left":
-            text_x_pos = 0 + 5
-
-        text_y_pos = (height / 2) + (text_height / 2)
-
-        return x + text_x_pos, y + text_y_pos
+        if self.background_colour == "transparent":
+            # Set transparent background
+            self.__cr.rectangle((0, 0, self.width, self.height), fill=(0, 0, 0, 0))
+        else:
+            self.__cr.rectangle(
+                (0, 0, self.width, self.height), fill=self.background_colour
+            )
 
     def set_surface_size(self, width: int, height: int) -> None:
         """Set surface size
 
         Args:
             width (int): Surface width
             height (int): Surface height
         """
-        height += self.bottom_margin
-        left, top, right, bottom = 0, 0, width, height
+        left, top, right, bottom = super().set_surface_size(width, height)
         self.__surface = self.__surface.crop((left, top, right, bottom))
 
     def get_image_size(self, image: str) -> tuple:
         """Get image size
 
         Args:
             image (str): Image path
@@ -606,10 +754,331 @@
 
     def save_surface(self, filename: str) -> None:
         """Save surface to PNG file
 
         Args:
             filename (str): PNG file name
         """
-        if self.output_type == "PNG":
-            if self.__surface is not None:
-                self.__surface.save(filename)
+
+        if self.__surface is not None:
+            self.__surface.save(filename)
+
+
+class SVGPainter(Painter):
+    def __init__(self, width: int, height: int):
+        """__init__ method
+
+        Args:
+            width (int): Width of the surface
+            height (int): Height of the surface
+        """
+        super().__init__(width, height)
+        self.__cr = None
+        self.elements = []
+
+    def draw_box(
+        self, x: int, y: int, width: int, height: int, box_fill_colour: str
+    ) -> None:
+        """Draw a rectagle"""
+
+        # Create a rectangle shape
+        rectangle = dw.Rectangle(x, y, width, height, fill=box_fill_colour)
+
+        self.elements.append(rectangle)
+
+    def draw_rounded_box(
+        self, x: int, y: int, width: int, height: int, box_fill_colour: str
+    ) -> None:
+        """Draw a rounded rectagle"""
+        shape = super().draw_rounded_box(x, y, width, height, box_fill_colour)
+        radius = 20
+        rectangle = dw.Rectangle(
+            x, y, width, height, rx=radius, ry=radius, fill=box_fill_colour
+        )
+
+        self.elements.append(rectangle)
+
+    def draw_arrowhead_box(
+        self, x: int, y: int, width: int, height: int, box_fill_colour: str
+    ) -> None:
+        """Draw a rounded rectagle"""
+        box_shape, arrowhead_shape = super().draw_arrowhead_box(
+            x, y, width, height, box_fill_colour
+        )
+
+        # Draw the rectangle
+        rectangle = dw.Rectangle(x, y, width, height, fill=box_fill_colour)
+
+        # Draw the arrowhead
+        poly = dw.Lines(arrowhead_shape, fill=box_fill_colour)
+        self.elements.append(rectangle)
+        self.elements.append(poly)
+
+    def draw_box_with_text(
+        self,
+        box_x: int,
+        box_y: int,
+        box_width: int,
+        box_height: int,
+        box_fill_colour: int,
+        text: str,
+        text_alignment: str,
+        text_font: str,
+        text_font_size: int,
+        text_font_colour: str,
+        style: str = "rectangle",
+    ) -> None:
+        box_x1, box_y1, box_x2, box_y2 = super().draw_box_with_text(
+            box_x,
+            box_y,
+            box_width,
+            box_height,
+            box_fill_colour,
+            text,
+            text_alignment,
+            text_font,
+            text_font_size,
+            text_font_colour,
+            style,
+        )
+        match style:
+            case "rectangle":
+                self.draw_box(
+                    box_x1,
+                    box_y1,
+                    box_width,
+                    box_height,
+                    box_fill_colour=box_fill_colour,
+                )
+            case "rounded":
+                self.draw_rounded_box(
+                    box_x1, box_y1, box_width, box_height, box_fill_colour
+                )
+            case "arrowhead":
+                self.draw_arrowhead_box(
+                    box_x1, box_y1, box_width, box_height, box_fill_colour
+                )
+            case _:
+                raise ValueError("Invalid style")
+
+        font = ImageFont.truetype(self.get_font_path(text_font), size=text_font_size)
+
+        multi_lines = []
+        wrap_lines = []
+
+        ### Make '\n' work
+        multi_lines = text.splitlines()
+
+        left, _, right, _ = font.getbbox("a")
+        single_char_width = right - left
+
+        ### wrap text
+        for line in multi_lines:
+            wrap_lines.extend(textwrap.wrap(line, int(box_width / single_char_width)))
+
+        pad = 4
+        line_count = len(wrap_lines)
+
+        for i, line in enumerate(wrap_lines):
+            font_width, font_height = self.get_text_dimension(
+                line, text_font, text_font_size
+            )
+
+            match text_alignment:
+                case "centre":
+                    x = box_x1 + (box_width - font_width) / 2
+                case "left":
+                    x = box_x1 + 15
+                case "right":
+                    x = box_x2 - font_width - 15
+                case _:
+                    x = box_x1 + (box_width - font_width) / 2
+
+            total_line_height = (font_height * line_count) + (pad * (line_count - 1))
+
+            single_line_height = font_height
+
+            y = (
+                box_y1
+                + ((box_height - total_line_height) / 2)
+                + ((single_line_height * i) + (pad * i))
+            )
+
+            txt = dw.Text(
+                line,
+                x=x,
+                y=y,
+                font_size=text_font_size,
+                stroke=text_font_colour,
+                text_anchor="start",
+                dominant_baseline="hanging",
+                font_family=text_font,
+            )
+            self.elements.append(txt)
+
+    def draw_diamond(
+        self, x: int, y: int, width: int, height: int, fill_colour: str
+    ) -> None:
+        """Draw a diamond"""
+
+        # Calculate the coordinates of the four points of the diamond.
+        points = super().draw_diamond(x, y, width, height, fill_colour)
+
+        # Use Pillow's ImageDraw module to draw a polygon with the given points and fill color.
+        x1, y1 = points[0]
+        x2, y2 = points[1]
+        x3, y3 = points[2]
+        x4, y4 = points[3]
+        diamond = dw.Lines(x1, y1, x2, y2, x3, y3, x4, y4, fill=fill_colour)
+        self.elements.append(diamond)
+
+    def draw_text(
+        self,
+        x: int,
+        y: int,
+        text: str,
+        font: str,
+        font_size: int,
+        font_colour: str,
+    ) -> None:
+        """Draw text"""
+        txt = dw.Text(
+            text,
+            x=x,
+            y=y,
+            font_size=font_size,
+            text_anchor="start",
+            dominant_baseline="middle",
+            font_family=font,
+            stroke=font_colour,
+        )
+        self.elements.append(txt)
+
+    def draw_line(
+        self,
+        x1: int,
+        y1: int,
+        x2: int,
+        y2: int,
+        line_colour: str,
+        line_transparency: int,
+        line_width: int,
+        line_style: str = "dashed",
+    ) -> None:
+        """Draw a line"""
+        r, g, b = ImageColor.getrgb(line_colour)
+
+        def linspace(start, stop, n):
+            if n == 1:
+                yield stop
+                return
+            h = (stop - start) / (n - 1)
+            for i in range(n):
+                yield start + h * i
+
+        if line_style == "solid":
+            line = dw.Line(
+                x1,
+                y1,
+                x2,
+                y2,
+                width=line_width,
+                fill=(r, g, b, int(255 * line_transparency)),
+            )
+            self.elements.append(line)
+        elif line_style == "dashed":
+            # given a line between x1, y1 and x2, y2, divide it into multiple shorter lines
+            # and draw them with a gap in between.
+
+            ### Calculate the number of dashes
+            gap_counts = int((y2 - y1) / 7)
+
+            for i, (x, y) in enumerate(
+                zip(
+                    linspace(x1, x2, gap_counts),
+                    linspace(y1, y2, gap_counts),
+                )
+            ):
+                if i % 2 == 0:
+                    line = dw.Line(x, y, x, y + 10, stroke=line_colour)
+                    self.elements.append(line)
+
+    def draw_cross_on_box(
+        self, x1: int, y1: int, x2: int, y2: int, colour: str
+    ) -> None:
+        """Draw a cross (vertical and horizontal lines) on a box"""
+
+        cross = dw.Line(
+            x1 + ((x2 - x1) / 2), y1, x1 + ((x2 - x1) / 2), y2, stroke="red"
+        )
+        self.elements.append(cross)
+
+    def draw_logo(self, image: str, x: int, y: int, width: int, height: int) -> None:
+        """Draw a logo"""
+        logo = Image.open(image)
+        logo = logo.resize((width, height))
+        logo = logo.convert("RGBA")
+
+        logo_image = dw.Image(x, y, width, height, image, embed=True)
+        # self.__cr.apped(logo_image)
+        self.elements.append(logo_image)
+
+    def get_text_dimension(self, text: str, font: str, font_size: int) -> tuple:
+        """Get text dimension"""
+        # Use Pillow's ImageFont module to get the dimensions of the text.
+        image_font = ImageFont.truetype(self.get_font_path(font), font_size)
+
+        left, _, right, bottom = image_font.getbbox(text)
+        font_width = right
+        font_height = bottom
+
+        return font_width, font_height
+
+    def set_background_colour(self) -> None:
+        """Set surface background colour"""
+        if self.background_colour == "transparent":
+            # Set transparent background
+            bg = dw.Rectangle(0, 0, self.width, self.height, fill="white")
+        else:
+            bg = dw.Rectangle(
+                0, 0, self.width, self.height, fill=self.background_colour
+            )
+
+        # self.__cr.append(bg)
+        self.elements.append(bg)
+
+    def set_surface_size(self, width: int, height: int) -> None:
+        """Set surface size"""
+        left, top, right, bottom = super().set_surface_size(width, height)
+
+        self.__cr = dw.Drawing(right, bottom)
+        for element in self.elements:
+            self.__cr.append(element)
+
+    def get_image_size(self, image: str) -> tuple:
+        """Get image size"""
+        with Image.open(image) as img:
+            return img.size
+
+    def save_surface(self, filename: str) -> None:
+        """Save surface to PNG file"""
+
+        if self.__cr is not None:
+            self.__cr.save_svg(filename)
+
+
+class PainterFactory:
+    """A factory class to create painter objects"""
+
+    def __init__(self):
+        self._painters = {}
+
+    def get_painter(self, painter_name, width, height):
+        if painter_name not in self._painters:
+            self._painters[painter_name] = self._create_painter(
+                painter_name, width, height
+            )
+        return self._painters[painter_name]
+
+    def _create_painter(self, painter_name, width, height):
+        # Return a painter object based on the painter_name without using if statement
+        return globals()[f"{painter_name.upper()}Painter"](width, height)
```

### Comparing `roadmapper-1.2.1/src/roadmapper/roadmap.py` & `roadmapper-1.3.0/src/roadmapper/roadmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from datetime import datetime
 from dataclasses import dataclass, field
 import time
 
-from .painter import Painter
+from .painter import PainterFactory
 from .title import Title
 from .subtitle import SubTitle
 from .footer import Footer
 from .timelinemode import TimelineMode
 from .timeline import Timeline
 from .group import Group
 from .marker import Marker
@@ -40,36 +40,43 @@
     """The main Roadmap class"""
 
     width: int = field(default=1200, init=True)
     height: int = field(default=600, init=True)
     auto_height: bool = field(default=True, init=True)
     colour_theme: str = field(default="DEFAULT", init=True)
     show_marker: bool = field(default=True, init=True)
+    painter_type: str = field(default="png", init=True)
 
     _title: Title = field(default=None, init=False)
     _subtitle: SubTitle = field(default=None, init=False)
     _timeline: Timeline = field(default=None, init=False)
     _groups: list[Group] = field(default_factory=list, init=False)
     _footer: Footer = field(default=None, init=False)
     _marker: Marker = field(default=None, init=False)
     _show_generic_dates: bool = field(default=False, init=False)
     _logo: Logo = field(default=None, init=False)
 
     def __post_init__(self):
         """This method is called after __init__() is called"""
         self.start_time = time.time()
-        self._painter = Painter(self.width, self.height)
+        factory = PainterFactory()
+        self._painter = factory.get_painter(self.painter_type, self.width, self.height)
         self._set_colour_theme(self.colour_theme)
         self._groups = []
         if self.show_marker == True:
             self._create_marker()
 
     def _set_colour_theme(self, palette: str) -> None:
         """This method sets the colour palette"""
         self._painter.set_colour_theme(palette)
+        
+    def set_background_colour(self, colour: str) -> None:
+        """This method sets the background colour"""
+        self._painter.background_colour = colour
+        self._painter.set_background_colour()
 
     def _create_marker(
         self,
         label_text_font: str = "",
         label_text_colour: str = "",
         label_text_size: int = 0,
         line_colour: str = "",
```

### Comparing `roadmapper-1.2.1/src/roadmapper/subtitle.py` & `roadmapper-1.3.0/src/roadmapper/subtitle.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,10 +64,11 @@
 
     def draw(self, painter: Painter) -> None:
         """Draw the title
 
         Args:
             painter (Painter): Pillow wrapper class instance
         """
+
         painter.draw_text(
             self.x, self.y, self.text, self.font, self.font_size, self.font_colour
         )
```

### Comparing `roadmapper-1.2.1/src/roadmapper/task.py` & `roadmapper-1.3.0/src/roadmapper/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,23 +545,23 @@
             height = box[3]
 
         box_width, box_height = (
             width,
             height,
         )
 
-        if (box_x == 0 and box_y == 0 and box_width == 0 and box_height == 0) != True:
+        if box_x != 0 or box_y != 0 or box_width != 0 or box_height != 0:
             painter.draw_box_with_text(
                 box_x,
                 box_y,
                 box_width,
                 box_height,
                 self.fill_colour,
                 self.text,
-                "centre",
+                self.text_alignment,
                 self.font,
                 self.font_size,
                 self.font_colour,
                 style=self.style,
             )
 
             for task in self.tasks:
```

### Comparing `roadmapper-1.2.1/src/roadmapper/timeline.py` & `roadmapper-1.3.0/src/roadmapper/timeline.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/timelineitem.py` & `roadmapper-1.3.0/src/roadmapper/timelineitem.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/timelineitemyear.py` & `roadmapper-1.3.0/src/roadmapper/timelineitemyear.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/timelinelocale.py` & `roadmapper-1.3.0/src/roadmapper/timelinelocale.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/timelinemode.py` & `roadmapper-1.3.0/src/roadmapper/timelinemode.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper/title.py` & `roadmapper-1.3.0/src/roadmapper/title.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/roadmapper.egg-info/PKG-INFO` & `roadmapper-1.3.0/src/roadmapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadmapper
-Version: 1.2.1
+Version: 1.3.0
 Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/roadmapper
 Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,16 +40,18 @@
 
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
-* Pillow 9.5.0
-* python-dateutil 2.8.2
+* python-dateutil >= 2.8.2
+* Pillow >= 10.0.0
+* drawsvg >= 2.2.0
+
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
 ## Installation
@@ -68,14 +70,15 @@
 ## Documentation
 Please refer to [Roadmapper Wiki](https://github.com/csgoh/roadmap-generator/wiki) for more information on how to use this RaC library.
 
 <br/>
 <hr>
 
 ## Code Example
+:point_right: Note: In order for the following code to work, you will need to download the `matariki-tech-logo.png` file to your local storage. The png file can be downloaded in the `\images\logo\` folder.
 
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
```

### Comparing `roadmapper-1.2.1/src/roadmapper.egg-info/SOURCES.txt` & `roadmapper-1.3.0/src/roadmapper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 src/roadmapper.egg-info/requires.txt
 src/roadmapper.egg-info/top_level.txt
 src/tests/__init__.py
 src/tests/compare_generated_roadmaps_test.py
 src/tests/conftest.py
 src/tests/roadmap_draw_test.py
 src/tests/test_cases.py
-src/tests/test_generate_roadmap.py
+src/tests/test_cases_svg.py
 src/tests/test_painter.py
 src/tests/test_roadmapper.py
+src/tests/test_roadmapper_svg.py
 src/tests/roadmap_generators/__init__.py
+src/tests/roadmap_generators/colour_theme.py
 src/tests/roadmap_generators/colour_theme_extensive.py
 src/tests/roadmap_generators/roadmap_abc.py
 src/tests/roadmap_generators/roadmap_generator.py
```

### Comparing `roadmapper-1.2.1/src/tests/compare_generated_roadmaps_test.py` & `roadmapper-1.3.0/src/tests/compare_generated_roadmaps_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,90 @@
 import os
 from typing import Type
 
 import pytest
 from PIL import Image, ImageChops
 
 from src.tests.roadmap_generators import roadmap_generator
+from src.tests.roadmap_generators.colour_theme import ColourTheme
 from src.tests.roadmap_generators.colour_theme_extensive import ColourThemeExtensive
 from src.tests.roadmap_generators.roadmap_abc import RoadmapABC
 
 dir_for_examples = "example_roadmaps"
 dir_for_generated = "generated_roadmaps"
 dir_for_diffs = "diffs_of_generated_roadmaps"
 
 suffix_for_examples = "Example"
 file_ending_for_examples = ".png"
 
 suffix_for_diffs = "Diff"
 file_ending_for_diffs = file_ending_for_examples
 
 
-def get_example_file_path(roadmap_class: Type[RoadmapABC]) -> str:
-    return dir_for_examples \
-        + "/" \
-        + roadmap_generator.get_roadmap_name_for(roadmap_class) \
-        + suffix_for_examples \
-        + file_ending_for_examples
-
-
-def get_example_roadmap_image(roadmap_class: Type[RoadmapABC]) -> Image:
-    path_of_example = get_example_file_path(roadmap_class)
-    return Image.open(path_of_example).convert("RGB")
-
-
-def get_generated_roadmap_image(roadmap_class: Type[RoadmapABC]) -> Image:
-    path_of_generated = roadmap_generator.get_generated_file_path_for(roadmap_class)
-    return Image.open(path_of_generated).convert("RGB")
-
-
 def ensure_presence_of_file_directory(directory):
     if directory and not os.path.exists(directory):
         os.makedirs(directory)
 
 
-def get_diff_file_path(roadmap_class: Type[RoadmapABC]) -> str:
+def get_diff_file_path_for(roadmap_class: Type[RoadmapABC], operating_system: str) -> str:
     ensure_presence_of_file_directory(dir_for_diffs)
     return dir_for_diffs \
         + "/" \
-        + roadmap_generator.get_roadmap_name_for(roadmap_class) \
+        + roadmap_generator.get_roadmap_name_for(roadmap_class, operating_system) \
         + suffix_for_diffs \
         + file_ending_for_diffs
 
 
-def handle_difference(diff, roadmap_class: Type[RoadmapABC]):
+def handle_difference(diff, roadmap_class: Type[RoadmapABC], operating_system: str):
     print("The generated roadmap looks different from the example.")
     print("Run the test locally to see the generated difference.")
-    diff_file_path = get_diff_file_path(roadmap_class)
+    diff_file_path = get_diff_file_path_for(roadmap_class, operating_system)
     diff.save(diff_file_path)
 
 
-@pytest.mark.ubuntu
+def get_generated_roadmap_image_for(roadmap_class: Type[RoadmapABC], operating_system: str) -> Image:
+    path_of_generated = roadmap_generator.get_generated_file_path_for(roadmap_class, operating_system)
+    return Image.open(path_of_generated).convert("RGB")
+
+
+def get_example_file_path_for(roadmap_class: Type[RoadmapABC], operating_system: str) -> str:
+    return dir_for_examples \
+        + "/" \
+        + roadmap_generator.get_roadmap_name_for(roadmap_class, operating_system) \
+        + suffix_for_examples \
+        + file_ending_for_examples
+
+
+def get_example_roadmap_image_for(roadmap_class: Type[RoadmapABC], operating_system: str) -> Image:
+    path_of_example = get_example_file_path_for(roadmap_class, operating_system)
+    return Image.open(path_of_example).convert("RGB")
+
+
+def compare_generated_roadmap_to_example(example_roadmap, generated_roadmap, operating_system, roadmap_class_to_test):
+    test_diff = ImageChops.difference(example_roadmap, generated_roadmap)
+    if test_diff.getbbox():
+        handle_difference(test_diff, roadmap_class_to_test, operating_system)
+        assert False
+    else:
+        assert True
+
+
+def generate_and_compare_roadmap_for_specific_platform(operating_system, roadmap_class_to_test):
+
+    roadmap_generator.generate_and_save_roadmap(roadmap_class_to_test, operating_system, dir_for_generated)
+    generated_roadmap = get_generated_roadmap_image_for(roadmap_class_to_test, operating_system)
+    example_roadmap = get_example_roadmap_image_for(roadmap_class_to_test, operating_system)
+
+    compare_generated_roadmap_to_example(example_roadmap, generated_roadmap, operating_system, roadmap_class_to_test)
+
+
 class TestCompareGeneratedRoadmaps:
-    def test_colour_theme_extensive(self):
-        roadmap_class_to_test = ColourThemeExtensive
-        roadmap_generator.generate_and_save_roadmap_in(roadmap_class_to_test, dir_for_generated)
-        example_roadmap = get_example_roadmap_image(roadmap_class_to_test)
-        generated_roadmap = get_generated_roadmap_image(roadmap_class_to_test)
-
-        test_diff = ImageChops.difference(example_roadmap, generated_roadmap)
-
-        if test_diff.getbbox():
-            handle_difference(test_diff, roadmap_class_to_test)
-            assert False
-        else:
-            assert True
+
+    @pytest.mark.ubuntu
+    @pytest.mark.parametrize("roadmap_class_to_test", [ColourThemeExtensive, ColourTheme])
+    def test_compare_generated_roadmaps_on_ubuntu(self, roadmap_class_to_test, operating_system_ubuntu):
+        generate_and_compare_roadmap_for_specific_platform(operating_system_ubuntu, roadmap_class_to_test)
+
+    @pytest.mark.macos
+    @pytest.mark.parametrize("roadmap_class_to_test", [ColourThemeExtensive, ColourTheme])
+    def test_compare_generated_roadmaps_on_macos(self, roadmap_class_to_test, operating_system_macos):
+        generate_and_compare_roadmap_for_specific_platform(operating_system_macos, roadmap_class_to_test)
```

### Comparing `roadmapper-1.2.1/src/tests/roadmap_draw_test.py` & `roadmapper-1.3.0/src/tests/roadmap_draw_test.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.2.1/src/tests/roadmap_generators/colour_theme_extensive.py` & `roadmapper-1.3.0/src/tests/roadmap_generators/colour_theme_extensive.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,11 +158,11 @@
 
 def is_arg_given():
     return len(sys.argv) > 1
 
 
 if __name__ == '__main__':
     if is_arg_given():
-        example_name = sys.argv[0]
+        example_name = sys.argv[1]
         ColourThemeExtensive().generate_and_save_as(file_name=example_name)
     else:
         ColourThemeExtensive().generate_and_save_as()
```

### Comparing `roadmapper-1.2.1/src/tests/test_cases.py` & `roadmapper-1.3.0/src/tests/test_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1322,7 +1322,59 @@
                     parallel_task1.add_milestone("Milestone 2", "2023-08-10")
                 task1.add_milestone(
                     "Milestone 1",
                     "2023-04-01",
                 )
         my_roadmap.draw()
         my_roadmap.save("../../images/with_context_manager.png")
+        
+def test_black_blackground():
+    with Roadmap(
+        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
+    ) as my_roadmap:
+        my_roadmap.set_background_colour("black")
+        my_roadmap.set_title("Black Background Test Roadmap")
+        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
+        with my_roadmap.add_group("Workstream 1") as group1:
+            with group1.add_task(
+                "Task 1-A",
+                "2023-01-01",
+                "2023-04-30",
+            ) as task1:
+                with task1.add_parallel_task(
+                    "Task 2-B",
+                    "2023-05-15",
+                    "2023-08-30",
+                ) as parallel_task1:
+                    parallel_task1.add_milestone("Milestone 2", "2023-08-10")
+                task1.add_milestone(
+                    "Milestone 1",
+                    "2023-04-01",
+                )
+        my_roadmap.draw()
+        my_roadmap.save("../../images/black_roadmap.png")
+        
+def test_transparent_blackground():
+    with Roadmap(
+        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
+    ) as my_roadmap:
+        my_roadmap.set_background_colour("transparent")
+        my_roadmap.set_title("Transparent Background Test Roadmap")
+        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
+        with my_roadmap.add_group("Workstream 1") as group1:
+            with group1.add_task(
+                "Task 1-A",
+                "2023-01-01",
+                "2023-04-30",
+            ) as task1:
+                with task1.add_parallel_task(
+                    "Task 2-B",
+                    "2023-05-15",
+                    "2023-08-30",
+                ) as parallel_task1:
+                    parallel_task1.add_milestone("Milestone 2", "2023-08-10")
+                task1.add_milestone(
+                    "Milestone 1",
+                    "2023-04-01",
+                )
+        my_roadmap.draw()
+        my_roadmap.save("../../images/transparent_roadmap.png")
```

### Comparing `roadmapper-1.2.1/src/tests/test_painter.py` & `roadmapper-1.3.0/src/tests/test_painter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from src.roadmapper.painter import Painter
+from src.roadmapper.painter import PNGPainter
 
 
 class TestPainter:
     def test_init(self):
-        painter = Painter(800, 600)
+        painter = PNGPainter(800, 600)
         assert painter.width == 800
         assert painter.height == 600
 
     # Tests that the colour theme is correctly set and that subsequent shapes and text are drawn with the correct colours.
     def test_set_colour_theme(self):
-        painter = Painter(500, 500)
+        painter = PNGPainter(500, 500)
         painter.set_colour_theme("ORANGEPEEL")
         assert painter.title_font == "Arial"
         assert painter.title_font_size == 26
         assert painter.title_font_colour == "#B45F06"
         assert painter.subtitle_font == "Arial"
         assert painter.subtitle_font_size == 18
         assert painter.subtitle_font_colour == "#B45F06"
@@ -44,22 +44,22 @@
         assert painter.milestone_fill_colour == "#B45F06"
         assert painter.footer_font == "Arial"
         assert painter.footer_font_size == 13
         assert painter.footer_font_colour == "#B45F06"
 
     # Tests that the get_text_dimension() method correctly calculates the dimensions of text for different fonts and font sizes.
     def test_get_text_dimension(self):
-        painter = Painter(100, 100)
+        painter = PNGPainter(100, 100)
         text = "Hello World"
         font = "Arial"
         font_size = 12
         width, height = painter.get_text_dimension(text, font, font_size)
         assert width > 0
         assert height > 0
 
     def test_get_text_dimension2(self):
-        painter = Painter(800, 600)
+        painter = PNGPainter(800, 600)
         text_width, text_height = painter.get_text_dimension("Hello World", "Arial", 12)
         print(f"text_width: {text_width}, text_height: {text_height}")
         # Linux returns different text width
-        assert (text_width == 62) or (text_width == 64)
+        assert text_width in [62, 64]
         assert text_height == 11
```

### Comparing `roadmapper-1.2.1/src/tests/test_roadmapper.py` & `roadmapper-1.3.0/src/tests/test_roadmapper_svg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import os
 from datetime import datetime
+
 from src.roadmapper.roadmap import Roadmap
 from src.roadmapper.timelinemode import TimelineMode
 import inspect
 
 
 def colour_theme_demo(
     mode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("SAMPLE ROADMAP 2022/2023")
     roadmap.set_subtitle("ABC Corporation")
     roadmap.set_timeline(
         mode,
         start_date,
         number_of_items,
@@ -47,19 +53,24 @@
 
 
 def colour_theme_demo_without_locale(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("SAMPLE ROADMAP 2022/2023")
     roadmap.set_subtitle("ABC Corporation")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -87,20 +98,25 @@
 
 def chinese_theme_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
     show_first_day_of_week=False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("示例路線圖 2022/2023")
     roadmap.set_subtitle("甲乙丙有限公司")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -130,20 +146,25 @@
 
 def japanese_theme_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
     show_first_day_of_week=False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("ロードマップの例 2022/2023")
     roadmap.set_subtitle("株式会社エー・ビー・シー")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -173,18 +194,20 @@
 
 def generic_date_test(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-11-01",
     number_of_items: int = 24,
     show_generic_dates: bool = False,
     show_first_day_of_week: bool = False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
-    roadmap = Roadmap(4400, 2000, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        4400, 2000, colour_theme=colour_theme, show_marker=True, painter_type="svg"
+    )
     roadmap.set_title("My Demo Roadmap!!!")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         show_first_day_of_week=show_first_day_of_week,
@@ -208,23 +231,24 @@
     roadmap.save(file_name)
 
 
 def parallel_task_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 14,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     roadmap = Roadmap(
         1200,
         612,
         auto_height=False,
         colour_theme=colour_theme,
         show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("ROADMAP EXAMPLE 2022/2023")
     roadmap.set_subtitle("This is a subtitle")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -249,24 +273,24 @@
     roadmap.save(file_name)
 
 
 def singleton_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2023-01-01",
     number_of_items: int = 2,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "BLUEMOUNTAIN",
 ) -> None:
-
     roadmap = Roadmap(
         600,
         612,
         auto_height=True,
         colour_theme=colour_theme,
         show_marker=False,
+        painter_type="svg",
     )
     roadmap.set_title("ROADMAP EXAMPLE")
     # roadmap.set_subtitle("This is a subtitle")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -286,31 +310,32 @@
     roadmap.save(file_name)
 
 
 def logo_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2023-01-01",
     number_of_items: int = 2,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "BLUEMOUNTAIN",
     auto_height: bool = True,
     logo_position: str = "top-left",
 ) -> None:
     file_name = "T_" + file_name
     roadmap = Roadmap(
         800,
         612,
         auto_height=auto_height,
         colour_theme=colour_theme,
         show_marker=False,
+        painter_type="svg",
     )
     frameinfo = inspect.getframeinfo(inspect.currentframe())
     title = f"{frameinfo.function}(), theme={colour_theme}, mode={timelinemode}"
 
-    roadmap.add_logo("images/logo/matariki-tech-logo.png", logo_position, 50, 50)
+    roadmap.add_logo("../../images/logo/matariki-tech-logo.png", logo_position, 50, 50)
     roadmap.set_title(title)
     roadmap.set_subtitle("This is a subtitle")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=False,
@@ -327,49 +352,59 @@
     roadmap.save(file_name)
 
 
 def test_dev():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    if not os.path.exists("images/test"):
-        os.mkdir("images/test")
+    if not os.path.exists("../../images/test"):
+        os.mkdir("../../images/test")
 
-    output_file = "images/test/colour_theme_demo_without_locale.png"
+    output_file = "../../images/test/colour_theme_demo_without_locale.svg"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     colour_theme_demo_without_locale(
         file_name=output_file,
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=14,
     )
 
     assert os.path.exists(output_file)
 
-    output_file = "images/test/demo-my-colour-chinese.png"
+    output_file = "../../images/test/demo-my-colour-chinese.svg"
     chinese_theme_demo(
         file_name=output_file,
         colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.WEEKLY,
         start_date="2023-01-01",
         number_of_items=14,
         locale_name="../json/zh_TW_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
     assert os.path.exists(output_file)
 
-    output_file = "images/test/demo-my-colour-japanese.png"
+    output_file = "../../images/test/demo-my-colour-japanese.svg"
     japanese_theme_demo(
         file_name=output_file,
         colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.MONTHLY,
         start_date="2023-01-01",
         number_of_items=14,
         locale_name="../json/ja_JP_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
 
     assert os.path.exists(output_file)
+
+
+# check if calling from main
+if __name__ == "__main__":
+    output_file = "../../images/test/colour_theme_demo_without_locale.svg"
+    colour_theme_demo_without_locale(
+        file_name=output_file,
+        timelinemode=TimelineMode.MONTHLY,
+        number_of_items=14,
+    )
```

