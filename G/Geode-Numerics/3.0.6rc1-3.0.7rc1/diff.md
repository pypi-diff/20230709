# Comparing `tmp/Geode_Numerics-3.0.6rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Numerics-3.0.7rc1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,14 @@
-Zip file size: 2824749 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat      205 b- defN 23-Jun-29 12:43 geode_numerics/__init__.py
--rw-rw-rw-  2.0 fat      193 b- defN 23-Jun-29 12:43 geode_numerics/scalar_function.py
--rw-rw-rw-  2.0 fat      178 b- defN 23-Jun-29 12:43 geode_numerics/surface.py
--rw-rw-rw-  2.0 fat  2266624 b- defN 23-Jun-29 12:44 geode_numerics/bin/Geode-Numerics_frame_field.dll
--rw-rw-rw-  2.0 fat  2145280 b- defN 23-Jun-29 12:44 geode_numerics/bin/Geode-Numerics_scalar_function.dll
--rw-rw-rw-  2.0 fat    60928 b- defN 23-Jun-29 12:44 geode_numerics/bin/Geode-Numerics_surface.dll
--rw-rw-rw-  2.0 fat   317864 b- defN 23-Jun-29 12:44 geode_numerics/bin/concrt140.dll
--rw-rw-rw-  2.0 fat   181760 b- defN 23-Jun-29 12:44 geode_numerics/bin/geode_numerics_py_scalar_function.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   130560 b- defN 23-Jun-29 12:44 geode_numerics/bin/geode_numerics_py_surface.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   566704 b- defN 23-Jun-29 12:44 geode_numerics/bin/msvcp140.dll
--rw-rw-rw-  2.0 fat    23944 b- defN 23-Jun-29 12:44 geode_numerics/bin/msvcp140_1.dll
--rw-rw-rw-  2.0 fat   186800 b- defN 23-Jun-29 12:44 geode_numerics/bin/msvcp140_2.dll
--rw-rw-rw-  2.0 fat    57264 b- defN 23-Jun-29 12:44 geode_numerics/bin/msvcp140_atomic_wait.dll
--rw-rw-rw-  2.0 fat    21424 b- defN 23-Jun-29 12:44 geode_numerics/bin/msvcp140_codecvt_ids.dll
--rw-rw-rw-  2.0 fat    98224 b- defN 23-Jun-29 12:44 geode_numerics/bin/vcruntime140.dll
--rw-rw-rw-  2.0 fat    37256 b- defN 23-Jun-29 12:44 geode_numerics/bin/vcruntime140_1.dll
--rw-rw-rw-  2.0 fat     2243 b- defN 23-Jun-29 12:44 Geode_Numerics-3.0.6rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-29 12:44 Geode_Numerics-3.0.6rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-29 12:44 Geode_Numerics-3.0.6rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1922 b- defN 23-Jun-29 12:44 Geode_Numerics-3.0.6rc1.dist-info/RECORD
-20 files, 6099488 bytes uncompressed, 2821567 bytes compressed:  53.7%
+Zip file size: 3096842 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-09 05:27 geode_numerics/__init__.py
+-rw-r--r--  2.0 unx      187 b- defN 23-Jul-09 05:27 geode_numerics/scalar_function.py
+-rw-r--r--  2.0 unx      172 b- defN 23-Jul-09 05:27 geode_numerics/surface.py
+-rwxr-xr-x  2.0 unx   208448 b- defN 23-Jul-09 05:28 geode_numerics/lib64/geode_numerics_py_scalar_function.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   130456 b- defN 23-Jul-09 05:28 geode_numerics/lib64/geode_numerics_py_surface.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  3417136 b- defN 23-Jul-09 05:28 geode_numerics/lib64/libGeode-Numerics_frame_field.so
+-rwxr-xr-x  2.0 unx  3349904 b- defN 23-Jul-09 05:28 geode_numerics/lib64/libGeode-Numerics_scalar_function.so
+-rwxr-xr-x  2.0 unx    80576 b- defN 23-Jul-09 05:28 geode_numerics/lib64/libGeode-Numerics_surface.so
+-rw-r--r--  2.0 unx     2180 b- defN 23-Jul-09 05:28 Geode_Numerics-3.0.7rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-09 05:28 Geode_Numerics-3.0.7rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-09 05:28 Geode_Numerics-3.0.7rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1208 b- defN 23-Jul-09 05:28 Geode_Numerics-3.0.7rc1.dist-info/RECORD
+12 files, 7190485 bytes uncompressed, 3094762 bytes compressed:  57.0%
```

## zipnote {}

```diff
@@ -3,59 +3,35 @@
 
 Filename: geode_numerics/scalar_function.py
 Comment: 
 
 Filename: geode_numerics/surface.py
 Comment: 
 
