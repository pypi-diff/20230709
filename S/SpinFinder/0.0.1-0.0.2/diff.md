# Comparing `tmp/spinfinder-0.0.1.tar.gz` & `tmp/spinfinder-0.0.2.tar.gz`

## Comparing `spinfinder-0.0.1.tar` & `spinfinder-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinfinder-0.0.1/scr/SpinFinder/__init__.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 spinfinder-0.0.1/scr/SpinFinder/ovchinnikov.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 spinfinder-0.0.1/scr/SpinFinder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 spinfinder-0.0.1/scr/SpinFinder/.ipynb_checkpoints/Untitled1-checkpoint.ipynb
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 spinfinder-0.0.1/scr/SpinFinder/.ipynb_checkpoints/gen_str-checkpoint.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 spinfinder-0.0.1/LICENSE
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spinfinder-0.0.1/README.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 spinfinder-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spinfinder-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spinfinder-0.0.2/scr/spinfinder/__init__.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 spinfinder-0.0.2/scr/spinfinder/spinfinder.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 spinfinder-0.0.2/scr/spinfinder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 spinfinder-0.0.2/scr/spinfinder/.ipynb_checkpoints/Untitled1-checkpoint.ipynb
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 spinfinder-0.0.2/scr/spinfinder/.ipynb_checkpoints/gen_str-checkpoint.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 spinfinder-0.0.2/LICENSE
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spinfinder-0.0.2/README.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 spinfinder-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spinfinder-0.0.2/PKG-INFO
```

### Comparing `spinfinder-0.0.1/scr/SpinFinder/ovchinnikov.py` & `spinfinder-0.0.2/scr/spinfinder/spinfinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # In[1]:
 
 
-def spin_finder(PATH):
+def ovchinnikov(PATH):
     from rdkit import Chem
     from openbabel import pybel
     import pandas as pd
     m = Chem.MolFromSmiles(next(pybel.readfile("xyz",PATH)).write(format="smi").split()[0].strip())
     A=Chem.rdmolops.GetAdjacencyMatrix(m)
     q=pd.DataFrame(A)
     q=q.rename(columns={0:'↑'},index={0:'↑'})
```

### Comparing `spinfinder-0.0.1/scr/SpinFinder/.ipynb_checkpoints/gen_str-checkpoint.py` & `spinfinder-0.0.2/scr/spinfinder/.ipynb_checkpoints/gen_str-checkpoint.py`

 * *Files identical despite different names*

### Comparing `spinfinder-0.0.1/LICENSE` & `spinfinder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spinfinder-0.0.1/README.md` & `spinfinder-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spinfinder-0.0.1/PKG-INFO` & `spinfinder-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpinFinder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Calculate the spin multiplicity of your PAH fast using Ovchinnikov's rule.
 Author-email: Stiv Llenga <stiv.llenga@h-its.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

