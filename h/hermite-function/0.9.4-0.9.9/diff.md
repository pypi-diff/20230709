# Comparing `tmp/hermite-function-0.9.4.tar.gz` & `tmp/hermite-function-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermite-function-0.9.4.tar", last modified: Sun Jan 22 21:48:33 2023, max compression
+gzip compressed data, was "hermite-function-0.9.9.tar", last modified: Sun Jul  9 15:25:38 2023, max compression
```

## Comparing `hermite-function-0.9.4.tar` & `hermite-function-0.9.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-01-22 21:48:33.233849 hermite-function-0.9.4/
--rw-rw-rw-   0        0        0     7481 2023-01-22 21:39:00.000000 hermite-function-0.9.4/HermiteFunction.py
--rw-rw-rw-   0        0        0     1094 2022-12-12 09:43:07.000000 hermite-function-0.9.4/LICENSE
--rw-rw-rw-   0        0        0     9733 2023-01-22 21:48:33.232834 hermite-function-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     9250 2023-01-22 21:45:03.000000 hermite-function-0.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-01-22 21:48:33.230837 hermite-function-0.9.4/hermite_function.egg-info/
--rw-rw-rw-   0        0        0     9733 2023-01-22 21:48:33.000000 hermite-function-0.9.4/hermite_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-22 21:48:33.000000 hermite-function-0.9.4/hermite_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-22 21:48:33.000000 hermite-function-0.9.4/hermite_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-01-22 21:48:33.000000 hermite-function-0.9.4/hermite_function.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-01-22 21:48:33.000000 hermite-function-0.9.4/hermite_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-22 21:48:33.234835 hermite-function-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      847 2023-01-22 21:47:27.000000 hermite-function-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:25:38.975150 hermite-function-0.9.9/
+-rw-rw-rw-   0        0        0     7237 2023-07-09 15:24:16.000000 hermite-function-0.9.9/HermiteFunction.py
+-rw-rw-rw-   0        0        0     1073 2023-07-09 15:24:16.000000 hermite-function-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     9732 2023-07-09 15:25:38.973702 hermite-function-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9006 2023-07-09 15:24:16.000000 hermite-function-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 15:25:38.972582 hermite-function-0.9.9/hermite_function.egg-info/
+-rw-rw-rw-   0        0        0     9732 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-09 15:25:38.000000 hermite-function-0.9.9/hermite_function.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:25:38.975797 hermite-function-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-07-09 15:25:08.000000 hermite-function-0.9.9/setup.py
```

### Comparing `hermite-function-0.9.4/HermiteFunction.py` & `hermite-function-0.9.9/HermiteFunction.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-import numpy as np
-from numpy.polynomial.hermite import Hermite
-from math import factorial
-from scipy.special import binom
-from itertools import zip_longest
-
-
-
-class HermiteFunction:
-    """A Hermite function series class."""
-    
-    #construction stuff
-    def __init__(self, coef):
-        """Creates a new Hermite function series.
-        
-        Parameters
-        ----------
-        coef : int or array_like
-            Index of hermite function
-            or list/array of coefficients in order of increasing degree.
-        
-        Returns
-        -------
-        hermite function series : HermiteFunction
-            A new Hermite function series object.
-        """
-        if isinstance(coef, int):
-            coef = [0]*coef + [1]
-        self.coef = np.array(coef)
-    
-    def random(deg, normed=False):
-        """Creates a Hermite function series
-        with random coefficients in [-1, 1[.
-        
-        Parameters
-        ----------
-        deg : int
-            Degree of the series (index deg not included).
-        normed : boolean, optional
-            True if the coefficients should be normed
-            to euclidian length 1 (default: False).
-        
-        Returns
-        -------
-        hermite function series : HermiteFunction
-            A new Hermite function series object.
-        """
-        coef = np.random.uniform(-1, +1, deg)
-        if normed:
-            coef /= np.linalg.norm(coef)
-        return HermiteFunction(coef)
-    
-    def fit(x, y, deg):
-        """Creates a least squares Hermite series fit.
-        
-        Parameters
-        ----------
-        x : number or array
-            x values.
-        y : number or array
-            y values.
-        deg : positive int
-            Degree series (index deg not included).
-        
-        Returns
-        -------
-        hermite function series : HermiteFunction
-            A least squares Hermite series fit.
-        """
-        #https://de.wikipedia.org/wiki/Multiple_lineare_Regression
-        X_T = np.array([HermiteFunction(i)(x) for i in range(deg)])
-        X = X_T.T
-        X_T_X = X_T @ X
-        X_T_X_inv = np.linalg.inv(X_T_X)
-        coef = np.dot(X_T_X_inv @ X_T, y)
-        
-        return HermiteFunction(coef)
-    
-    
-    #Hilbert space stuff
-    def dot(self, other):
-        """Returns the $L_\mathbb{R}^2$ dot product of self with other.
-        
-        Parameters
-        ----------
-        other : HermiteFunction
-            Other factor.
-        
-        Returns
-        -------
-        dot product : complex
-            The dot product of self and other.
-        """
-        return np.vdot(np.pad(self.coef,
-                    (0, max(0, len(other.coef)-len(self.coef)))),
-                np.pad(other.coef,
-                    (0, max(0, len(self.coef)-len(other.coef)))))
-    
-    def norm(self):
-        """Returns $L_\mathbb{R}^2$ norm of self.
-        
-        Returns
-        -------
-        norm : number
-            The norm of self.
-        """
-        return np.linalg.norm(self.coef)
-    
-    def __mul__(self, other):
-        """Scalar/elementwise multiplies other to the coefficients
-        and returns the result as a new series object.
-        
-        Parameters
-        ----------
-        other : number, array or HermiteFunction
-            Other factor.
-        
-        Returns
-        -------
-        hermite function series : HermiteFunction
-            The product of self and other.
-        """
-        if isinstance(other, HermiteFunction):
-            return HermiteFunction([a*b for a, b \
-                in zip_longest(self.coef, other.coef, fillvalue=0)])
-        else:
-            return HermiteFunction(self.coef * other)
-    
-    def __rmul__(self, other):
-        return self.__mul__(other)
-    
-    def __add__(self, other):
-        """Adds other to the coefficients
-        and returns the result as a new series object.
-        
-        Parameters
-        ----------
-        other : number, array or HermiteFunction
-            Other summand.
-        
-        Returns
-        -------
-        hermite function series : HermiteFunction
-            The sum of self and other.
-        """
-        if isinstance(other, HermiteFunction):
-            return HermiteFunction([a+b for a, b \
-                in zip_longest(self.coef, other.coef, fillvalue=0)])
-        else:
-            return HermiteFunction(self.coef + other)
-    
-    def __radd__(self, other):
-        return self.__add__(other)
-    
-    
-    #function stuff
-    def __call__(self, x):
-        """Evaluates the series at the given point(s).
-        
-        Parameters
-        ----------
-        x : number or array
-            Point(s) where to evaluate the series.
-        
-        Returns
-        -------
-        y : number or array
-            The value(s) at the given point(s).
-        """
-        y = 0
-        for n, c in enumerate(self.coef):
-            y += Hermite([0]*n+[c])(x) \
-                / np.sqrt(2**n * factorial(n) * np.sqrt(np.pi))
-        return y * np.exp(-x**2 / 2)
-    
-    def der(self, n=1):
-        """Returns the n-th derivative of this series.
-        
-        Parameters
-        ----------
-        n : positive integer, optional
-            Degree of differentiation (default: 1).
-        
-        Returns
-        -------
-        hermite function series : HermiteFunction
-            The n-th derivative of this series.
-        """
-        coef = self.coef
-        for _ in range(n):
-            i = np.arange(len(coef)+1)
-            coef = np.append(coef[1:], [0, 0])*np.sqrt((i+1)/2) \
-                    - np.append([0], coef)*np.sqrt(i/2)
-        return HermiteFunction(coef)
-    
-    def prod_reorder(self, other):
-        """Returns the product of self and other, divided by h_0.
-        
-        Parameters
-        ----------
-        other : HermiteFunction
-            Other factor.
-        
-        Returns
-        -------
-        hermite function series : HermiteFunction
-            The product of self and other, divided by h_0.
-        """
-        coef = np.zeros(len(self.coef)+len(other.coef)-1)
-        for b in range(len(coef)):
-            for n in range(b, len(self.coef)+len(other.coef)-1, 2):
-                for d in range(-b, b+1, 2):
-                    i, j = (n-d)//2, (n+d)//2
-                    k = (n-b)//2
-                    if 0<=i<len(self.coef) and 0<=j<len(other.coef):
-                        coef[b] += self.coef[i] * other.coef[j] \
-                            * factorial(k) * binom(i, k) * binom(j, k) \
-                            * np.sqrt(factorial(b)/(factorial(i)*factorial(j)))
-        return HermiteFunction(coef)
-    
-    def kin(self):
-        """Returns the kinetic energy of this series.
-        
-        Returns
-        -------
-        kinetic energy : float
-            The kinetic energy of this series.
-        """
-        return self.der().norm()**2 / 2
-    
-    
-    #python stuff
-    def __str__(self):
-        """Returns a Latex representation.
-        
-        Returns
-        -------
-        string : string
-            A Latex representation.
-        """
-        s = f'{self.coef[0]:.1f} h_0'
-        for i, c in enumerate(self.coef[1:]):
-            s += f' + {c:.1f} h_{i+1}'
-        return s
+import numpy as np
+from numpy.polynomial.hermite import Hermite
+from math import factorial
+from scipy.special import binom
+from itertools import zip_longest
+
+
+
+class HermiteFunction:
+    """A Hermite function series class."""
+    
+    #construction stuff
+    def __init__(self, coef):
+        """Creates a new Hermite function series.
+        
+        Parameters
+        ----------
+        coef : int or array_like
+            Index of hermite function
+            or list/array of coefficients in order of increasing degree.
+        
+        Returns
+        -------
+        hermite function series : HermiteFunction
+            A new Hermite function series object.
+        """
+        if isinstance(coef, int):
+            coef = [0]*coef + [1]
+        self.coef = np.array(coef)
+    
+    def random(deg, normed=False):
+        """Creates a Hermite function series
+        with random coefficients in [-1, 1[.
+        
+        Parameters
+        ----------
+        deg : int
+            Degree of the series (index deg not included).
+        normed : boolean, optional
+            True if the coefficients should be normed
+            to euclidian length 1 (default: False).
+        
+        Returns
+        -------
+        hermite function series : HermiteFunction
+            A new Hermite function series object.
+        """
+        coef = np.random.uniform(-1, +1, deg)
+        if normed:
+            coef /= np.linalg.norm(coef)
+        return HermiteFunction(coef)
+    
+    def fit(x, y, deg):
+        """Creates a least squares Hermite series fit.
+        
+        Parameters
+        ----------
+        x : number or array
+            x values.
+        y : number or array
+            y values.
+        deg : positive int
+            Degree series (index deg not included).
+        
+        Returns
+        -------
+        hermite function series : HermiteFunction
+            A least squares Hermite series fit.
+        """
+        #https://de.wikipedia.org/wiki/Multiple_lineare_Regression
+        X_T = np.array([HermiteFunction(i)(x) for i in range(deg)])
+        X = X_T.T
+        X_T_X = X_T @ X
+        X_T_X_inv = np.linalg.inv(X_T_X)
+        coef = np.dot(X_T_X_inv @ X_T, y)
+        
+        return HermiteFunction(coef)
+    
+    
+    #Hilbert space stuff
+    def dot(self, other):
+        """Returns the $L_\mathbb{R}^2$ dot product of self with other.
+        
+        Parameters
+        ----------
+        other : HermiteFunction
+            Other factor.
+        
+        Returns
+        -------
+        dot product : complex
+            The dot product of self and other.
+        """
+        return np.vdot(np.pad(self.coef,
+                    (0, max(0, len(other.coef)-len(self.coef)))),
+                np.pad(other.coef,
+                    (0, max(0, len(self.coef)-len(other.coef)))))
+    
+    def norm(self):
+        """Returns $L_\mathbb{R}^2$ norm of self.
+        
+        Returns
+        -------
+        norm : number
+            The norm of self.
+        """
+        return np.linalg.norm(self.coef)
+    
+    def __mul__(self, other):
+        """Scalar/elementwise multiplies other to the coefficients
+        and returns the result as a new series object.
+        
+        Parameters
+        ----------
+        other : number, array or HermiteFunction
+            Other factor.
+        
+        Returns
+        -------
+        hermite function series : HermiteFunction
+            The product of self and other.
+        """
+        if isinstance(other, HermiteFunction):
+            return HermiteFunction([a*b for a, b \
+                in zip_longest(self.coef, other.coef, fillvalue=0)])
+        else:
+            return HermiteFunction(self.coef * other)
+    
+    def __rmul__(self, other):
+        return self.__mul__(other)
+    
+    def __add__(self, other):
+        """Adds other to the coefficients
+        and returns the result as a new series object.
+        
+        Parameters
+        ----------
+        other : number, array or HermiteFunction
+            Other summand.
+        
+        Returns
+        -------
+        hermite function series : HermiteFunction
+            The sum of self and other.
+        """
+        if isinstance(other, HermiteFunction):
+            return HermiteFunction([a+b for a, b \
+                in zip_longest(self.coef, other.coef, fillvalue=0)])
+        else:
+            return HermiteFunction(self.coef + other)
+    
+    def __radd__(self, other):
+        return self.__add__(other)
+    
+    
+    #function stuff
+    def __call__(self, x):
+        """Evaluates the series at the given point(s).
+        
+        Parameters
+        ----------
+        x : number or array
+            Point(s) where to evaluate the series.
+        
+        Returns
+        -------
+        y : number or array
+            The value(s) at the given point(s).
+        """
+        y = 0
+        for n, c in enumerate(self.coef):
+            y += Hermite([0]*n+[c])(x) \
+                / np.sqrt(2**n * factorial(n) * np.sqrt(np.pi))
+        return y * np.exp(-x**2 / 2)
+    
+    def der(self, n=1):
+        """Returns the n-th derivative of this series.
+        
+        Parameters
+        ----------
+        n : positive integer, optional
+            Degree of differentiation (default: 1).
+        
+        Returns
+        -------
+        hermite function series : HermiteFunction
+            The n-th derivative of this series.
+        """
+        coef = self.coef
+        for _ in range(n):
+            i = np.arange(len(coef)+1)
+            coef = np.append(coef[1:], [0, 0])*np.sqrt((i+1)/2) \
+                    - np.append([0], coef)*np.sqrt(i/2)
+        return HermiteFunction(coef)
+    
+    def prod_reorder(self, other):
+        """Returns the product of self and other, divided by h_0.
+        
+        Parameters
+        ----------
+        other : HermiteFunction
+            Other factor.
+        
+        Returns
+        -------
+        hermite function series : HermiteFunction
+            The product of self and other, divided by h_0.
+        """
+        coef = np.zeros(len(self.coef)+len(other.coef)-1)
+        for b in range(len(coef)):
+            for n in range(b, len(self.coef)+len(other.coef)-1, 2):
+                for d in range(-b, b+1, 2):
+                    i, j = (n-d)//2, (n+d)//2
+                    k = (n-b)//2
+                    if 0<=i<len(self.coef) and 0<=j<len(other.coef):
+                        coef[b] += self.coef[i] * other.coef[j] \
+                            * factorial(k) * binom(i, k) * binom(j, k) \
+                            * np.sqrt(factorial(b)/(factorial(i)*factorial(j)))
+        return HermiteFunction(coef)
+    
+    def kin(self):
+        """Returns the kinetic energy of this series.
+        
+        Returns
+        -------
+        kinetic energy : float
+            The kinetic energy of this series.
+        """
+        return self.der().norm()**2 / 2
+    
+    
+    #python stuff
+    def __str__(self):
+        """Returns a Latex representation.
+        
+        Returns
+        -------
+        string : string
+            A Latex representation.
+        """
+        s = f'{self.coef[0]:.1f} h_0'
+        for i, c in enumerate(self.coef[1:]):
+            s += f' + {c:.1f} h_{i+1}'
+        return s
```

### Comparing `hermite-function-0.9.4/PKG-INFO` & `hermite-function-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hermite-function
-Version: 0.9.4
+Version: 0.9.9
 Summary: A Hermite function series module.
