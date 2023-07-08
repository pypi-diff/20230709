# Comparing `tmp/nir-0.0.3.tar.gz` & `tmp/nir-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nir-0.0.3.tar", last modified: Wed Jul  5 19:09:23 2023, max compression
+gzip compressed data, was "nir-0.0.4.tar", last modified: Sat Jul  8 23:46:41 2023, max compression
```

## Comparing `nir-0.0.3.tar` & `nir-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:09:23.929984 nir-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-05 19:09:23.929984 nir-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-05 19:09:14.000000 nir-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:09:23.929984 nir-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-05 19:09:14.000000 nir-0.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:09:23.929984 nir-0.0.3/nir/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-05 19:09:14.000000 nir-0.0.3/nir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-05 19:09:14.000000 nir-0.0.3/nir/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-05 19:09:14.000000 nir-0.0.3/nir/read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:09:23.929984 nir-0.0.3/nir/test/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-05 19:09:14.000000 nir-0.0.3/nir/test/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 19:09:14.000000 nir-0.0.3/nir/test/test_readwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-05 19:09:14.000000 nir-0.0.3/nir/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:09:23.929984 nir-0.0.3/nir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-05 19:09:23.000000 nir-0.0.3/nir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 19:09:23.000000 nir-0.0.3/nir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:09:23.000000 nir-0.0.3/nir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 19:09:23.000000 nir-0.0.3/nir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 19:09:23.000000 nir-0.0.3/nir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-05 19:09:14.000000 nir-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:09:23.929984 nir-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:46:41.586617 nir-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-08 23:46:33.000000 nir-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-08 23:46:33.000000 nir-0.0.4/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/nir/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 23:46:33.000000 nir-0.0.4/nir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-08 23:46:33.000000 nir-0.0.4/nir/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-08 23:46:33.000000 nir-0.0.4/nir/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-08 23:46:33.000000 nir-0.0.4/nir/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/nir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 23:46:41.000000 nir-0.0.4/nir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-08 23:46:33.000000 nir-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:46:41.586617 nir-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:41.586617 nir-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 23:46:33.000000 nir-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-08 23:46:33.000000 nir-0.0.4/tests/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-08 23:46:33.000000 nir-0.0.4/tests/test_readwrite.py
```

### Comparing `nir-0.0.3/PKG-INFO` & `nir-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.3
+Version: 0.0.4
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,14 +20,15 @@
 # NIR: Neuromorphic Intermediate Representation specification
 
 NIR defines neuron models and connectivity for arbitrary networks that include spiking neurons. Neuron models are defined as dynamical system equations, because time is an essential component of neuromorphic systems. The goal is to provide a common format that different spiking neural network (SNN) frameworks can convert to. That allows a user to train an SNN in framework X and convert it to framework Y. Framework X might offer particularly fast training while framework Y might offer deployment to neuromorphic hardware.
 
 ## Computational units
 On top of popular primitives such as convolutional or fully connected/linear computations, we define additional compuational primitives that are specific to neuromorphic computing and hardware implementations thereof. Computational units that are not specifically neuromorphic take inspiration from the Pytorch ecosystem in terms of naming and parameters (such as Conv2d that uses groups/strides). Example definitons of computational units:
 
+$$\text{I}: [ R ]$$
 
 $$\text{LI}: [ \tau, R, v_{leak}]$$
 
 $$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
 
 $$\text{Linear}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
 
@@ -47,20 +48,29 @@
 A \rightarrow B \\
 B \rightarrow C
 $$
 
 ## Format
 The intermediate represenation can be stored as hdf5 file, which benefits from compression. 
 
