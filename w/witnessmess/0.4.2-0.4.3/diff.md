# Comparing `tmp/witnessmess-0.4.2-py3-none-any.whl.zip` & `tmp/witnessmess-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 15387 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1173 b- defN 23-Feb-28 18:44 witnessmess/__init__.py
--rw-r--r--  2.0 unx    17034 b- defN 23-Feb-28 18:44 witnessmess/_cm.py
--rw-r--r--  2.0 unx     7425 b- defN 23-Feb-28 18:44 witnessmess/_dm.py
--rw-r--r--  2.0 unx     2933 b- defN 23-Feb-28 18:44 witnessmess/_pi.py
--rw-r--r--  2.0 unx     7652 b- defN 23-Feb-28 18:44 witnessmess-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5310 b- defN 23-Feb-28 18:44 witnessmess-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-28 18:44 witnessmess-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Feb-28 18:44 witnessmess-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      712 b- defN 23-Feb-28 18:44 witnessmess-0.4.2.dist-info/RECORD
-9 files, 42343 bytes uncompressed, 14169 bytes compressed:  66.5%
+Zip file size: 15468 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1173 b- defN 23-Jul-09 04:35 witnessmess/__init__.py
+-rw-r--r--  2.0 unx    17034 b- defN 23-Jul-09 04:35 witnessmess/_cm.py
+-rw-r--r--  2.0 unx     7425 b- defN 23-Jul-09 04:35 witnessmess/_dm.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-Jul-09 04:35 witnessmess/_pi.py
+-rw-r--r--  2.0 unx     7652 b- defN 23-Jul-09 04:36 witnessmess-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5449 b- defN 23-Jul-09 04:36 witnessmess-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 04:36 witnessmess-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-09 04:36 witnessmess-0.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      712 b- defN 23-Jul-09 04:36 witnessmess-0.4.3.dist-info/RECORD
+9 files, 42557 bytes uncompressed, 14250 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: witnessmess/_dm.py
 Comment: 
 
 Filename: witnessmess/_pi.py
 Comment: 
 
-Filename: witnessmess-0.4.2.dist-info/LICENSE
+Filename: witnessmess-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: witnessmess-0.4.2.dist-info/METADATA
+Filename: witnessmess-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: witnessmess-0.4.2.dist-info/WHEEL
+Filename: witnessmess-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: witnessmess-0.4.2.dist-info/top_level.txt
+Filename: witnessmess-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: witnessmess-0.4.2.dist-info/RECORD
+Filename: witnessmess-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## witnessmess/__init__.py

```diff
@@ -4,15 +4,15 @@
 
 '''
 Witnessing genuine multi-partite entanglement from a subset of marginalia both
 in multi-partite qubit systems and multi-mode continuous variable Gaussian
 systems.
 '''
 
-version = '0.4.2'
+version = '0.4.3'
 
 # Genuine multi-partite entanglement witness for discrete variable multi-qudit
 # systems inferred from their density matrices.
 
 from ._dm import (
     dm_optimal_witness, 
     dm_is_physical
```

## witnessmess/_pi.py

```diff
@@ -1,15 +1,14 @@
 #!/bin/env python
 
 # 2019 - 2023 Jan Provaznik (jan@provaznik.pro)
 #
 # Shared components.
 
 import picos
-import mosek
 
 # The number $K$ of unique unordered bi-partitions of $N$ elements is given by
 # the Stirling number of the second kind [4] as $K := 2^{N - 1} - 1$.
 #
 # [4] https://en.wikipedia.org/wiki/Stirling_numbers_of_the_second_kind
 
 def bipartition_count (N):
@@ -63,21 +62,26 @@
     Returns
     -------
     bool
         True if license was deemed good enough.
     '''
 
     try:
+        import mosek
+    except ImportError as error:
+        return False
+
+    try:
         mosek_env = picos.solvers.get_solver('mosek')._get_environment()
         mosek_env.checkoutlicense(mosek.feature.pton)
         mosek_env.checkinall()
-        return 1
     except mosek.Error as error:
-        return 0
+        return False
 
+    return True
 
 def picos_debug_constraints (problem):
     '''
     Use on solved problem to debug constraint values.
 
     Parameters
     ----------
```

## Comparing `witnessmess-0.4.2.dist-info/LICENSE` & `witnessmess-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `witnessmess-0.4.2.dist-info/METADATA` & `witnessmess-0.4.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: witnessmess
-Version: 0.4.2
+Version: 0.4.3
 Summary: Witnessing multi-partite entanglement.
 Home-page: https://provaznik.pro/witnessmess
 Author: Jan Provaznik
 Author-email: jan@provaznik.pro
 License: LGPL
 Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: picos (>=2.4)
-Requires-Dist: numpy (>=1.22)
-Requires-Dist: scipy (>=1.8)
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 WITNESS MESS provides procedures for witnessing genuine multi-partite
 entanglement from a subset of marginalia both in multi-partite qubit systems
 and multi-mode continuous variable Gaussian systems.
 
-Examples
-
-  See the examples directory. Both discrete and continuous variable examples
-  are provided.
-
 Prerequisites
 
   A suitable semi-definite optimizer is required. 
 
   - MOSEK is a commercial optimization software. Free personal licenses are
     provided to members of academia. It is preferred for its unmatched speed
     and versatility. 
 
   - CVXOPT is an open source convex optimization software. It can be used as
     well, however, it is considerably slower than MOSEK.
 
+Installation
+
+  As of release 0.4.2 it is possible to retrieve the latest release of the 
+  package from PyPi by running 'pip install --user witnessmess' 
+
+Examples
+
+  See the examples directory. Both discrete and continuous variable examples
+  are provided.
+
 Documentation
 
   Genuine multipartite entanglement can be witnessed with a pair of functions
   that determine optimal entanglement witnesses for particular, either discrete
   or (Gaussian) continuous variable, quantum states.
 
   Please note that the definition of covariance matrices follows the
```

