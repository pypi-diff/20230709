# Comparing `tmp/Nuitka-1.7.2.tar.gz` & `tmp/Nuitka-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-1.7.2.tar", last modified: Sat Jul  8 07:29:17 2023, max compression, from Unix
+gzip compressed data, was "Nuitka-1.7.3.tar", last modified: Sun Jul  9 21:23:18 2023, max compression, from Unix
```

## Comparing `Nuitka-1.7.2.tar` & `Nuitka-1.7.3.tar`

### file list

```diff
@@ -1,1807 +1,1807 @@
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)  2833663 2023-07-08 07:29:13.000000 Nuitka-1.7.2/Changelog.pdf
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   843525 2023-07-08 07:28:59.000000 Nuitka-1.7.2/Changelog.rst
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   812243 2023-07-08 07:29:07.000000 Nuitka-1.7.2/Developer_Manual.pdf
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   152515 2023-07-08 07:28:59.000000 Nuitka-1.7.2/Developer_Manual.rst
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11348 2023-07-08 07:28:59.000000 Nuitka-1.7.2/LICENSE.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1723 2023-07-08 07:28:59.000000 Nuitka-1.7.2/MANIFEST.in
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.765277 Nuitka-1.7.2/Nuitka.egg-info/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    79137 2023-07-08 07:29:15.000000 Nuitka-1.7.2/Nuitka.egg-info/PKG-INFO
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76769 2023-07-08 07:29:15.000000 Nuitka-1.7.2/Nuitka.egg-info/SOURCES.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        1 2023-07-08 07:29:15.000000 Nuitka-1.7.2/Nuitka.egg-info/dependency_links.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      393 2023-07-08 07:29:15.000000 Nuitka-1.7.2/Nuitka.egg-info/entry_points.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        1 2023-07-08 07:29:15.000000 Nuitka-1.7.2/Nuitka.egg-info/not-zip-safe
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        7 2023-07-08 07:29:15.000000 Nuitka-1.7.2/Nuitka.egg-info/top_level.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    79137 2023-07-08 07:29:15.895278 Nuitka-1.7.2/PKG-INFO
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   345695 2023-07-08 07:29:05.000000 Nuitka-1.7.2/README.pdf
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76929 2023-07-08 07:28:59.000000 Nuitka-1.7.2/README.rst
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/bin/
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1135 2023-07-08 07:28:59.000000 Nuitka-1.7.2/bin/autoformat-nuitka-source
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1134 2023-07-08 07:28:59.000000 Nuitka-1.7.2/bin/check-nuitka-with-pylint
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1150 2023-07-08 07:28:59.000000 Nuitka-1.7.2/bin/compare_with_cpython
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3079 2023-07-08 07:28:59.000000 Nuitka-1.7.2/bin/compare_with_xml
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1163 2023-07-08 07:28:59.000000 Nuitka-1.7.2/bin/measure-construct-performance
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1685 2023-07-08 07:28:59.000000 Nuitka-1.7.2/bin/nuitka
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1685 2023-07-08 07:28:59.000000 Nuitka-1.7.2/bin/nuitka-run
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/doc/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/doc/Logo/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7321 2023-07-08 07:28:59.000000 Nuitka-1.7.2/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7401 2023-07-08 07:28:59.000000 Nuitka-1.7.2/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17917 2023-07-08 07:28:59.000000 Nuitka-1.7.2/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/doc/images/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7585 2023-07-08 07:28:59.000000 Nuitka-1.7.2/doc/images/Nuitka-Logo-Horizontal.png
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4452 2023-07-08 07:28:59.000000 Nuitka-1.7.2/doc/images/Nuitka-Logo-Symbol.png
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9828 2023-07-08 07:28:59.000000 Nuitka-1.7.2/doc/images/Nuitka-Logo-Vertical.png
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31239 2023-07-08 07:29:14.000000 Nuitka-1.7.2/doc/nuitka2-run.1
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31263 2023-07-08 07:29:14.000000 Nuitka-1.7.2/doc/nuitka2.1
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31252 2023-07-08 07:29:15.000000 Nuitka-1.7.2/doc/nuitka3-run.1
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31276 2023-07-08 07:29:15.000000 Nuitka-1.7.2/doc/nuitka3.1
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/lib/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4250 2023-07-08 07:28:59.000000 Nuitka-1.7.2/lib/hints.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/misc/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      901 2023-07-08 07:28:59.000000 Nuitka-1.7.2/misc/nuitka-run.bat
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1038 2023-07-08 07:28:59.000000 Nuitka-1.7.2/misc/nuitka.bat
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/nuitka/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7529 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Builtins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5437 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/BytecodeCaching.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3440 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Bytecodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1884 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/CacheCleanup.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11148 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Constants.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2447 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    37438 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/MainControl.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8064 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/ModuleRegistry.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    55485 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/OptionParsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65509 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Options.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5022 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/OutputDirectories.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14550 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/PostProcessing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5770 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Progress.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7472 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/PythonFlavors.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4061 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/PythonOperators.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12179 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/PythonVersions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9062 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Serialization.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4670 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/SourceCodeReferences.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11235 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Tracing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3395 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/TreeXML.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15235 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Variables.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2055 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/Version.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5615 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5295 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/__past__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/nuitka/build/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34131 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/Backend.scons
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8300 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/CCompilerVersion.scons
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2716 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/DataComposerInterface.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18756 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/Onefile.scons
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15698 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/SconsCaching.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31010 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/SconsCompilerSettings.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5527 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/SconsHacks.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15827 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/SconsInterface.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2671 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/SconsProgress.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12022 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/SconsSpawn.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24338 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/SconsUtils.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/include/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.775277 Nuitka-1.7.2/nuitka/build/include/nuitka/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7972 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/allocator.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3470 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/builtins.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4604 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/calling.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1977 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/checkers.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1261 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/checksum_tools.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9571 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2002 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_cell.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9325 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16949 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_frame.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5972 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_function.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9136 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_generator.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1838 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_method.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7408 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/constants.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1293 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/constants_blob.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34083 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/exceptions.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3473 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/filesystem_paths.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6253 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/freelists.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    86326 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/hedley.h
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3393 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/attributes.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2663 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/boolean.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1181 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1135 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/bytes.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9335 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13140 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10616 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10615 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13140 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13139 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10616 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1743 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/complex.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13109 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1206 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/floats.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3897 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/import_hard.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1798 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/indexes.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2941 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/ints.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9992 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/iterators.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3411 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/lists.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1633 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1328 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/mappings.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4573 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12685 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5663 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5641 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5663 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5422 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5460 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5115 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2799 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15778 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13210 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5791 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4714 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5115 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5824 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5438 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15100 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8670 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3767 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3753 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3767 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4846 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3011 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2727 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10626 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9201 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5147 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4349 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3011 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4975 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4826 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3297 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/raising.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2178 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1146 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1112 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/sequences.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1025 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/sets.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8419 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/slices.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1242 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/strings.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17575 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/subscripts.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5720 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helper/tuples.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14411 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/helpers.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5375 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/importing.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12979 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/incbin.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14427 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/prelude.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2870 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/printing.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1761 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/python_pgo.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2243 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/safe_string_ops.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3840 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/threading.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3144 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/tracing.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2936 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/include/nuitka/unfreezing.h
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/appdirs/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1097 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24824 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/atomicwrites/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1069 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6794 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/bin/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1331 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/bin/scons.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/clcache/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/clcache/clcache/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1585 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       93 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65424 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1491 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      243 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2522 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10517 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1915 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5404 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6438 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/glob2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1359 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/glob2/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       82 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6859 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4463 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8304 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1467 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       85 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/README.rst
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2423 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2685 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1726 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12719 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65386 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1626 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12281 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1400 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50849 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4428 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24500 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36528 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9197 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28559 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17473 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4340 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7308 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30853 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1722 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35875 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27644 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17080 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4214 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20501 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3316 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1466 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       84 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2616 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2685 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1726 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12719 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65386 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1626 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12281 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1400 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50849 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4428 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24500 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36528 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9197 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28559 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17474 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4340 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7308 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30853 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1722 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35875 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27644 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17080 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4214 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20501 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3316 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/lib/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47844 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    33996 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8083 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27693 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6938 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17622 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    96183 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7358 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21540 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16000 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9589 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4197 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   121420 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4164 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    49503 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.785278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1950 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1950 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1950 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1965 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2736 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2614 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8467 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9314 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3131 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1989 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2483 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1718 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1605 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2170 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4179 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1882 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14948 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39700 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12950 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4810 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3751 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3233 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2011 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14663 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14029 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    52665 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40719 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24133 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14053 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2305 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34903 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40510 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2166 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2433 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2859 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18084 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2078 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2004 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9248 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2784 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14869 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19499 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20832 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3763 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5149 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2290 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2328 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2657 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31283 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2379 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2267 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2681 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2720 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2796 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2147 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2936 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2935 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3432 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3785 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2777 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1711 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      142 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29618 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3428 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2681 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2433 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1844 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3472 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4782 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2025 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2256 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2460 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2639 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1810 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2333 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2140 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1902 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2077 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2043 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18600 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25816 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3328 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8394 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3953 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2309 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2945 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6919 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4381 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4658 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4224 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2168 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13881 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1804 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11380 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    72761 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6841 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3579 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2618 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4375 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2827 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2513 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1991 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1819 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2123 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2502 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4695 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1927 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2349 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2473 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5992 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1831 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3730 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13016 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3415 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    48938 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3007 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3784 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4404 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3557 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5612 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11034 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6824 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1563 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.795278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8120 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3596 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1818 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1742 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2465 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1776 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19253 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    44500 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19664 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7509 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2107 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53545 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34985 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13596 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28403 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7533 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20988 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    96818 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7752 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22350 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16068 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9565 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5239 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   135413 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5758 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    63474 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8354 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11500 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3180 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2227 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2739 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1767 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1654 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1460 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2219 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4476 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1931 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4003 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16962 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    41186 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13880 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4853 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3812 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3643 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2328 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15053 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13779 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53260 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39394 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26467 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14489 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35863 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42204 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2211 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18207 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2152 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2057 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10674 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2855 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15165 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    33537 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21762 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4464 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50660 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1667 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2316 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2475 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2840 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8618 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2226 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2978 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2977 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1653 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3827 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3389 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      313 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3631 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3444 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8494 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1753 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29765 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3472 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1630 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1977 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3686 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2580 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2948 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2655 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1645 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1859 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2765 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2386 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2189 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1944 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2123 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2085 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15791 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26195 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13924 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4041 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2351 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2987 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7808 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4956 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5235 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4808 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2475 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14751 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1847 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12588 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82939 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6883 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3663 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2660 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4904 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2877 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2567 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1652 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1868 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2088 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2176 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2366 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1658 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1976 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5335 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2583 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2515 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6756 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1873 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3773 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13982 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3201 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53803 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3064 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3818 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4459 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3643 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5579 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11655 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6504 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1647 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.805278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6869 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1784 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19816 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9002 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2149 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.815278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    56578 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35213 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11061 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27408 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7884 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21423 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    97269 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3979 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7515 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21937 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16583 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9430 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.815278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5126 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   136271 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6167 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    63768 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8183 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.815278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12836 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3087 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2107 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2630 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1674 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1536 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1311 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2076 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4356 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1805 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3860 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14831 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    41983 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14673 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.815278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7394 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4357 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3546 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1972 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15577 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.815278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13597 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53509 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42760 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26676 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14272 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36753 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    41191 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.815278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2122 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15570 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2014 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1943 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13182 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2734 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15027 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    38783 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22570 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4368 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    32724 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1578 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2228 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2386 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2616 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7993 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2141 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1661 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2893 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2889 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1567 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3742 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3296 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      343 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3534 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3259 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7461 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1663 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3379 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1544 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1891 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3616 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2377 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2437 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2526 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1557 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1772 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2677 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2206 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2096 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1851 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1954 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1995 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19180 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25826 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2588 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4649 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7652 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6064 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3931 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2266 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2900 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8622 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4577 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4517 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4113 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2387 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14473 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1752 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12902 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    84784 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6788 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3576 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4817 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2788 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2479 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1563 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1780 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1999 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2006 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2271 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1569 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1888 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4879 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2419 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2429 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6412 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1786 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3687 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12548 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4076 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    71693 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6632 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15278 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3134 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3896 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4672 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3536 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5588 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12708 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6785 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      353 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4307 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1644 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3395 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21614 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9295 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2032 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1467 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10126 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      558 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4690 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1873 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/pkg_resources/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   107452 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      538 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1591 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      283 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3687 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      283 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      287 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      307 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      888 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      596 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1106 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      857 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1376 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5943 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/gui.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10790 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    57572 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6948 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9533 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      333 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1101 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13170 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4883 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28639 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3851 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2837 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    43006 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2533 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2445 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2061 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1440 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25495 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6794 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14184 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8999 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51277 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4165 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1101 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9776 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4921 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25145 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3290 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2719 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    43298 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2559 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2445 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1132 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1440 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25542 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6746 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17711 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9122 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    52446 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4171 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1101 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9607 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4881 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25554 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3294 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2723 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42954 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2533 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2445 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1138 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1440 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25495 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6854 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14097 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8970 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51695 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4165 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1530 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18198 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10157 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4455 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3763 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/debug.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13662 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3009 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2441 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34422 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/fse.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14748 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20216 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/huf.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13930 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/mem.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26976 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11706 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2728 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2497 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3828 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15880 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.825278 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    54982 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9164 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1321 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    80283 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    66784 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2253 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7906 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   138334 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/inline_copy/zstd/zstd.h
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.835278 Nuitka-1.7.2/nuitka/build/static_src/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82114 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8250 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledCellType.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    56307 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    70973 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledCoroutineType.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35861 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledFrameType.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   100376 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledFunctionType.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    60649 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledGeneratorType.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    48526 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21638 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/CompiledMethodType.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18993 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersAllocator.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    37540 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersAttributes.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21783 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersBuiltin.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   107641 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3033 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersBytes.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13057 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersCalling.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   470655 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1617 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersChecksumTools.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2991 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersClasses.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   317872 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonEq.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4673 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   313003 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonGe.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   312414 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonGt.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   316217 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonLe.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   315628 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonLt.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   314618 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonNe.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36068 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19313 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersDeepcopy.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    38364 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersDictionaries.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24295 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7035 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersExceptions.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6668 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersFiles.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28131 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2426 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersFloats.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1774 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersHeapStorage.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14585 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersImport.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14756 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersImportHard.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18433 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersLists.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13915 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersListsGenerated.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1640 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersMappings.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3513 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersMatching.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   181243 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16700 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77943 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77782 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77943 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    67487 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1236 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    68748 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6274 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    83405 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13776 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   183202 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   188514 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3404 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    66453 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    78891 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1023 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77305 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    70465 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    68005 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   149580 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4071 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53224 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53122 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53224 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76512 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47568 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17742 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   136100 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   142211 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    74142 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82669 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    45052 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82842 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76343 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3219 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersProfiling.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3805 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersPythonPgo.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15369 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersRaising.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3758 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersSafeStrings.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3730 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersSequences.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1946 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersSlices.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26642 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersStrings.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4037 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersTuples.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5578 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/HelpersTypes.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11986 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/InspectPatcher.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/MainProgram.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    58634 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4537 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6427 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17285 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30910 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/OnefileBootstrap.c
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8021 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.845278 Nuitka-1.7.2/nuitka/code_generation/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6414 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/AsyncgenCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10599 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/AttributeCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21864 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2339 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/BranchCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16009 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/BuiltinCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35905 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/CallCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4896 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ClassCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51441 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/CodeGeneration.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2375 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/CodeHelperSelection.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14392 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/CodeHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4879 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/CodeObjectCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17570 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ComparisonCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4446 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7335 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ConditionalCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6539 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ConstantCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31186 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/Contexts.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8484 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/CoroutineCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1574 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/CtypesCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28478 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/DictCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2125 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/Emission.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9325 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ErrorCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12304 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/EvalCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8975 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ExceptionCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7350 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2093 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ExpressionCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17725 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/FrameCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27968 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/FunctionCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7690 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/GeneratorCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5943 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/GlobalConstants.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6911 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1794 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/IdCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13318 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ImportCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1396 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/Indentation.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1506 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/IndexCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1033 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/InjectCCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3432 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/IntegerCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12010 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/IteratorCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2022 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/LabelCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2612 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/LineNumberCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15906 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ListCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6375 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/LoaderCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9951 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/LocalsDictCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3135 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/LoopCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1597 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/MatchCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6291 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ModuleCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8118 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/Namify.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12777 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/OperationCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29459 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/PackageResourceCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3021 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/PrintCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5474 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/PythonAPICodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13095 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/RaisingCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3443 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/Reports.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5234 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/ReturnCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6517 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/SetCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13949 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/SliceCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9809 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/StringCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8188 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/SubscriptCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11176 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/TryCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3786 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/TupleCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14717 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/VariableCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9121 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/VariableDeclarations.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8099 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/YieldCodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.845278 Nuitka-1.7.2/nuitka/code_generation/c_types/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6069 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeBases.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3399 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1804 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1378 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3610 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5128 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5211 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3955 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19628 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2852 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeVoids.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/c_types/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.845278 Nuitka-1.7.2/nuitka/code_generation/templates/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2845 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5865 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2921 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2290 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6339 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3321 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3306 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2335 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4217 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21244 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6640 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2475 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.845278 Nuitka-1.7.2/nuitka/code_generation/templates_c/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11231 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5847 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23760 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5238 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1905 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1843 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2817 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12819 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2044 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2762 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1544 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7197 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12850 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4288 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2088 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2118 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3933 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7407 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4292 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3860 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4487 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11579 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19317 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2843 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3635 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11102 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15380 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2979 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10421 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2557 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3020 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2984 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3173 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.845278 Nuitka-1.7.2/nuitka/containers/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1435 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/containers/Namedtuples.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6553 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/containers/OrderedDicts.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      554 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/containers/OrderedSets.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4397 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/containers/OrderedSetsFallback.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/containers/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.845278 Nuitka-1.7.2/nuitka/distutils/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1964 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/distutils/Build.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14219 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/distutils/DistutilCommands.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/distutils/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.845278 Nuitka-1.7.2/nuitka/finalizations/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1224 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/finalizations/Finalization.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6110 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/finalizations/FinalizeMarkups.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/finalizations/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.855278 Nuitka-1.7.2/nuitka/freezer/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7311 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/DependsExe.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2584 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/DllDependenciesCommon.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11494 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/DllDependenciesMacOS.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7211 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/DllDependenciesPosix.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6620 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/DllDependenciesWin32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17058 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/IncludedDataFiles.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9492 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/IncludedEntryPoints.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9015 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/Onefile.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26319 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/Standalone.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/freezer/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.855278 Nuitka-1.7.2/nuitka/importing/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11007 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/IgnoreListing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2899 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/ImportCache.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6719 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/ImportResolving.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28463 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/Importing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4738 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/PreloadedPackages.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14918 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/Recursion.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10981 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/StandardLibrary.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/importing/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.855278 Nuitka-1.7.2/nuitka/nodes/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3637 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/AsyncgenNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4082 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/AttributeLookupNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13567 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/AttributeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   378745 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/AttributeNodesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3823 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinAllNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4098 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinAnyNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2496 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinComplexNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1698 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinDecodingNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2727 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4694 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinDictNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4948 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinFormatNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2142 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinHashNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5334 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinIntegerNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12723 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinIteratorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1996 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinLenNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3606 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinNextNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3240 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinOpenNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   245536 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18589 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinRangeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9067 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinRefNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3307 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinSumNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13543 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinTypeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1573 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BuiltinVarsNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26113 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/BytesNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6478 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/CallNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1550 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/Checkers.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   604445 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ChildrenHavingMixins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8448 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ClassNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6585 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/CodeObjectSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21683 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ComparisonNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30314 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ConditionalNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    46536 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ConstantRefNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12213 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ContainerMakingNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2834 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ContainerOperationNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4581 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/CoroutineNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1714 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/CtypesNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51021 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/DictionaryNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7856 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ExceptionNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7317 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ExecEvalNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    44996 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ExpressionBases.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    49273 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ExpressionBasesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21278 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ExpressionShapeMixins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12156 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/FrameNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3544 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/FunctionAttributeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39803 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/FunctionNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5376 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/FutureSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6256 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/GeneratorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6850 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/GlobalsLocalsNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76798 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/HardImportNodesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5508 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ImportHardNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    45937 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ImportNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2733 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/IndicatorMixins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1502 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/InjectCNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11228 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/IterationHandles.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11002 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/KeyValuePairNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16320 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ListOperationNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23094 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/LocalsDictNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14922 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/LocalsScopes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15581 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/LoopNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1712 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/MatchNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6534 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ModuleAttributeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30972 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ModuleNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24899 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/NodeBases.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15128 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/NodeMakingHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5550 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/NodeMetaClasses.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31894 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/OperatorNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9134 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/OperatorNodesUnary.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4202 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/OsSysNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12442 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/OutlineNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31534 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/PackageMetadataNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7901 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/PackageResourceNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3407 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/PrintNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6772 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/ReturnNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4715 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/SideEffectNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12501 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/SliceNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    94880 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/StatementBasesGenerated.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9430 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/StatementNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28658 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/StrNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3504 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/StringConcatenationNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8640 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/SubscriptNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17853 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/TryNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2405 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/TypeMatchNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11061 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/TypeNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39522 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/VariableAssignNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10746 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/VariableDelNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4574 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/VariableNameNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30982 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/VariableRefNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4748 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/VariableReleaseNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3902 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/YieldNodes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.855278 Nuitka-1.7.2/nuitka/nodes/shapes/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   156243 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4387 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4567 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/shapes/ShapeMixins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42374 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/shapes/StandardShapes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/nodes/shapes/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.855278 Nuitka-1.7.2/nuitka/optimizations/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3279 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/BytecodeDemotion.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3920 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/FunctionInlining.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2144 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/Graphs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10762 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/Optimization.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    52058 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2272 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/Tags.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40896 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/TraceCollections.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23977 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/ValueTraces.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/optimizations/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.855278 Nuitka-1.7.2/nuitka/pgo/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4663 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/pgo/PGO.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/pgo/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.855278 Nuitka-1.7.2/nuitka/plugins/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40838 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/PluginBase.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    57611 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/Plugins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/plugins/standard/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22510 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3460 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10383 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/DataFilesPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4404 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/DelvewheelPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5675 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/DillPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13744 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/DllFilesPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2062 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/EnumPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1905 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/EventletPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1880 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/GeventPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3482 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/GiPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5027 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/GlfwPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18335 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/ImplicitImports.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4948 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/KivyPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7239 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6352 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1187 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/NumpyPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6595 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1917 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/PbrPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4665 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6992 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/PmwPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50293 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2986 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/PywebViewPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1160 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/TensorflowPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12242 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/TkinterPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1140 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/TorchPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10191 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/TransformersPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3175 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/TrioPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5640 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/UpxPlugin.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   160395 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2221 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9867 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/reports/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2209 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/reports/LicenseReport.rst.j2
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17538 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/reports/Reports.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/reports/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/specs/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5911 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2786 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2541 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/BuiltinListOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26455 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/BuiltinParameterSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6065 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1159 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4802 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5263 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/HardImportSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18740 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/ParameterSpecs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/specs/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1603 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/Basics.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/commercial/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      815 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/commercial/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/data_composer/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14250 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/data_composer/DataComposer.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/data_composer/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1306 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/data_composer/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/environments/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2449 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/environments/CreateEnvironment.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3735 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/environments/Virtualenv.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/environments/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/general/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/general/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/general/dll_report/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/general/dll_report/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2366 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/general/dll_report/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/general/find_module/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3920 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/general/find_module/FindModuleCode.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/general/find_module/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/onefile_compressor/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10194 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/onefile_compressor/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1311 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/onefile_compressor/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/podman/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1872 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/podman/Podman.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/podman/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6612 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/podman/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/profiler/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/profiler/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2529 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/profiler/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/scanning/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3344 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2095 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/scanning/DisplayPackageData.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/scanning/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/specialize/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51143 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/specialize/CTypeDescriptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7685 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/specialize/Common.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39625 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/specialize/SpecializeC.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34664 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/specialize/SpecializePython.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/specialize/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/testing/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    55396 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/Common.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1483 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/Constructs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8940 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/OutputComparison.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1278 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/Pythons.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8024 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/RuntimeTracing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5371 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/SearchModes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3375 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/Valgrind.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/testing/check_reference_counts/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3064 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/testing/compare_with_cpython/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29429 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/testing/find_sxs_modules/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1949 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/testing/measure_construct_performance/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8755 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/testing/run_nuitka_tests/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36321 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.865278 Nuitka-1.7.2/nuitka/tools/watch/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/watch/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9503 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tools/watch/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/nuitka/tree/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47126 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/Building.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    74608 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ComplexCallHelperFunctions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1700 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/Extractions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2572 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/InternalModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1511 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/Operations.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2807 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationAssertStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42768 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationAssignmentStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2948 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationBooleanExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11693 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationCallExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15072 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationClasses.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    37638 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationClasses3.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6430 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationComparisonExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22111 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationContractionExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11061 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationDictionaryCreation.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14607 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationExecStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7782 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationForLoopStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29594 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationFunctionStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13437 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationImportStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6577 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationLambdaExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20962 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationMatchStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2409 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationMultidist.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8194 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationNamespacePackages.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4658 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationPrintStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15371 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationSequenceCreation.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4824 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14615 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationTryExceptStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6982 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5674 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14341 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationWithStatements.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3088 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/ReformulationYieldExpressions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12746 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/SourceHandling.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3757 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/SyntaxErrors.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22973 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/TreeHelpers.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20012 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/VariableClosure.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/tree/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/nuitka/utils/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2655 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/AppDirs.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3248 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/CStrings.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3653 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/CommandLineOptions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4297 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Distributions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5794 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Download.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12645 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Execution.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36129 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/FileOperations.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2885 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Hashing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2362 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Images.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6816 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Importing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8149 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/InstalledPythons.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2224 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/InstanceCounters.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4336 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Jinja2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1238 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Json.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4304 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/MacOSApp.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5040 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/MemoryUsage.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9062 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/ModuleNames.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4309 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/ReExecute.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3815 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Rest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22701 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/SharedLibraries.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3664 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Shebang.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2591 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Signing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6207 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/StaticLibraries.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2602 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/ThreadedExecutor.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2772 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Timing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10826 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Utils.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10574 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/WindowsFileUsage.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19540 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/WindowsResources.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6108 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/Yaml.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-08 07:28:59.000000 Nuitka-1.7.2/nuitka/utils/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      834 2023-07-08 07:28:59.000000 Nuitka-1.7.2/pyproject.toml
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       38 2023-07-08 07:29:15.895278 Nuitka-1.7.2/setup.cfg
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15624 2023-07-08 07:28:59.000000 Nuitka-1.7.2/setup.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/basics/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1766 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/AssertsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5934 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/AssignmentsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5866 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/AssignmentsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4055 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/BranchingTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1104 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/BuiltinOverload.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3749 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/BuiltinSuperTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17080 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/BuiltinsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      866 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ClassMinimalTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4764 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ClassesTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3414 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ClassesTest32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1406 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ClassesTest34.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4698 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ComparisonChainsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4639 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ConstantsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      995 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ConstantsTest27.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1628 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/DecoratorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2317 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/DefaultParametersTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1127 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/DoubleDeletionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      806 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/EmptyModuleTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14387 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ExceptionRaisingTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      961 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ExceptionRaisingTest32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1458 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ExceptionRaisingTest33.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6747 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ExecEvalTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1417 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ExtremeClosureTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1658 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/FunctionObjectsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12335 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/FunctionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3603 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/FunctionsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2627 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/FunctionsTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      890 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/FutureTest32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5809 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/GeneratorExpressionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1041 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/GeneratorExpressionsTest_37.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3824 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/GlobalStatementTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1286 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/HelloWorldTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2469 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ImportingTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1296 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/InplaceOperationsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4227 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/InspectionTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1504 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/InspectionTest_35.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1618 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/InspectionTest_36.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1671 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/LambdasTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2731 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/LateClosureAssignmentTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2923 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ListContractionsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3329 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/LoopingTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1536 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/MainProgramsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1925 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ModuleAttributesTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1988 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/OperatorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14903 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/OrderChecksTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1827 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/OrderChecksTest27.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1452 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/OverflowFunctionsTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5853 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ParameterErrorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1899 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ParameterErrorsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      863 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/PrintFutureTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1413 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/PrintingTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      878 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/RecursionTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23840 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ReferencingTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2076 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ReferencingTest27.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7819 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ReferencingTest33.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4902 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ReferencingTest35.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5092 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ReferencingTest36.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2899 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ReferencingTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1630 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/SlotsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1159 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/ThreadedGeneratorsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22966 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TrickAssignmentsTest32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1541 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TrickAssignmentsTest35.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1788 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TrickAssignmentsTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2086 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TryContinueFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2212 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TryExceptContinueTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2275 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TryExceptFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2304 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TryExceptFramesTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2842 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TryReturnFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2328 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/TryYieldFinallyTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1093 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/UnicodeTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1877 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/UnpackingTest35.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2095 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/VarargsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4879 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/WithStatementsTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3070 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/YieldFromTest33.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3821 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/run_all.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2271 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/basics/run_xml.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/onefile/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1213 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/onefile/HelloWorldTest.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1307 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/onefile/KeyboardInterruptTest.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5816 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/onefile/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/optimizations/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      958 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/ArgumentTypes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1055 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/Attributes.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1021 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/Calls.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      921 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/Conditions.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      909 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/DecodingOperations.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1212 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/FormatStrings36.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1150 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/HardImports.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      974 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/HardImports_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      918 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/Iterations.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1260 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/Len.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2262 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/Operations.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1333 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/Subscripts.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8736 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/optimizations/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/packages/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/packages/package_import_success_after_failure/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2382 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/packages/package_import_success_after_failure/variable_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      942 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1168 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3671 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/tests/packages/sub_package/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.875278 Nuitka-1.7.2/tests/packages/sub_package/kitty/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1230 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/sub_package/kitty/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      908 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/sub_package/kitty/bigkitty.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      910 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/sub_package/kitty/smallkitty.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      929 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1053 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/hello.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      966 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/miau.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      968 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/purr.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.755277 Nuitka-1.7.2/tests/packages/top_level_attributes_3/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/packages/top_level_attributes_3/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2336 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      907 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/plugins/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/plugins/code_signing/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1170 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/code_signing/CodeSigningMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/plugins/data_files/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1332 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/data_files/DataFilesMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/plugins/data_files/data_files_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      924 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/data_files/data_files_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/data_files/data_files_package/lala.txt
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/plugins/data_files/data_files_package/sub_dir/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      255 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/plugins/parameters/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1019 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/parameters/ParametersMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2168 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/parameters/parameter-using-plugin.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3861 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/plugins/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/absolute_import/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      867 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/absolute_import/foobar/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      796 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/absolute_import/foobar/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1043 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/absolute_import/foobar/foobar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      879 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/absolute_import/foobar/local.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      860 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/absolute_import/foobar/util.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports1/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports1/CasedImportingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports1/path1/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports1/path1/Some_Module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports1/path1/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports1/path2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports1/path2/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports1/path2/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports2/CasedImportingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports2/path1/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports2/path1/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports2/path1/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports2/path2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports2/path2/Some_Module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports2/path2/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports3/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1075 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports3/CasedImportingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports3/path1/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports3/path1/Some_Module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports3/path1/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports3/path2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports3/path2/Some_Module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/case_imports3/path2/Some_Package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/cyclic_imports/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      801 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      875 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      875 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      842 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/dash_import/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      888 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/dash_import/DashImportMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      817 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/dash_import/dash-module.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      817 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/dash_import/plus+module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/dash_main/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/dash_main/Dash-Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/deep/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      898 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/deep/DeepProgramMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/deep/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      980 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/deep/some_package/DeepBrother.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      909 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/deep/some_package/DeepChild.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/deep/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/deep/some_package/deep_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      876 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      952 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/deep/some_package/deep_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/dunderinit_imports/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      794 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/dunderinit_imports/package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      797 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/dunderinit_imports/package/SubModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      857 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/dunderinit_imports/package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/import_variants/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1005 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/import_variants/ImportVariationsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/import_variants/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      946 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/import_variants/some_package/Child1.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1098 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/import_variants/some_package/Child2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      822 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/import_variants/some_package/Child3.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      994 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/import_variants/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/main_raises/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      911 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/main_raises/ErrorMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/main_raises/ErrorRaising.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/main_raises2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1080 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/main_raises2/ErrorRaising.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/module_attributes/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1529 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1744 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1611 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1744 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1611 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1744 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1611 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/module_exits/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      869 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_exits/ErrorExitingModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      867 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_exits/Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/module_object_replacing/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1078 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1359 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/multiprocessing_using/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      990 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/multiprocessing_using/foo/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/multiprocessing_using/foo/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      836 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/multiprocessing_using/foo/__main__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1758 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/multiprocessing_using/foo/entry.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/named_imports/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      846 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/named_imports/NamedImportsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/named_imports/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/named_imports/some_package/SomeModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      824 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/named_imports/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/named_imports/some_package/sub_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_code/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_code/PackageInitCodeMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_code/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_code/some_package/SomeModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_code/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_contains_main/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      789 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_contains_main/PackageContainsMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_contains_main/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      801 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_contains_main/local.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_init_import/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      823 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_init_import/PackageInitImportMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_init_import/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1008 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1169 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_init_import/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_init_issue/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      789 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_init_issue/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_init_issue/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_init_issue/some_package/child_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      795 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_missing_init/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      926 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_missing_init/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      965 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_missing_init/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_missing_init/some_package/sub_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      977 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_module_collision/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      901 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_module_collision/Something/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_module_collision/Something/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      801 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_module_collision/something.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_overload/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      852 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_overload/Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_overload/foo/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_overload/foo/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_overload/foo/bar.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_overload/foo/bar2.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_prevents_submodule/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2972 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_prevents_submodule/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1078 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.765277 Nuitka-1.7.2/tests/programs/package_program/
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/package_program/PackageAsMain/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      888 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_program/PackageAsMain/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1630 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/package_program/PackageAsMain/__main__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1728 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/pkgutil_usage/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1261 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/pkgutil_usage/package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       13 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       14 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       14 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1553 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/pkgutil_usage/package/__init__.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/plugin_import/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      859 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/plugin_import/PluginImportMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/plugin_import/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      771 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/plugin_import/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      781 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/plugin_import/some_package/some_module.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/reimport_main_dynamic/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      911 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/reimport_main_static/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      898 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/relative_import/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      842 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/relative_import/RelativeImportMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/relative_import/dircache.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/resource_reader37/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1169 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/resource_reader37/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       13 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/resource_reader37/some_package/__init__.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6615 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/stdlib_overload/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1171 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/stdlib_overload/pyexpat.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.885278 Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/__init__.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      909 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1236 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/tests/programs/syntax_errors/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      791 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/syntax_errors/IndentationErroring.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/syntax_errors/SyntaxErroring.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1079 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/tests/programs/unicode_bom/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      963 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      846 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/unicode_bom/unicode_bom.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/tests/programs/with space/
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      826 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/programs/with space/Space Main.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/tests/reflected/
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14061 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/reflected/compile_itself.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1243 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/run-tests
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/tests/standalone/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1058 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/BrotliUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2554 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/CtypesUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1136 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/FlaskUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      990 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/GlfwUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1184 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/GtkUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1025 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/HexEncodingTest_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1086 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/IdnaUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1151 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/LxmlUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1431 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/MatplotlibUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2538 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/MetadataPackagesUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1727 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/NumpyUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      947 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/OpenGLUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1379 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PandasUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1066 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PasslibUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1216 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PendulumUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2074 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PkgResourcesRequiresUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1067 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PmwUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1085 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PyQt5Plugins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1105 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PyQt5SSLSupport.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2050 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PyQt5Using.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1085 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PyQt6Plugins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2050 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PyQt6Using.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1091 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PySide6Plugins.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1757 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/PySide6Using.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1323 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/RsaUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      973 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/ShlibUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1537 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/SocketUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1941 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/TkInterUsing.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3228 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/Urllib3Using.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1200 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/Win32ComUsing.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9531 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/run_all.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/tests/standalone/zip_importer/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1264 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/standalone/zip_importer/ZipImporterMain.py
-drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-08 07:29:15.895278 Nuitka-1.7.2/tests/syntax/
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      811 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/AsyncgenReturn36.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      868 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/BreakWithoutLoop.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      791 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/ClassReturn.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      970 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/ClosureDel_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      849 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/ContinueWithoutLoop.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      791 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/DuplicateArgument.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1111 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/ExecWithNesting_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      826 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/FutureBraces.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      805 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/FutureUnknown.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1041 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/GeneratorExpressions38.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      879 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/GeneratorReturn_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      792 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/GlobalForParameter.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      995 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/Importing32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/IndentationError.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      915 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/LateFutureImport.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      841 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/MisplacedFutureImport.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/ModuleReturn.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      883 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      794 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/NonlocalForParameter32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      868 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/NonlocalNotFound32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      908 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/StarImportExtra.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      869 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/SyntaxError.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      874 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/TryExceptAllNotLast.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      875 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/TryFinallyContinue_37.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      776 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/UnpackNoTuple.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/UnpackTwoStars32.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      793 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/YieldFromInModule.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      804 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/YieldInAsync35.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      923 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/YieldInGenexp38.py
--rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      781 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/YieldInModule.py
--rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2203 2023-07-08 07:28:59.000000 Nuitka-1.7.2/tests/syntax/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.679920 Nuitka-1.7.3/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)  2833663 2023-07-09 21:23:13.000000 Nuitka-1.7.3/Changelog.pdf
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   843525 2023-07-09 21:22:58.000000 Nuitka-1.7.3/Changelog.rst
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   812243 2023-07-09 21:23:07.000000 Nuitka-1.7.3/Developer_Manual.pdf
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   152515 2023-07-09 21:22:58.000000 Nuitka-1.7.3/Developer_Manual.rst
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11348 2023-07-09 21:22:58.000000 Nuitka-1.7.3/LICENSE.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1723 2023-07-09 21:22:58.000000 Nuitka-1.7.3/MANIFEST.in
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/Nuitka.egg-info/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    79137 2023-07-09 21:23:16.000000 Nuitka-1.7.3/Nuitka.egg-info/PKG-INFO
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76769 2023-07-09 21:23:16.000000 Nuitka-1.7.3/Nuitka.egg-info/SOURCES.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        1 2023-07-09 21:23:16.000000 Nuitka-1.7.3/Nuitka.egg-info/dependency_links.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      393 2023-07-09 21:23:16.000000 Nuitka-1.7.3/Nuitka.egg-info/entry_points.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        1 2023-07-09 21:23:16.000000 Nuitka-1.7.3/Nuitka.egg-info/not-zip-safe
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        7 2023-07-09 21:23:16.000000 Nuitka-1.7.3/Nuitka.egg-info/top_level.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    79137 2023-07-09 21:23:16.679920 Nuitka-1.7.3/PKG-INFO
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   345695 2023-07-09 21:23:04.000000 Nuitka-1.7.3/README.pdf
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76929 2023-07-09 21:22:58.000000 Nuitka-1.7.3/README.rst
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/bin/
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1135 2023-07-09 21:22:58.000000 Nuitka-1.7.3/bin/autoformat-nuitka-source
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1134 2023-07-09 21:22:58.000000 Nuitka-1.7.3/bin/check-nuitka-with-pylint
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1150 2023-07-09 21:22:58.000000 Nuitka-1.7.3/bin/compare_with_cpython
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3079 2023-07-09 21:22:58.000000 Nuitka-1.7.3/bin/compare_with_xml
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1163 2023-07-09 21:22:58.000000 Nuitka-1.7.3/bin/measure-construct-performance
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1685 2023-07-09 21:22:58.000000 Nuitka-1.7.3/bin/nuitka
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1685 2023-07-09 21:22:58.000000 Nuitka-1.7.3/bin/nuitka-run
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/doc/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/doc/Logo/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7321 2023-07-09 21:22:58.000000 Nuitka-1.7.3/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7401 2023-07-09 21:22:58.000000 Nuitka-1.7.3/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17917 2023-07-09 21:22:58.000000 Nuitka-1.7.3/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/doc/images/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7585 2023-07-09 21:22:58.000000 Nuitka-1.7.3/doc/images/Nuitka-Logo-Horizontal.png
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4452 2023-07-09 21:22:58.000000 Nuitka-1.7.3/doc/images/Nuitka-Logo-Symbol.png
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9828 2023-07-09 21:22:58.000000 Nuitka-1.7.3/doc/images/Nuitka-Logo-Vertical.png
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31239 2023-07-09 21:23:15.000000 Nuitka-1.7.3/doc/nuitka2-run.1
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31263 2023-07-09 21:23:15.000000 Nuitka-1.7.3/doc/nuitka2.1
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31252 2023-07-09 21:23:16.000000 Nuitka-1.7.3/doc/nuitka3-run.1
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31276 2023-07-09 21:23:16.000000 Nuitka-1.7.3/doc/nuitka3.1
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/lib/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4250 2023-07-09 21:22:58.000000 Nuitka-1.7.3/lib/hints.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/misc/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      901 2023-07-09 21:22:58.000000 Nuitka-1.7.3/misc/nuitka-run.bat
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1038 2023-07-09 21:22:58.000000 Nuitka-1.7.3/misc/nuitka.bat
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/nuitka/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7529 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Builtins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5437 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/BytecodeCaching.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3440 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Bytecodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1884 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/CacheCleanup.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11148 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Constants.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2447 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    37438 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/MainControl.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8064 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/ModuleRegistry.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    55485 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/OptionParsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65509 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Options.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5022 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/OutputDirectories.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14550 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/PostProcessing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5770 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Progress.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7472 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/PythonFlavors.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4061 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/PythonOperators.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12179 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/PythonVersions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9062 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Serialization.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4670 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/SourceCodeReferences.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11235 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Tracing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3395 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/TreeXML.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15235 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Variables.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2055 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/Version.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5615 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5295 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/__past__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.539920 Nuitka-1.7.3/nuitka/build/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34131 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/Backend.scons
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8300 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/CCompilerVersion.scons
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2716 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/DataComposerInterface.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18756 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/Onefile.scons
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15698 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/SconsCaching.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31010 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/SconsCompilerSettings.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5527 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/SconsHacks.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15827 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/SconsInterface.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2671 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/SconsProgress.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12022 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/SconsSpawn.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24338 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/SconsUtils.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/include/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/include/nuitka/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7972 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/allocator.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3470 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/builtins.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4604 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/calling.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1977 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/checkers.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1261 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/checksum_tools.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9571 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2002 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_cell.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9325 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16949 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_frame.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5972 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_function.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9136 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_generator.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1838 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_method.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7408 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/constants.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1293 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/constants_blob.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34083 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/exceptions.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3473 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6253 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/freelists.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    86326 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/hedley.h
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3393 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/attributes.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2663 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/boolean.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1181 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1135 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/bytes.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9335 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13140 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10616 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10615 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13140 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13139 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10616 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1743 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/complex.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13109 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1206 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/floats.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3897 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1798 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/indexes.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2941 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/ints.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9992 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/iterators.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3411 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/lists.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1633 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1328 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/mappings.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4573 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12685 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5663 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5641 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5663 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5422 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5460 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5115 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2799 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15778 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13210 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5791 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4714 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5115 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5824 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5438 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15100 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8670 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3767 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3753 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3767 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4846 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3011 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2727 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10626 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9201 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5147 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4349 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3011 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4975 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4826 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3297 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/raising.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2178 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1146 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1112 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/sequences.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1025 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/sets.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8419 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/slices.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1242 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/strings.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17575 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5720 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helper/tuples.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14411 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/helpers.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5375 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/importing.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12979 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/incbin.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14427 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/prelude.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2870 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/printing.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1761 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/python_pgo.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2243 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3840 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/threading.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3144 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/tracing.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2936 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/include/nuitka/unfreezing.h
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/appdirs/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1097 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24824 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/atomicwrites/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1069 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6794 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/bin/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1331 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/bin/scons.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/clcache/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/clcache/clcache/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1585 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       93 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65424 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1491 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      243 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2522 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10517 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1915 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5404 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6438 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/glob2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1359 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/glob2/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       82 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6859 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4463 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8304 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1467 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       85 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/README.rst
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.549920 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2423 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2685 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1726 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12719 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65386 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1626 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12281 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1400 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50849 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4428 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24500 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36528 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9197 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28559 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17473 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4340 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7308 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30853 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1722 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35875 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27644 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17080 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4214 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20501 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3316 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1466 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       84 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2616 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2685 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1726 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12719 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    65386 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1626 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12281 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1400 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50849 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4428 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24500 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36528 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9197 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28559 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17474 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4340 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7308 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30853 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1722 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35875 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27644 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17080 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4214 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20501 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3316 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47844 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    33996 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8083 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27693 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6938 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17622 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    96183 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7358 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21540 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16000 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9589 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4197 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   121420 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4164 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    49503 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1950 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1950 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1950 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1965 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2736 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2614 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8467 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9314 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3131 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1989 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2483 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1718 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1605 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2170 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4179 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1882 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14948 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39700 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12950 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4810 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3751 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3233 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2011 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14663 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.559920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14029 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    52665 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40719 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24133 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14053 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2305 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34903 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40510 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2166 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2433 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2859 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18084 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2078 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2004 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9248 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2784 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14869 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19499 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20832 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3763 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5149 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2290 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2328 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2657 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31283 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2379 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2267 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2681 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2720 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2796 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2147 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2936 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2935 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3432 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3785 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2777 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1711 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      142 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29618 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3428 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2681 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2433 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1844 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3472 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4782 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2025 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2256 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2460 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2639 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1810 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2333 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2140 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1902 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2077 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2043 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18600 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25816 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3328 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8394 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3953 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2309 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2945 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6919 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4381 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4658 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4224 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2168 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13881 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1804 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11380 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    72761 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6841 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3579 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2618 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4375 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2827 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2513 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1991 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1819 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2123 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2502 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4695 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1927 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2349 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2473 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5992 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1831 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3730 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13016 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3415 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    48938 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3007 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3784 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4404 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3557 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5612 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11034 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6824 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1563 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8120 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3596 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1818 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1742 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2465 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1776 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19253 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    44500 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19664 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7509 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2107 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53545 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34985 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13596 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28403 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7533 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20988 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    96818 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7752 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22350 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16068 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9565 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5239 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   135413 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5758 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    63474 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8354 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11500 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3180 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2227 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2739 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1767 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1654 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1460 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2219 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4476 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1931 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4003 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16962 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    41186 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13880 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4853 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3812 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3643 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2328 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15053 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.569920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13779 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53260 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39394 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26467 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14489 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35863 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42204 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.579920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2211 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18207 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.579920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2152 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2057 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10674 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2855 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15165 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    33537 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21762 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4464 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50660 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1667 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2316 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2475 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2840 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8618 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2226 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2978 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2977 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1653 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3827 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3389 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.579920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      313 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3631 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3444 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8494 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1753 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.579920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29765 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3472 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1630 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1977 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3686 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2580 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2948 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2655 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1645 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1859 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2765 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2386 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2189 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1944 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2123 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2085 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15791 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26195 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13924 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4041 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2351 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2987 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7808 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4956 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5235 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4808 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2475 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14751 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1847 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12588 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82939 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6883 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3663 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2660 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4904 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2877 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2567 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1652 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1868 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2088 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2176 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2366 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1658 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1976 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5335 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2583 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2515 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6756 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1873 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3773 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13982 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3201 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53803 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.579920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3064 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3818 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4459 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3643 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5579 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11655 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6504 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1647 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.579920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6869 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1784 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19816 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9002 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2149 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.579920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    56578 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35213 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11061 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27408 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7884 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21423 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    97269 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3979 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7515 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21937 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16583 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9430 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5126 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   136271 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6167 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    63768 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8183 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12836 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3087 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2107 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2630 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1674 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1536 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1311 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2076 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4356 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1805 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3860 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14831 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    41983 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14673 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7394 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4357 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3546 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1972 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15577 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13597 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53509 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42760 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26676 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14272 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36753 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    41191 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2122 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15570 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2014 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1943 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13182 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2734 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15027 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    38783 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22570 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4368 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    32724 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1578 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2228 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2386 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2616 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7993 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2141 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1661 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2893 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2889 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1567 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3742 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3296 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      343 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3534 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3259 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7461 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1663 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3379 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1544 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1891 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3616 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2377 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2437 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2526 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1557 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1772 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2677 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2206 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2096 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1851 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1954 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1995 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19180 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25826 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2588 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4649 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7652 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6064 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3931 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2266 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2900 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8622 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4577 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4517 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4113 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2387 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14473 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1752 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12902 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    84784 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6788 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3576 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4817 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2788 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2479 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1563 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1780 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1999 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2006 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2271 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1569 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1888 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4879 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2419 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2429 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6412 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1786 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3687 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12548 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4076 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    71693 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6632 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15278 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.589920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3134 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3896 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4672 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3536 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5588 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12708 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6785 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      353 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4307 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1644 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3395 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21614 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9295 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2032 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1467 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10126 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      558 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4690 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1873 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/pkg_resources/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   107452 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      538 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.519920 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1591 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      283 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3687 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      283 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      287 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      307 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      888 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      596 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1106 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      857 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1376 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5943 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/gui.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10790 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    57572 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6948 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9533 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      333 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1101 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13170 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4883 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28639 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3851 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2837 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    43006 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2533 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2445 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2061 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1440 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25495 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6794 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14184 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8999 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51277 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4165 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1101 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9776 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4921 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25145 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3290 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2719 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    43298 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2559 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2445 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1132 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1440 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25542 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6746 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17711 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9122 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    52446 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4171 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1101 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9607 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4881 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25554 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3294 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2723 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42954 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2533 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2445 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1138 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1440 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    25495 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6854 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14097 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8970 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51695 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4165 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2573 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1530 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18198 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10157 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4455 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3763 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13662 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3009 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2441 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34422 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14748 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20216 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13930 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26976 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11706 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2728 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2497 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3828 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15880 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.599920 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    54982 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9164 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1321 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    80283 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    66784 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2253 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7906 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   138334 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/inline_copy/zstd/zstd.h
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.619920 Nuitka-1.7.3/nuitka/build/static_src/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82114 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8250 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledCellType.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    56307 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    70973 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35861 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledFrameType.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   100376 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledFunctionType.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    60649 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    48526 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21638 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/CompiledMethodType.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18993 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersAllocator.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    37540 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersAttributes.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21783 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersBuiltin.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   107641 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3033 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersBytes.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13057 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersCalling.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   470655 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1617 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2991 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersClasses.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   317872 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4673 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   313003 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   312414 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   316217 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   315628 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   314618 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36068 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19313 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    38364 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersDictionaries.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24295 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7035 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersExceptions.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6668 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersFiles.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28131 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2426 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersFloats.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1774 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14585 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersImport.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14756 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersImportHard.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18433 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersLists.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13915 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1640 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersMappings.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3513 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersMatching.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   181243 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16700 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77943 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77782 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77943 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    67487 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1236 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    68748 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6274 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    83405 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13776 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   183202 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   188514 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3404 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    66453 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    78891 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1023 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    77305 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    70465 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    68005 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   149580 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4071 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53224 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53122 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    53224 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76512 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47568 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17742 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   136100 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   142211 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    74142 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82669 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    45052 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    82842 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76343 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3219 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersProfiling.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3805 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15369 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersRaising.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3758 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3730 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersSequences.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1946 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersSlices.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26642 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersStrings.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4037 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersTuples.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5578 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/HelpersTypes.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11986 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/InspectPatcher.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/MainProgram.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    58634 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4537 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6427 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17285 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30910 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/OnefileBootstrap.c
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8021 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.619920 Nuitka-1.7.3/nuitka/code_generation/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6414 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/AsyncgenCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10599 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/AttributeCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21864 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2339 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/BranchCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16009 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/BuiltinCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    35905 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/CallCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4896 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ClassCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51441 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/CodeGeneration.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2375 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/CodeHelperSelection.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14392 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/CodeHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4879 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/CodeObjectCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17570 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ComparisonCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4446 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7335 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ConditionalCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6539 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ConstantCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31186 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/Contexts.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8484 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/CoroutineCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1574 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/CtypesCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28478 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/DictCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2125 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/Emission.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9325 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ErrorCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12304 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/EvalCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8975 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ExceptionCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7350 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2093 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ExpressionCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17725 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/FrameCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    27968 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/FunctionCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7690 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/GeneratorCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5943 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/GlobalConstants.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6911 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1794 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/IdCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13318 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ImportCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1396 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/Indentation.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1506 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/IndexCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1033 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/InjectCCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3432 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/IntegerCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12010 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/IteratorCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2022 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/LabelCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2612 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/LineNumberCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15906 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ListCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6375 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/LoaderCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9951 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/LocalsDictCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3135 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/LoopCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1597 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/MatchCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6291 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ModuleCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8118 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/Namify.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12777 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/OperationCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29459 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/PackageResourceCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3021 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/PrintCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5474 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/PythonAPICodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13095 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/RaisingCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3443 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/Reports.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5234 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/ReturnCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6517 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/SetCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13949 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/SliceCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9809 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/StringCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8188 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/SubscriptCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11176 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/TryCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3786 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/TupleCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14717 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/VariableCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9121 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/VariableDeclarations.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8099 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/YieldCodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.619920 Nuitka-1.7.3/nuitka/code_generation/c_types/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6069 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeBases.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3399 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1804 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1378 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3610 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5128 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5211 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3955 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19628 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2852 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/c_types/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.619920 Nuitka-1.7.3/nuitka/code_generation/templates/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2845 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5865 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2921 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2290 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6339 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3321 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3306 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2335 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4217 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21244 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6640 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2475 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.629920 Nuitka-1.7.3/nuitka/code_generation/templates_c/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11231 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5847 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23760 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5238 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1905 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1843 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2817 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12819 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2044 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2762 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1544 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7197 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12850 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4288 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2088 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2118 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3933 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7407 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4292 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3860 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4487 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11579 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19317 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2843 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3635 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11102 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15380 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2979 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10421 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2557 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3020 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2984 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3173 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.629920 Nuitka-1.7.3/nuitka/containers/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1435 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/containers/Namedtuples.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6553 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/containers/OrderedDicts.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      554 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/containers/OrderedSets.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4397 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/containers/OrderedSetsFallback.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/containers/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.629920 Nuitka-1.7.3/nuitka/distutils/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1964 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/distutils/Build.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14219 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/distutils/DistutilCommands.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/distutils/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.629920 Nuitka-1.7.3/nuitka/finalizations/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1224 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/finalizations/Finalization.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6110 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/finalizations/FinalizeMarkups.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/finalizations/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.629920 Nuitka-1.7.3/nuitka/freezer/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7311 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/DependsExe.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2584 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/DllDependenciesCommon.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11494 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/DllDependenciesMacOS.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7211 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/DllDependenciesPosix.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6620 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/DllDependenciesWin32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17058 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/IncludedDataFiles.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9492 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/IncludedEntryPoints.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9015 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/Onefile.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26319 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/Standalone.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/freezer/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.629920 Nuitka-1.7.3/nuitka/importing/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11007 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/IgnoreListing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2899 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/ImportCache.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6719 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/ImportResolving.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28463 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/Importing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4738 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/PreloadedPackages.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14918 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/Recursion.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10981 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/StandardLibrary.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/importing/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/nodes/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3637 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/AsyncgenNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4082 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/AttributeLookupNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13567 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/AttributeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   378745 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/AttributeNodesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3823 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinAllNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4098 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinAnyNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2496 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinComplexNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1698 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2727 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4694 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinDictNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4948 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinFormatNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2142 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinHashNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5334 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12723 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1996 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinLenNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3606 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinNextNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3240 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinOpenNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   245536 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18589 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinRangeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9067 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinRefNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3307 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinSumNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13543 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinTypeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1573 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BuiltinVarsNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26113 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/BytesNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6478 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/CallNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1550 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/Checkers.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   604445 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ChildrenHavingMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8448 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ClassNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6585 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/CodeObjectSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21683 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ComparisonNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30314 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ConditionalNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    46536 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ConstantRefNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12213 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ContainerMakingNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2834 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ContainerOperationNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4581 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/CoroutineNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1714 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/CtypesNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51021 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/DictionaryNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7856 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ExceptionNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7317 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ExecEvalNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    44996 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ExpressionBases.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    49273 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    21278 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ExpressionShapeMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12156 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/FrameNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3544 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/FunctionAttributeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39803 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/FunctionNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5376 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/FutureSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6256 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/GeneratorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6850 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    76798 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/HardImportNodesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5508 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ImportHardNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    45942 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ImportNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2733 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/IndicatorMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1502 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/InjectCNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11228 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/IterationHandles.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11002 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/KeyValuePairNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    16320 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ListOperationNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23094 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/LocalsDictNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14922 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/LocalsScopes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15581 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/LoopNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1712 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/MatchNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6534 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ModuleAttributeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30972 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ModuleNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    24899 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/NodeBases.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15128 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/NodeMakingHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5550 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/NodeMetaClasses.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31894 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/OperatorNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9134 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/OperatorNodesUnary.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4202 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/OsSysNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12442 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/OutlineNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    31534 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/PackageMetadataNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7901 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/PackageResourceNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3407 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/PrintNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6772 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/ReturnNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4715 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/SideEffectNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12501 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/SliceNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    94880 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/StatementBasesGenerated.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9430 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/StatementNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    28658 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/StrNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3504 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/StringConcatenationNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8640 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/SubscriptNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17853 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/TryNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2405 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/TypeMatchNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11061 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/TypeNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39522 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/VariableAssignNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10746 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/VariableDelNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4574 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/VariableNameNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    30982 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/VariableRefNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4748 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/VariableReleaseNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3902 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/YieldNodes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/nodes/shapes/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   156243 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4387 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4567 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/shapes/ShapeMixins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42374 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/shapes/StandardShapes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/nodes/shapes/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/optimizations/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3279 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/BytecodeDemotion.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3920 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/FunctionInlining.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2144 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/Graphs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10762 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/Optimization.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    52058 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2272 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/Tags.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40896 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/TraceCollections.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23977 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/ValueTraces.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/optimizations/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/pgo/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4663 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/pgo/PGO.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/pgo/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/plugins/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    40838 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/PluginBase.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    57611 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/Plugins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/plugins/standard/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22510 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3460 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10383 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4404 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/DelvewheelPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5675 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/DillPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13744 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2062 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/EnumPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1905 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/EventletPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1880 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/GeventPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3482 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/GiPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5027 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/GlfwPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18335 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/ImplicitImports.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4948 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/KivyPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7239 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6352 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1187 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/NumpyPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6595 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1917 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/PbrPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4665 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6992 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/PmwPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    50293 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2986 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1160 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12242 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/TkinterPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1140 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/TorchPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10191 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/TransformersPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3175 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/TrioPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5640 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/UpxPlugin.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)   160906 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2221 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9867 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/reports/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2209 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/reports/LicenseReport.rst.j2
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17538 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/reports/Reports.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/reports/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/specs/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5911 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2786 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2541 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    26455 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/BuiltinParameterSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6065 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1159 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4802 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5263 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/HardImportSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    18740 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/ParameterSpecs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/specs/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1603 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/Basics.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/commercial/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      815 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/commercial/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/data_composer/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14250 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/data_composer/DataComposer.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/data_composer/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1306 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/data_composer/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/environments/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2449 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/environments/CreateEnvironment.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3735 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/environments/Virtualenv.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/environments/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/general/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/general/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/general/dll_report/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/general/dll_report/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2366 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/general/dll_report/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/general/find_module/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3920 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/general/find_module/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/onefile_compressor/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10194 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/onefile_compressor/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1311 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/onefile_compressor/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/podman/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1872 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/podman/Podman.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/podman/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6612 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/podman/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/profiler/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/profiler/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2529 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/profiler/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/scanning/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3344 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2095 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/scanning/DisplayPackageData.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/scanning/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.639920 Nuitka-1.7.3/nuitka/tools/specialize/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    51143 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7685 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/specialize/Common.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    39625 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/specialize/SpecializeC.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    34664 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/specialize/SpecializePython.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/specialize/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tools/testing/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    55396 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/Common.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1483 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/Constructs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8940 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/OutputComparison.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1278 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/Pythons.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8024 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/RuntimeTracing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5371 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/SearchModes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3375 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/Valgrind.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tools/testing/check_reference_counts/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3064 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tools/testing/compare_with_cpython/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29429 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tools/testing/find_sxs_modules/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1949 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tools/testing/measure_construct_performance/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8755 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tools/testing/run_nuitka_tests/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36321 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tools/watch/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/watch/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9503 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tools/watch/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/tree/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    47138 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/Building.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    74608 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1700 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/Extractions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2572 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/InternalModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1511 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/Operations.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2807 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationAssertStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    42768 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2948 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11693 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationCallExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15072 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationClasses.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    37638 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationClasses3.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6430 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22111 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationContractionExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    11061 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14607 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationExecStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7782 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationForLoopStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    29594 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationFunctionStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    13437 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationImportStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6577 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20962 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationMatchStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2409 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationMultidist.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8194 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationNamespacePackages.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4658 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationPrintStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15371 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationSequenceCreation.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4824 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14615 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6982 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5674 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14341 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationWithStatements.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3088 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/ReformulationYieldExpressions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12746 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/SourceHandling.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3757 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/SyntaxErrors.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22973 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/TreeHelpers.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    20012 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/VariableClosure.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/tree/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/nuitka/utils/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2655 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/AppDirs.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3248 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/CStrings.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3653 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/CommandLineOptions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4297 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Distributions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5794 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Download.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12645 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Execution.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    36129 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/FileOperations.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2885 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Hashing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2362 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Images.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6816 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Importing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8149 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/InstalledPythons.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2224 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/InstanceCounters.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4336 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Jinja2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1238 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Json.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4304 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/MacOSApp.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5040 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/MemoryUsage.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9062 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/ModuleNames.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4309 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/ReExecute.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3815 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Rest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22701 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/SharedLibraries.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3664 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Shebang.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2591 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Signing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6207 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/StaticLibraries.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2602 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/ThreadedExecutor.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2772 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Timing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10826 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Utils.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    10574 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/WindowsFileUsage.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    19540 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/WindowsResources.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6108 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/Yaml.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      833 2023-07-09 21:22:58.000000 Nuitka-1.7.3/nuitka/utils/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      834 2023-07-09 21:22:58.000000 Nuitka-1.7.3/pyproject.toml
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       38 2023-07-09 21:23:16.679920 Nuitka-1.7.3/setup.cfg
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    15624 2023-07-09 21:22:58.000000 Nuitka-1.7.3/setup.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.649920 Nuitka-1.7.3/tests/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/basics/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1766 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/AssertsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5934 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/AssignmentsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5866 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/AssignmentsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4055 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/BranchingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1104 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/BuiltinOverload.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3749 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/BuiltinSuperTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    17080 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/BuiltinsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      866 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ClassMinimalTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4764 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ClassesTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3414 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ClassesTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1406 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ClassesTest34.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4698 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ComparisonChainsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4639 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ConstantsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      995 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ConstantsTest27.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1628 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/DecoratorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2317 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/DefaultParametersTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1127 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/DoubleDeletionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      806 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/EmptyModuleTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14387 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ExceptionRaisingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      961 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ExceptionRaisingTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1458 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ExceptionRaisingTest33.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6747 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ExecEvalTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1417 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ExtremeClosureTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1658 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/FunctionObjectsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    12335 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/FunctionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3603 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/FunctionsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2627 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/FunctionsTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      890 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/FutureTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5809 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/GeneratorExpressionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1041 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/GeneratorExpressionsTest_37.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3824 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/GlobalStatementTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1286 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/HelloWorldTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2469 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ImportingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1296 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/InplaceOperationsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4227 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/InspectionTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1504 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/InspectionTest_35.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1618 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/InspectionTest_36.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1671 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/LambdasTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2731 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/LateClosureAssignmentTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2923 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ListContractionsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3329 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/LoopingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1536 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/MainProgramsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1925 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ModuleAttributesTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1988 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/OperatorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14903 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/OrderChecksTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1827 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/OrderChecksTest27.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1452 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/OverflowFunctionsTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5853 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ParameterErrorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1899 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ParameterErrorsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      863 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/PrintFutureTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1413 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/PrintingTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      878 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/RecursionTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    23840 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ReferencingTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2076 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ReferencingTest27.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     7819 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ReferencingTest33.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4902 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ReferencingTest35.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5092 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ReferencingTest36.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2899 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ReferencingTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1630 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/SlotsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1159 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/ThreadedGeneratorsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    22966 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TrickAssignmentsTest32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1541 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TrickAssignmentsTest35.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1788 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TrickAssignmentsTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2086 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TryContinueFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2212 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TryExceptContinueTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2275 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TryExceptFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2304 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TryExceptFramesTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2842 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TryReturnFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2328 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/TryYieldFinallyTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1093 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/UnicodeTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1877 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/UnpackingTest35.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2095 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/VarargsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     4879 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/WithStatementsTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3070 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/YieldFromTest33.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3821 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/run_all.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2271 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/basics/run_xml.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/onefile/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1213 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/onefile/HelloWorldTest.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1307 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/onefile/KeyboardInterruptTest.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     5816 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/onefile/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/optimizations/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      958 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/ArgumentTypes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1055 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/Attributes.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1021 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/Calls.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      921 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/Conditions.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      909 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/DecodingOperations.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1212 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/FormatStrings36.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1150 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/HardImports.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      974 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/HardImports_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      918 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/Iterations.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1260 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/Len.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2262 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/Operations.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1333 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/Subscripts.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     8736 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/optimizations/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/packages/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/packages/package_import_success_after_failure/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2382 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/packages/package_import_success_after_failure/variable_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      942 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1168 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3671 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.529920 Nuitka-1.7.3/tests/packages/sub_package/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/packages/sub_package/kitty/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1230 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/sub_package/kitty/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      908 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/sub_package/kitty/bigkitty.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      910 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/sub_package/kitty/smallkitty.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      929 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1053 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/hello.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      966 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/miau.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      968 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/purr.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.529920 Nuitka-1.7.3/tests/packages/top_level_attributes_3/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/packages/top_level_attributes_3/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2336 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      907 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/plugins/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/plugins/code_signing/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1170 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/code_signing/CodeSigningMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/plugins/data_files/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1332 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/data_files/DataFilesMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/plugins/data_files/data_files_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      924 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/data_files/data_files_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/data_files/data_files_package/lala.txt
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      255 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/plugins/parameters/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1019 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/parameters/ParametersMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2168 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/parameters/parameter-using-plugin.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3861 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/plugins/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/absolute_import/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      867 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/absolute_import/foobar/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      796 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/absolute_import/foobar/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1043 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/absolute_import/foobar/foobar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      879 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/absolute_import/foobar/local.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      860 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/absolute_import/foobar/util.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports1/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports1/CasedImportingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports1/path1/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports1/path1/Some_Module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports1/path1/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports1/path2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports1/path2/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports1/path2/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports2/CasedImportingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports2/path1/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports2/path1/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports2/path1/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports2/path2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports2/path2/Some_Module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports2/path2/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports3/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1075 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports3/CasedImportingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports3/path1/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports3/path1/Some_Module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports3/path1/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports3/path2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports3/path2/Some_Module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/case_imports3/path2/Some_Package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/cyclic_imports/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      801 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      875 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      875 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      842 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/dash_import/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      888 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/dash_import/DashImportMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      817 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/dash_import/dash-module.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      817 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/dash_import/plus+module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/dash_main/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/dash_main/Dash-Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/deep/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      898 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/deep/DeepProgramMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/deep/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      980 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/deep/some_package/DeepBrother.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      909 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/deep/some_package/DeepChild.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/deep/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/deep/some_package/deep_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      876 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      952 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/deep/some_package/deep_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/dunderinit_imports/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      794 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/dunderinit_imports/package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      797 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      857 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/dunderinit_imports/package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/import_variants/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1005 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/import_variants/ImportVariationsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/import_variants/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      946 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/import_variants/some_package/Child1.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1098 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/import_variants/some_package/Child2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      822 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/import_variants/some_package/Child3.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      994 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/import_variants/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.659920 Nuitka-1.7.3/tests/programs/main_raises/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      911 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/main_raises/ErrorMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/main_raises/ErrorRaising.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/main_raises2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1080 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      808 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/main_raises2/ErrorRaising.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/module_attributes/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1529 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1744 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1611 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1744 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1611 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1744 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1611 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/module_exits/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      869 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_exits/ErrorExitingModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      867 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_exits/Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/module_object_replacing/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1078 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1359 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/multiprocessing_using/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      990 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/multiprocessing_using/foo/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      836 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1758 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/multiprocessing_using/foo/entry.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/named_imports/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      846 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/named_imports/NamedImportsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/named_imports/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/named_imports/some_package/SomeModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      824 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/named_imports/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/named_imports/some_package/sub_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_code/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_code/PackageInitCodeMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_code/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_code/some_package/SomeModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_code/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_contains_main/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      789 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_contains_main/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      801 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_contains_main/local.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_init_import/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      823 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_init_import/PackageInitImportMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_init_import/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1008 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1169 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_init_import/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_init_issue/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      789 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_init_issue/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_init_issue/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_init_issue/some_package/child_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      798 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      795 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_missing_init/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      926 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_missing_init/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      965 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_missing_init/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_missing_init/some_package/sub_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      977 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_module_collision/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      901 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_module_collision/Something/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_module_collision/Something/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      801 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_module_collision/something.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_overload/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      852 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_overload/Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_overload/foo/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_overload/foo/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_overload/foo/bar.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_overload/foo/bar2.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_prevents_submodule/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2972 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_prevents_submodule/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1078 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.529920 Nuitka-1.7.3/tests/programs/package_program/
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/package_program/PackageAsMain/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      888 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1630 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/package_program/PackageAsMain/__main__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1728 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/pkgutil_usage/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1261 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/pkgutil_usage/package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       13 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       14 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       14 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1553 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/pkgutil_usage/package/__init__.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/plugin_import/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      859 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/plugin_import/PluginImportMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/plugin_import/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      771 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/plugin_import/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      781 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/plugin_import/some_package/some_module.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/reimport_main_dynamic/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      911 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/reimport_main_static/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      898 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/relative_import/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      842 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/relative_import/RelativeImportMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/relative_import/dircache.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/resource_reader37/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1169 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/resource_reader37/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)       13 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/resource_reader37/some_package/__init__.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     6615 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/stdlib_overload/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1171 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/stdlib_overload/pyexpat.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      769 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      909 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      810 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1236 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/syntax_errors/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      791 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/syntax_errors/IndentationErroring.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1079 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/unicode_bom/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      963 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      846 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/unicode_bom/unicode_bom.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/programs/with space/
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      826 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/programs/with space/Space Main.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/reflected/
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)    14061 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/reflected/compile_itself.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1243 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/run-tests
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/standalone/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1058 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/BrotliUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2554 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/CtypesUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1136 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/FlaskUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      990 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/GlfwUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1184 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/GtkUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1025 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/HexEncodingTest_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1086 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/IdnaUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1151 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/LxmlUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1431 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/MatplotlibUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2538 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/MetadataPackagesUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1727 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/NumpyUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      947 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/OpenGLUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1379 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PandasUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1066 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PasslibUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1216 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PendulumUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2074 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1067 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PmwUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1085 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PyQt5Plugins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1105 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PyQt5SSLSupport.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2050 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PyQt5Using.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1085 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PyQt6Plugins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2050 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PyQt6Using.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1091 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PySide6Plugins.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1757 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/PySide6Using.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1323 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/RsaUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      973 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/ShlibUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1537 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/SocketUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1941 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/TkInterUsing.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     3228 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/Urllib3Using.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1200 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/Win32ComUsing.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     9531 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/run_all.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.669920 Nuitka-1.7.3/tests/standalone/zip_importer/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1264 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/standalone/zip_importer/ZipImporterMain.py
+drwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)        0 2023-07-09 21:23:16.679920 Nuitka-1.7.3/tests/syntax/
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      811 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/AsyncgenReturn36.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      868 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/BreakWithoutLoop.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      791 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/ClassReturn.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      970 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/ClosureDel_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      849 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/ContinueWithoutLoop.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      791 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/DuplicateArgument.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1111 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/ExecWithNesting_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      826 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/FutureBraces.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      805 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/FutureUnknown.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     1041 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/GeneratorExpressions38.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      879 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/GeneratorReturn_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      792 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/GlobalForParameter.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      995 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/Importing32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      799 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/IndentationError.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      915 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/LateFutureImport.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      841 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/MisplacedFutureImport.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      800 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/ModuleReturn.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      883 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      794 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/NonlocalForParameter32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      868 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/NonlocalNotFound32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      908 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/StarImportExtra.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      869 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/SyntaxError.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      874 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/TryExceptAllNotLast.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      875 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/TryFinallyContinue_37.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      776 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/UnpackNoTuple.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      809 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/UnpackTwoStars32.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      793 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/YieldFromInModule.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      804 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/YieldInAsync35.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      923 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/YieldInGenexp38.py
+-rw-r--r--   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)      781 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/YieldInModule.py
+-rwxr-xr-x   0 nuitka-buildslave  (2001) nuitka-buildslave  (2001)     2203 2023-07-09 21:22:58.000000 Nuitka-1.7.3/tests/syntax/run_all.py
```

### Comparing `Nuitka-1.7.2/Changelog.pdf` & `Nuitka-1.7.3/Changelog.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'2799825'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'2799825'*

 * *DEBUG:pdfminer.psparser:seek: 2799825*

 * *DEBUG:pdfminer.psparser:nexttoken: (2799825, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=2799825, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 2799829, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799830, b'0 1680\n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799837, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799857, b'0000000073 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799877, b'0000000172 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799897, b'0000000279 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799917, b'0000000391 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799937, b'0000000496 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799957, b'0000000705 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799977, b'0000000914 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2799997, b'0000001123 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2800017, b'0000001332 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2800037, b'0000001541 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2800057, b'0000001655 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2800077, b'0000001766 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 2800097, b'0000001976 00000 n \n'*

 * *[ truncated after 25 lines; 71393 ignored ]*

```diff
@@ -12186,21 +12186,21 @@
 </object>
 
 <object id="348">
 <dict size="9">
 <key>Author</key>
 <value><string size="0"></string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230708092910+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230709232310+00&#39;00&#39;</string></value>
 <key>Creator</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230708092910+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230709232310+00&#39;00&#39;</string></value>
 <key>Producer</key>
 <value><string size="41">ReportLab PDF Library - www.reportlab.com</string></value>
 <key>Subject</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Title</key>
 <value><string size="16">Nuitka Changelog</string></value>
 <key>Trapped</key>
@@ -35333,16 +35333,16 @@
 </dict>
 </object>
 
 <trailer>
 <dict size="4">
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#162;&#171;&#129;&#148;&#191;&#195;+ZO&#242;.&#190;&#173;&#139;&#34;F</string>
-<string size="16">&#162;&#171;&#129;&#148;&#191;&#195;+ZO&#242;.&#190;&#173;&#139;&#34;F</string>
+<string size="16">&#172;?&#221;Z|&#200;&#178;vL&#10;&#19;{&#140;2&#12;&#252;</string>
+<string size="16">&#172;?&#221;Z|&#200;&#178;vL&#10;&#19;{&#140;2&#12;&#252;</string>
 </list></value>
 <key>Info</key>
 <value><ref id="348" /></value>
 <key>Root</key>
 <value><ref id="347" /></value>
 <key>Size</key>
 <value><number>1680</number></value>
```

### Comparing `Nuitka-1.7.2/Changelog.rst` & `Nuitka-1.7.3/Changelog.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/Developer_Manual.pdf` & `Nuitka-1.7.3/Developer_Manual.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'798508'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'798508'*

 * *DEBUG:pdfminer.psparser:seek: 798508*

 * *DEBUG:pdfminer.psparser:nexttoken: (798508, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=798508, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 798512, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 798513, b'0 675\n'*

 * *DEBUG:pdfminer.psparser:nextline: 798519, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798539, b'0000000073 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798559, b'0000000204 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798579, b'0000000311 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798599, b'0000006874 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798619, b'0000007598 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798639, b'0000007868 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798659, b'0000007980 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798679, b'0000008149 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798699, b'0000008318 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798719, b'0000008487 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798739, b'0000008657 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798759, b'0000008827 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 798779, b'0000008997 00000 n \n'*

 * *[ truncated after 25 lines; 32054 ignored ]*

```diff
@@ -12877,21 +12877,21 @@
 </object>
 
 <object id="384">
 <dict size="9">
 <key>Author</key>
 <value><string size="0"></string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230708092906+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230709232306+00&#39;00&#39;</string></value>
 <key>Creator</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230708092906+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230709232306+00&#39;00&#39;</string></value>
 <key>Producer</key>
 <value><string size="41">ReportLab PDF Library - www.reportlab.com</string></value>
 <key>Subject</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Title</key>
 <value><string size="23">Nuitka Developer Manual</string></value>
 <key>Trapped</key>
@@ -17679,16 +17679,16 @@
 </dict>
 </object>
 
 <trailer>
 <dict size="4">
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#247;&#226;&#19;o&#129;&#163;&#28;&#7;&#248;V&#204;7&#142;]&#218;_</string>
-<string size="16">&#247;&#226;&#19;o&#129;&#163;&#28;&#7;&#248;V&#204;7&#142;]&#218;_</string>
+<string size="16">&#251;&#196;U&#226;Q&#219;&#216;&#201;&#186;&#232;&#196;&#239;&#24;&#213;_&#225;</string>
+<string size="16">&#251;&#196;U&#226;Q&#219;&#216;&#201;&#186;&#232;&#196;&#239;&#24;&#213;_&#225;</string>
 </list></value>
 <key>Info</key>
 <value><ref id="384" /></value>
 <key>Root</key>
 <value><ref id="383" /></value>
 <key>Size</key>
 <value><number>675</number></value>
```

### Comparing `Nuitka-1.7.2/Developer_Manual.rst` & `Nuitka-1.7.3/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/LICENSE.txt` & `Nuitka-1.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/MANIFEST.in` & `Nuitka-1.7.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/Nuitka.egg-info/PKG-INFO` & `Nuitka-1.7.3/Nuitka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 1.7.2
+Version: 1.7.3
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Commercial, https://nuitka.net/doc/commercial.html
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-1.7.2/Nuitka.egg-info/SOURCES.txt` & `Nuitka-1.7.3/Nuitka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/PKG-INFO` & `Nuitka-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 1.7.2
+Version: 1.7.3
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Commercial, https://nuitka.net/doc/commercial.html
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-1.7.2/README.pdf` & `Nuitka-1.7.3/README.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 0% similar despite different names*

#### dumppdf -adt {}

 * *error from `dumppdf -adt {}`:*

 * *DEBUG:pdfminer.psparser:seek: 0*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b''*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'%%EOF'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'340862'*

 * *DEBUG:pdfminer.pdfdocument:find_xref: b'startxref'*

 * *DEBUG:pdfminer.pdfdocument:xref found: pos=b'340862'*

 * *DEBUG:pdfminer.psparser:seek: 340862*

 * *DEBUG:pdfminer.psparser:nexttoken: (340862, /b'xref')*

 * *DEBUG:pdfminer.pdfdocument:read_xref_from: start=340862, token=/b'xref'*

 * *DEBUG:pdfminer.psparser:nextline: 340866, b'\n'*

 * *DEBUG:pdfminer.psparser:nextline: 340867, b'0 230\n'*

 * *DEBUG:pdfminer.psparser:nextline: 340873, b'0000000000 65535 f \n'*

 * *DEBUG:pdfminer.psparser:nextline: 340893, b'0000000073 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 340913, b'0000000195 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 340933, b'0000000302 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 340953, b'0000000414 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 340973, b'0000000519 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 340993, b'0000000687 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 341013, b'0000000802 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 341033, b'0000000970 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 341053, b'0000001089 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 341073, b'0000001320 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 341093, b'0000001528 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 341113, b'0000001717 00000 n \n'*

 * *DEBUG:pdfminer.psparser:nextline: 341133, b'0000001912 00000 n \n'*

 * *[ truncated after 25 lines; 10014 ignored ]*

```diff
@@ -2453,21 +2453,21 @@
 </object>
 
 <object id="72">
 <dict size="9">
 <key>Author</key>
 <value><string size="0"></string></value>
 <key>CreationDate</key>
-<value><string size="23">D:20230708092905+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230709232304+00&#39;00&#39;</string></value>
 <key>Creator</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Keywords</key>
 <value><string size="0"></string></value>
 <key>ModDate</key>
-<value><string size="23">D:20230708092905+00&#39;00&#39;</string></value>
+<value><string size="23">D:20230709232304+00&#39;00&#39;</string></value>
 <key>Producer</key>
 <value><string size="41">ReportLab PDF Library - www.reportlab.com</string></value>
 <key>Subject</key>
 <value><string size="13">&#40;unspecified&#41;</string></value>
 <key>Title</key>
 <value><string size="18">Nuitka User Manual</string></value>
 <key>Trapped</key>
@@ -5206,16 +5206,16 @@
 </dict>
 </object>
 
 <trailer>
 <dict size="4">
 <key>ID</key>
 <value><list size="2">
-<string size="16">&#62;U&#130;&#171;&#218;&#137;&#23;s&#161;&#157;R+&#216;&#236;&#21;7</string>
-<string size="16">&#62;U&#130;&#171;&#218;&#137;&#23;s&#161;&#157;R+&#216;&#236;&#21;7</string>
+<string size="16">&#226;&#3;&#128;&#92;&#5;&#226;&#149;&#154;ib&#232;=&#243;&#92;&#233;z</string>
+<string size="16">&#226;&#3;&#128;&#92;&#5;&#226;&#149;&#154;ib&#232;=&#243;&#92;&#233;z</string>
 </list></value>
 <key>Info</key>
 <value><ref id="72" /></value>
 <key>Root</key>
 <value><ref id="71" /></value>
 <key>Size</key>
 <value><number>230</number></value>
```

### Comparing `Nuitka-1.7.2/README.rst` & `Nuitka-1.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/bin/autoformat-nuitka-source` & `Nuitka-1.7.3/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/bin/check-nuitka-with-pylint` & `Nuitka-1.7.3/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/bin/compare_with_cpython` & `Nuitka-1.7.3/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/bin/compare_with_xml` & `Nuitka-1.7.3/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/bin/measure-construct-performance` & `Nuitka-1.7.3/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/bin/nuitka` & `Nuitka-1.7.3/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/bin/nuitka-run` & `Nuitka-1.7.3/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-1.7.3/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-1.7.3/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-1.7.3/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-1.7.3/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-1.7.3/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-1.7.3/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/doc/nuitka2-run.1` & `Nuitka-1.7.3/doc/nuitka2-run.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA-RUN "1" "July 2023" "nuitka-run 1.7.2" "User Commands"
+.TH NUITKA-RUN "1" "July 2023" "nuitka-run 1.7.3" "User Commands"
 .SH NAME
 nuitka-run \- the Python compiler
 .SH SYNOPSIS
 .B nuitka-run
 [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
```

### Comparing `Nuitka-1.7.2/doc/nuitka2.1` & `Nuitka-1.7.3/doc/nuitka2.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA "1" "July 2023" "nuitka 1.7.2" "User Commands"
+.TH NUITKA "1" "July 2023" "nuitka 1.7.3" "User Commands"
 .SH NAME
 nuitka \- the Python compiler
 .SH SYNOPSIS
 .B nuitka
 [\fI\,--module\/\fR] [\fI\,--run\/\fR] [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
```

### Comparing `Nuitka-1.7.2/doc/nuitka3-run.1` & `Nuitka-1.7.3/doc/nuitka3-run.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA-RUN "1" "July 2023" "nuitka-run 1.7.2" "User Commands"
+.TH NUITKA-RUN "1" "July 2023" "nuitka-run 1.7.3" "User Commands"
 .SH NAME
 nuitka-run \- the Python compiler
 .SH SYNOPSIS
 .B nuitka-run
 [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
```

### Comparing `Nuitka-1.7.2/doc/nuitka3.1` & `Nuitka-1.7.3/doc/nuitka3.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.48.1.
-.TH NUITKA "1" "July 2023" "nuitka 1.7.2" "User Commands"
+.TH NUITKA "1" "July 2023" "nuitka 1.7.3" "User Commands"
 .SH NAME
 nuitka \- the Python compiler
 .SH SYNOPSIS
 .B nuitka
 [\fI\,--module\/\fR] [\fI\,--run\/\fR] [\fI\,options\/\fR] \fI\,main_module.py\/\fR
 .SH OPTIONS
 .TP
```

### Comparing `Nuitka-1.7.2/lib/hints.py` & `Nuitka-1.7.3/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/misc/nuitka-run.bat` & `Nuitka-1.7.3/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/misc/nuitka.bat` & `Nuitka-1.7.3/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Builtins.py` & `Nuitka-1.7.3/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/BytecodeCaching.py` & `Nuitka-1.7.3/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Bytecodes.py` & `Nuitka-1.7.3/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/CacheCleanup.py` & `Nuitka-1.7.3/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Constants.py` & `Nuitka-1.7.3/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Errors.py` & `Nuitka-1.7.3/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/MainControl.py` & `Nuitka-1.7.3/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/ModuleRegistry.py` & `Nuitka-1.7.3/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/OptionParsing.py` & `Nuitka-1.7.3/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Options.py` & `Nuitka-1.7.3/nuitka/Options.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/OutputDirectories.py` & `Nuitka-1.7.3/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/PostProcessing.py` & `Nuitka-1.7.3/nuitka/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Progress.py` & `Nuitka-1.7.3/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/PythonFlavors.py` & `Nuitka-1.7.3/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/PythonOperators.py` & `Nuitka-1.7.3/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/PythonVersions.py` & `Nuitka-1.7.3/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Serialization.py` & `Nuitka-1.7.3/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/SourceCodeReferences.py` & `Nuitka-1.7.3/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Tracing.py` & `Nuitka-1.7.3/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/TreeXML.py` & `Nuitka-1.7.3/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Variables.py` & `Nuitka-1.7.3/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/Version.py` & `Nuitka-1.7.3/nuitka/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V1.7.2
+Nuitka V1.7.3
 Copyright (C) 2023 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-1.7.2/nuitka/__init__.py` & `Nuitka-1.7.3/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/__main__.py` & `Nuitka-1.7.3/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/__past__.py` & `Nuitka-1.7.3/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/Backend.scons` & `Nuitka-1.7.3/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/CCompilerVersion.scons` & `Nuitka-1.7.3/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/DataComposerInterface.py` & `Nuitka-1.7.3/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/Onefile.scons` & `Nuitka-1.7.3/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/SconsCaching.py` & `Nuitka-1.7.3/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/SconsCompilerSettings.py` & `Nuitka-1.7.3/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/SconsHacks.py` & `Nuitka-1.7.3/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/SconsInterface.py` & `Nuitka-1.7.3/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/SconsProgress.py` & `Nuitka-1.7.3/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/SconsSpawn.py` & `Nuitka-1.7.3/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/SconsUtils.py` & `Nuitka-1.7.3/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/__init__.py` & `Nuitka-1.7.3/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/allocator.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/builtins.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/calling.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/checkers.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/constants.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/freelists.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/hedley.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/helpers.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/importing.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/incbin.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/prelude.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/printing.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/threading.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/tracing.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-1.7.3/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-1.7.3/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-1.7.3/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-1.7.3/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-1.7.3/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-1.7.3/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/gui.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/gui.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-1.7.3/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-1.7.3/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-1.7.3/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersImport.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersLists.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-1.7.3/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-1.7.3/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/MainProgram.c` & `Nuitka-1.7.3/nuitka/build/static_src/MainProgram.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-1.7.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-1.7.3/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-1.7.3/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/AttributeCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-1.7.3/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/BranchCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/CallCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ClassCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/CodeGeneration.py` & `Nuitka-1.7.3/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-1.7.3/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/CodeHelpers.py` & `Nuitka-1.7.3/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-1.7.3/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ConstantCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/Contexts.py` & `Nuitka-1.7.3/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/CtypesCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/DictCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/Emission.py` & `Nuitka-1.7.3/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ErrorCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/EvalCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-1.7.3/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/FrameCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/FunctionCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/GlobalConstants.py` & `Nuitka-1.7.3/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/IdCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ImportCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/Indentation.py` & `Nuitka-1.7.3/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/IndexCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/InjectCCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/IntegerCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/IteratorCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/LabelCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ListCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/LoaderCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/LoopCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/MatchCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ModuleCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/Namify.py` & `Nuitka-1.7.3/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/OperationCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/PrintCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-1.7.3/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/RaisingCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/Reports.py` & `Nuitka-1.7.3/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/ReturnCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/SetCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/SliceCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/StringCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/TryCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/TupleCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/VariableCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-1.7.3/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/YieldCodes.py` & `Nuitka-1.7.3/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/__init__.py` & `Nuitka-1.7.3/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/c_types/__init__.py` & `Nuitka-1.7.3/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates/__init__.py` & `Nuitka-1.7.3/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-1.7.3/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/containers/Namedtuples.py` & `Nuitka-1.7.3/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/containers/OrderedDicts.py` & `Nuitka-1.7.3/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/containers/OrderedSets.py` & `Nuitka-1.7.3/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-1.7.3/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/containers/__init__.py` & `Nuitka-1.7.3/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/distutils/Build.py` & `Nuitka-1.7.3/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/distutils/DistutilCommands.py` & `Nuitka-1.7.3/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/distutils/__init__.py` & `Nuitka-1.7.3/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/finalizations/Finalization.py` & `Nuitka-1.7.3/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-1.7.3/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/finalizations/__init__.py` & `Nuitka-1.7.3/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/DependsExe.py` & `Nuitka-1.7.3/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-1.7.3/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-1.7.3/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-1.7.3/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-1.7.3/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-1.7.3/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-1.7.3/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/Onefile.py` & `Nuitka-1.7.3/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/Standalone.py` & `Nuitka-1.7.3/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/freezer/__init__.py` & `Nuitka-1.7.3/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/IgnoreListing.py` & `Nuitka-1.7.3/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/ImportCache.py` & `Nuitka-1.7.3/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/ImportResolving.py` & `Nuitka-1.7.3/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/Importing.py` & `Nuitka-1.7.3/nuitka/importing/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/PreloadedPackages.py` & `Nuitka-1.7.3/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/Recursion.py` & `Nuitka-1.7.3/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/StandardLibrary.py` & `Nuitka-1.7.3/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/importing/__init__.py` & `Nuitka-1.7.3/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-1.7.3/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-1.7.3/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/AttributeNodes.py` & `Nuitka-1.7.3/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-1.7.3/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/BytesNodes.py` & `Nuitka-1.7.3/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/CallNodes.py` & `Nuitka-1.7.3/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/Checkers.py` & `Nuitka-1.7.3/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-1.7.3/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ClassNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-1.7.3/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ComparisonNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ConditionalNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/CoroutineNodes.py` & `Nuitka-1.7.3/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/CtypesNodes.py` & `Nuitka-1.7.3/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/DictionaryNodes.py` & `Nuitka-1.7.3/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ExceptionNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ExpressionBases.py` & `Nuitka-1.7.3/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-1.7.3/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-1.7.3/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/FrameNodes.py` & `Nuitka-1.7.3/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-1.7.3/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/FunctionNodes.py` & `Nuitka-1.7.3/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/FutureSpecs.py` & `Nuitka-1.7.3/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/GeneratorNodes.py` & `Nuitka-1.7.3/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-1.7.3/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-1.7.3/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ImportHardNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ImportNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ImportNodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1076,27 +1076,27 @@
             while True:
                 module_name = module_name.getPackageName()
 
                 if not module_name:
                     break
 
                 (
-                    _module_name_found,
+                    found_module_name,
                     module_filename,
                     module_kind,
                     finding,
                 ) = locateModule(
                     module_name=module_name,
                     parent_package=parent_package,
                     level=level,
                 )
 
                 self.used_modules.append(
                     makeModuleUsageAttempt(
-                        module_name=module_name,
+                        module_name=found_module_name,
                         filename=module_filename,
                         module_kind=module_kind,
                         finding=finding,
                         level=level,
                         source_ref=self.source_ref,
                     )
                 )
```

### Comparing `Nuitka-1.7.2/nuitka/nodes/IndicatorMixins.py` & `Nuitka-1.7.3/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/InjectCNodes.py` & `Nuitka-1.7.3/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/IterationHandles.py` & `Nuitka-1.7.3/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-1.7.3/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ListOperationNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-1.7.3/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/LocalsScopes.py` & `Nuitka-1.7.3/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/LoopNodes.py` & `Nuitka-1.7.3/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/MatchNodes.py` & `Nuitka-1.7.3/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ModuleNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/NodeBases.py` & `Nuitka-1.7.3/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-1.7.3/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-1.7.3/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/OperatorNodes.py` & `Nuitka-1.7.3/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-1.7.3/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/OsSysNodes.py` & `Nuitka-1.7.3/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/OutlineNodes.py` & `Nuitka-1.7.3/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-1.7.3/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-1.7.3/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/PrintNodes.py` & `Nuitka-1.7.3/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/ReturnNodes.py` & `Nuitka-1.7.3/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/SideEffectNodes.py` & `Nuitka-1.7.3/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/SliceNodes.py` & `Nuitka-1.7.3/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-1.7.3/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/StatementNodes.py` & `Nuitka-1.7.3/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/StrNodes.py` & `Nuitka-1.7.3/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-1.7.3/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/SubscriptNodes.py` & `Nuitka-1.7.3/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/TryNodes.py` & `Nuitka-1.7.3/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-1.7.3/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/TypeNodes.py` & `Nuitka-1.7.3/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-1.7.3/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/VariableDelNodes.py` & `Nuitka-1.7.3/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/VariableNameNodes.py` & `Nuitka-1.7.3/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/VariableRefNodes.py` & `Nuitka-1.7.3/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-1.7.3/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/YieldNodes.py` & `Nuitka-1.7.3/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/__init__.py` & `Nuitka-1.7.3/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-1.7.3/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-1.7.3/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-1.7.3/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-1.7.3/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/nodes/shapes/__init__.py` & `Nuitka-1.7.3/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-1.7.3/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/FunctionInlining.py` & `Nuitka-1.7.3/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/Graphs.py` & `Nuitka-1.7.3/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/Optimization.py` & `Nuitka-1.7.3/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-1.7.3/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/Tags.py` & `Nuitka-1.7.3/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/TraceCollections.py` & `Nuitka-1.7.3/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/ValueTraces.py` & `Nuitka-1.7.3/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/optimizations/__init__.py` & `Nuitka-1.7.3/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/pgo/PGO.py` & `Nuitka-1.7.3/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/pgo/__init__.py` & `Nuitka-1.7.3/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/PluginBase.py` & `Nuitka-1.7.3/nuitka/plugins/PluginBase.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/Plugins.py` & `Nuitka-1.7.3/nuitka/plugins/Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/__init__.py` & `Nuitka-1.7.3/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-1.7.3/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/TransformersPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-1.7.3/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/__init__.py` & `Nuitka-1.7.3/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-1.7.3/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -776,14 +776,21 @@
 - module-name: 'fsspec.transaction'
   anti-bloat:
     - description: 'remove optional dask usage'
       replacements_plain:
         'import distributed': 'raise ImportError'
       when: 'not use_dask'
 
+- module-name: 'future.standard_library'
+  anti-bloat:
+    - description: 'remove unittest reference'
+      replacements_plain:
+        'from future.moves.test import support': 'raise ImportError'
+      when: 'not use_unittest'
+
 - module-name: 'gevent'
   implicit-imports:
     - depends:
         - '_cffi_backend'
         - 'gevent._config'
         - 'gevent.core'
         - 'gevent.resolver_thread'
@@ -1378,14 +1385,21 @@
   anti-bloat:
     - description: 'remove pytest reference'
       change_function:
         'doctests': 'un-callable'
         'runtests': 'un-callable'
       when: 'not use_pytest'
 
+- module-name: 'multiprocessing.util'
+  anti-bloat:
+    - description: 'remove unittest reference'
+      change_function:
+        '_cleanup_tests': 'un-callable'
+      when: 'not use_unittest'
+
 - module-name: 'nacl._sodium'
   implicit-imports:
     - depends:
         - '_cffi_backend'
 
 - module-name: 'networkx'
   anti-bloat:
@@ -2508,14 +2522,19 @@
         - 'pymoo.cython.*'
 
 - module-name: 'pymoo.gradient.toolbox'
   implicit-imports:
     - depends:
         - 'autograd.numpy'
 
+- module-name: 'pymssql'
+  implicit-imports:
+    - depends:
+        - 'pymssql._mssql'
+
 - module-name: 'pyodbc'
   implicit-imports:
     - depends:
         - 'hashlib'
         - 'decimal'
 
 - module-name: 'pyparsing'
```

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-1.7.3/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-1.7.3/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-1.7.3/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/reports/Reports.py` & `Nuitka-1.7.3/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/reports/__init__.py` & `Nuitka-1.7.3/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-1.7.3/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-1.7.3/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-1.7.3/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-1.7.3/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-1.7.3/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-1.7.3/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-1.7.3/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/HardImportSpecs.py` & `Nuitka-1.7.3/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/ParameterSpecs.py` & `Nuitka-1.7.3/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/specs/__init__.py` & `Nuitka-1.7.3/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/Basics.py` & `Nuitka-1.7.3/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/__init__.py` & `Nuitka-1.7.3/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/commercial/__init__.py` & `Nuitka-1.7.3/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-1.7.3/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/data_composer/__init__.py` & `Nuitka-1.7.3/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/data_composer/__main__.py` & `Nuitka-1.7.3/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-1.7.3/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/environments/Virtualenv.py` & `Nuitka-1.7.3/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/environments/__init__.py` & `Nuitka-1.7.3/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/general/__init__.py` & `Nuitka-1.7.3/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-1.7.3/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-1.7.3/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/general/find_module/FindModuleCode.py` & `Nuitka-1.7.3/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/general/find_module/__init__.py` & `Nuitka-1.7.3/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-1.7.3/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-1.7.3/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-1.7.3/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/podman/Podman.py` & `Nuitka-1.7.3/nuitka/tools/podman/Podman.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/podman/__init__.py` & `Nuitka-1.7.3/nuitka/tools/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/podman/__main__.py` & `Nuitka-1.7.3/nuitka/tools/podman/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/profiler/__init__.py` & `Nuitka-1.7.3/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/profiler/__main__.py` & `Nuitka-1.7.3/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-1.7.3/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-1.7.3/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/scanning/__init__.py` & `Nuitka-1.7.3/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-1.7.3/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/specialize/Common.py` & `Nuitka-1.7.3/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-1.7.3/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-1.7.3/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/specialize/__init__.py` & `Nuitka-1.7.3/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/Common.py` & `Nuitka-1.7.3/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/Constructs.py` & `Nuitka-1.7.3/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/OutputComparison.py` & `Nuitka-1.7.3/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/Pythons.py` & `Nuitka-1.7.3/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-1.7.3/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/SearchModes.py` & `Nuitka-1.7.3/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/Valgrind.py` & `Nuitka-1.7.3/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/__init__.py` & `Nuitka-1.7.3/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-1.7.3/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-1.7.3/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-1.7.3/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-1.7.3/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-1.7.3/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-1.7.3/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-1.7.3/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-1.7.3/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-1.7.3/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-1.7.3/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/watch/__init__.py` & `Nuitka-1.7.3/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tools/watch/__main__.py` & `Nuitka-1.7.3/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/Building.py` & `Nuitka-1.7.3/nuitka/tree/Building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1309,15 +1309,15 @@
                 else:
                     source_diff = getSourceCodeDiff(original_source_code, source_code)
 
                     for line in source_diff:
                         plugins_logger.warning(line)
 
                     if len(contributing_plugins) == 1:
-                        contributing_plugins[0].sysexit(
+                        next(iter(contributing_plugins[0])).sysexit(
                             "Making changes to '%s' that cause SyntaxError '%s'"
                             % (module_name, e)
                         )
                     else:
                         plugins_logger.sysexit(
                             "One of the plugins '%s' is making changes to '%s' that cause SyntaxError '%s'"
                             % (",".join(contributing_plugins), module_name, e)
```

### Comparing `Nuitka-1.7.2/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-1.7.3/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/Extractions.py` & `Nuitka-1.7.3/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/InternalModule.py` & `Nuitka-1.7.3/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/Operations.py` & `Nuitka-1.7.3/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationClasses.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationClasses3.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationMultidist.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-1.7.3/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/SourceHandling.py` & `Nuitka-1.7.3/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/SyntaxErrors.py` & `Nuitka-1.7.3/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/TreeHelpers.py` & `Nuitka-1.7.3/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/VariableClosure.py` & `Nuitka-1.7.3/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/tree/__init__.py` & `Nuitka-1.7.3/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/AppDirs.py` & `Nuitka-1.7.3/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/CStrings.py` & `Nuitka-1.7.3/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/CommandLineOptions.py` & `Nuitka-1.7.3/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Distributions.py` & `Nuitka-1.7.3/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Download.py` & `Nuitka-1.7.3/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Execution.py` & `Nuitka-1.7.3/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/FileOperations.py` & `Nuitka-1.7.3/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Hashing.py` & `Nuitka-1.7.3/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Images.py` & `Nuitka-1.7.3/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Importing.py` & `Nuitka-1.7.3/nuitka/utils/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/InstalledPythons.py` & `Nuitka-1.7.3/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/InstanceCounters.py` & `Nuitka-1.7.3/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Jinja2.py` & `Nuitka-1.7.3/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Json.py` & `Nuitka-1.7.3/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/MacOSApp.py` & `Nuitka-1.7.3/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/MemoryUsage.py` & `Nuitka-1.7.3/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/ModuleNames.py` & `Nuitka-1.7.3/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/ReExecute.py` & `Nuitka-1.7.3/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Rest.py` & `Nuitka-1.7.3/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/SharedLibraries.py` & `Nuitka-1.7.3/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Shebang.py` & `Nuitka-1.7.3/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Signing.py` & `Nuitka-1.7.3/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/StaticLibraries.py` & `Nuitka-1.7.3/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/ThreadedExecutor.py` & `Nuitka-1.7.3/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Timing.py` & `Nuitka-1.7.3/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Utils.py` & `Nuitka-1.7.3/nuitka/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/WindowsFileUsage.py` & `Nuitka-1.7.3/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/WindowsResources.py` & `Nuitka-1.7.3/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/Yaml.py` & `Nuitka-1.7.3/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/nuitka/utils/__init__.py` & `Nuitka-1.7.3/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/pyproject.toml` & `Nuitka-1.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/setup.py` & `Nuitka-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/AssertsTest.py` & `Nuitka-1.7.3/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/AssignmentsTest.py` & `Nuitka-1.7.3/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/AssignmentsTest32.py` & `Nuitka-1.7.3/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/BranchingTest.py` & `Nuitka-1.7.3/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/BuiltinOverload.py` & `Nuitka-1.7.3/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/BuiltinSuperTest.py` & `Nuitka-1.7.3/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/BuiltinsTest.py` & `Nuitka-1.7.3/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ClassMinimalTest.py` & `Nuitka-1.7.3/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ClassesTest.py` & `Nuitka-1.7.3/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ClassesTest32.py` & `Nuitka-1.7.3/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ClassesTest34.py` & `Nuitka-1.7.3/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ComparisonChainsTest.py` & `Nuitka-1.7.3/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ConstantsTest.py` & `Nuitka-1.7.3/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ConstantsTest27.py` & `Nuitka-1.7.3/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/DecoratorsTest.py` & `Nuitka-1.7.3/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/DefaultParametersTest.py` & `Nuitka-1.7.3/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/DoubleDeletionsTest.py` & `Nuitka-1.7.3/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/EmptyModuleTest.py` & `Nuitka-1.7.3/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ExceptionRaisingTest.py` & `Nuitka-1.7.3/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-1.7.3/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-1.7.3/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ExecEvalTest.py` & `Nuitka-1.7.3/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ExtremeClosureTest.py` & `Nuitka-1.7.3/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/FunctionObjectsTest.py` & `Nuitka-1.7.3/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/FunctionsTest.py` & `Nuitka-1.7.3/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/FunctionsTest32.py` & `Nuitka-1.7.3/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/FunctionsTest_2.py` & `Nuitka-1.7.3/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/FutureTest32.py` & `Nuitka-1.7.3/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-1.7.3/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-1.7.3/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/GlobalStatementTest.py` & `Nuitka-1.7.3/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/HelloWorldTest_2.py` & `Nuitka-1.7.3/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ImportingTest.py` & `Nuitka-1.7.3/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/InplaceOperationsTest.py` & `Nuitka-1.7.3/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/InspectionTest.py` & `Nuitka-1.7.3/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/InspectionTest_35.py` & `Nuitka-1.7.3/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/InspectionTest_36.py` & `Nuitka-1.7.3/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/LambdasTest.py` & `Nuitka-1.7.3/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-1.7.3/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ListContractionsTest.py` & `Nuitka-1.7.3/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/LoopingTest.py` & `Nuitka-1.7.3/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/MainProgramsTest.py` & `Nuitka-1.7.3/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ModuleAttributesTest.py` & `Nuitka-1.7.3/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/OperatorsTest.py` & `Nuitka-1.7.3/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/OrderChecksTest.py` & `Nuitka-1.7.3/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/OrderChecksTest27.py` & `Nuitka-1.7.3/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-1.7.3/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ParameterErrorsTest.py` & `Nuitka-1.7.3/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ParameterErrorsTest32.py` & `Nuitka-1.7.3/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/PrintFutureTest.py` & `Nuitka-1.7.3/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/PrintingTest_2.py` & `Nuitka-1.7.3/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/RecursionTest.py` & `Nuitka-1.7.3/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ReferencingTest.py` & `Nuitka-1.7.3/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ReferencingTest27.py` & `Nuitka-1.7.3/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ReferencingTest33.py` & `Nuitka-1.7.3/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ReferencingTest35.py` & `Nuitka-1.7.3/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ReferencingTest36.py` & `Nuitka-1.7.3/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ReferencingTest_2.py` & `Nuitka-1.7.3/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/SlotsTest.py` & `Nuitka-1.7.3/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-1.7.3/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-1.7.3/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-1.7.3/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-1.7.3/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TryContinueFinallyTest.py` & `Nuitka-1.7.3/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TryExceptContinueTest.py` & `Nuitka-1.7.3/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TryExceptFinallyTest.py` & `Nuitka-1.7.3/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TryExceptFramesTest.py` & `Nuitka-1.7.3/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TryReturnFinallyTest.py` & `Nuitka-1.7.3/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/TryYieldFinallyTest.py` & `Nuitka-1.7.3/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/UnicodeTest.py` & `Nuitka-1.7.3/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/UnpackingTest35.py` & `Nuitka-1.7.3/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/VarargsTest.py` & `Nuitka-1.7.3/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/WithStatementsTest.py` & `Nuitka-1.7.3/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/YieldFromTest33.py` & `Nuitka-1.7.3/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/run_all.py` & `Nuitka-1.7.3/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/basics/run_xml.py` & `Nuitka-1.7.3/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/onefile/HelloWorldTest.py` & `Nuitka-1.7.3/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-1.7.3/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/onefile/run_all.py` & `Nuitka-1.7.3/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/ArgumentTypes.py` & `Nuitka-1.7.3/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/Attributes.py` & `Nuitka-1.7.3/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/Calls.py` & `Nuitka-1.7.3/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/Conditions.py` & `Nuitka-1.7.3/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/DecodingOperations.py` & `Nuitka-1.7.3/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/FormatStrings36.py` & `Nuitka-1.7.3/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/HardImports.py` & `Nuitka-1.7.3/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/HardImports_2.py` & `Nuitka-1.7.3/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/Iterations.py` & `Nuitka-1.7.3/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/Len.py` & `Nuitka-1.7.3/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/Operations.py` & `Nuitka-1.7.3/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/Subscripts.py` & `Nuitka-1.7.3/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/optimizations/run_all.py` & `Nuitka-1.7.3/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-1.7.3/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-1.7.3/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-1.7.3/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/run_all.py` & `Nuitka-1.7.3/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-1.7.3/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-1.7.3/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-1.7.3/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-1.7.3/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-1.7.3/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-1.7.3/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/plugins/code_signing/CodeSigningMain.py` & `Nuitka-1.7.3/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-1.7.3/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-1.7.3/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/plugins/parameters/ParametersMain.py` & `Nuitka-1.7.3/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-1.7.3/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/plugins/run_all.py` & `Nuitka-1.7.3/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-1.7.3/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-1.7.3/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-1.7.3/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/absolute_import/foobar/local.py` & `Nuitka-1.7.3/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/absolute_import/foobar/util.py` & `Nuitka-1.7.3/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-1.7.3/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-1.7.3/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-1.7.3/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-1.7.3/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-1.7.3/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-1.7.3/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-1.7.3/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-1.7.3/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-1.7.3/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-1.7.3/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-1.7.3/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-1.7.3/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-1.7.3/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-1.7.3/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-1.7.3/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-1.7.3/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-1.7.3/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/dash_import/DashImportMain.py` & `Nuitka-1.7.3/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/dash_import/dash-module.py` & `Nuitka-1.7.3/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/dash_import/plus+module.py` & `Nuitka-1.7.3/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/dash_main/Dash-Main.py` & `Nuitka-1.7.3/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/deep/DeepProgramMain.py` & `Nuitka-1.7.3/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-1.7.3/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-1.7.3/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/deep/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-1.7.3/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-1.7.3/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-1.7.3/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-1.7.3/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-1.7.3/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-1.7.3/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-1.7.3/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-1.7.3/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-1.7.3/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/main_raises/ErrorMain.py` & `Nuitka-1.7.3/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-1.7.3/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-1.7.3/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-1.7.3/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-1.7.3/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-1.7.3/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-1.7.3/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-1.7.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-1.7.3/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_exits/Main.py` & `Nuitka-1.7.3/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-1.7.3/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-1.7.3/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-1.7.3/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-1.7.3/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-1.7.3/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-1.7.3/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-1.7.3/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-1.7.3/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-1.7.3/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-1.7.3/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-1.7.3/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_code/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-1.7.3/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_contains_main/__init__.py` & `Nuitka-1.7.3/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_contains_main/local.py` & `Nuitka-1.7.3/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-1.7.3/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-1.7.3/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-1.7.3/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-1.7.3/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-1.7.3/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-1.7.3/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-1.7.3/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-1.7.3/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-1.7.3/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-1.7.3/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_module_collision/something.py` & `Nuitka-1.7.3/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_overload/Main.py` & `Nuitka-1.7.3/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_overload/foo/__init__.py` & `Nuitka-1.7.3/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_overload/foo/bar.py` & `Nuitka-1.7.3/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_overload/foo/bar2.py` & `Nuitka-1.7.3/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-1.7.3/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-1.7.3/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-1.7.3/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-1.7.3/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-1.7.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-1.7.3/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-1.7.3/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-1.7.3/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-1.7.3/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-1.7.3/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-1.7.3/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-1.7.3/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/relative_import/dircache.py` & `Nuitka-1.7.3/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-1.7.3/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/run_all.py` & `Nuitka-1.7.3/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-1.7.3/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-1.7.3/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-1.7.3/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-1.7.3/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-1.7.3/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-1.7.3/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-1.7.3/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-1.7.3/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/programs/with space/Space Main.py` & `Nuitka-1.7.3/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/reflected/compile_itself.py` & `Nuitka-1.7.3/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/run-tests` & `Nuitka-1.7.3/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/BrotliUsing.py` & `Nuitka-1.7.3/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/CtypesUsing.py` & `Nuitka-1.7.3/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/FlaskUsing.py` & `Nuitka-1.7.3/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/GlfwUsing.py` & `Nuitka-1.7.3/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/GtkUsing.py` & `Nuitka-1.7.3/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/HexEncodingTest_2.py` & `Nuitka-1.7.3/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/IdnaUsing.py` & `Nuitka-1.7.3/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/LxmlUsing.py` & `Nuitka-1.7.3/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/MatplotlibUsing.py` & `Nuitka-1.7.3/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-1.7.3/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/NumpyUsing.py` & `Nuitka-1.7.3/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/OpenGLUsing.py` & `Nuitka-1.7.3/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PandasUsing.py` & `Nuitka-1.7.3/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PasslibUsing.py` & `Nuitka-1.7.3/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PendulumUsing.py` & `Nuitka-1.7.3/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-1.7.3/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PmwUsing.py` & `Nuitka-1.7.3/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PyQt5Plugins.py` & `Nuitka-1.7.3/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-1.7.3/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PyQt5Using.py` & `Nuitka-1.7.3/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PyQt6Plugins.py` & `Nuitka-1.7.3/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PyQt6Using.py` & `Nuitka-1.7.3/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PySide6Plugins.py` & `Nuitka-1.7.3/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/PySide6Using.py` & `Nuitka-1.7.3/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/RsaUsing.py` & `Nuitka-1.7.3/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/ShlibUsing.py` & `Nuitka-1.7.3/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/SocketUsing.py` & `Nuitka-1.7.3/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/TkInterUsing.py` & `Nuitka-1.7.3/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/Urllib3Using.py` & `Nuitka-1.7.3/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/Win32ComUsing.py` & `Nuitka-1.7.3/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/run_all.py` & `Nuitka-1.7.3/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-1.7.3/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/AsyncgenReturn36.py` & `Nuitka-1.7.3/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/BreakWithoutLoop.py` & `Nuitka-1.7.3/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/ClassReturn.py` & `Nuitka-1.7.3/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/ClosureDel_2.py` & `Nuitka-1.7.3/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-1.7.3/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/DuplicateArgument.py` & `Nuitka-1.7.3/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/ExecWithNesting_2.py` & `Nuitka-1.7.3/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/FutureBraces.py` & `Nuitka-1.7.3/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/FutureUnknown.py` & `Nuitka-1.7.3/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/GeneratorExpressions38.py` & `Nuitka-1.7.3/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/GeneratorReturn_2.py` & `Nuitka-1.7.3/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/GlobalForParameter.py` & `Nuitka-1.7.3/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/Importing32.py` & `Nuitka-1.7.3/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/IndentationError.py` & `Nuitka-1.7.3/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/LateFutureImport.py` & `Nuitka-1.7.3/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/MisplacedFutureImport.py` & `Nuitka-1.7.3/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/ModuleReturn.py` & `Nuitka-1.7.3/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-1.7.3/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/NonlocalForParameter32.py` & `Nuitka-1.7.3/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/NonlocalNotFound32.py` & `Nuitka-1.7.3/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/StarImportExtra.py` & `Nuitka-1.7.3/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/SyntaxError.py` & `Nuitka-1.7.3/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-1.7.3/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-1.7.3/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/UnpackNoTuple.py` & `Nuitka-1.7.3/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/UnpackTwoStars32.py` & `Nuitka-1.7.3/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/YieldFromInModule.py` & `Nuitka-1.7.3/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/YieldInAsync35.py` & `Nuitka-1.7.3/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/YieldInGenexp38.py` & `Nuitka-1.7.3/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/YieldInModule.py` & `Nuitka-1.7.3/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-1.7.2/tests/syntax/run_all.py` & `Nuitka-1.7.3/tests/syntax/run_all.py`

 * *Files identical despite different names*

