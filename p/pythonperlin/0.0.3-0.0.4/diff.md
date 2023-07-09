# Comparing `tmp/pythonperlin-0.0.3.tar.gz` & `tmp/pythonperlin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonperlin-0.0.3.tar", last modified: Sat Jul 30 21:46:59 2022, max compression
+gzip compressed data, was "pythonperlin-0.0.4.tar", last modified: Sun Jul  9 20:27:08 2023, max compression
```

## Comparing `pythonperlin-0.0.3.tar` & `pythonperlin-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2022-07-30 21:46:59.865442 pythonperlin-0.0.3/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-03-14 22:36:32.000000 pythonperlin-0.0.3/LICENSE
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4661 2022-07-30 21:46:59.865323 pythonperlin-0.0.3/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4165 2022-03-20 21:01:58.000000 pythonperlin-0.0.3/README.md
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2022-07-30 21:46:59.864521 pythonperlin-0.0.3/pythonperlin/
--rw-r--r--   0 timpyrkov   (501) staff       (20)      162 2022-03-18 20:54:21.000000 pythonperlin-0.0.3/pythonperlin/__init__.py
--rw-r--r--   0 timpyrkov   (501) staff       (20)     7149 2022-07-30 20:27:18.000000 pythonperlin-0.0.3/pythonperlin/perlin.py
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2022-07-30 21:46:59.865186 pythonperlin-0.0.3/pythonperlin.egg-info/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4661 2022-07-30 21:46:59.000000 pythonperlin-0.0.3/pythonperlin.egg-info/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2022-07-30 21:46:59.000000 pythonperlin-0.0.3/pythonperlin.egg-info/SOURCES.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2022-07-30 21:46:59.000000 pythonperlin-0.0.3/pythonperlin.egg-info/dependency_links.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2022-07-30 21:46:59.000000 pythonperlin-0.0.3/pythonperlin.egg-info/requires.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2022-07-30 21:46:59.000000 pythonperlin-0.0.3/pythonperlin.egg-info/top_level.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2022-07-30 21:46:59.865486 pythonperlin-0.0.3/setup.cfg
--rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2022-07-30 21:45:07.000000 pythonperlin-0.0.3/setup.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-09 20:27:08.460412 pythonperlin-0.0.4/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-11-01 23:50:58.000000 pythonperlin-0.0.4/LICENSE
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     4955 2023-07-09 20:27:08.460301 pythonperlin-0.0.4/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     4459 2023-07-09 20:22:37.000000 pythonperlin-0.0.4/README.md
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-09 20:27:08.459393 pythonperlin-0.0.4/pythonperlin/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      162 2022-11-01 23:50:58.000000 pythonperlin-0.0.4/pythonperlin/__init__.py
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     8254 2023-07-09 20:18:56.000000 pythonperlin-0.0.4/pythonperlin/perlin.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-09 20:27:08.460130 pythonperlin-0.0.4/pythonperlin.egg-info/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     4955 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/SOURCES.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/dependency_links.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/requires.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2023-07-09 20:27:08.000000 pythonperlin-0.0.4/pythonperlin.egg-info/top_level.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-09 20:27:08.460454 pythonperlin-0.0.4/setup.cfg
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2023-07-09 20:19:35.000000 pythonperlin-0.0.4/setup.py
```

### Comparing `pythonperlin-0.0.3/LICENSE` & `pythonperlin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonperlin-0.0.3/PKG-INFO` & `pythonperlin-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.3
+Version: 0.0.4
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,23 +16,29 @@
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![PyPI](https://img.shields.io/pypi/v/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![License](https://img.shields.io/pypi/l/pythonperlin?style=plastic)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/pythonperlin/badge/?version=latest)](https://pythonperlin.readthedocs.io/en/latest/?badge=latest)
 
 # PythonPerlin
-## Perlin noise in python -- generative art texture to seamlessly tile in any dimensions
+## Perlin noise in python -- procedural generative art tool to seamlessly tile texture patterns in any dimensions
 #
 
 
 # Installation
 ```
 pip install pythonperlin
 ```
 
+More examples and animations can be found at:
+
+https://github.com/timpyrkov/procedural-art/
+
+https://www.instagram.com/timpyrkov/
+
 # Generate Perlin noise
 ```
 import pylab as plt
 from pythonperlin import perlin
 
 # Set grid shape for randomly seeded gradients
 shape = (4,4)
@@ -43,31 +49,31 @@
 # Generate noise
 x = perlin(shape, dens=dens, seed=0)
 
 # Test that noise tiles seamlessly
 x = np.concatenate([x] * 2, axis=1)
 
 plt.figure(figsize=(12,6))
-plt.imshow(x, cmap=plt.get_cmap('prism'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_tile.png)
 
 
 # Generate domain warping
 
 Add noise to grid coordinates and generate noise again
 ```
 dens = 32
 shape = (4,4)
-x = perlin(shape, dens=dens, seed=0, warp=True)
+x = perlin(shape, dens=dens, seed=0, warp=2)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('prism'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_warp.png)
 
 
 # Generate octaves
@@ -81,23 +87,23 @@
 # Set density - output shape will be shape * dens = (256,256)
 dens = 32
 
 # Generate noise
 x = perlin(shape, dens=dens, seed=0)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('viridis'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 
-# Generate noise array with 2 additional octaves
-x = perlin(shape, dens=dens, seed=0, octaves=2)
+# Generate noise array with 4 additional octaves
+x = perlin(shape, dens=dens, seed=0, octaves=4)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('viridis'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_no_octaves.png) ![](media/img_with_octaves.png)
 
 
 # Generate water caustics
@@ -133,25 +139,26 @@
 ```
 dens = 32
 shape = (8,8)
 x = perlin(shape, dens=dens)
 
 n = 8
 delta = dens
+color = plt.get_cmap('tab20').colors[::-1]
 plt.figure(figsize=(6,6))
 for i in range(n):
     r = x[delta * i] + 1
     r = np.concatenate([r, (r[0],)])
     phi = 2 * np.pi * np.linspace(0, 1, len(r))
-    scale = 1 - i / n
+    scale = 1 - i / (n + 2)
     z = scale * r * np.exp(1j * phi)
     ax = plt.gca()
     zorder = max([ch.zorder for ch in ax.get_children()])
-    plt.fill(z.real, z.imag, c='dodgerblue', zorder=zorder+1)
-    plt.plot(z.real, z.imag, c='blue', lw=2, zorder=zorder+2)
+    plt.fill(z.real, z.imag, c=color[2*i], zorder=zorder+1)
+    plt.plot(z.real, z.imag, c=color[2*i+1], lw=2, zorder=zorder+2)
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_flower.png)
 
 
 # Generate vector field
@@ -160,20 +167,22 @@
 ```
 dens = 6
 shape = (3,3)
 x = perlin(shape, dens=dens)
 z = np.exp(2j * np.pi * x)
 
 shape = z.shape
+colors = plt.get_cmap('Accent').colors
 plt.figure(figsize=(6,6))
 for i in range(shape[0]):
     for j in range(shape[1]):
         di = 0.5 * z[i,j].real
         dj = 0.5 * z[i,j].imag
-        plt.arrow(i, j, di, dj, color='dodgerblue', width=0.1)
+        color = colors[(di > 0) + 2 * (dj > 0)]
+        plt.arrow(i, j, di, dj, color=color, width=0.1)
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_vectors.png)
 
 
 # Sound of Perlin noise
```

### Comparing `pythonperlin-0.0.3/README.md` & `pythonperlin-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![PyPI](https://img.shields.io/pypi/v/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![License](https://img.shields.io/pypi/l/pythonperlin?style=plastic)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/pythonperlin/badge/?version=latest)](https://pythonperlin.readthedocs.io/en/latest/?badge=latest)
 
 # PythonPerlin
-## Perlin noise in python -- generative art texture to seamlessly tile in any dimensions
+## Perlin noise in python -- procedural generative art tool to seamlessly tile texture patterns in any dimensions
 #
 
 
 # Installation
 ```
 pip install pythonperlin
 ```
 
+More examples and animations can be found at:
+
+https://github.com/timpyrkov/procedural-art/
+
+https://www.instagram.com/timpyrkov/
+
 # Generate Perlin noise
 ```
 import pylab as plt
 from pythonperlin import perlin
 
 # Set grid shape for randomly seeded gradients
 shape = (4,4)
@@ -27,31 +33,31 @@
 # Generate noise
 x = perlin(shape, dens=dens, seed=0)
 
 # Test that noise tiles seamlessly
 x = np.concatenate([x] * 2, axis=1)
 
 plt.figure(figsize=(12,6))
-plt.imshow(x, cmap=plt.get_cmap('prism'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_tile.png)
 
 
 # Generate domain warping
 
 Add noise to grid coordinates and generate noise again
 ```
 dens = 32
 shape = (4,4)
-x = perlin(shape, dens=dens, seed=0, warp=True)
+x = perlin(shape, dens=dens, seed=0, warp=2)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('prism'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_warp.png)
 
 
 # Generate octaves
@@ -65,23 +71,23 @@
 # Set density - output shape will be shape * dens = (256,256)
 dens = 32
 
 # Generate noise
 x = perlin(shape, dens=dens, seed=0)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('viridis'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 
-# Generate noise array with 2 additional octaves
-x = perlin(shape, dens=dens, seed=0, octaves=2)
+# Generate noise array with 4 additional octaves
+x = perlin(shape, dens=dens, seed=0, octaves=4)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('viridis'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_no_octaves.png) ![](media/img_with_octaves.png)
 
 
 # Generate water caustics
@@ -117,25 +123,26 @@
 ```
 dens = 32
 shape = (8,8)
 x = perlin(shape, dens=dens)
 
 n = 8
 delta = dens
+color = plt.get_cmap('tab20').colors[::-1]
 plt.figure(figsize=(6,6))
 for i in range(n):
     r = x[delta * i] + 1
     r = np.concatenate([r, (r[0],)])
     phi = 2 * np.pi * np.linspace(0, 1, len(r))
-    scale = 1 - i / n
+    scale = 1 - i / (n + 2)
     z = scale * r * np.exp(1j * phi)
     ax = plt.gca()
     zorder = max([ch.zorder for ch in ax.get_children()])
-    plt.fill(z.real, z.imag, c='dodgerblue', zorder=zorder+1)
-    plt.plot(z.real, z.imag, c='blue', lw=2, zorder=zorder+2)
+    plt.fill(z.real, z.imag, c=color[2*i], zorder=zorder+1)
+    plt.plot(z.real, z.imag, c=color[2*i+1], lw=2, zorder=zorder+2)
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_flower.png)
 
 
 # Generate vector field
@@ -144,20 +151,22 @@
 ```
 dens = 6
 shape = (3,3)
 x = perlin(shape, dens=dens)
 z = np.exp(2j * np.pi * x)
 
 shape = z.shape
+colors = plt.get_cmap('Accent').colors
 plt.figure(figsize=(6,6))
 for i in range(shape[0]):
     for j in range(shape[1]):
         di = 0.5 * z[i,j].real
         dj = 0.5 * z[i,j].imag
-        plt.arrow(i, j, di, dj, color='dodgerblue', width=0.1)
+        color = colors[(di > 0) + 2 * (dj > 0)]
+        plt.arrow(i, j, di, dj, color=color, width=0.1)
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_vectors.png)
 
 
 # Sound of Perlin noise
```

### Comparing `pythonperlin-0.0.3/pythonperlin/perlin.py` & `pythonperlin-0.0.4/pythonperlin/perlin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
 
 import numpy as np
+from scipy.interpolate import interp1d
 import itertools
 
 
 def smoothstep(x):
     """
     Smoothstep for interpolation
 
-
     """
     return 3 * np.power(x, 2) - 2 * np.power(x, 3)
 
 
 def smootherstep(x):
     """
     Smootherstep for interpolation
 
-
     """
     return 6 * np.power(x, 5) - 15 * np.power(x, 4) + 10 * np.power(x, 3)
 
 
 def make_grads(*shape, seed=None):
     """
     Make n-dimensional random gradient vectors
@@ -200,67 +199,69 @@
             new_noise.append(d * fade)
         for i in range(len(new_noise))[::2]:
             noise.append(new_noise[i] + new_noise[i + 1])
     noise = noise[0].astype(float)
     return noise
 
 
-def domain_warping(*shape, grid=None, seed=0, smooth=smoothstep):
+def domain_warping(*shape, grid=None, seed=0, warp=0.0, smooth=smoothstep):
     """
     Apply domain warping to grid
 
     Parameters
     ----------
     *shape
         Integers or tuple of integers
     grid : ndarray
         Grid float coordinates
     seed : int, default None
         Numpy random seed
+    warp : float, default 0.0
+        Magnitude of domain warping
     smooth : {smoothstep, smootherstep, None}, default smoothstep
         Smooth function or None
 
     Returns
     -------
     grid : ndarray
         Grid float coordinates
 
     """
     nnode, ndim = grid.shape
     vmax = np.max(grid, axis=0)
     for i in range(ndim):
         grads = make_grads(*shape, seed=seed)
-        warp = calc_grid(grid, grads, smooth=smooth)
+        w = calc_grid(grid, grads, smooth=smooth)
         x = grid[:,i]
         vmax = int(x.max()) + 1
-        x = x + warp
+        x = x + warp * w
         mask = x < 0
         x[mask] = x[mask] + vmax
         mask = x >= vmax
         x[mask] = x[mask] - vmax
         grid[:,i] = x
     return grid
 
 
-def perlin(*shape, dens=1, seed=None, octaves=0, warp=False, smooth=smoothstep):
+def perlin(*shape, dens=1, octaves=0, seed=None, warp=0.0, smooth=smoothstep):
     """
     Generate Perlin noise
     
     Parameters
     ----------
     *shape
         Integers or tuple of integers
     dens : int, default 1 (white noise)
         Number of points between each two gradients along an axis
-    seed : int, default None
-        Numpy random seed
     octaves : int, default 0
         Number of additional octaves
-    warp : bool, default False
-        If True, apply domain warping
+    seed : int, default None
+        Numpy random seed
+    warp : float, default 0.0
+        Magnitude of domain warping
     smooth : {smoothstep, smootherstep, None}, default smoothstep
         Smooth function or None
 
     Returns
     -------
     noise : ndarray
         Noise grid
@@ -272,25 +273,59 @@
     >>> x = perlin(shape, dens=8)
 
     """
     shape = tuple(shape[0]) if isinstance(shape[0], (tuple, list)) else shape
     noise_shape = tuple(dens * s for s in shape)
     grid = make_grid(*shape, dens=dens)
     if warp:
-        grid = domain_warping(*shape, grid=grid, seed=seed, smooth=smooth)
+        grid = domain_warping(*shape, grid=grid, seed=seed, warp=warp, smooth=smooth)
     grads = make_grads(*shape, seed=seed)
     noise = calc_grid(grid, grads, smooth=smooth)
     for i in range(octaves):
         grid = 2 * grid
+        scale = 1 / 2**(i+1)
         shape = tuple(2 * s for s in shape)
         grads = make_grads(*shape, seed=seed)
-        noise += 0.5 * calc_grid(grid, grads, smooth=smooth)
+        noise += scale * calc_grid(grid, grads, smooth=smooth)
     noise = noise.reshape(noise_shape)
     return noise
 
 
+def extend(x, n=2, axis=0, kind='linear', mode='full'):
+    """
+    Extend by inserting N new dots between grid nodes along an axis
+    
+    Parameters
+    ----------
+    x : ndarray
+        Array of values
+    n : int, default 2
+        Number of dots to insert between grid nodes along specified axis
+    axis : int, default 0
+        Specifies the axis to extend
+    kind : str, default 'linear'
+        See description of 'kind' parameter for scipy.interpolate.interp1d()
+    mode : {'full', 'same'}, default 'full'
+        'full;'' keep all values, 'same' truncates to the original size
+
+    Returns
+    -------
+    ndarray
+        Array of extended values
+
+    """
+    m = x.shape[axis]
+    l = np.linspace(0, 1, m)
+    f = interp1d(l, x, kind, axis)
+    l = np.linspace(0, 1, (n + 1) * (m - 1) + 1)
+    x_ = f(l)
+    if mode == 'same':
+        slc = [slice(None)] * x.ndim
+        slc[axis] = slice(0, n)
+        x_ = x_[tuple(slc)]
+    return x_
```

### Comparing `pythonperlin-0.0.3/pythonperlin.egg-info/PKG-INFO` & `pythonperlin-0.0.4/pythonperlin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.3
+Version: 0.0.4
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,23 +16,29 @@
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![PyPI](https://img.shields.io/pypi/v/pythonperlin?style=plastic)](https://pypi.org/project/pythonperlin/)
 [![License](https://img.shields.io/pypi/l/pythonperlin?style=plastic)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/pythonperlin/badge/?version=latest)](https://pythonperlin.readthedocs.io/en/latest/?badge=latest)
 
 # PythonPerlin
-## Perlin noise in python -- generative art texture to seamlessly tile in any dimensions
+## Perlin noise in python -- procedural generative art tool to seamlessly tile texture patterns in any dimensions
 #
 
 
 # Installation
 ```
 pip install pythonperlin
 ```
 
+More examples and animations can be found at:
+
+https://github.com/timpyrkov/procedural-art/
+
+https://www.instagram.com/timpyrkov/
+
 # Generate Perlin noise
 ```
 import pylab as plt
 from pythonperlin import perlin
 
 # Set grid shape for randomly seeded gradients
 shape = (4,4)
@@ -43,31 +49,31 @@
 # Generate noise
 x = perlin(shape, dens=dens, seed=0)
 
 # Test that noise tiles seamlessly
 x = np.concatenate([x] * 2, axis=1)
 
 plt.figure(figsize=(12,6))
-plt.imshow(x, cmap=plt.get_cmap('prism'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_tile.png)
 
 
 # Generate domain warping
 
 Add noise to grid coordinates and generate noise again
 ```
 dens = 32
 shape = (4,4)
-x = perlin(shape, dens=dens, seed=0, warp=True)
+x = perlin(shape, dens=dens, seed=0, warp=2)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('prism'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_warp.png)
 
 
 # Generate octaves
@@ -81,23 +87,23 @@
 # Set density - output shape will be shape * dens = (256,256)
 dens = 32
 
 # Generate noise
 x = perlin(shape, dens=dens, seed=0)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('viridis'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 
-# Generate noise array with 2 additional octaves
-x = perlin(shape, dens=dens, seed=0, octaves=2)
+# Generate noise array with 4 additional octaves
+x = perlin(shape, dens=dens, seed=0, octaves=4)
 
 plt.figure(figsize=(6,6))
-plt.imshow(x, cmap=plt.get_cmap('viridis'))
+plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_no_octaves.png) ![](media/img_with_octaves.png)
 
 
 # Generate water caustics
@@ -133,25 +139,26 @@
 ```
 dens = 32
 shape = (8,8)
 x = perlin(shape, dens=dens)
 
 n = 8
 delta = dens
+color = plt.get_cmap('tab20').colors[::-1]
 plt.figure(figsize=(6,6))
 for i in range(n):
     r = x[delta * i] + 1
     r = np.concatenate([r, (r[0],)])
     phi = 2 * np.pi * np.linspace(0, 1, len(r))
-    scale = 1 - i / n
+    scale = 1 - i / (n + 2)
     z = scale * r * np.exp(1j * phi)
     ax = plt.gca()
     zorder = max([ch.zorder for ch in ax.get_children()])
-    plt.fill(z.real, z.imag, c='dodgerblue', zorder=zorder+1)
-    plt.plot(z.real, z.imag, c='blue', lw=2, zorder=zorder+2)
+    plt.fill(z.real, z.imag, c=color[2*i], zorder=zorder+1)
+    plt.plot(z.real, z.imag, c=color[2*i+1], lw=2, zorder=zorder+2)
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_flower.png)
 
 
 # Generate vector field
@@ -160,20 +167,22 @@
 ```
 dens = 6
 shape = (3,3)
 x = perlin(shape, dens=dens)
 z = np.exp(2j * np.pi * x)
 
 shape = z.shape
+colors = plt.get_cmap('Accent').colors
 plt.figure(figsize=(6,6))
 for i in range(shape[0]):
     for j in range(shape[1]):
         di = 0.5 * z[i,j].real
         dj = 0.5 * z[i,j].imag
-        plt.arrow(i, j, di, dj, color='dodgerblue', width=0.1)
+        color = colors[(di > 0) + 2 * (dj > 0)]
+        plt.arrow(i, j, di, dj, color=color, width=0.1)
 plt.axis('off')
 plt.show()
 ```
 ![](media/img_vectors.png)
 
 
 # Sound of Perlin noise
```

### Comparing `pythonperlin-0.0.3/setup.py` & `pythonperlin-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="pythonperlin",
-    version="0.0.3",
+    version="0.0.4",
     author="Tim Pyrkov",
     author_email="tim.pyrkov@gmail.com",
     description="Perlin noise in python - seamlessly tile in any dimensions",
     long_description=read("README.md"),
     license = "MIT License",
     long_description_content_type="text/markdown",
     url="https://github.com/timpyrkov/pythonperlin",
```