-Filename: geode_numerics/bin/Geode-Numerics_frame_field.dll
+Filename: geode_numerics/lib64/geode_numerics_py_scalar_function.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_numerics/bin/Geode-Numerics_scalar_function.dll
+Filename: geode_numerics/lib64/geode_numerics_py_surface.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_numerics/bin/Geode-Numerics_surface.dll
+Filename: geode_numerics/lib64/libGeode-Numerics_frame_field.so
 Comment: 
 
-Filename: geode_numerics/bin/concrt140.dll
+Filename: geode_numerics/lib64/libGeode-Numerics_scalar_function.so
 Comment: 
 
-Filename: geode_numerics/bin/geode_numerics_py_scalar_function.cp39-win_amd64.pyd
+Filename: geode_numerics/lib64/libGeode-Numerics_surface.so
 Comment: 
 
-Filename: geode_numerics/bin/geode_numerics_py_surface.cp39-win_amd64.pyd
+Filename: Geode_Numerics-3.0.7rc1.dist-info/METADATA
 Comment: 
 
-Filename: geode_numerics/bin/msvcp140.dll
+Filename: Geode_Numerics-3.0.7rc1.dist-info/WHEEL
 Comment: 
 
-Filename: geode_numerics/bin/msvcp140_1.dll
+Filename: Geode_Numerics-3.0.7rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: geode_numerics/bin/msvcp140_2.dll
-Comment: 
-
-Filename: geode_numerics/bin/msvcp140_atomic_wait.dll
-Comment: 
-
-Filename: geode_numerics/bin/msvcp140_codecvt_ids.dll
-Comment: 
-
-Filename: geode_numerics/bin/vcruntime140.dll
-Comment: 
-
-Filename: geode_numerics/bin/vcruntime140_1.dll
-Comment: 
-
-Filename: Geode_Numerics-3.0.6rc1.dist-info/METADATA
-Comment: 
-
-Filename: Geode_Numerics-3.0.6rc1.dist-info/WHEEL
-Comment: 
-
-Filename: Geode_Numerics-3.0.6rc1.dist-info/top_level.txt
-Comment: 
-
-Filename: Geode_Numerics-3.0.6rc1.dist-info/RECORD
+Filename: Geode_Numerics-3.0.7rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_numerics/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .surface import *
-from .scalar_function import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .surface import *
+from .scalar_function import *
```

## geode_numerics/scalar_function.py

```diff
@@ -1,8 +1,8 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-
-from .bin.geode_numerics_py_scalar_function import *
-NumericsScalarFunctionLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+
+from .lib64.geode_numerics_py_scalar_function import *
+NumericsScalarFunctionLibrary.initialize()
```

## geode_numerics/surface.py

```diff
@@ -1,8 +1,8 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-
-from .bin.geode_numerics_py_surface import *
-NumericsSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+
+from .lib64.geode_numerics_py_surface import *
+NumericsSurfaceLibrary.initialize()
```

## Comparing `Geode_Numerics-3.0.6rc1.dist-info/METADATA` & `Geode_Numerics-3.0.7rc1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-Metadata-Version: 2.1
-Name: Geode-Numerics
-Version: 3.0.6rc1
-Summary: Numerical algorithm module
-Home-page: https://github.com/Geode-solutions/Geode-Numerics
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.4.0rc2)
-
-<h1 align="center">Geode-Numerics<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Numerics OpenGeode module</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Numerics_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Numerics_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-  <img src="https://img.shields.io/static/v1?label=macOS&logo=apple&logoColor=white&message=support&color=success" alt="macOS support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-  <a href="https://doi.org/10.5281/zenodo.3610370">
-    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
-  </a>
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Numerics
+Version: 3.0.7rc1
+Summary: Numerical algorithm module
+Home-page: https://github.com/Geode-solutions/Geode-Numerics
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: opengeode-core (==14.*,>=14.4.1rc3)
+
+<h1 align="center">Geode-Numerics<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Numerics OpenGeode module</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Numerics_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Numerics_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+  <img src="https://img.shields.io/static/v1?label=macOS&logo=apple&logoColor=white&message=support&color=success" alt="macOS support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+  <a href="https://doi.org/10.5281/zenodo.3610370">
+    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
+  </a>
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: Geode-Numerics Version: 3.0.6rc1 Summary: Numerical
+Metadata-Version: 2.1 Name: Geode-Numerics Version: 3.0.7rc1 Summary: Numerical
 algorithm module Home-page: https://github.com/Geode-solutions/Geode-Numerics
 Author: Geode-solutions Author-email: contact@geode-solutions.com License:
-Proprietary Platform: UNKNOWN Description-Content-Type: text/markdown Requires-
-Dist: opengeode-core (==14.*,>=14.4.0rc2)
+Proprietary Description-Content-Type: text/markdown Requires-Dist: opengeode-
+core (==14.*,>=14.4.1rc3)
                 ****** Geode-Numericsby Geode-solutions ******
                       **** Numerics OpenGeode module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
      [Windows support] [Ubuntu support] [Red Hat support] [macOS support]
 [Language] [License] [Semantic-release] [Slack_invite] [DOI] Copyright (c) 2019
                            - 2023, Geode-solutions
```

