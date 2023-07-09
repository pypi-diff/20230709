# Comparing `tmp/conjugate_models-0.1.0.tar.gz` & `tmp/conjugate_models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjugate_models-0.1.0.tar", max compression
+gzip compressed data, was "conjugate_models-0.1.1.tar", max compression
```

## Comparing `conjugate_models-0.1.0.tar` & `conjugate_models-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-06-23 11:07:04.395485 conjugate_models-0.1.0/LICENSE
--rw-r--r--   0        0        0     1283 2023-07-01 07:16:53.975139 conjugate_models-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-23 11:08:52.007050 conjugate_models-0.1.0/conjugate/__init__.py
--rw-r--r--   0        0        0      602 2023-06-28 20:24:26.365975 conjugate_models-0.1.0/conjugate/_typing.py
--rw-r--r--   0        0        0     5886 2023-07-01 07:25:22.378952 conjugate_models-0.1.0/conjugate/distributions.py
--rw-r--r--   0        0        0     5253 2023-07-01 07:28:25.489397 conjugate_models-0.1.0/conjugate/models.py
--rw-r--r--   0        0        0     4973 2023-06-30 05:36:09.292273 conjugate_models-0.1.0/conjugate/plot.py
--rw-r--r--   0        0        0        0 2023-06-23 11:08:47.618556 conjugate_models-0.1.0/conjugate/py.typed
--rw-r--r--   0        0        0      427 2023-06-30 05:20:32.103345 conjugate_models-0.1.0/conjugate/slice.py
--rw-r--r--   0        0        0      759 2023-06-29 05:25:29.844324 conjugate_models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 conjugate_models-0.1.0/setup.py
--rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 conjugate_models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-23 11:07:04.395485 conjugate_models-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1283 2023-07-09 14:15:32.199934 conjugate_models-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 11:08:52.007050 conjugate_models-0.1.1/conjugate/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-28 20:24:26.365975 conjugate_models-0.1.1/conjugate/_typing.py
+-rw-r--r--   0        0        0     7185 2023-07-09 14:14:21.892133 conjugate_models-0.1.1/conjugate/distributions.py
+-rw-r--r--   0        0        0     5252 2023-07-09 12:16:12.574649 conjugate_models-0.1.1/conjugate/models.py
+-rw-r--r--   0        0        0     5586 2023-07-09 12:54:38.337368 conjugate_models-0.1.1/conjugate/plot.py
+-rw-r--r--   0        0        0        0 2023-06-23 11:08:47.618556 conjugate_models-0.1.1/conjugate/py.typed
+-rw-r--r--   0        0        0      427 2023-06-30 05:20:32.103345 conjugate_models-0.1.1/conjugate/slice.py
+-rw-r--r--   0        0        0     1313 2023-07-09 14:12:27.858687 conjugate_models-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 conjugate_models-0.1.1/setup.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 conjugate_models-0.1.1/PKG-INFO
```

### Comparing `conjugate_models-0.1.0/LICENSE` & `conjugate_models-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conjugate_models-0.1.0/README.md` & `conjugate_models-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `conjugate_models-0.1.0/conjugate/_typing.py` & `conjugate_models-0.1.1/conjugate/_typing.py`

 * *Files identical despite different names*

### Comparing `conjugate_models-0.1.0/conjugate/distributions.py` & `conjugate_models-0.1.1/conjugate/distributions.py`

 * *Files 26% similar despite different names*

```diff
@@ -88,14 +88,37 @@
         return cls(alpha=alpha, beta=beta)
 
     @property
     def dist(self):
         return stats.beta(self.alpha, self.beta)
 
 
+@dataclass 
+class Binomial(DiscretePlotMixin, SliceMixin):
+    """Binomial distribution.
+    
+    Args: 
+        n: number of trials
+        p: probability of success
+    
+    """
+    n: NUMERIC
+    p: NUMERIC
+
+    def __post_init__(self):
+        if isinstance(self.n, np.ndarray):
+            self.max_value = self.n.max()
+        else:
+            self.max_value = self.n
+
+    @property
+    def dist(self):
+        return stats.binom(n=self.n, p=self.p)
+
+
 class VectorizedDist:
     def __init__(self, params: np.ndarray, dist: Any):
         self.params = params
         self.dist = dist
 
     def rvs(self, size: int = 1) -> np.ndarray:
         return np.stack([self.dist(param).rvs(size=size) for param in self.params])
@@ -262,7 +285,51 @@
 
     """
     p: NUMERIC
 
     @property
     def dist(self):
         return stats.geom(self.p)
+
+
+@dataclass
+class Normal(ContinuousPlotDistMixin, SliceMixin):
+    """Normal distribution.
+    
+    Args:
+        mu: mean
+        sigma: standard deviation
+
+    """
+    mu: NUMERIC
+    sigma: NUMERIC
+
+    @property
+    def dist(self):
+        return stats.norm(self.mu, self.sigma)
+    
+    def __mul__(self, other):
+        sigma = ((self.sigma ** 2) * other) ** 0.5
+        return Normal(mu=self.mu * other, sigma=sigma)
+    
+    __rmul__ = __mul__
+
+
+@dataclass
+class Uniform(ContinuousPlotDistMixin, SliceMixin):
+    """Uniform distribution.
+    
+    Args:
+        low: lower bound
+        high: upper bound
+
+    """
+    low: NUMERIC
+    high: NUMERIC
+
+    def __post_init__(self):
+        self.min_value = self.low
+        self.max_value = self.high
+
+    @property
+    def dist(self):
+        return stats.uniform(self.low, self.high)
```