-## Frameworks that currently support NIR:
-* work in progress
-* another work in progress
+## Frameworks that currently support NIR
+
+| **Framework** | **Write to NIR** | **Read from NIR** |
+| --------------- | :--: | :--: |
+| [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
+| [Nengo](https://nengo.ai) | ⬚ | ⬚ |
+| [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
+| [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
+| [Sinabs](https://sinabs.readthedocs.io) | ⬚ | ⬚ |
+| [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
+| [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
+| [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
-## Acknowledgements
 
+## Acknowledgements
 Authors (in alphabetical order):
 * [Steven Abreu](https://github.com/stevenabreu7)
 * [Felix Bauer](https://github.com/bauerfe)
 * [Jason Eshraghian](https://github.com/jeshraghian)
 * [Matthias Jobst](https://github.com/matjobst)
 * [Gregor Lenz](https://github.com/biphasic)
 * [Jens Egholm Pedersen](https://github.com/jegp)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nir-0.0.3/README.md` & `nir-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # NIR: Neuromorphic Intermediate Representation specification
 
 NIR defines neuron models and connectivity for arbitrary networks that include spiking neurons. Neuron models are defined as dynamical system equations, because time is an essential component of neuromorphic systems. The goal is to provide a common format that different spiking neural network (SNN) frameworks can convert to. That allows a user to train an SNN in framework X and convert it to framework Y. Framework X might offer particularly fast training while framework Y might offer deployment to neuromorphic hardware.
 
 ## Computational units
 On top of popular primitives such as convolutional or fully connected/linear computations, we define additional compuational primitives that are specific to neuromorphic computing and hardware implementations thereof. Computational units that are not specifically neuromorphic take inspiration from the Pytorch ecosystem in terms of naming and parameters (such as Conv2d that uses groups/strides). Example definitons of computational units:
 
+$$\text{I}: [ R ]$$
 
 $$\text{LI}: [ \tau, R, v_{leak}]$$
 
 $$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
 
 $$\text{Linear}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
 
@@ -28,20 +29,29 @@
 A \rightarrow B \\
 B \rightarrow C
 $$
 
 ## Format
 The intermediate represenation can be stored as hdf5 file, which benefits from compression. 
 
-## Frameworks that currently support NIR:
-* work in progress
-* another work in progress
+## Frameworks that currently support NIR
+
+| **Framework** | **Write to NIR** | **Read from NIR** |
+| --------------- | :--: | :--: |
+| [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
+| [Nengo](https://nengo.ai) | ⬚ | ⬚ |
+| [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
+| [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
+| [Sinabs](https://sinabs.readthedocs.io) | ⬚ | ⬚ |
+| [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
+| [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
+| [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
-## Acknowledgements
 
+## Acknowledgements
 Authors (in alphabetical order):
 * [Steven Abreu](https://github.com/stevenabreu7)
 * [Felix Bauer](https://github.com/bauerfe)
 * [Jason Eshraghian](https://github.com/jeshraghian)
 * [Matthias Jobst](https://github.com/matjobst)
 * [Gregor Lenz](https://github.com/biphasic)
 * [Jens Egholm Pedersen](https://github.com/jegp)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nir-0.0.3/nir/ir.py` & `nir-0.0.4/nir/ir.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,79 +16,99 @@
 
 
 class NIRNode:
     """Basic Neural Intermediate Representation Unit (NIRUnit)"""
 
     pass
 
+
 @dataclass
 class Input(NIRNode):
     """Input Node.
 
     This is a virtual node, which allows feeding in data into the graph.
     """
-    shape: np.ndarray # Shape of input data
+
+    shape: np.ndarray  # Shape of input data
+
 
 @dataclass
 class Output(NIRNode):
     """Output Node.
-    
+
     Defines an output of the graph.
     """
+
     pass
 
 
 @dataclass
+class I(NIRNode):
+    """Integrator
+
+    The integrator neuron model is defined by the following equation:
+
+    .. math::
+        \dot{v} = R I
+    """
+
+    r: np.ndarray
+
+
+@dataclass
 class LI(NIRNode):
-    """Leaky integrator neuron model.
+    r"""Leaky integrator neuron model.
 
     The leaky integrator neuron model is defined by the following equation:
-    $$
-    \tau \dot{v} = (v_{leak} - v) + R I
-    $$
-    Where $\tau$ is the time constant, $v$ is the membrane potential,
-    $v_{leak}$ is the leak voltage, $R$ is the resistance, and $I$ is the
-    input current.
+
+    .. math::
+        \tau \dot{v} = (v_{leak} - v) + R I
+
+    Where :math:`\tau` is the time constant, :math:`v` is the membrane potential,
+    :math:`v_{leak}` is the leak voltage, :math:`R` is the resistance, and :math:`I`
+    is the input current.
     """
 
     tau: np.ndarray  # Time constant
     r: np.ndarray  # Resistance
     v_leak: np.ndarray  # Leak voltage
 
 
 @dataclass
 class LIF(NIRNode):
-    """Leaky integrate and-fire-neuron model.
+    r"""Leaky integrate and-fire-neuron model.
 
     The leaky integrate-and-fire neuron model is defined by the following equations:
-    $$
-    \tau \dot{v} = (v_{leak} - v) + R I
-    z = \being{cases}
-        1 & v > v_th \\
-        0 & else
-    \end{cases}
-    v = \begin{cases}
-        v-v_{th} & z=1 \\
-        v & else
-    \end{cases}
-    $$
+    
+    .. math::
+        \tau \dot{v} = (v_{leak} - v) + R I
+    
+        z = \begin{cases} 
+            1 & v > v_{thr} \\ 
+            0 & else
+        \end{cases}
+
+        v = \begin{cases}
+            v-v_{thr} & z=1 \\
+            v & else
+        \end{cases}
+
     Where $\tau$ is the time constant, $v$ is the membrane potential,
     $v_{leak}$ is the leak voltage, $R$ is the resistance, $v_th$ is
     the firing threshold, and $I$ is the input current.
     """
 
     tau: np.ndarray  # Time constant
     r: np.ndarray  # Resistance
     v_leak: np.ndarray  # Leak voltage
-    v_th: np.ndarray  # Firing threshold
+    v_threshold: np.ndarray  # Firing threshold
 
 
 @dataclass
 class Linear(NIRNode):
-
     weights: np.ndarray  # Weights M * N
     bias: np.ndarray  # Bias M
 
 
 @dataclass
 class Conv1d(NIRNode):
     """Convolutional layer in 1d"""
@@ -107,7 +127,21 @@
 
     weights: np.ndarray  # Weights C_out * C_in * X * Y
     stride: int  # Stride
     padding: int  # Padding
     dilation: int  # Dilation
     groups: int  # Groups
     bias: np.ndarray  # Bias C_out
+
+
+@dataclass
+class Threshold(NIRNode):
+    """Threshold node."""
+
+    threshold: np.ndarray  # Firing threshold
+
+
+@dataclass
+class Delay(NIRNode):
+    """Simple delay node."""
+
+    delay: np.ndarray  # Delay
```

### Comparing `nir-0.0.3/nir/read.py` & `nir-0.0.4/nir/read.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,40 +6,49 @@
 
 
 def read(filename: typing.Union[str, pathlib.Path]) -> nir.NIR:
     """Load a NIR from a HDF/conn5 file."""
     with h5py.File(filename, "r") as f:
         nodes = []
         for k, node in f["nodes"].items():
-            if node["type"][()] == b"Input":
+            if node["type"][()] == b"Delay":
                 nodes.append(
-                    nir.Input(
-                        shape=node["shape"][()],
+                    nir.Delay(
+                        delay=node["delay"][()],
                     )
                 )
-            elif node["type"][()] == b"Output":
+            elif node["type"][()] == b"I":
                 nodes.append(
-                    nir.Output(
+                    nir.I(
+                        r=node["r"][()],
                     )
                 )
+            elif node["type"][()] == b"Input":
+                nodes.append(
+                    nir.Input(
+                        shape=node["shape"][()],
+                    )
+                )
+            elif node["type"][()] == b"Output":
+                nodes.append(nir.Output())
             elif node["type"][()] == b"LI":
                 nodes.append(
                     nir.LI(
                         tau=node["tau"][()],
                         r=node["r"][()],
                         v_leak=node["v_leak"][()],
                     )
                 )
             elif node["type"][()] == b"LIF":
                 nodes.append(
                     nir.LIF(
                         tau=node["tau"][()],
                         r=node["r"][()],
                         v_leak=node["v_leak"][()],
-                        v_th=node["v_th"][()],
+                        v_threshold=node["v_threshold"][()],
                     )
                 )
             elif node["type"][()] == b"Linear":
                 nodes.append(
                     nir.Linear(
                         weights=node["weights"][()],
                         bias=node["bias"][()],
@@ -63,11 +72,17 @@
                         stride=node["stride"][()],
                         padding=node["padding"][()],
                         dilation=node["dilation"][()],
                         groups=node["groups"][()],
                         bias=node["bias"][()],
                     )
                 )
+            elif node["type"][()] == b"Threshold":
+                nodes.append(
+                    nir.Threshold(
+                        threshold=node["threshold"][()],
+                    )
+                )
             else:
                 raise ValueError(f"Unknown unit type: {node['type'][()]}")
         edges = f["edges"][()]
         return nir.NIR(nodes=nodes, edges=edges)
```

### Comparing `nir-0.0.3/nir/test/test_readwrite.py` & `nir-0.0.4/tests/test_readwrite.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,30 +18,80 @@
 
 
 def test_simple():
     ir = nir.NIR(nodes=[nir.Linear(weights=[1, 2, 3], bias=4)], edges=[(0, 0)])
     factory_test_graph(ir)
 
 
+def test_integrator():
+    ir = nir.NIR(
+        nodes=[nir.Linear(weights=[1], bias=0), nir.I(r=2)],
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
 
 
 def test_leaky_integrator_and_fire():
     ir = nir.NIR(
-        nodes=[nir.Linear(weights=[1], bias=0), nir.LIF(tau=1, r=2, v_leak=3, v_th=4)],
+        nodes=[
+            nir.Linear(weights=[1], bias=0),
+            nir.LIF(tau=1, r=2, v_leak=3, v_threshold=4),
+        ],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
 
+
 def test_simple_with_read_write():
     ir = nir.NIR(
-        nodes=[nir.Input(shape=[3,]),
-               nir.Linear(weights=[1, 2, 3], bias=4),
-               nir.Output()],
-        edges=[(0, 1), (1,2)]
+        nodes=[
+            nir.Input(
+                shape=[
+                    3,
+                ]
+            ),
+            nir.Linear(weights=[1, 2, 3], bias=4),
+            nir.Output(),
+        ],
+        edges=[(0, 1), (1, 2)],
+    )
+    factory_test_graph(ir)
+
+
+def test_delay():
+    ir = nir.NIR(
+        nodes=[
+            nir.Input(
+                shape=[
+                    3,
+                ]
+            ),
+            nir.Delay(delay=[1, 2, 3]),
+            nir.Output(),
+        ],
+        edges=[(0, 1), (1, 2)],
+    )
+    factory_test_graph(ir)
+
+
+def test_threshold():
+    ir = nir.NIR(
+        nodes=[
+            nir.Input(
+                shape=[
+                    3,
+                ]
+            ),
+            nir.Threshold(threshold=[2.0, 2.5, 2.8]),
+            nir.Output(),
+        ],
+        edges=[(0, 1), (1, 2)],
     )
     factory_test_graph(ir)
```

### Comparing `nir-0.0.3/nir/write.py` & `nir-0.0.4/nir/write.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 import numpy as np
 
 import nir
 
 
 def write(filename: typing.Union[str, pathlib.Path], graph: nir.NIR) -> None:
     def convert_node(node: nir.NIRNode) -> dict:
-        if isinstance(node, nir.Input):
+        if isinstance(node, nir.Delay):
+            return {"type": "Delay", "delay": node.delay}
+        elif isinstance(node, nir.I):
+            return {"type": "I", "r": node.r}
+        elif isinstance(node, nir.Input):
             return {
                 "type": "Input",
                 "shape": node.shape,
             }
-        elif isinstance(node, nir.Output):
-            return {
-                "type": "Output",
-            }
         elif isinstance(node, nir.LI):
             return {
                 "type": "LI",
                 "tau": node.tau,
                 "r": node.r,
                 "v_leak": node.v_leak,
             }
         elif isinstance(node, nir.LIF):
             return {
                 "type": "LIF",
                 "tau": node.tau,
                 "r": node.r,
                 "v_leak": node.v_leak,
-                "v_th": node.v_th,
+                "v_threshold": node.v_threshold,
             }
         elif isinstance(node, nir.Linear):
             return {
                 "type": "Linear",
                 "weights": node.weights,
                 "bias": node.bias,
             }
@@ -55,14 +55,20 @@
                 "weights": node.weights,
                 "stride": node.stride,
                 "padding": node.padding,
                 "dilation": node.dilation,
                 "groups": node.groups,
                 "bias": node.bias,
             }
+        elif isinstance(node, nir.Output):
+            return {
+                "type": "Output",
+            }
+        elif isinstance(node, nir.Threshold):
+            return {"type": "Threshold", "threshold": node.threshold}
         else:
             raise ValueError(f"Unknown node type: {node}")
 
     """Write a NIR to a HDF5 file."""
     with h5py.File(filename, "w") as f:
         nodes_group = f.create_group("nodes")
         for i, node in enumerate(graph.nodes):
```

### Comparing `nir-0.0.3/nir.egg-info/PKG-INFO` & `nir-0.0.4/nir.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.3
+Version: 0.0.4
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,14 +20,15 @@
 # NIR: Neuromorphic Intermediate Representation specification
 
 NIR defines neuron models and connectivity for arbitrary networks that include spiking neurons. Neuron models are defined as dynamical system equations, because time is an essential component of neuromorphic systems. The goal is to provide a common format that different spiking neural network (SNN) frameworks can convert to. That allows a user to train an SNN in framework X and convert it to framework Y. Framework X might offer particularly fast training while framework Y might offer deployment to neuromorphic hardware.
 
 ## Computational units
 On top of popular primitives such as convolutional or fully connected/linear computations, we define additional compuational primitives that are specific to neuromorphic computing and hardware implementations thereof. Computational units that are not specifically neuromorphic take inspiration from the Pytorch ecosystem in terms of naming and parameters (such as Conv2d that uses groups/strides). Example definitons of computational units:
 
+$$\text{I}: [ R ]$$
 
 $$\text{LI}: [ \tau, R, v_{leak}]$$
 
 $$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
 
 $$\text{Linear}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
 
@@ -47,20 +48,29 @@
 A \rightarrow B \\
 B \rightarrow C
 $$
 
 ## Format
 The intermediate represenation can be stored as hdf5 file, which benefits from compression. 
 
-## Frameworks that currently support NIR:
-* work in progress
-* another work in progress
+## Frameworks that currently support NIR
+
+| **Framework** | **Write to NIR** | **Read from NIR** |
+| --------------- | :--: | :--: |
+| [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
+| [Nengo](https://nengo.ai) | ⬚ | ⬚ |
+| [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
+| [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
+| [Sinabs](https://sinabs.readthedocs.io) | ⬚ | ⬚ |
+| [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
+| [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
+| [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
-## Acknowledgements
 
+## Acknowledgements
 Authors (in alphabetical order):
 * [Steven Abreu](https://github.com/stevenabreu7)
 * [Felix Bauer](https://github.com/bauerfe)
 * [Jason Eshraghian](https://github.com/jeshraghian)
 * [Matthias Jobst](https://github.com/matjobst)
 * [Gregor Lenz](https://github.com/biphasic)
 * [Jens Egholm Pedersen](https://github.com/jegp)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nir-0.0.3/pyproject.toml` & `nir-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "nir"
-version = "0.0.3"
+version = "0.0.4"
 description = "Neuromorphic Intermediate Representation"
 authors = [
   { name = "Steven Abreu", email = "s.abreu@rug.nl" },
   { name = "Felix Bauer", email = "felix.bauer@synsense.ai" },
   { name = "Jason Eshraghian", email = "jeshragh@ucsc.edu" },
   { name = "Matthias Jobst", email = "matthias.jobst2@tu-dresden.de" },
   { name = "Gregor Lenz", email = "mail@lenzgregor.com" },
```