-Home-page: https://github.com/goessl/hermite-function
+Home-page: https://github.com/goessl/hermitefunction
 Author: Sebastian Gössl
 Author-email: goessl@student.tugraz.at
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `hermite-function-0.9.4/README.md` & `hermite-function-0.9.9/hermite_function.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: hermite-function
+Version: 0.9.9
+Summary: A Hermite function series module.
+Home-page: https://github.com/goessl/hermitefunction
+Author: Sebastian Gössl
+Author-email: goessl@student.tugraz.at
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Hermite Function Series
 
 A Hermite function series package.
 
 
 ```python
 from HermiteFunction import HermiteFunction
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hermite-function-0.9.4/hermite_function.egg-info/PKG-INFO` & `hermite-function-0.9.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,259 +1,244 @@
-Metadata-Version: 2.1
-Name: hermite-function
-Version: 0.9.4
-Summary: A Hermite function series module.
-Home-page: https://github.com/goessl/hermite-function
-Author: Sebastian Gössl
-Author-email: goessl@student.tugraz.at
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hermite Function Series
-
-A Hermite function series package.
-
-
-```python
-from HermiteFunction import HermiteFunction
-import numpy as np
-import matplotlib.pyplot as plt
-
-x = np.linspace(-4, +4, 1000)
-for n in range(5):
-    poly = HermiteFunction(n)
-    plt.plot(x, poly(x), label='$h_{}$'.format(n))
-plt.legend(loc='lower right')
-plt.show()
-```
-
-
-    
-![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/hermite_functions.png)
-    
-
-
-## Installation
-
-```
-pip install hermite-function
-```
-
-## Usage
-
-This package provides a single class, `HermiteFunction`, to handle Hermite function series.
-
-A series can be initialized in three ways:
- - With the constructor, that takes an non-negative integer to create a pure Hermite function with the given index, or an array-like of coefficients to create a Hermite function series.
- - With the random factory for a Hermite series with random indices up to a given degree.
- - By fitting a data set.
-
-
-```python
-f = HermiteFunction((1, 2, 3))
-g = HermiteFunction.random(15)
-h = HermiteFunction.fit(x, g(x), 10)
-plt.plot(x, f(x), label='$f$'), plt.plot(x, g(x), '--', label='$g$'), plt.plot(x, h(x), ':', label='$h$')
-plt.legend()
-plt.show()
-```
-
-
-    
-![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/initialization.png)
-    
-
-
-Methods for functions, simple evaluation and differentiation to an arbitrary degree, are implemented.
-
-
-```python
-f_p = f.der()
-f_pp = f.der(2)
-plt.plot(x, f(x), label='$f$'), plt.plot(x, f_p(x), '--', label='$f\'$'), plt.plot(x, f_pp(x), ':', label='$f\'\'$')
-plt.legend()
-plt.show()
-```
-
-
-    
-![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/differentiation.png)
-    
-
-
-Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space. Like vector addition, scalar (or elementwise) multiplication, inner product and norm.
-
-
-```python
-g = HermiteFunction(4)
-h = f + g
-i = 0.5 * f
-plt.plot(x, f(x), label='$f$'), plt.plot(x, g(x), '--', label='$g$'), plt.plot(x, h(x), ':', label='$h$'), plt.plot(x, i(x), '-.', label='$i$')
-plt.legend()
-plt.show()
-```
-
-
-    
-![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/algebra.png)
-    
-
-
-
-```python
-f.dot(h), f.norm()
-```
-
-
-
-
-    (14, 3.7416573867739413)
-
-
-
-But also the more exotic methods, the evaluation of the kinetic energy and finding $h$ to fulfill $fg=h_0h$ for a given $f, g$ (so $h=\frac{fg}{h_0}$).
-
-
-```python
-f.kin(), str(f.prod_reorder(g))
-```
-
-
-
-
-    (12.378679656440358,
-     '0.0 h_0 + 0.0 h_1 + 7.3 h_2 + 4.0 h_3 + 18.0 h_4 + 4.5 h_5 + 11.6 h_6')
-
-
-
-## Proofs
-
-***Note: [Githubs Latex rendering is buggy](https://github.com/community/community/discussions/17384), therefore better have a look at the [notebook](README.ipynb) that generated this markdown you are reading right now.***
-
-In the following let
-$$
-    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
-$$
-where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
-$$
-    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
-$$
-from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-### Hilbert space operations
-
-Nothing unusual. All the standard $L_\mathbb{R}^2$ operations.
-
-#### Scalar product
-
-$$
-    \langle f|g\rangle_{L_\mathbb{R}^2} = \sum_{k=0}^\infty f_k^*g_k
-$$
-
-#### Norm
-
-$$
-    ||f||_{L_\mathbb{R}^2} = \sqrt{\sum_{k=0}^\infty |f_k|^2}
-$$
-
-#### Scalar multiplication
-
-$$
-    af = \sum_{k=0}^\infty af_kh_k
-$$
-
-#### Addition
-
-$$
-    f+g = \sum_{k=0}^\infty (f_k+g_k)h_k
-$$
-
-### Function operations
-
-#### Evaluation
-
-$$
-    f(x) = \sum_{k=0}^\infty f_kh_k(x)
-$$
-
-#### Differentiation
-
-$$
-    \begin{aligned}
-        f' &= \sum_k f_k h_k' &&\mid h'_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
-        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
-        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} &&\mid k-1 \to k, \ k+1 \to k \\
-        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k &&\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
-        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
-        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
-    \end{aligned} \\
-    \begin{pmatrix}
-        f'_0 \\
-        f'_1 \\
-        f'_2 \\
-        f'_3 \\
-        \vdots
-    \end{pmatrix} = \begin{pmatrix}
-        0                   & \sqrt{\frac{1}{2}}  & 0                   & 0                  & \\
-        -\sqrt{\frac{1}{2}} & 0                   & \sqrt{\frac{2}{2}}  & 0                  & \cdots \\
-        0                   & -\sqrt{\frac{2}{2}} & 0                   & \sqrt{\frac{3}{2}} & \\
-        0                   & 0                   & -\sqrt{\frac{3}{2}} & 0                  & \\
-                            & \vdots              &                     &                    & \ddots
-    \end{pmatrix} \begin{pmatrix}
-        f_0 \\
-        f_1 \\
-        f_2 \\
-        f_3 \\
-        \vdots
-    \end{pmatrix}
-$$
-With $h'_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia-Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
-
-#### Integration
-
-TODO
-
-#### Kinetic energy
-
-$$
-    T = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)f''(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||_{L_{\mathbb{R}}^2}^2
-$$
-
-#### ''Multiplication''
-
-The product of two Hermite functions is
-$$
-    \begin{aligned}
-        &h_i(x) h_j(x) &&\mid h_j(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^jj!\sqrt{\pi}}}H_j(x) \\
-        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}} H_i(x)H_j(x) &&\mid H_j(x) = 2^\frac{j}{2}\tilde{H}_j(\sqrt{2}x) \\
-        &= \frac{e^{-x^2}}{\sqrt{2^{i+j} i!j! \pi}} 2^\frac{i+j}{2} \tilde{H}_i(\sqrt{2}x) \tilde{H}_j(\sqrt{2}x) &&\mid \tilde{H}_i\tilde{H}_j = \sum_{k=0}^{\min\{i, j\}}k!\binom{i}{k}\binom{j}{k}\tilde{H}_{i+j-2k} \\
-        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}} 2^\frac{i+j}{2} \sum_{k=0}^{\min\{i, j\}} k!\binom{i}{k}\binom{j}{k} \tilde{H}_{i+j-2k}(\sqrt{2}x) &&\mid \cdot1=2^{k-k} \\
-        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}}\sum_{j=0}^{\min\{i, j\}} 2^kk!\binom{i}{k}\binom{j}{k}2^\frac{i+j-2k}{2} \tilde{H}_{i+j-2k}(\sqrt{2}x) &&\mid H_j(x)=2^\frac{j}{2} \tilde{H}_j(\sqrt{2}x) \\
-        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}}\sum_{k=0}^{\min\{i, j\}} 2^kk!\binom{i}{k}\binom{j}{k} H_{i+j-2k}(x) &&\mid h_j(x)=\frac{e^{-\frac{x^2}{2}}}{\sqrt{2^jj!\sqrt{\pi}}} H_j(x) \\
-        &= \frac{e^{-\frac{x^2}{2}}}{\sqrt{i!j! \sqrt{\pi}}}\sum_{j=0}^{\min\{i, j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{(i+j-2k)!} h_{i+j-2k}(x) &&\mid h_0(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt[4]{\pi}} \\
-        &= h_0(x)\sum_{k=0}^{\min\{i,j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{\frac{(i+j-2k)!}{i!j!}} h_{i+j-2k}(x) \\
-        &= h_0(x)\sum_{k=0}^{\min\{i,j\}} \frac{\sqrt{i!j!(i+j-2k)!}}{k!(i-k)!(j-k)!} h_{i+j-2k}(x)
-    \end{aligned}
-$$
-With
- - $h_j(x)=\frac{e^{-\frac{x^2}{2}}}{\sqrt{2^jj!\sqrt{\pi}}}H_j(x)$, $H_j(x)=2^\frac{j}{2} \tilde{H}_j(\sqrt{2}x)$ and $h_0(x)=\frac{e^{-\frac{x^2}{2}}}{\sqrt[4]{\pi}}$ from [Wikipedia-Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions),
- - $H_j(x)=2^\frac{j}{2}\tilde{H}_j(\sqrt{2}x)$ from [Wikipedia-Hermite polynomials](https://en.wikipedia.org/wiki/Hermite_polynomials\#Definition),
- - $\tilde{H}_i\tilde{H}_j=\sum_{k=0}^{\min\{i, j\}}k!\binom{i}{k}\binom{j}{k}\tilde{H}_{i+j-2k}$ from [some file I found on the internet](https://ncatlab.org/nlab/files/HermitePolynomialsAndHermiteFunctions.pdf) eq. A.8.
-
-Therefore follows for the products of Hermite series:
-$$
-    \begin{aligned}
-        fg &= \sum_if_ih_i \sum_jg_jh_j = \sum_{i, j}f_ig_j h_ih_j \\
-        &\qquad\mid h_ih_j = h_0\sum_{k=0}^{\min\{i,j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{\frac{(i+j-2k)!}{i!j!}} h_{i+j-2k} \\
-        &= h_0 \sum_{i, j} f_ig_j \sum_{k=0}^{\min\{i,j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{\frac{(i+j-2k)!}{i!j!}} h_{i+j-2k} \\
-        &\vdots \\
-        &\text{(some steps I am not able to prove)} \\
-        &\vdots \\
-        &= h_0 \sum_{b=0}^\infty \sum_{n=b}^\infty \sum_{d=-b, 2}^{+b} f_{\frac{n-d}{2}}g_{\frac{n+d}{2}} \left(\frac{n-b}{2}\right)!\binom{\frac{n-d}{2}}{\frac{n-b}{2}}\binom{\frac{n+d}{2}}{\frac{n-b}{2}}\sqrt{\frac{\left(\frac{n-b}{2}\right)!}{\left(\frac{n-d}{2}\right)!\left(\frac{n+d}{2}\right)!}} h_b \\
-        &= h_0 \sum_{b=0}^\infty \sum_{n=b}^\infty \sum_{d=0}^b f_{\frac{n+b}{2}-d}g_{\frac{n-b}{2}+d} \left(\frac{n-b}{2}\right)!\binom{\frac{n+b}{2}-d}{\frac{n-b}{2}}\binom{\frac{n-b}{2}+d}{\frac{n-b}{2}}\sqrt{\frac{\left(\frac{n-b}{2}\right)!}{\left(\frac{n+b}{2}-d\right)!\left(\frac{n-b}{2}+d\right)!}} h_b
-    \end{aligned}
-$$
+# Hermite Function Series
+
+A Hermite function series package.
+
+
+```python
+from HermiteFunction import HermiteFunction
+import numpy as np
+import matplotlib.pyplot as plt
+
+x = np.linspace(-4, +4, 1000)
+for n in range(5):
+    poly = HermiteFunction(n)
+    plt.plot(x, poly(x), label='$h_{}$'.format(n))
+plt.legend(loc='lower right')
+plt.show()
+```
+
+
+    
+![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/hermite_functions.png)
+    
+
+
+## Installation
+
+```
+pip install hermite-function
+```
+
+## Usage
+
+This package provides a single class, `HermiteFunction`, to handle Hermite function series.
+
+A series can be initialized in three ways:
+ - With the constructor, that takes an non-negative integer to create a pure Hermite function with the given index, or an array-like of coefficients to create a Hermite function series.
+ - With the random factory for a Hermite series with random indices up to a given degree.
+ - By fitting a data set.
+
+
+```python
+f = HermiteFunction((1, 2, 3))
+g = HermiteFunction.random(15)
+h = HermiteFunction.fit(x, g(x), 10)
+plt.plot(x, f(x), label='$f$'), plt.plot(x, g(x), '--', label='$g$'), plt.plot(x, h(x), ':', label='$h$')
+plt.legend()
+plt.show()
+```
+
+
+    
+![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/initialization.png)
+    
+
+
+Methods for functions, simple evaluation and differentiation to an arbitrary degree, are implemented.
+
+
+```python
+f_p = f.der()
+f_pp = f.der(2)
+plt.plot(x, f(x), label='$f$'), plt.plot(x, f_p(x), '--', label='$f\'$'), plt.plot(x, f_pp(x), ':', label='$f\'\'$')
+plt.legend()
+plt.show()
+```
+
+
+    
+![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/differentiation.png)
+    
+
+
+Hilbert space operations are also provided, where the Hermite functions are used as an orthonormal basis of the $L_\mathbb{R}^2$ space. Like vector addition, scalar (or elementwise) multiplication, inner product and norm.
+
+
+```python
+g = HermiteFunction(4)
+h = f + g
+i = 0.5 * f
+plt.plot(x, f(x), label='$f$'), plt.plot(x, g(x), '--', label='$g$'), plt.plot(x, h(x), ':', label='$h$'), plt.plot(x, i(x), '-.', label='$i$')
+plt.legend()
+plt.show()
+```
+
+
+    
+![png](https://raw.githubusercontent.com/goessl/hermite_function/main/readme/algebra.png)
+    
+
+
+
+```python
+f.dot(h), f.norm()
+```
+
+
+
+
+    (14, 3.7416573867739413)
+
+
+
+But also the more exotic methods, the evaluation of the kinetic energy and finding $h$ to fulfill $fg=h_0h$ for a given $f, g$ (so $h=\frac{fg}{h_0}$).
+
+
+```python
+f.kin(), str(f.prod_reorder(g))
+```
+
+
+
+
+    (12.378679656440358,
+     '0.0 h_0 + 0.0 h_1 + 7.3 h_2 + 4.0 h_3 + 18.0 h_4 + 4.5 h_5 + 11.6 h_6')
+
+
+
+## Proofs
+
+***Note: [Githubs Latex rendering is buggy](https://github.com/community/community/discussions/17384), therefore better have a look at the [notebook](README.ipynb) that generated this markdown you are reading right now.***
+
+In the following let
+$$
+    f=\sum_{k=0}^\infty f_k h_k, \ g=\sum_{k=0}^\infty g_k h_k.
+$$
+where $h_k$ are the Hermite functions, defined by the Hermite polynomials $H_k$:
+$$
+    h_k(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^kk!\sqrt{\pi}}} H_k(x)
+$$
+from [Wikipedia - Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+### Hilbert space operations
+
+Nothing unusual. All the standard $L_\mathbb{R}^2$ operations.
+
+#### Scalar product
+
+$$
+    \langle f|g\rangle_{L_\mathbb{R}^2} = \sum_{k=0}^\infty f_k^*g_k
+$$
+
+#### Norm
+
+$$
+    ||f||_{L_\mathbb{R}^2} = \sqrt{\sum_{k=0}^\infty |f_k|^2}
+$$
+
+#### Scalar multiplication
+
+$$
+    af = \sum_{k=0}^\infty af_kh_k
+$$
+
+#### Addition
+
+$$
+    f+g = \sum_{k=0}^\infty (f_k+g_k)h_k
+$$
+
+### Function operations
+
+#### Evaluation
+
+$$
+    f(x) = \sum_{k=0}^\infty f_kh_k(x)
+$$
+
+#### Differentiation
+
+$$
+    \begin{aligned}
+        f' &= \sum_k f_k h_k' &&\mid h'_k = \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \\
+        &= \sum_k f_k \left( \sqrt{\frac{k}{2}}h_{k-1} - \sqrt{\frac{k+1}{2}}h_{k+1} \right) \\
+        &= \sum_{k=0}^\infty f_k\sqrt{\frac{k}{2}} h_{k-1} - \sum_{k=0}^\infty f_k\sqrt{\frac{k+1}{2}} h_{k+1} &&\mid k-1 \to k, \ k+1 \to k \\
+        &= \sum_{k=-1}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=1}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k &&\mid -0+0 = -\sqrt{\frac{-1+1}{2}}f_{-1+1}h_{-1} + \sqrt{\frac{0}{2}}f_{0-1} h_0 \\
+        &= \sum_{k=0}^\infty \sqrt{\frac{k+1}{2}}f_{k+1} h_k - \sum_{k=0}^\infty \sqrt{\frac{k}{2}}f_{k-1} h_k \\
+        &= \sum_k \left( \sqrt{\frac{k+1}{2}}f_{k+1} - \sqrt{\frac{k}{2}}f_{k-1} \right) h_k
+    \end{aligned} \\
+    \begin{pmatrix}
+        f'_0 \\
+        f'_1 \\
+        f'_2 \\
+        f'_3 \\
+        \vdots
+    \end{pmatrix} = \begin{pmatrix}
+        0                   & \sqrt{\frac{1}{2}}  & 0                   & 0                  & \\
+        -\sqrt{\frac{1}{2}} & 0                   & \sqrt{\frac{2}{2}}  & 0                  & \cdots \\
+        0                   & -\sqrt{\frac{2}{2}} & 0                   & \sqrt{\frac{3}{2}} & \\
+        0                   & 0                   & -\sqrt{\frac{3}{2}} & 0                  & \\
+                            & \vdots              &                     &                    & \ddots
+    \end{pmatrix} \begin{pmatrix}
+        f_0 \\
+        f_1 \\
+        f_2 \\
+        f_3 \\
+        \vdots
+    \end{pmatrix}
+$$
+With $h'_k=\sqrt{\frac{k}{2}}h_{k+1}-\sqrt{\frac{k+1}{2}}h_{k-1}$ from [Wikipedia-Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions).
+
+#### Integration
+
+TODO
+
+#### Kinetic energy
+
+$$
+    T = -\frac{1}{2}\int_{\mathbb{R}}f^*(x)f''(x)dx = +\frac{1}{2}\int_{\mathbb{R}}|f'(x)|^2dx = \frac{1}{2}||f'||_{L_{\mathbb{R}}^2}^2
+$$
+
+#### ''Multiplication''
+
+The product of two Hermite functions is
+$$
+    \begin{aligned}
+        &h_i(x) h_j(x) &&\mid h_j(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt{2^jj!\sqrt{\pi}}}H_j(x) \\
+        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}} H_i(x)H_j(x) &&\mid H_j(x) = 2^\frac{j}{2}\tilde{H}_j(\sqrt{2}x) \\
+        &= \frac{e^{-x^2}}{\sqrt{2^{i+j} i!j! \pi}} 2^\frac{i+j}{2} \tilde{H}_i(\sqrt{2}x) \tilde{H}_j(\sqrt{2}x) &&\mid \tilde{H}_i\tilde{H}_j = \sum_{k=0}^{\min\{i, j\}}k!\binom{i}{k}\binom{j}{k}\tilde{H}_{i+j-2k} \\
+        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}} 2^\frac{i+j}{2} \sum_{k=0}^{\min\{i, j\}} k!\binom{i}{k}\binom{j}{k} \tilde{H}_{i+j-2k}(\sqrt{2}x) &&\mid \cdot1=2^{k-k} \\
+        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}}\sum_{j=0}^{\min\{i, j\}} 2^kk!\binom{i}{k}\binom{j}{k}2^\frac{i+j-2k}{2} \tilde{H}_{i+j-2k}(\sqrt{2}x) &&\mid H_j(x)=2^\frac{j}{2} \tilde{H}_j(\sqrt{2}x) \\
+        &= \frac{e^{-x^2}}{\sqrt{2^{i+j}i!j!\pi}}\sum_{k=0}^{\min\{i, j\}} 2^kk!\binom{i}{k}\binom{j}{k} H_{i+j-2k}(x) &&\mid h_j(x)=\frac{e^{-\frac{x^2}{2}}}{\sqrt{2^jj!\sqrt{\pi}}} H_j(x) \\
+        &= \frac{e^{-\frac{x^2}{2}}}{\sqrt{i!j! \sqrt{\pi}}}\sum_{j=0}^{\min\{i, j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{(i+j-2k)!} h_{i+j-2k}(x) &&\mid h_0(x) = \frac{e^{-\frac{x^2}{2}}}{\sqrt[4]{\pi}} \\
+        &= h_0(x)\sum_{k=0}^{\min\{i,j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{\frac{(i+j-2k)!}{i!j!}} h_{i+j-2k}(x) \\
+        &= h_0(x)\sum_{k=0}^{\min\{i,j\}} \frac{\sqrt{i!j!(i+j-2k)!}}{k!(i-k)!(j-k)!} h_{i+j-2k}(x)
+    \end{aligned}
+$$
+With
+ - $h_j(x)=\frac{e^{-\frac{x^2}{2}}}{\sqrt{2^jj!\sqrt{\pi}}}H_j(x)$, $H_j(x)=2^\frac{j}{2} \tilde{H}_j(\sqrt{2}x)$ and $h_0(x)=\frac{e^{-\frac{x^2}{2}}}{\sqrt[4]{\pi}}$ from [Wikipedia-Hermite functions](https://en.wikipedia.org/wiki/Hermite_polynomials\#Hermite_functions),
+ - $H_j(x)=2^\frac{j}{2}\tilde{H}_j(\sqrt{2}x)$ from [Wikipedia-Hermite polynomials](https://en.wikipedia.org/wiki/Hermite_polynomials\#Definition),
+ - $\tilde{H}_i\tilde{H}_j=\sum_{k=0}^{\min\{i, j\}}k!\binom{i}{k}\binom{j}{k}\tilde{H}_{i+j-2k}$ from [some file I found on the internet](https://ncatlab.org/nlab/files/HermitePolynomialsAndHermiteFunctions.pdf) eq. A.8.
+
+Therefore follows for the products of Hermite series:
+$$
+    \begin{aligned}
+        fg &= \sum_if_ih_i \sum_jg_jh_j = \sum_{i, j}f_ig_j h_ih_j \\
+        &\qquad\mid h_ih_j = h_0\sum_{k=0}^{\min\{i,j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{\frac{(i+j-2k)!}{i!j!}} h_{i+j-2k} \\
+        &= h_0 \sum_{i, j} f_ig_j \sum_{k=0}^{\min\{i,j\}} k!\binom{i}{k}\binom{j}{k}\sqrt{\frac{(i+j-2k)!}{i!j!}} h_{i+j-2k} \\
+        &\vdots \\
+        &\text{(some steps I am not able to prove)} \\
+        &\vdots \\
+        &= h_0 \sum_{b=0}^\infty \sum_{n=b}^\infty \sum_{d=-b, 2}^{+b} f_{\frac{n-d}{2}}g_{\frac{n+d}{2}} \left(\frac{n-b}{2}\right)!\binom{\frac{n-d}{2}}{\frac{n-b}{2}}\binom{\frac{n+d}{2}}{\frac{n-b}{2}}\sqrt{\frac{\left(\frac{n-b}{2}\right)!}{\left(\frac{n-d}{2}\right)!\left(\frac{n+d}{2}\right)!}} h_b \\
+        &= h_0 \sum_{b=0}^\infty \sum_{n=b}^\infty \sum_{d=0}^b f_{\frac{n+b}{2}-d}g_{\frac{n-b}{2}+d} \left(\frac{n-b}{2}\right)!\binom{\frac{n+b}{2}-d}{\frac{n-b}{2}}\binom{\frac{n-b}{2}+d}{\frac{n-b}{2}}\sqrt{\frac{\left(\frac{n-b}{2}\right)!}{\left(\frac{n+b}{2}-d\right)!\left(\frac{n-b}{2}+d\right)!}} h_b
+    \end{aligned}
+$$
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