### Comparing `conjugate_models-0.1.0/conjugate/models.py` & `conjugate_models-0.1.1/conjugate/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -165,8 +165,8 @@
 
 def exponetial_gamma(x_total: NUMERIC, n: NUMERIC, gamma_prior: Gamma) -> Gamma:
     """Posterior distribution for an exponential likelihood with a gamma prior"""
     alpha_post, beta_post = get_exponential_gamma_posterior_params(
         alpha=gamma_prior.alpha, beta=gamma_prior.beta, x_total=x_total, n=n
     )
 
-    return Gamma(alpha=alpha_post, beta=beta_post)
+    return Gamma(alpha=alpha_post, beta=beta_post)
```

### Comparing `conjugate_models-0.1.0/conjugate/plot.py` & `conjugate_models-0.1.1/conjugate/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,37 @@
 
     def rvs(self, size, *args, **kwargs) -> np.ndarray:
         ...
 
 
 LABEL_INPUT = Union[str, Iterable[str], Callable[[int], str]]
 
+def resolve_label(label: LABEL_INPUT, yy: np.ndarray):
+    """
+
+    https://stackoverflow.com/questions/73662931/matplotlib-plot-a-numpy-array-as-many-lines-with-a-single-label
+    """
+    if yy.ndim == 1:
+        return label
+
+    ncols = yy.shape[1]
+    if ncols != 1:
+        if isinstance(label, str):
+            return [f"{label} {i}" for i in range(1, ncols + 1)]
+
+        if callable(label):
+            return [label(i) for i in range(1, ncols + 1)]
+            
+        if isinstance(label, Iterable):
+            return label
+
+        raise ValueError("Label must be a string, iterable, or callable.")
+
+    return label
+
 
 class PlotDistMixin:
     """Base mixin in order to support plotting. Requires the dist attribute of the scipy distribution."""
     @property
     def dist(self) -> Distribution:
         raise NotImplementedError("Implement this property in the subclass.")
 
@@ -47,37 +70,14 @@
         """Make sure that the values are ready for plotting."""
         for value in asdict(self).values():
             if not isinstance(value, float):
                 return x[:, None]
 
         return x
 
-    def _resolve_label(self, label: LABEL_INPUT, yy: np.ndarray):
-        """
-
-        https://stackoverflow.com/questions/73662931/matplotlib-plot-a-numpy-array-as-many-lines-with-a-single-label
-        """
-        if yy.ndim == 1:
-            return label
-
-        ncols = yy.shape[1]
-        if ncols != 1:
-            if isinstance(label, Iterable):
-                return label
-
-            if isinstance(label, str):
-                label = lambda i: f"{label} {i}"
-
-            if callable(label):
-                return [label(i) for i in range(1, ncols + 1)]
-
-            raise ValueError("Label must be a string, iterable, or callable.")
-
-        return label
-
     def _settle_axis(self, ax: Optional[plt.Axes] = None) -> plt.Axes:
         return ax if ax is not None else plt.gca()
 
 
 class ContinuousPlotDistMixin(PlotDistMixin):
     """Functionality for plot_pdf method of continuous distributions."""
     def plot_pdf(self, ax: Optional[plt.Axes] = None, **kwargs) -> plt.Axes:
