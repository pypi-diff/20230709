# Comparing `tmp/nir-0.0.4.tar.gz` & `tmp/nir-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nir-0.0.4.tar", last modified: Sat Jul  8 23:46:41 2023, max compression
+gzip compressed data, was "nir-0.0.5.tar", last modified: Sat Jul  8 23:58:59 2023, max compression
```

## Comparing `nir-0.0.4.tar` & `nir-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:46:41.586617 nir-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-08 23:46:33.000000 nir-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-08 23:46:33.000000 nir-0.0.4/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/nir/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 23:46:33.000000 nir-0.0.4/nir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-08 23:46:33.000000 nir-0.0.4/nir/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-08 23:46:33.000000 nir-0.0.4/nir/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-08 23:46:33.000000 nir-0.0.4/nir/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/nir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-08 23:46:33.000000 nir-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:46:41.586617 nir-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:33.000000 nir-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-08 23:46:33.000000 nir-0.0.4/tests/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-08 23:46:33.000000 nir-0.0.4/tests/test_readwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:58:59.248926 nir-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-08 23:58:51.000000 nir-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-08 23:58:51.000000 nir-0.0.5/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/nir/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 23:58:51.000000 nir-0.0.5/nir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-08 23:58:51.000000 nir-0.0.5/nir/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-08 23:58:51.000000 nir-0.0.5/nir/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-08 23:58:51.000000 nir-0.0.5/nir/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/nir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-08 23:58:51.000000 nir-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:58:59.248926 nir-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:51.000000 nir-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-08 23:58:51.000000 nir-0.0.5/tests/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-08 23:58:51.000000 nir-0.0.5/tests/test_readwrite.py
```

### Comparing `nir-0.0.4/PKG-INFO` & `nir-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.4
+Version: 0.0.5
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nir-0.0.4/README.md` & `nir-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nir-0.0.4/docs/source/conf.py` & `nir-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nir-0.0.4/nir/ir.py` & `nir-0.0.5/nir/ir.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,14 +51,38 @@
         \dot{v} = R I
     """
 
     r: np.ndarray
 
 
 @dataclass
+class IF(NIRNode):
+    """Integrate-and-fire neuron model.
+
+   The integrate-and-fire neuron model is defined by the following equations:
+
+   .. math::
+        \dot{V} = R I
+
+        z = \begin{cases} 
+            1 & v > v_{threshold} \\ 
+            0 & else
+        \end{cases}
+
+        v = \begin{cases}
+            v-v_{thr} & z=1 \\
+            v & else
+            \end{cases}
+    """
+
+    r: np.ndarray  # Resistance
+    v_threshold: np.ndarray  # Firing threshold
+
+
+@dataclass
 class LI(NIRNode):
     r"""Leaky integrator neuron model.
 
     The leaky integrator neuron model is defined by the following equation:
 
     .. math::
         \tau \dot{v} = (v_{leak} - v) + R I
```

### Comparing `nir-0.0.4/nir/read.py` & `nir-0.0.5/nir/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,21 @@
                 )
             elif node["type"][()] == b"I":
                 nodes.append(
                     nir.I(
                         r=node["r"][()],
                     )
                 )
+            elif node["type"][()] == b"IF":
+                nodes.append(
+                    nir.IF(
+                        r=node["r"][()],
+                        v_threshold=node["v_threshold"][()],
+                    )
+                )
             elif node["type"][()] == b"Input":
                 nodes.append(
                     nir.Input(
                         shape=node["shape"][()],
                     )
                 )
             elif node["type"][()] == b"Output":
```

### Comparing `nir-0.0.4/nir/write.py` & `nir-0.0.5/nir/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 def write(filename: typing.Union[str, pathlib.Path], graph: nir.NIR) -> None:
     def convert_node(node: nir.NIRNode) -> dict:
         if isinstance(node, nir.Delay):
             return {"type": "Delay", "delay": node.delay}
         elif isinstance(node, nir.I):
             return {"type": "I", "r": node.r}
+        elif isinstance(node, nir.IF):
+            return {"type": "IF", "r": node.r, "v_threshold": node.v_threshold}
         elif isinstance(node, nir.Input):
             return {
                 "type": "Input",
                 "shape": node.shape,
             }
         elif isinstance(node, nir.LI):
             return {
```

### Comparing `nir-0.0.4/nir.egg-info/PKG-INFO` & `nir-0.0.5/nir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.4
+Version: 0.0.5
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nir-0.0.4/pyproject.toml` & `nir-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "nir"
-version = "0.0.4"
+version = "0.0.5"
 description = "Neuromorphic Intermediate Representation"
 authors = [
   { name = "Steven Abreu", email = "s.abreu@rug.nl" },
   { name = "Felix Bauer", email = "felix.bauer@synsense.ai" },
   { name = "Jason Eshraghian", email = "jeshragh@ucsc.edu" },
   { name = "Matthias Jobst", email = "matthias.jobst2@tu-dresden.de" },
   { name = "Gregor Lenz", email = "mail@lenzgregor.com" },
```

### Comparing `nir-0.0.4/tests/test_ir.py` & `nir-0.0.5/tests/test_ir.py`

 * *Files identical despite different names*

### Comparing `nir-0.0.4/tests/test_readwrite.py` & `nir-0.0.5/tests/test_readwrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,22 @@
     ir = nir.NIR(
         nodes=[nir.Linear(weights=[1], bias=0), nir.I(r=2)],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
 
 
+def test_integrator():
+    ir = nir.NIR(
+        nodes=[nir.Linear(weights=[1], bias=0), nir.IF(r=2, v_threshold=3)],
+        edges=[(0, 0)],
+    )
+    factory_test_graph(ir)
+
+
 def test_leaky_integrator():
     ir = nir.NIR(
         nodes=[nir.Linear(weights=[1], bias=0), nir.LI(tau=1, r=2, v_leak=3)],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
```

