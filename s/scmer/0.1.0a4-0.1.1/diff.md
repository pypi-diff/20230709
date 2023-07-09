# Comparing `tmp/scmer-0.1.0a4.tar.gz` & `tmp/scmer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmer-0.1.0a4.tar", last modified: Sun Feb 12 08:38:16 2023, max compression
+gzip compressed data, was "scmer-0.1.1.tar", last modified: Sun Jul  9 03:32:40 2023, max compression
```

## Comparing `scmer-0.1.0a4.tar` & `scmer-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 shaoheng  (1000) shaoheng  (1000)        0 2023-02-12 08:38:16.571257 scmer-0.1.0a4/
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     1066 2023-02-11 23:00:48.000000 scmer-0.1.0a4/LICENSE
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      129 2023-02-12 08:38:10.000000 scmer-0.1.0a4/MANIFEST.in
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     2189 2023-02-12 08:38:16.571257 scmer-0.1.0a4/PKG-INFO
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     1760 2023-02-11 23:00:48.000000 scmer-0.1.0a4/README.md
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)       54 2023-02-11 23:00:48.000000 scmer-0.1.0a4/requirements.txt
-drwxrwxr-x   0 shaoheng  (1000) shaoheng  (1000)        0 2023-02-12 08:38:16.571257 scmer-0.1.0a4/scmer/
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      140 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/__init__.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     3263 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/_base_selector.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     2396 2023-02-12 08:20:40.000000 scmer-0.1.0a4/scmer/_base_torch_model.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     2289 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/_comparison.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      827 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/_interfaces.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)    33182 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/_owlqn.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)    20018 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/_tsne_l1.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     5975 2023-02-12 08:20:44.000000 scmer-0.1.0a4/scmer/_tsne_torch_models.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)    22337 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/_umap_l1.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     5638 2023-02-12 08:20:44.000000 scmer-0.1.0a4/scmer/_umap_torch_models.py
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     1157 2023-02-11 23:00:48.000000 scmer-0.1.0a4/scmer/_utils.py
-drwxrwxr-x   0 shaoheng  (1000) shaoheng  (1000)        0 2023-02-12 08:38:16.571257 scmer-0.1.0a4/scmer.egg-info/
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     2189 2023-02-12 08:38:16.000000 scmer-0.1.0a4/scmer.egg-info/PKG-INFO
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      434 2023-02-12 08:38:16.000000 scmer-0.1.0a4/scmer.egg-info/SOURCES.txt
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)        1 2023-02-12 08:38:16.000000 scmer-0.1.0a4/scmer.egg-info/dependency_links.txt
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)       54 2023-02-12 08:38:16.000000 scmer-0.1.0a4/scmer.egg-info/requires.txt
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)        6 2023-02-12 08:38:16.000000 scmer-0.1.0a4/scmer.egg-info/top_level.txt
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)       38 2023-02-12 08:38:16.571257 scmer-0.1.0a4/setup.cfg
--rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      797 2023-02-12 08:37:35.000000 scmer-0.1.0a4/setup.py
+drwxrwxr-x   0 shaoheng  (1000) shaoheng  (1000)        0 2023-07-09 03:32:40.437646 scmer-0.1.1/
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     1066 2023-02-11 23:00:48.000000 scmer-0.1.1/LICENSE
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      103 2023-02-25 15:22:15.000000 scmer-0.1.1/MANIFEST.in
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     3057 2023-07-09 03:32:40.437646 scmer-0.1.1/PKG-INFO
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     2630 2023-07-09 03:16:00.000000 scmer-0.1.1/README.md
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)       54 2023-02-11 23:00:48.000000 scmer-0.1.1/requirements.txt
+drwxrwxr-x   0 shaoheng  (1000) shaoheng  (1000)        0 2023-07-09 03:32:40.437646 scmer-0.1.1/scmer/
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      140 2023-02-11 23:00:48.000000 scmer-0.1.1/scmer/__init__.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     3263 2023-02-11 23:00:48.000000 scmer-0.1.1/scmer/_base_selector.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     2396 2023-02-12 08:20:40.000000 scmer-0.1.1/scmer/_base_torch_model.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     2289 2023-02-11 23:00:48.000000 scmer-0.1.1/scmer/_comparison.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      827 2023-02-11 23:00:48.000000 scmer-0.1.1/scmer/_interfaces.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)    33182 2023-02-11 23:00:48.000000 scmer-0.1.1/scmer/_owlqn.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)    20158 2023-07-09 03:16:00.000000 scmer-0.1.1/scmer/_tsne_l1.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     5975 2023-02-12 08:20:44.000000 scmer-0.1.1/scmer/_tsne_torch_models.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)    22521 2023-07-09 03:32:28.000000 scmer-0.1.1/scmer/_umap_l1.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     5638 2023-02-12 08:20:44.000000 scmer-0.1.1/scmer/_umap_torch_models.py
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     1157 2023-02-11 23:00:48.000000 scmer-0.1.1/scmer/_utils.py
+drwxrwxr-x   0 shaoheng  (1000) shaoheng  (1000)        0 2023-07-09 03:32:40.437646 scmer-0.1.1/scmer.egg-info/
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)     3057 2023-07-09 03:32:40.000000 scmer-0.1.1/scmer.egg-info/PKG-INFO
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      434 2023-07-09 03:32:40.000000 scmer-0.1.1/scmer.egg-info/SOURCES.txt
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)        1 2023-07-09 03:32:40.000000 scmer-0.1.1/scmer.egg-info/dependency_links.txt
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)       54 2023-07-09 03:32:40.000000 scmer-0.1.1/scmer.egg-info/requires.txt
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)        6 2023-07-09 03:32:40.000000 scmer-0.1.1/scmer.egg-info/top_level.txt
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)       38 2023-07-09 03:32:40.437646 scmer-0.1.1/setup.cfg
+-rw-rw-r--   0 shaoheng  (1000) shaoheng  (1000)      795 2023-07-09 03:20:21.000000 scmer-0.1.1/setup.py
```

### Comparing `scmer-0.1.0a4/LICENSE` & `scmer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/PKG-INFO` & `scmer-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scmer
-Version: 0.1.0a4
+Version: 0.1.1
 Summary: Manifold preserving marker selection for single-cell data
 Home-page: https://scmer.readthedocs.io/
 Author: Shaoheng Liang
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SCMER - Manifold Preserving Feature Selection 
 [![Documentation Status](https://readthedocs.org/projects/scmer/badge/?version=latest)](https://scmer.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/scmer?color=blue&logo=pypi)](https://pypi.org/project/scmer) ![PyPI - Downloads](https://img.shields.io/pypi/dm/scmer) [![Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://doi.org/10.24433/CO.6781338.v1)
 
 SCMER is a feature selection methods designed for single-cell data analysis. 
@@ -20,21 +20,34 @@
 It can also be used for data integration by using features in one modality to match the manifold of another modality.
 
 ## Tutorials ##
 Tutorials are available at https://scmer.readthedocs.io/en/latest/examples.html
 
 You may start with the [Melanoma data (Tiorsh et al.)](https://scmer.readthedocs.io/en/latest/melanoma.html).
 
+### Running in R ###
+Python is more established in machine learning tasks, but many people prefer R as their primary language in data science. Luckily, a thin wrapper is what you need to run SCMER in R. Please see this short [tutorial](https://htmlpreview.github.io/?https://github.com/KChen-lab/SCMER/blob/master/notebooks/melanoma-gpu-with-batch-in-r.nb.html).
+
 ## Full Documentation ##
 Detailed documentation is available at https://scmer.readthedocs.io/en/latest/
 
 The mechanism and capabilities of SCMER is detailed in our pre-print [Single-Cell Manifold Preserving Feature Selection (SCMER)](https://www.biorxiv.org/content/10.1101/2020.12.01.407262v1)
 
+
+
+## Additional package info
+Using GPU can be tricky sometimes. Here is a [list of package versions](https://github.com/KChen-lab/SCMER/blob/master/notebooks/package_versions.txt) we successfully used with GPU.
+
 ## Publication ##
 Single-cell manifold-preserving feature selection for detecting rare cell populations *Nature Computational Science* (2021)
 - Paid access: https://www.nature.com/articles/s43588-021-00070-7
 - Free access (no download): https://rdcu.be/ckZGT
 - BioRxiv preprint: https://www.biorxiv.org/content/10.1101/2020.12.01.407262v1.full
 
 ## Contact ##
 I do monitor the "Issues" and aim to clear any issues in a few weeks.
 If you have an urgent request, please email liang.shaoheng@rice.edu.
+
+## Version log ##
+- 0.1.1 (6/8/2023) Fixed an issue that caused an error when `np.matrix` is used instead of `np.array`.
+- 0.1.0a4 (2/12/2023) Fixed an issue that caused an error when batch correction is enabled on GPU runs. CPU runs were not affected. 
+- 0.1.0a3 (2/17/2021) Initial version.
```

### Comparing `scmer-0.1.0a4/README.md` & `scmer-0.1.1/scmer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,53 @@
+Metadata-Version: 2.1
+Name: scmer
+Version: 0.1.1
+Summary: Manifold preserving marker selection for single-cell data
+Home-page: https://scmer.readthedocs.io/
+Author: Shaoheng Liang
+Author-email: 
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SCMER - Manifold Preserving Feature Selection 
 [![Documentation Status](https://readthedocs.org/projects/scmer/badge/?version=latest)](https://scmer.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/scmer?color=blue&logo=pypi)](https://pypi.org/project/scmer) ![PyPI - Downloads](https://img.shields.io/pypi/dm/scmer) [![Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://doi.org/10.24433/CO.6781338.v1)
 
 SCMER is a feature selection methods designed for single-cell data analysis. 
 It selects a compact sets of markers that preserve the manifold in the original data.
 It can also be used for data integration by using features in one modality to match the manifold of another modality.
 
 ## Tutorials ##
 Tutorials are available at https://scmer.readthedocs.io/en/latest/examples.html
 
 You may start with the [Melanoma data (Tiorsh et al.)](https://scmer.readthedocs.io/en/latest/melanoma.html).
 
+### Running in R ###
+Python is more established in machine learning tasks, but many people prefer R as their primary language in data science. Luckily, a thin wrapper is what you need to run SCMER in R. Please see this short [tutorial](https://htmlpreview.github.io/?https://github.com/KChen-lab/SCMER/blob/master/notebooks/melanoma-gpu-with-batch-in-r.nb.html).
+
 ## Full Documentation ##
 Detailed documentation is available at https://scmer.readthedocs.io/en/latest/
 
 The mechanism and capabilities of SCMER is detailed in our pre-print [Single-Cell Manifold Preserving Feature Selection (SCMER)](https://www.biorxiv.org/content/10.1101/2020.12.01.407262v1)
 
+
+
+## Additional package info
+Using GPU can be tricky sometimes. Here is a [list of package versions](https://github.com/KChen-lab/SCMER/blob/master/notebooks/package_versions.txt) we successfully used with GPU.
+
 ## Publication ##
 Single-cell manifold-preserving feature selection for detecting rare cell populations *Nature Computational Science* (2021)
 - Paid access: https://www.nature.com/articles/s43588-021-00070-7
 - Free access (no download): https://rdcu.be/ckZGT
 - BioRxiv preprint: https://www.biorxiv.org/content/10.1101/2020.12.01.407262v1.full
 
 ## Contact ##
 I do monitor the "Issues" and aim to clear any issues in a few weeks.
 If you have an urgent request, please email liang.shaoheng@rice.edu.
+
+## Version log ##
+- 0.1.1 (6/8/2023) Fixed an issue that caused an error when `np.matrix` is used instead of `np.array`.
+- 0.1.0a4 (2/12/2023) Fixed an issue that caused an error when batch correction is enabled on GPU runs. CPU runs were not affected. 
+- 0.1.0a3 (2/17/2021) Initial version.
```

### Comparing `scmer-0.1.0a4/scmer/_base_selector.py` & `scmer-0.1.1/scmer/_base_selector.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer/_base_torch_model.py` & `scmer-0.1.1/scmer/_base_torch_model.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer/_comparison.py` & `scmer-0.1.1/scmer/_comparison.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer/_interfaces.py` & `scmer-0.1.1/scmer/_interfaces.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer/_owlqn.py` & `scmer-0.1.1/scmer/_owlqn.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer/_tsne_l1.py` & `scmer-0.1.1/scmer/_tsne_l1.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,24 @@
         :param beta: The beta associated with P, if calculated in advance
         :param must_keep: A boolean vector indicating if a feature must be kept.
             Those features will have a fixed weight 1.
         :return:
         """
         tictoc = TicToc()
 
+        trans = True
+
+        X = np.array(X)
+        
         if X_teacher is None: # if there is no other assay to mimic, just mimic itself
             X_teacher = X
+            trans = False
+        else:
+            X_teacher = np.array(X_teacher)
+
 
         if batches is None:
             if must_keep is None and (isinstance(self._lasso, float) or isinstance(self._lasso, str)):
                 model_class = _RegTsneModel  # _SimpleRegTsneModel
             else:
                 model_class = _RegTsneModel
             if self._n_pcs is None:
```

### Comparing `scmer-0.1.0a4/scmer/_tsne_torch_models.py` & `scmer-0.1.1/scmer/_tsne_torch_models.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer/_umap_l1.py` & `scmer-0.1.1/scmer/_umap_l1.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,25 @@
         :param beta: The beta associated with P, if calculated in advance
         :param must_keep: A boolean vector indicating if a feature must be kept.
             Those features will have a fixed weight 1.
         :return:
         """
         tictoc = TicToc()
         trans = True
+
+        X = np.array(X)
+
+        if must_keep is not None:
+            must_keep = np.array(must_keep, dtype=float)
+        
         if X_teacher is None: # if there is no other assay to mimic, just mimic itself
             X_teacher = X
             trans = False
+        else:
+            X_teacher = np.array(X_teacher)
 
         if batches is None:
             if must_keep is None and (isinstance(self._lasso, float) or isinstance(self._lasso, str)):
                 model_class = _RegUmapModel #_SimpleRegTsneModel
             else:
                 model_class = _RegUmapModel
```

### Comparing `scmer-0.1.0a4/scmer/_umap_torch_models.py` & `scmer-0.1.1/scmer/_umap_torch_models.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer/_utils.py` & `scmer-0.1.1/scmer/_utils.py`

 * *Files identical despite different names*

### Comparing `scmer-0.1.0a4/scmer.egg-info/PKG-INFO` & `scmer-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 2.1
-Name: scmer
-Version: 0.1.0a4
-Summary: Manifold preserving marker selection for single-cell data
-Home-page: https://scmer.readthedocs.io/
-Author: Shaoheng Liang
-Author-email: 
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SCMER - Manifold Preserving Feature Selection 
 [![Documentation Status](https://readthedocs.org/projects/scmer/badge/?version=latest)](https://scmer.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/scmer?color=blue&logo=pypi)](https://pypi.org/project/scmer) ![PyPI - Downloads](https://img.shields.io/pypi/dm/scmer) [![Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://doi.org/10.24433/CO.6781338.v1)
 
 SCMER is a feature selection methods designed for single-cell data analysis. 
 It selects a compact sets of markers that preserve the manifold in the original data.
 It can also be used for data integration by using features in one modality to match the manifold of another modality.
 
 ## Tutorials ##
 Tutorials are available at https://scmer.readthedocs.io/en/latest/examples.html
 
 You may start with the [Melanoma data (Tiorsh et al.)](https://scmer.readthedocs.io/en/latest/melanoma.html).
 
+### Running in R ###
+Python is more established in machine learning tasks, but many people prefer R as their primary language in data science. Luckily, a thin wrapper is what you need to run SCMER in R. Please see this short [tutorial](https://htmlpreview.github.io/?https://github.com/KChen-lab/SCMER/blob/master/notebooks/melanoma-gpu-with-batch-in-r.nb.html).
+
 ## Full Documentation ##
 Detailed documentation is available at https://scmer.readthedocs.io/en/latest/
 
 The mechanism and capabilities of SCMER is detailed in our pre-print [Single-Cell Manifold Preserving Feature Selection (SCMER)](https://www.biorxiv.org/content/10.1101/2020.12.01.407262v1)
 
+
+
+## Additional package info
+Using GPU can be tricky sometimes. Here is a [list of package versions](https://github.com/KChen-lab/SCMER/blob/master/notebooks/package_versions.txt) we successfully used with GPU.
+
 ## Publication ##
 Single-cell manifold-preserving feature selection for detecting rare cell populations *Nature Computational Science* (2021)
 - Paid access: https://www.nature.com/articles/s43588-021-00070-7
 - Free access (no download): https://rdcu.be/ckZGT
 - BioRxiv preprint: https://www.biorxiv.org/content/10.1101/2020.12.01.407262v1.full
 
 ## Contact ##
 I do monitor the "Issues" and aim to clear any issues in a few weeks.
 If you have an urgent request, please email liang.shaoheng@rice.edu.
+
+## Version log ##
+- 0.1.1 (6/8/2023) Fixed an issue that caused an error when `np.matrix` is used instead of `np.array`.
+- 0.1.0a4 (2/12/2023) Fixed an issue that caused an error when batch correction is enabled on GPU runs. CPU runs were not affected. 
+- 0.1.0a3 (2/17/2021) Initial version.
```

### Comparing `scmer-0.1.0a4/setup.py` & `scmer-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scmer",
-    version="v0.1.0a4",
+    version="v0.1.1",
     author="Shaoheng Liang",
     author_email="",
     description="Manifold preserving marker selection for single-cell data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://scmer.readthedocs.io/",
     packages=['scmer'], #setuptools.find_packages(),
@@ -18,9 +18,9 @@
         l.strip() for l in Path('requirements.txt').read_text('utf-8').splitlines()
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.6',
 )
```