@@ -93,27 +93,48 @@
         """
         ax = self._settle_axis(ax=ax)
 
         x = self._create_x_values()
         x = self._reshape_x_values(x)
 
         return self._create_plot_on_axis(x, ax, **kwargs)
+    
+    @property 
+    def min_value(self) -> float:
+        if not hasattr(self, "_min_value"):
+            self._min_value = 0.0
+
+        return self._min_value
+    
+    @min_value.setter
+    def min_value(self, value: float) -> None:
+        self._min_value = value
+
+    def set_min_value(self, value: float) -> "ContinuousPlotDistMixin":
+        """Set the minimum value for plotting."""
+        self.min_value = value
+
+        return self
+
+    def set_bounds(self, lower: float, upper: float) -> "ContinuousPlotDistMixin":
+        """Set both the min and max values for plotting."""
+        return self.set_min_value(lower).set_max_value(upper)
 
     def _create_x_values(self) -> np.ndarray:
-        return np.linspace(0, self.max_value, 100)
+        return np.linspace(self.min_value, self.max_value, 100)
 
     def _setup_labels(self, ax) -> None:
         ax.set_xlabel("Domain")
         ax.set_ylabel("Density $f(x)$")
 
     def _create_plot_on_axis(self, x, ax, **kwargs) -> plt.Axes:
         yy = self.dist.pdf(x)
         if "label" in kwargs:
             label = kwargs.pop("label")
-            label = self._resolve_label(label, yy)
+            label = resolve_label(label, yy)
         else:
             label = None
 
         ax.plot(x, yy, label=label, **kwargs)
         self._setup_labels(ax=ax)
         ax.set_ylim(0, None)
         return ax
@@ -156,15 +177,15 @@
     def _create_x_values(self) -> np.ndarray:
         return np.arange(0, self.max_value + 1, 1)
 
     def _create_plot_on_axis(self, x, ax, mark, **kwargs) -> plt.Axes:
         yy = self.dist.pmf(x)
         if "label" in kwargs:
             label = kwargs.pop("label")
-            label = self._resolve_label(label, yy)
+            label = resolve_label(label, yy)
         else:
             label = None
 
         ax.plot(x, yy, mark, label=label, **kwargs)
         if self.max_value <= 15:
             ax.set_xticks(x.ravel())
```

### Comparing `conjugate_models-0.1.0/setup.py` & `conjugate_models-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 modules = \
 ['py']
 install_requires = \
 ['matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.3,<2.0.0', 'pandas', 'scipy<1.10.0']
 
 setup_kwargs = {
     'name': 'conjugate-models',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Bayesian Conjugate Models in Python',
     'long_description': '# conjugate priors\nBayesian conjugate models in Python\n\n\n## Installation\n\n```bash \npip install conjugate-models\n```\n\n## Basic Usage\n\n```python \nfrom conjugate.distributions import Beta, BetaBinomial\nfrom conjugate.models import binomial_beta, binomial_beta_posterior_predictive\n\n# Observed Data\nX = 4\nN = 10\n\n# Analytics\nprior = Beta(1, 1)\nprior_predictive: BetaBinomial = binomial_beta_posterior_predictive(n=N, beta=prior)\n\nposterior: Beta = binomial_beta(n=N, x=X, beta_prior=prior)\nposterior_predictive: BetaBinomial = binomial_beta_posterior_predictive(n=N, beta=posterior) \n\n# Figure\nimport matplotlib.pyplot as plt\n\nfig, axes = plt.subplots(ncols=2)\n\nax = axes[0]\nax = posterior.plot_pdf(ax=ax, label="posterior")\nprior.plot_pdf(ax=ax, label="prior")\nax.axvline(x=X/N, color="black", ymax=0.05, label="MLE")\nax.set_title("Success Rate")\nax.legend()\n\nax = axes[1]\nposterior_predictive.plot_pmf(ax=ax, label="posterior predictive")\nprior_predictive.plot_pmf(ax=ax, label="prior predictive")\nax.axvline(x=X, color="black", ymax=0.05, label="Sample")\nax.set_title("Number of Successes")\nax.legend()\nplt.show()\n```\n\n<img height=400 src="docs/images/binomial-beta.png" title="Binomial Beta Comparison">\n\nMore examples on in the [documentation](https://wd60622.github.io/conjugate/).',
     'author': 'Will Dean',
     'author_email': 'wd60622@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://wd60622.github.io/conjugate/',
     'packages': packages,
     'package_data': package_data,
     'py_modules': modules,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `conjugate_models-0.1.0/PKG-INFO` & `conjugate_models-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 Metadata-Version: 2.1
 Name: conjugate-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bayesian Conjugate Models in Python
+Home-page: https://wd60622.github.io/conjugate/
 License: MIT
 Author: Will Dean
 Author-email: wd60622@gmail.com
 Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas
 Requires-Dist: scipy (<1.10.0)
+Project-URL: Documentation, https://wd60622.github.io/conjugate/
+Project-URL: Repository, https://github.com/wd60622/conjugate
 Description-Content-Type: text/markdown
 
 # conjugate priors
 Bayesian conjugate models in Python
 
 
 ## Installation
```

