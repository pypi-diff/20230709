# Comparing `tmp/CircuitCalculator-0.0.8.tar.gz` & `tmp/CircuitCalculator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircuitCalculator-0.0.8.tar", last modified: Wed Apr  5 14:12:47 2023, max compression
+gzip compressed data, was "CircuitCalculator-0.0.9.tar", last modified: Wed Apr  5 14:53:27 2023, max compression
```

## Comparing `CircuitCalculator-0.0.8.tar` & `CircuitCalculator-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.614900 CircuitCalculator-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 14:12:47.614900 CircuitCalculator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:12:47.614900 CircuitCalculator-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.610900 CircuitCalculator-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.610900 CircuitCalculator-0.0.8/src/CircuitCalculator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.610900 CircuitCalculator-0.0.8/src/CircuitCalculator/Circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Circuit/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Circuit/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/EquivalentSources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.614900 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/labelmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/supernodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Network/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/NodalAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/PlottingTemplates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.614900 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleAnalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleAnalysis/Elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleAnalysis/Layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.614900 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/Display.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/Elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/src/CircuitCalculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.610900 CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 14:12:47.000000 CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-05 14:12:47.000000 CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:12:47.000000 CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-05 14:12:47.000000 CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 14:12:47.000000 CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:12:47.614900 CircuitCalculator-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-05 14:12:38.000000 CircuitCalculator-0.0.8/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.190033 CircuitCalculator-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:53:27.190033 CircuitCalculator-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.182033 CircuitCalculator-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/EquivalentSources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/labelmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/supernodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Network/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/NodalAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/PlottingTemplates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/Elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/Layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/DiagramParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/Display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/Elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/SchemdrawTranslatorTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/src/CircuitCalculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 14:53:27.000000 CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:53:27.186033 CircuitCalculator-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-05 14:53:18.000000 CircuitCalculator-0.0.9/tests/test_integration.py
```

### Comparing `CircuitCalculator-0.0.8/LICENSE` & `CircuitCalculator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/PKG-INFO` & `CircuitCalculator-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CircuitCalculator
```

### Comparing `CircuitCalculator-0.0.8/README.md` & `CircuitCalculator-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Circuit/circuit.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/circuit.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Circuit/components.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/components.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Circuit/transformers.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Circuit/transformers.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/EquivalentSources.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/EquivalentSources.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Network/elements.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/elements.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Network/loaders.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/loaders.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Network/network.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/network.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Network/supernodes.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/supernodes.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Network/transformers.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Network/transformers.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/NodalAnalysis.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/NodalAnalysis.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/PlottingTemplates.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/PlottingTemplates.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleAnalysis/Elements.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/Elements.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleAnalysis/Layout.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/Layout.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleAnalysis/PointerDiagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             draw_pointer(height=self._arrow_base*self._max_length, width=self._arrow_length*self._max_length)
         x_min, x_max = self.ax.get_xlim()
         y_min, y_max = self.ax.get_ylim()
         self.ax.set_xlim(xmin=min(x_min, y_min), xmax=max(x_max, y_max))
         self.ax.set_ylim(ymin=min(x_min, y_min), ymax=max(x_max, y_max))
         self.ax.legend(
             handles=[line for line in self.ax.lines],
-            ncols=len(self.ax.lines),
+            ncol=len(self.ax.lines),
             loc='upper center',
             bbox_to_anchor=(0.5, 1.1),
             frameon=False
         )
 
     def add_pointer(self, z: complex, z0: complex = 0, **kwargs):
         self._max_length = max(self._max_length, np.abs(z))
```

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/CircuitComponentTranslators.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/DiagramParser.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/DiagramParser.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/Display.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/Display.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/Elements.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/Elements.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/SimpleCircuit/NetworkBranchTranslators.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator/Utils.py` & `CircuitCalculator-0.0.9/src/CircuitCalculator/Utils.py`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/PKG-INFO` & `CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircuitCalculator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for analysing and calculating electric networks.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CircuitCalculator
```

### Comparing `CircuitCalculator-0.0.8/src/CircuitCalculator.egg-info/SOURCES.txt` & `CircuitCalculator-0.0.9/src/CircuitCalculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CircuitCalculator-0.0.8/tests/test_integration.py` & `CircuitCalculator-0.0.9/tests/test_integration.py`

 * *Files identical despite different names*

