# Comparing `tmp/gpx-concatenator-1.0.tar.gz` & `tmp/gpx-concatenator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx-concatenator-1.0.tar", last modified: Sun Jul  9 14:05:12 2023, max compression
+gzip compressed data, was "gpx-concatenator-1.0.1.tar", last modified: Sun Jul  9 14:40:15 2023, max compression
```

## Comparing `gpx-concatenator-1.0.tar` & `gpx-concatenator-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:05:12.925641 gpx-concatenator-1.0/
--rw-r--r--   0 teolebras   (501) staff       (20)      154 2023-07-09 14:05:12.924683 gpx-concatenator-1.0/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)     3980 2023-07-09 12:34:30.000000 gpx-concatenator-1.0/README.md
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:05:12.912188 gpx-concatenator-1.0/gpx_concatenator/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0/gpx_concatenator/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0/gpx_concatenator/gpx_colorizer.py
--rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0/gpx_concatenator/gpx_concatenator.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0/gpx_concatenator/gpx_file.py
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:05:12.917355 gpx-concatenator-1.0/gpx_concatenator.egg-info/
--rw-r--r--   0 teolebras   (501) staff       (20)      154 2023-07-09 14:05:12.000000 gpx-concatenator-1.0/gpx_concatenator.egg-info/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)      386 2023-07-09 14:05:12.000000 gpx-concatenator-1.0/gpx_concatenator.egg-info/SOURCES.txt
--rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-09 14:05:12.000000 gpx-concatenator-1.0/gpx_concatenator.egg-info/dependency_links.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-09 14:05:12.000000 gpx-concatenator-1.0/gpx_concatenator.egg-info/entry_points.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-09 14:05:12.000000 gpx-concatenator-1.0/gpx_concatenator.egg-info/top_level.txt
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:05:12.920925 gpx-concatenator-1.0/scripts/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0/scripts/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1194 2023-07-09 14:02:58.000000 gpx-concatenator-1.0/scripts/main.py
--rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-09 14:05:12.925900 gpx-concatenator-1.0/setup.cfg
--rw-r--r--   0 teolebras   (501) staff       (20)      368 2023-07-09 14:04:56.000000 gpx-concatenator-1.0/setup.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:40:15.016413 gpx-concatenator-1.0.1/
+-rw-r--r--   0 teolebras   (501) staff       (20)     1070 2023-07-09 14:10:22.000000 gpx-concatenator-1.0.1/LICENSE
+-rw-r--r--   0 teolebras   (501) staff       (20)     3997 2023-07-09 14:40:15.015863 gpx-concatenator-1.0.1/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)     3777 2023-07-09 14:15:47.000000 gpx-concatenator-1.0.1/README.md
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:40:14.888907 gpx-concatenator-1.0.1/gpx_concatenator/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0.1/gpx_concatenator/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.1/gpx_concatenator/gpx_colorizer.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0.1/gpx_concatenator/gpx_concatenator.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.1/gpx_concatenator/gpx_file.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:40:14.987664 gpx-concatenator-1.0.1/gpx_concatenator.egg-info/
+-rw-r--r--   0 teolebras   (501) staff       (20)     3997 2023-07-09 14:40:14.000000 gpx-concatenator-1.0.1/gpx_concatenator.egg-info/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)      394 2023-07-09 14:40:14.000000 gpx-concatenator-1.0.1/gpx_concatenator.egg-info/SOURCES.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-09 14:40:14.000000 gpx-concatenator-1.0.1/gpx_concatenator.egg-info/dependency_links.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-09 14:40:14.000000 gpx-concatenator-1.0.1/gpx_concatenator.egg-info/entry_points.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-09 14:40:14.000000 gpx-concatenator-1.0.1/gpx_concatenator.egg-info/top_level.txt
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-09 14:40:15.014877 gpx-concatenator-1.0.1/scripts/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0.1/scripts/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1194 2023-07-09 14:02:58.000000 gpx-concatenator-1.0.1/scripts/main.py
+-rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-09 14:40:15.016670 gpx-concatenator-1.0.1/setup.cfg
+-rw-r--r--   0 teolebras   (501) staff       (20)      585 2023-07-09 14:39:24.000000 gpx-concatenator-1.0.1/setup.py
```

### Comparing `gpx-concatenator-1.0/README.md` & `gpx-concatenator-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,70 @@
-# GPX File Concatenator
+# GPX Concatenator
 
-This project provides a set of Python scripts for concatenating and colorizing GPX (GPS Exchange Format) files. It allows you to combine multiple GPX files into a single output file and optionally add colorization to the tracks.
+GPX Concatenator is a Python project that provides a set of scripts for concatenating and colorizing GPX (GPS Exchange Format) files.
 
 ## Files
 
 The project consists of the following files:
 
-1. **gpx_concatenator.py**: This file contains the `GPXConcatenator` class, which handles the concatenation of multiple GPX files. It takes a list of input file paths, an output file path, and optional flags to enable metadata and colorization. The `concatenate_files` method iterates over the input files, extracts the tracks using the `GPXFile` class, and appends them to the output GPX file's XML structure. If colorization is enabled, it utilizes the `GPXColorizer` class to assign colors to the tracks and add color metadata to the GPX file.
+1. **gpx_concatenator.py**: This file contains the `GPXConcatenator` class, responsible for concatenating multiple GPX files. It takes a list of input file paths, an output file path, and optional flags to enable metadata and colorization. The `concatenate_files` method extracts tracks from the input files using the `GPXFile` class and appends them to the output GPX file's XML structure. If colorization is enabled, the `GPXColorizer` class assigns distinct colors to the tracks and adds color metadata to the GPX file.
 
-2. **gpx_colorizer.py**: This file contains the `GPXColorizer` class, which is responsible for colorizing tracks in a GPX file. It provides methods for assigning distinct colors to each track based on its name. The `_generate_distinct_colors` method generates a list of distinct colors based on the number of tracks. The `_add_color_extensions` method adds color information to the GPX file's XML structure, and the `colorize_tracks` method applies colorization to the tracks.
+2. **gpx_colorizer.py**: This file contains the `GPXColorizer` class, which colorizes tracks in a GPX file. It assigns distinct colors to each track based on its name and adds color information to the GPX file's XML structure.
 
-3. **gpx_file.py**: This file contains the `GPXFile` class, which provides methods for working with individual GPX files. The `__init__` method initializes the class with a file path and parses the XML structure of the GPX file. The `extract_metadata` method extracts the metadata element from the GPX file's XML structure, and the `extract_tracks` method extracts a list of track elements from the XML structure.
+3. **gpx_file.py**: This file contains the `GPXFile` class, providing methods for working with individual GPX files. It initializes with a file path, parses the GPX file's XML structure, and extracts metadata and track elements.
 
-4. **main.py**: This file serves as the entry point of the project. It demonstrates how to use the `GPXConcatenator` class to concatenate and colorize GPX files. The script initializes the `GPXConcatenator` class with a list of input file paths, an output file path, and flags to enable metadata and colorization. It then calls the `concatenate_files` method to perform the concatenation and colorization process.
+4. **main.py**: This file serves as the entry point of the project. It demonstrates how to use the `GPXConcatenator` class to concatenate and colorize GPX files. The script initializes the `GPXConcatenator` class with input file paths, an output file path, and flags for metadata and colorization. The `concatenate_files` method performs the concatenation and colorization process.
+
+## Installation
+
+To install `gpx-concatenator`, you can use pip, the Python package manager. Open a terminal and run the following command:
+
+```
+pip install gpx-concatenator
+```
 
 ## Usage
 
-To use this project, follow these steps:
+Once installed, you can use the `gpx-concatenator` command to concatenate and colorize GPX files. Here's an example usage:
+
+```
+gpx-concatenator --input-dir <input-directory> --output-file <output-file-name> --enable-metadata --enable-coloring
+```
+
+Replace `<input-directory>` with the directory containing the input GPX files, and `<output-file-name>` with the desired name of the output GPX file. The `--enable-metadata` flag enables metadata in the output file, and the `--enable-coloring` flag enables coloring of the tracks.
 
-1. Place the GPX files that you want to concatenate in the `input` directory or specify a different input directory using the `--input-dir` command-line parameter.
+### Command-line Arguments
 
-2. Run the `main.py` script using a Python interpreter and specify the desired command-line parameters. Here are some examples:
+The following command-line arguments are available:
 
-   ```shell
-   # Run the script with default parameters
-   python main.py
+- `--input-dir`: Specifies the directory containing the input GPX files. The default value is `input`.
 
-   # Specify a different input directory
-   python main.py --input-dir my_input_dir
+- `--output-file`: Specifies the name of the output GPX file. The default value is `output.gpx`.
 
-   # Specify a different output file name
-   python main.py --output-file my_output.gpx
+- `--enable-metadata`: Enables metadata in the output GPX file. This is an optional flag.
 
-   # Enable metadata and coloring
-   python main.py --enable-metadata --enable-coloring
-The concatenated and colorized GPX file will be generated based on the specified parameters.
+- `--enable-coloring`: Enables coloring of the tracks in the output GPX file. This is an optional flag.
 
-## Requirements
+For more information on available command-line arguments, use the `--help` flag:
 
-- Python 3.x
-- The following Python packages: `xml.etree.ElementTree`, `xml.dom.minidom`
+```
+gpx-concatenator --help
+```
 
-## Disclaimer
+### Input Files
 
-This project is provided as-is without any warranty. Use it at your own risk.
+Place the GPX files that you want to concatenate in the specified input directory. The files will be concatenated in alphabetical order based on their names.
 
-Please ensure that you have the necessary permissions and rights to use the GPX files you provide as input.
+### Output File
 
-## Contributions
+The concatenated GPX file will be created with the specified name in the current working directory. If the file already exists, it will be overwritten.
 
-Contributions to this project are welcome! If you find any issues or have ideas for improvements, feel free to submit a pull request or open an issue.
+## License
 
-We appreciate your feedback and contributions to make this project better.
+This project is licensed under the MIT License.
 
 
      _                 _          _                         
     (_)               | |        (_)                        
      _  __ _ _ __ ___ | |__  _ __ _  __ _ _ __  _ __   __ _ 
     | |/ _` | '_ ` _ \| '_ \| '__| |/ _` | '_ \| '_ \ / _` |
     | | (_| | | | | | | |_) | |  | | (_| | | | | | | | (_| |
```

### Comparing `gpx-concatenator-1.0/gpx_concatenator/gpx_colorizer.py` & `gpx-concatenator-1.0.1/gpx_concatenator/gpx_colorizer.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0/gpx_concatenator/gpx_concatenator.py` & `gpx-concatenator-1.0.1/gpx_concatenator/gpx_concatenator.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0/gpx_concatenator/gpx_file.py` & `gpx-concatenator-1.0.1/gpx_concatenator/gpx_file.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0/scripts/main.py` & `gpx-concatenator-1.0.1/scripts/main.py`

 * *Files identical despite different names*

