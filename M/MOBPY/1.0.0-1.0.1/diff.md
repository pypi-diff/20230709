# Comparing `tmp/MOBPY-1.0.0.tar.gz` & `tmp/MOBPY-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MOBPY-1.0.0.tar", last modified: Tue Jul  4 19:48:07 2023, max compression
+gzip compressed data, was "MOBPY-1.0.1.tar", last modified: Sun Jul  9 08:29:17 2023, max compression
```

## Comparing `MOBPY-1.0.0.tar` & `MOBPY-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-04 19:48:07.343406 MOBPY-1.0.0/
--rw-r--r--   0 chentahung   (501) staff       (20)     1073 2023-07-04 10:05:44.000000 MOBPY-1.0.0/LICENSE
--rw-r--r--   0 chentahung   (501) staff       (20)     6825 2023-07-04 19:48:07.343247 MOBPY-1.0.0/PKG-INFO
--rw-r--r--   0 chentahung   (501) staff       (20)     6200 2023-07-04 19:44:50.000000 MOBPY-1.0.0/README.md
--rw-r--r--   0 chentahung   (501) staff       (20)      695 2023-07-04 19:46:07.000000 MOBPY-1.0.0/pyproject.toml
--rw-r--r--   0 chentahung   (501) staff       (20)       38 2023-07-04 19:48:07.343460 MOBPY-1.0.0/setup.cfg
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-04 19:48:07.340530 MOBPY-1.0.0/src/
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-04 19:48:07.341468 MOBPY-1.0.0/src/MOBPY/
--rw-r--r--   0 chentahung   (501) staff       (20)     9878 2023-07-04 19:32:49.000000 MOBPY-1.0.0/src/MOBPY/MOB.py
--rw-------   0 chentahung   (501) staff       (20)        0 2022-10-18 10:30:40.000000 MOBPY-1.0.0/src/MOBPY/__ init __.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-04 19:48:07.342178 MOBPY-1.0.0/src/MOBPY/categorical/
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:26.000000 MOBPY-1.0.0/src/MOBPY/categorical/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-04 19:48:07.342754 MOBPY-1.0.0/src/MOBPY/numeric/
--rw-r--r--   0 chentahung   (501) staff       (20)     5675 2023-07-04 19:32:42.000000 MOBPY-1.0.0/src/MOBPY/numeric/Monotone.py
--rw-r--r--   0 chentahung   (501) staff       (20)     3185 2023-06-11 15:50:05.000000 MOBPY-1.0.0/src/MOBPY/numeric/MonotoneNode.py
--rw-r--r--   0 chentahung   (501) staff       (20)    14951 2023-07-04 10:09:42.000000 MOBPY-1.0.0/src/MOBPY/numeric/OptimalBinning.py
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:33.000000 MOBPY-1.0.0/src/MOBPY/numeric/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-04 19:48:07.343047 MOBPY-1.0.0/src/MOBPY/plot/
--rw-r--r--   0 chentahung   (501) staff       (20)     3710 2023-07-04 10:29:46.000000 MOBPY-1.0.0/src/MOBPY/plot/MOB_PLOT.py
--rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:39.000000 MOBPY-1.0.0/src/MOBPY/plot/__init__.py
-drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-04 19:48:07.342013 MOBPY-1.0.0/src/MOBPY.egg-info/
--rw-r--r--   0 chentahung   (501) staff       (20)     6825 2023-07-04 19:48:07.000000 MOBPY-1.0.0/src/MOBPY.egg-info/PKG-INFO
--rw-r--r--   0 chentahung   (501) staff       (20)      423 2023-07-04 19:48:07.000000 MOBPY-1.0.0/src/MOBPY.egg-info/SOURCES.txt
--rw-r--r--   0 chentahung   (501) staff       (20)        1 2023-07-04 19:48:07.000000 MOBPY-1.0.0/src/MOBPY.egg-info/dependency_links.txt
--rw-r--r--   0 chentahung   (501) staff       (20)        6 2023-07-04 19:48:07.000000 MOBPY-1.0.0/src/MOBPY.egg-info/top_level.txt
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.522137 MOBPY-1.0.1/
+-rw-r--r--   0 chentahung   (501) staff       (20)     1073 2023-07-04 10:05:44.000000 MOBPY-1.0.1/LICENSE
+-rw-r--r--   0 chentahung   (501) staff       (20)     7993 2023-07-09 08:29:17.521984 MOBPY-1.0.1/PKG-INFO
+-rw-r--r--   0 chentahung   (501) staff       (20)     7368 2023-07-05 17:45:58.000000 MOBPY-1.0.1/README.md
+-rw-r--r--   0 chentahung   (501) staff       (20)      695 2023-07-09 08:11:48.000000 MOBPY-1.0.1/pyproject.toml
+-rw-r--r--   0 chentahung   (501) staff       (20)       38 2023-07-09 08:29:17.522197 MOBPY-1.0.1/setup.cfg
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.517715 MOBPY-1.0.1/src/
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.519416 MOBPY-1.0.1/src/MOBPY/
+-rw-r--r--   0 chentahung   (501) staff       (20)    10854 2023-07-09 08:10:21.000000 MOBPY-1.0.1/src/MOBPY/MOB.py
+-rw-------   0 chentahung   (501) staff       (20)        0 2022-10-18 10:30:40.000000 MOBPY-1.0.1/src/MOBPY/__ init __.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.520211 MOBPY-1.0.1/src/MOBPY/categorical/
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:26.000000 MOBPY-1.0.1/src/MOBPY/categorical/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.521465 MOBPY-1.0.1/src/MOBPY/numeric/
+-rw-r--r--   0 chentahung   (501) staff       (20)     5192 2023-07-09 08:03:26.000000 MOBPY-1.0.1/src/MOBPY/numeric/Monotone.py
+-rw-r--r--   0 chentahung   (501) staff       (20)     3185 2023-06-11 15:50:05.000000 MOBPY-1.0.1/src/MOBPY/numeric/MonotoneNode.py
+-rw-r--r--   0 chentahung   (501) staff       (20)    14951 2023-07-04 10:09:42.000000 MOBPY-1.0.1/src/MOBPY/numeric/OptimalBinning.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:33.000000 MOBPY-1.0.1/src/MOBPY/numeric/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.521819 MOBPY-1.0.1/src/MOBPY/plot/
+-rw-r--r--   0 chentahung   (501) staff       (20)     3710 2023-07-04 10:29:46.000000 MOBPY-1.0.1/src/MOBPY/plot/MOB_PLOT.py
+-rw-r--r--   0 chentahung   (501) staff       (20)        0 2023-07-04 18:56:39.000000 MOBPY-1.0.1/src/MOBPY/plot/__init__.py
+drwxr-xr-x   0 chentahung   (501) staff       (20)        0 2023-07-09 08:29:17.520039 MOBPY-1.0.1/src/MOBPY.egg-info/
+-rw-r--r--   0 chentahung   (501) staff       (20)     7993 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/PKG-INFO
+-rw-r--r--   0 chentahung   (501) staff       (20)      423 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/SOURCES.txt
+-rw-r--r--   0 chentahung   (501) staff       (20)        1 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/dependency_links.txt
+-rw-r--r--   0 chentahung   (501) staff       (20)        6 2023-07-09 08:29:17.000000 MOBPY-1.0.1/src/MOBPY.egg-info/top_level.txt
```

### Comparing `MOBPY-1.0.0/LICENSE` & `MOBPY-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MOBPY-1.0.0/PKG-INFO` & `MOBPY-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: MOBPY
-Version: 1.0.0
+Version: 1.0.1
 Summary: MOB is a statistical approach to transform continuous variables into optimal and monotonic categorical variables.
 Author-email: "Chen, Ta-Hung" <denny20700@gmail.com>
 Project-URL: Homepage, https://github.com/ChenTaHung/Monotonic-Optimal-Binning
 Project-URL: Bug Tracker, https://github.com/ChenTaHung/Monotonic-Optimal-Binning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1><p align = 'center'><strong> Monotonic-Optimal-Binning</strong> </p></h1>
+<h1><p align = 'center'><strong> Monotonic-Optimal-Binning </strong> </p></h1>
+<h3><p align = 'center'><strong> Python implementation (MOBPY) </strong> </p></h3>
 
-**MOB** is a statistical approach to transform continuous variables into optimal and monotonic categorical variables. In this proejct, we extend the application so that the user can choose whether merge the bins under a `statistics` base or a `bins size` base to obtain the optimal result based on the users' expectation.<br>
+[**MOB**](https://pypi.org/project/MOBPY/) is a statistical approach to transform continuous variables into optimal and monotonic categorical variables. In this project, we have expanded the application to allow the users to merge the bins based on `statistics` or `bin size`. This is a Python-based project that enables the users to achieve monotone optimal binning results aligned with their expectations.<br>
 
 <h2><strong> Installation </strong></h2>
 
 ```bash
 python3 -m pip install MOBPY
 ```
 
 <h2><strong> Usage </strong></h2>
 
 
-<h3><span style = 'font-size:larger'> Example :</span></h3>
+**_Example_**:
 
 ```python
 import pandas as pd
 from MOBPY.MOB import MOB
 
 
 if __name__ == '__main__' :
@@ -53,35 +54,44 @@
     StatsBinning = MOB_ALGO.runMOB(mergeMethod='Stats') # Run under the statistical base. 
     
 ```
 
 
 The `runMOB` method will return a `pandas.DataFrame` which shows the binning result of the variable and also the WoE summary information for each bin. 
 
-<p align = 'center'><img src = 'doc/images/Durationinmonth%20bins%20summary.png' alt = 'Image' style = 'width: 1200px'/></p>
+<p align = 'center'><img src = 'https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/images/Durationinmonth%20bins%20summary.png' alt = 'Image' style = 'width: 800px'/></p>
 
 And after we receive the binning result dataframe, we can plot it by using `MOBPY.plot.MOB_PLOT.plotBinsSummary` to visualize the binning summary result.
 
 ```python
 from MOBPY.plot.MOB_PLOT import MOB_PLOT
 
 # plot the bin summary data.
 print('Bins Size Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = SizeBinning, var_name = 'Durationinmonth')
 
 print('Statisitcal Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = StatsBinning, var_name = 'Durationinmonth')
 ```
 
-<p align = 'center'><img src = 'doc/charts/Durationinmonth-Size.png' alt = 'Image' style = 'width: 1200px'/></p>
+<p align = 'center'><img src = 'https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Durationinmonth-Size.png' alt = 'Image' style = 'width: 1200px'/></p>
 
 
+<h2> <strong> Highlighted Features </strong></h2>
 
+**_User Preferences_**:
 
-Normally, the result of `Stats` (statistical base) and `Size` (bins size base) will be identical, but when the data appears to be quite extreme in the binning process, the `Size` method will prefer to make the population of each bin between the maximum and minimum limitation, while the `Stats` method will remain to conduct the algorithm through a stricter logic based on the testing hypothesis results.
+The MOB algorithm offers two user preference settings (**`mergeMethod`** argument):
+
+1. `Size`: This setting allows you to optimize the sample size of each bin within specified maximum and minimum limits while ensuring that the minimum number of bins constraint is maintained.
+
+2. `Stats`: With this setting, the algorithm applies a stricter approach based on hypothesis testing results.<br>
+
+
+Typically, the `'Stats'` (statistical-based) and `'Size'` (bin size-based) methods yield identical results. However, when dealing with data under certain scenarios where the `'Size'` method, employed by **MOB**, tends to prioritize maintaining the population of each bin within the maximum and minimum limits. In contrast, the `'Stats'` method adheres to a more rigorous logic based on the results of hypothesis testing.
 
 For example, 
 
 ```python
 # run the MOB algorithm to discretize the variable 'Creditamount'.
 MOB_ALGO = MOB(data = df, var = 'Creditamount', response = 'default', exclude_value = None) 
 # Set Binning Constraints (Must-Do!)
@@ -97,66 +107,67 @@
 # plot the bin summary data.
 print('Bins Size Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = SizeBinning, var_name = 'Durationinmonth')
 print('Statisitcal Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = StatsBinning, var_name = 'Durationinmonth')
 ```
 
-<div style="width: 100%;">
-  <table style="width: 100%;">
+<div>
+  <table >
     <thead>
       <tr>
         <th style="text-align: center;">SizeBinning</th>
         <th style="text-align: center;">StatsBinning</th>
       </tr>
     </thead>
     <tbody>
       <tr>
-        <td style="text-align: center;">mergeMethod = 'Size' (bins size base)</td>
-        <td style="text-align: center;">mergeMethod = 'Stats' (statistical base)</td>
+        <td style="text-align: center;">runMOB(mergeMethod='Size') (bins size base)</td>
+        <td style="text-align: center;">runMOB(mergeMethod='Stats') (statistical base)</td>
+      </tr>
+      <tr>
+        <td>
+            <img src="https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Creditamount-Size.png" width="400" >
+        </td>
+        <td>
+           <img src="https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Creditamount-Stats.png" width="400">
+        </td>
       </tr>
     </tbody>
   </table>
-
-  <div style="display: flex; justify-content: center;">
-    <img src="doc/charts/Creditamount-Size.png" alt="Image 1" style="width: 50%;" />
-    <img src="doc/charts/Creditamount-Stats.png" alt="Image 2" style="width: 50%;" />
-  </div>
 </div>
-<br>
 
-The left side image is the result generated by **`mergeMethod = 'Size'`** (bins size base), and the right side is the result generated by **`mergeMethod = 'Stats'`** (statistical base).We can see that the **Size method** merge the bins that do not meet the minimum sample population and maintain the bins number in order to prevent from exceeding the minimum bins limitation.<br><br>
+The left side image is the result generated by **`mergeMethod = 'Size'`** (bin size-based), and the right side is the result generated by **`mergeMethod = 'Stats'`** (statistical-based). We can see that the `'Size'` method is designed to merge bins that fail to meet the minimum sample population requirement. This approach ensures that the number of bins remains within the specified limit, preventing it from exceeding the minimum bin limitation. By merging bins that fall short of the population threshold, the `'Size'` method effectively maintains a balanced distribution of data across the bins..<br><br>
 
 
+<h2><strong> Full Documentation </strong></h2>
+
+↪ [Full API Reference](https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/MOBPY-API-Ref.md)<br><br>
 
 <h2> <strong> Environment </strong></h2>
 
 ```bash
 OS : macOS Ventura
 
 IDE: Visual Studio Code 1.79.2 (Universal)
 
 Language : Python 3.9.7 
     - pandas 1.3.4
     - numpy 1.20.3
     - scipy 1.7.1
     - matplotlib 3.7.1
 ```
-<br>
-
-<h2><strong> Citation </strong></h2>
-
-- [Mironchyk, Pavel, and Viktor Tchistiakov. "Monotone optimal binning algorithm for credit risk modeling." Utr. Work. Pap (2017).](https://www.researchgate.net/profile/Viktor-Tchistiakov/publication/322520135_Monotone_optimal_binning_algorithm_for_credit_risk_modeling/links/5a5dd1a8458515c03edf9a97/Monotone-optimal-binning-algorithm-for-credit-risk-modeling.pdf)
-
 
 
 <h2><strong> Reference </strong></h2>
 
 - Testing Dataset : [German Credit Risk](https://www.kaggle.com/datasets/uciml/german-credit) from [Kaggle](https://www.kaggle.com/)
 
+- [Mironchyk, Pavel, and Viktor Tchistiakov. "Monotone optimal binning algorithm for credit risk modeling." Utr. Work. Pap (2017).](https://www.researchgate.net/profile/Viktor-Tchistiakov/publication/322520135_Monotone_optimal_binning_algorithm_for_credit_risk_modeling/links/5a5dd1a8458515c03edf9a97/Monotone-optimal-binning-algorithm-for-credit-risk-modeling.pdf)
+
 - GitHub Project : [Monotone Optimal Binning (SAS 9.4 version)](https://github.com/cdfq384903/MonotonicOptimalBinning)
 
 <h2><strong> Authors </strong></h2>
 
 
 1. Chen, Ta-Hung (Denny) <br>
     - LinkedIn Profile : https://www.linkedin.com/in/dennychen-tahung/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MOBPY-1.0.0/README.md` & `MOBPY-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-<h1><p align = 'center'><strong> Monotonic-Optimal-Binning</strong> </p></h1>
+<h1><p align = 'center'><strong> Monotonic-Optimal-Binning </strong> </p></h1>
+<h3><p align = 'center'><strong> Python implementation (MOBPY) </strong> </p></h3>
 
-**MOB** is a statistical approach to transform continuous variables into optimal and monotonic categorical variables. In this proejct, we extend the application so that the user can choose whether merge the bins under a `statistics` base or a `bins size` base to obtain the optimal result based on the users' expectation.<br>
+[**MOB**](https://pypi.org/project/MOBPY/) is a statistical approach to transform continuous variables into optimal and monotonic categorical variables. In this project, we have expanded the application to allow the users to merge the bins based on `statistics` or `bin size`. This is a Python-based project that enables the users to achieve monotone optimal binning results aligned with their expectations.<br>
 
 <h2><strong> Installation </strong></h2>
 
 ```bash
 python3 -m pip install MOBPY
 ```
 
 <h2><strong> Usage </strong></h2>
 
 
-<h3><span style = 'font-size:larger'> Example :</span></h3>
+**_Example_**:
 
 ```python
 import pandas as pd
 from MOBPY.MOB import MOB
 
 
 if __name__ == '__main__' :
@@ -39,35 +40,44 @@
     StatsBinning = MOB_ALGO.runMOB(mergeMethod='Stats') # Run under the statistical base. 
     
 ```
 
 
 The `runMOB` method will return a `pandas.DataFrame` which shows the binning result of the variable and also the WoE summary information for each bin. 
 
-<p align = 'center'><img src = 'doc/images/Durationinmonth%20bins%20summary.png' alt = 'Image' style = 'width: 1200px'/></p>
+<p align = 'center'><img src = 'https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/images/Durationinmonth%20bins%20summary.png' alt = 'Image' style = 'width: 800px'/></p>
 
 And after we receive the binning result dataframe, we can plot it by using `MOBPY.plot.MOB_PLOT.plotBinsSummary` to visualize the binning summary result.
 
 ```python
 from MOBPY.plot.MOB_PLOT import MOB_PLOT
 
 # plot the bin summary data.
 print('Bins Size Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = SizeBinning, var_name = 'Durationinmonth')
 
 print('Statisitcal Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = StatsBinning, var_name = 'Durationinmonth')
 ```
 
-<p align = 'center'><img src = 'doc/charts/Durationinmonth-Size.png' alt = 'Image' style = 'width: 1200px'/></p>
+<p align = 'center'><img src = 'https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Durationinmonth-Size.png' alt = 'Image' style = 'width: 1200px'/></p>
 
 
+<h2> <strong> Highlighted Features </strong></h2>
 
+**_User Preferences_**:
 
-Normally, the result of `Stats` (statistical base) and `Size` (bins size base) will be identical, but when the data appears to be quite extreme in the binning process, the `Size` method will prefer to make the population of each bin between the maximum and minimum limitation, while the `Stats` method will remain to conduct the algorithm through a stricter logic based on the testing hypothesis results.
+The MOB algorithm offers two user preference settings (**`mergeMethod`** argument):
+
+1. `Size`: This setting allows you to optimize the sample size of each bin within specified maximum and minimum limits while ensuring that the minimum number of bins constraint is maintained.
+
+2. `Stats`: With this setting, the algorithm applies a stricter approach based on hypothesis testing results.<br>
+
+
+Typically, the `'Stats'` (statistical-based) and `'Size'` (bin size-based) methods yield identical results. However, when dealing with data under certain scenarios where the `'Size'` method, employed by **MOB**, tends to prioritize maintaining the population of each bin within the maximum and minimum limits. In contrast, the `'Stats'` method adheres to a more rigorous logic based on the results of hypothesis testing.
 
 For example, 
 
 ```python
 # run the MOB algorithm to discretize the variable 'Creditamount'.
 MOB_ALGO = MOB(data = df, var = 'Creditamount', response = 'default', exclude_value = None) 
 # Set Binning Constraints (Must-Do!)
@@ -83,66 +93,67 @@
 # plot the bin summary data.
 print('Bins Size Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = SizeBinning, var_name = 'Durationinmonth')
 print('Statisitcal Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = StatsBinning, var_name = 'Durationinmonth')
 ```
 
-<div style="width: 100%;">
-  <table style="width: 100%;">
+<div>
+  <table >
     <thead>
       <tr>
         <th style="text-align: center;">SizeBinning</th>
         <th style="text-align: center;">StatsBinning</th>
       </tr>
     </thead>
     <tbody>
       <tr>
-        <td style="text-align: center;">mergeMethod = 'Size' (bins size base)</td>
-        <td style="text-align: center;">mergeMethod = 'Stats' (statistical base)</td>
+        <td style="text-align: center;">runMOB(mergeMethod='Size') (bins size base)</td>
+        <td style="text-align: center;">runMOB(mergeMethod='Stats') (statistical base)</td>
+      </tr>
+      <tr>
+        <td>
+            <img src="https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Creditamount-Size.png" width="400" >
+        </td>
+        <td>
+           <img src="https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Creditamount-Stats.png" width="400">
+        </td>
       </tr>
     </tbody>
   </table>
-
-  <div style="display: flex; justify-content: center;">
-    <img src="doc/charts/Creditamount-Size.png" alt="Image 1" style="width: 50%;" />
-    <img src="doc/charts/Creditamount-Stats.png" alt="Image 2" style="width: 50%;" />
-  </div>
 </div>
-<br>
 
-The left side image is the result generated by **`mergeMethod = 'Size'`** (bins size base), and the right side is the result generated by **`mergeMethod = 'Stats'`** (statistical base).We can see that the **Size method** merge the bins that do not meet the minimum sample population and maintain the bins number in order to prevent from exceeding the minimum bins limitation.<br><br>
+The left side image is the result generated by **`mergeMethod = 'Size'`** (bin size-based), and the right side is the result generated by **`mergeMethod = 'Stats'`** (statistical-based). We can see that the `'Size'` method is designed to merge bins that fail to meet the minimum sample population requirement. This approach ensures that the number of bins remains within the specified limit, preventing it from exceeding the minimum bin limitation. By merging bins that fall short of the population threshold, the `'Size'` method effectively maintains a balanced distribution of data across the bins..<br><br>
 
 
+<h2><strong> Full Documentation </strong></h2>
+
+↪ [Full API Reference](https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/MOBPY-API-Ref.md)<br><br>
 
 <h2> <strong> Environment </strong></h2>
 
 ```bash
 OS : macOS Ventura
 
 IDE: Visual Studio Code 1.79.2 (Universal)
 
 Language : Python 3.9.7 
     - pandas 1.3.4
     - numpy 1.20.3
     - scipy 1.7.1
     - matplotlib 3.7.1
 ```
-<br>
-
-<h2><strong> Citation </strong></h2>
-
-- [Mironchyk, Pavel, and Viktor Tchistiakov. "Monotone optimal binning algorithm for credit risk modeling." Utr. Work. Pap (2017).](https://www.researchgate.net/profile/Viktor-Tchistiakov/publication/322520135_Monotone_optimal_binning_algorithm_for_credit_risk_modeling/links/5a5dd1a8458515c03edf9a97/Monotone-optimal-binning-algorithm-for-credit-risk-modeling.pdf)
-
 
 
 <h2><strong> Reference </strong></h2>
 
 - Testing Dataset : [German Credit Risk](https://www.kaggle.com/datasets/uciml/german-credit) from [Kaggle](https://www.kaggle.com/)
 
+- [Mironchyk, Pavel, and Viktor Tchistiakov. "Monotone optimal binning algorithm for credit risk modeling." Utr. Work. Pap (2017).](https://www.researchgate.net/profile/Viktor-Tchistiakov/publication/322520135_Monotone_optimal_binning_algorithm_for_credit_risk_modeling/links/5a5dd1a8458515c03edf9a97/Monotone-optimal-binning-algorithm-for-credit-risk-modeling.pdf)
+
 - GitHub Project : [Monotone Optimal Binning (SAS 9.4 version)](https://github.com/cdfq384903/MonotonicOptimalBinning)
 
 <h2><strong> Authors </strong></h2>
 
 
 1. Chen, Ta-Hung (Denny) <br>
     - LinkedIn Profile : https://www.linkedin.com/in/dennychen-tahung/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MOBPY-1.0.0/pyproject.toml` & `MOBPY-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "MOBPY"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Chen, Ta-Hung", email="denny20700@gmail.com" }
 ]
 description = "MOB is a statistical approach to transform continuous variables into optimal and monotonic categorical variables."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `MOBPY-1.0.0/src/MOBPY/MOB.py` & `MOBPY-1.0.1/src/MOBPY/MOB.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pandas as pd
 import numpy as np
+from typing import Union
 from MOBPY.numeric.Monotone import Monotone
 from MOBPY.numeric.OptimalBinning import OptimalBinning
 
 class MOB:
     def __init__(self, data, var, response, exclude_value = None) :
         self._data = data
         self._var = var
@@ -20,15 +21,15 @@
         self.df_sel : selected data subset
         
         '''
         if self._data[self._var].isna().sum() > 0 :
             _isNaExist = True
         else :
             _isNaExist = False
-        
+              
         # check exclude values exist
         if isinstance(exclude_value, list) :
             if self._data[self._var].isin(exclude_value).sum() > 0 : #contains exclude value
                 _isExcValueExist = True
             else :
                 _isExcValueExist = False
         elif isinstance(exclude_value, (float, int)) :
@@ -38,35 +39,36 @@
                 _isExcValueExist = False
         elif exclude_value == None :
             _isExcValueExist = False
         else :
             _isExcValueExist = False
             
         
-        if _isNaExist & _isExcValueExist :
+        if _isNaExist & _isExcValueExist : #both contains missing and exclude values
             self._df_missing = self._data.loc[self._data[self._var].isna(), :]
             
-            if isinstance(self._exclude_value, list) :
+            if isinstance(exclude_value, list) :
                 self._df_excvalue = self._data.loc[self._data[self._var].isin(exclude_value), :]
+                self._df_sel = self._data.loc[(self._data[self._var].notnull()) & ~(self._data[self._var].isin(exclude_value))]
             elif isinstance(exclude_value, (float, int)) :
                 self._df_excvalue = self._data.loc[self._data[self._var] == exclude_value, :]
-                
-            self._df_sel = self._data.loc[(self._data[self._var].notnull()) & (self._data[self._var] != exclude_value)]
+                self._df_sel = self._data.loc[(self._data[self._var].notnull()) & (self._data[self._var] != exclude_value)]
             
         elif _isNaExist & ~_isExcValueExist: #only contain missing
             self._df_missing = self._data.loc[self._data[self._var].isna(), :]
             self._df_sel = self._data.loc[self._data[self._var].notnull()]
             
         elif ~_isNaExist & _isExcValueExist : #only contain exclude condition
             if isinstance(exclude_value, list) :
                 self._df_excvalue = self._data.loc[self._data[self._var].isin(exclude_value), :]
+                self._df_sel = self._data.loc[~self._data[self._var].isin(exclude_value)]
             elif isinstance(exclude_value, (float, int)) :
                 self._df_excvalue = self._data.loc[self._data[self._var] == exclude_value, :]
-                
-            self._df_sel = self._data.loc[self._data[self._var] != exclude_value]
+                self._df_sel = self._data.loc[self._data[self._var] != exclude_value]
+        
         else:
             self._df_sel = self._data
             
         self._isNaExist = _isNaExist
         self._isExcValueExist = _isExcValueExist
         # binning constraints
         self._max_bins = 6
@@ -75,115 +77,116 @@
         self._max_samples = 0.4
         self._min_samples = 0.05
         self._min_bads = 0.05
         self._maximize_bins = True
         self._finishBinningTable = None
         
     @property
-    def data(self) :
+    def data(self) -> pd.DataFrame:
         return self._data
-    @data.setter
-    def data(self, value) :
-        self._data = value
     
     @property
-    def var(self):
+    def var(self) -> str :
         return self._var
         
     @property
-    def response(self):
+    def response(self) -> str:
         return self._response
     
     @property
-    def exclude_value(self):
+    def exclude_value(self) -> Union[list, int, float, None]:
         return self._exclude_value
 
     @property
-    def constraintsStatus(self):
+    def constraintsStatus(self) -> bool:
         return self._constraintsStatus
     
     @property
-    def isNaExist(self):
+    def isNaExist(self) -> bool:
         return self._isNaExist
     
     @property
-    def isExcValueExist(self) :
+    def isExcValueExist(self) -> bool:
         return self._isExcValueExist
     
     @property
-    def df_missing(self):
+    def df_missing(self) -> pd.DataFrame:
         return self._df_missing
     
     @property
-    def df_excvalue(self):
+    def df_excvalue(self) -> pd.DataFrame:
         return self._df_excvalue
     
     @property
-    def df_sel(self):
+    def df_sel(self) -> pd.DataFrame:
         return self._df_sel
     
     @property
-    def max_bins(self) :
+    def max_bins(self) -> int:
         return self._max_bins
-    # @max_bins.setter
-    # def max_bins(self, value):
-    #     self._max_bins = value
 
     @property
-    def min_bins(self):
+    def min_bins(self) -> int:
         return self._min_bins
         
     @property
-    def init_pvalue(self) :
+    def init_pvalue(self) -> float:
         return self._init_pvalue
         
     @property
-    def max_samples(self) :
+    def max_samples(self) -> Union[int, float]:
         return self._max_samples
 
     @property
-    def min_samples(self) :
+    def min_samples(self) -> Union[int, float] :
         return self._min_samples
     
     @property
-    def min_bads(self):
+    def min_bads(self) -> Union[int, float]:
         return self._min_bads
     
     @property
-    def maximize_bins(self) :
+    def maximize_bins(self) -> bool :
         return self._maximize_bins
     
     @property
-    def finishBinningTable(self) :
+    def finishBinningTable(self) -> pd.DataFrame :
         return self._finishBinningTable
     
     def setBinningConstraints(self, max_bins :int = 6, min_bins :int = 4, max_samples = 0.4, min_samples = 0.05, min_bads = 0.05, init_pvalue: float = 0.4, maximize_bins :bool = True) -> None:
         self._max_bins = max_bins
         self._min_bins = min_bins
         self._init_pvalue = init_pvalue
         self._max_samples = max_samples
         self._min_samples = min_samples
         self._min_bads = min_bads
         self._maximize_bins = maximize_bins
         self._constraintsStatus = True
            
-    def __summarizeBins(self, FinalOptTable):
+    def __summarizeBins(self, FinalOptTable) -> pd.DataFrame:
         
         FinalOptTable = FinalOptTable[['start', 'end', 'total', 'bads', 'mean']].rename(columns = {'total': 'nsamples', 'bad' : 'bads', 'mean' : 'bad_rate'})
         FinalOptTable['dist_obs'] = FinalOptTable['nsamples'] / FinalOptTable['nsamples'].sum()
         FinalOptTable['dist_bads'] = FinalOptTable['bads'] / FinalOptTable['bads'].sum()
         FinalOptTable['goods'] = FinalOptTable['nsamples'] - FinalOptTable['bads']
         FinalOptTable['dist_goods'] = FinalOptTable['goods'] / FinalOptTable['goods'].sum()
         FinalOptTable['woe'] = np.log(FinalOptTable['dist_goods']/FinalOptTable['dist_bads'])
-        FinalOptTable['iv_grp'] = (FinalOptTable['dist_goods'] - FinalOptTable['dist_bads']) * FinalOptTable['woe']
         
-        # TODO : Missing Data bads = 0 時候 woe 計算 (exc_value 同理） adjusted woe
+        # adjusted woe replacement when encounter zero bads or zero goods
+        if (FinalOptTable['bads'] == 0).sum() + (FinalOptTable['goods']).sum() > 0 :
+            adj_goods = FinalOptTable.loc[(FinalOptTable['bads'] == 0) | (FinalOptTable['goods'] == 0), 'goods'] + 0.5
+            adj_bads = FinalOptTable.loc[(FinalOptTable['bads'] == 0) | (FinalOptTable['goods'] == 0), 'bads'] + 0.5
+            adj_dist_goods = adj_goods / FinalOptTable['goods'].sum()
+            adj_dist_bads = adj_bads / FinalOptTable['bads'].sum()
+            FinalOptTable.loc[(FinalOptTable['bads'] == 0) | (FinalOptTable['goods'] == 0), 'woe'] = np.log(adj_dist_goods/adj_dist_bads)
+
+        FinalOptTable['iv_grp'] = (FinalOptTable['dist_goods'] - FinalOptTable['dist_bads']) * FinalOptTable['woe']
         return FinalOptTable      
       
-    def runMOB(self, mergeMethod, sign = 'auto') :
+    def runMOB(self, mergeMethod, sign = 'auto') -> pd.DataFrame :
         if self.constraintsStatus == False :
             raise Exception('Please set the constraints first by using "setBinningConstraints" method.')
         
         # Monotone
         MonotoneTuner = Monotone(data = self.df_sel, var = self.var, response = self.response)
         MonoTable = MonotoneTuner.tuneMonotone(sign = sign)
         self.MonoTable = MonoTable
@@ -204,15 +207,15 @@
             missingDF = pd.DataFrame({
                 'start' : ['Missing'],
                 'end' : ['Missing'],
                 'total' : [len(self.df_missing)],
                 'bads' : [self.df_missing[self.response].sum()],
                 'mean' : [(self.df_missing[self.response].sum()) / (len(self.df_missing))]})
                 
-            excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename({self.var: 'start','count':'total', 'sum':'bads'})
+            excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename(columns={self.var: 'start','count':'total', 'sum':'bads'})
             excludeValueDF['start'] = excludeValueDF['start'].astype(str)
             excludeValueDF.insert(1, 'end', excludeValueDF['start'])
             excludeValueDF['mean'] = excludeValueDF['bads'] / excludeValueDF['total']
             
             completeBinningTable = pd.concat([finishBinningTable, missingDF, excludeValueDF], axis = 0, ignore_index = True)
         elif self.isNaExist & ~self.isExcValueExist : # contains missing but no special values
             missingDF = pd.DataFrame({
@@ -220,15 +223,15 @@
                 'end' : ['Missing'],
                 'total' : [len(self.df_missing)],
                 'bads' : [self.df_missing[self.response].sum()],
                 'mean' : [(self.df_missing[self.response].sum()) / (len(self.df_missing))]})
             
             completeBinningTable = pd.concat([finishBinningTable, missingDF], axis = 0, ignore_index = True)
         elif ~self.isNaExist & self.isExcValueExist : # contains special values but no missing data
-            excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename({self.var: 'start','count':'total', 'sum':'bads'})
+            excludeValueDF = self.df_excvalue.groupby(self.var)[self.response].agg(['count', 'sum']).reset_index().fillna(0).rename(columns={self.var: 'start','count':'total', 'sum':'bads'})
             excludeValueDF['start'] = excludeValueDF['start'].astype(str)
             excludeValueDF.insert(1, 'end', excludeValueDF['start'])
             excludeValueDF['mean'] = excludeValueDF['bads'] / excludeValueDF['total']
             
             completeBinningTable = pd.concat([finishBinningTable, excludeValueDF], axis = 0, ignore_index = True)
         else : # clean data with no missing and special values
             completeBinningTable = finishBinningTable
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `MOBPY-1.0.0/src/MOBPY/numeric/Monotone.py` & `MOBPY-1.0.1/src/MOBPY/numeric/Monotone.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #%%
 import pandas as pd
+from typing import Union
 import os
 # os.chdir('/Users/chentahung/Desktop/git/mob-py/src/main/python')
 from MOBPY.numeric.MonotoneNode import MonotoneNode
 
 class Monotone :
     def __init__(self, data, var, response, exclude_value = None, metric = 'mean') :
         '''
@@ -22,59 +23,53 @@
         self._var = var
         self._response = response
         self._metric = metric
         self._exclude_value = exclude_value
             
 
     @property
-    def data(self) :
+    def data(self) -> pd.DataFrame:
         return self._data
     
     @property
-    def var(self) :
+    def var(self) -> str :
         return self._var
     
     @property
-    def response(self) :
+    def response(self) -> str :
         return self._response
 
     @property
-    def metric(self) :
+    def metric(self) -> str :
         return self._metric
     
     @property
-    def exclude_value(self) :
+    def exclude_value(self) -> Union[list, int, float, None]:
         return self._exclude_value
     
     def __selectSign(self) -> str:
         '''
         decide `sign` argument
         '''
         if self.data[[self.var, self.response]].corr().iloc[1,0] > 0 :
             sign = '+'
         else :
             sign = '-'
         
         return sign
     
-    def __initMonoTable(self) :
+    def __initMonoTable(self) -> pd.DataFrame:
         '''
         initialize sorted table to check constraints or reverse trend on metric
         '''
         df = self.data.copy()
-        # count = Total
-        # sum = Bad
-        if df[self.var].isna().sum() == 0 and self.exclude_value == None : # no missing values and no exclude_value specified
-            return df.groupby(self.var)[self.response].agg(['count', 'sum', 'std']).reset_index().fillna(0)
-        elif df[self.var].isna().sum() != 0 and self.exclude_value == None :
-            return df[df[self.var].notnull()].groupby(self.var)[self.response].agg(['count', 'sum', 'std']).reset_index().fillna(0)
-        elif df[self.var].isna().sum() == 0 and self.exclude_value != None :
-            return df[df[self.var] != self.exclude_value].groupby(self.var)[self.response].agg(['count', 'sum', 'std']).reset_index().fillna(0)
-        
-    def tuneMonotone(self, initialization : bool = True, sign = 'auto'):
+
+        return df.groupby(self.var)[self.response].agg(['count', 'sum', 'std']).reset_index().fillna(0)
+    
+    def tuneMonotone(self, initialization : bool = True, sign = 'auto') -> pd.DataFrame:
         if sign == 'auto' :
             sign = self.__selectSign()
         else :
             sign = sign
 
         if initialization :
             df = self.__initMonoTable()
@@ -119,15 +114,15 @@
                     cur.pre.update(cur.mergeTotal, cur.mergeBad, cur.mergeStd, cur.endValue)
                     cur.pre.next = cur.next
                     if cur.next is not None:
                         cur.next.pre = cur.pre
                     cur = cur.pre
                 cur = cur.next
         else :
-            raise("Invalid sign : <string>  [auto|+|-]")
+            raise("Invalid sign : <string>  {auto,+,-}")
 
         # store result
         cur = root
         startValueList = []
         endValueList = []
         binTotalList = []
         binBadList = []
```

### Comparing `MOBPY-1.0.0/src/MOBPY/numeric/MonotoneNode.py` & `MOBPY-1.0.1/src/MOBPY/numeric/MonotoneNode.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.0.0/src/MOBPY/numeric/OptimalBinning.py` & `MOBPY-1.0.1/src/MOBPY/numeric/OptimalBinning.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.0.0/src/MOBPY/plot/MOB_PLOT.py` & `MOBPY-1.0.1/src/MOBPY/plot/MOB_PLOT.py`

 * *Files identical despite different names*

### Comparing `MOBPY-1.0.0/src/MOBPY.egg-info/PKG-INFO` & `MOBPY-1.0.1/src/MOBPY.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: MOBPY
-Version: 1.0.0
+Version: 1.0.1
 Summary: MOB is a statistical approach to transform continuous variables into optimal and monotonic categorical variables.
 Author-email: "Chen, Ta-Hung" <denny20700@gmail.com>
 Project-URL: Homepage, https://github.com/ChenTaHung/Monotonic-Optimal-Binning
 Project-URL: Bug Tracker, https://github.com/ChenTaHung/Monotonic-Optimal-Binning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1><p align = 'center'><strong> Monotonic-Optimal-Binning</strong> </p></h1>
+<h1><p align = 'center'><strong> Monotonic-Optimal-Binning </strong> </p></h1>
+<h3><p align = 'center'><strong> Python implementation (MOBPY) </strong> </p></h3>
 
-**MOB** is a statistical approach to transform continuous variables into optimal and monotonic categorical variables. In this proejct, we extend the application so that the user can choose whether merge the bins under a `statistics` base or a `bins size` base to obtain the optimal result based on the users' expectation.<br>
+[**MOB**](https://pypi.org/project/MOBPY/) is a statistical approach to transform continuous variables into optimal and monotonic categorical variables. In this project, we have expanded the application to allow the users to merge the bins based on `statistics` or `bin size`. This is a Python-based project that enables the users to achieve monotone optimal binning results aligned with their expectations.<br>
 
 <h2><strong> Installation </strong></h2>
 
 ```bash
 python3 -m pip install MOBPY
 ```
 
 <h2><strong> Usage </strong></h2>
 
 
-<h3><span style = 'font-size:larger'> Example :</span></h3>
+**_Example_**:
 
 ```python
 import pandas as pd
 from MOBPY.MOB import MOB
 
 
 if __name__ == '__main__' :
@@ -53,35 +54,44 @@
     StatsBinning = MOB_ALGO.runMOB(mergeMethod='Stats') # Run under the statistical base. 
     
 ```
 
 
 The `runMOB` method will return a `pandas.DataFrame` which shows the binning result of the variable and also the WoE summary information for each bin. 
 
-<p align = 'center'><img src = 'doc/images/Durationinmonth%20bins%20summary.png' alt = 'Image' style = 'width: 1200px'/></p>
+<p align = 'center'><img src = 'https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/images/Durationinmonth%20bins%20summary.png' alt = 'Image' style = 'width: 800px'/></p>
 
 And after we receive the binning result dataframe, we can plot it by using `MOBPY.plot.MOB_PLOT.plotBinsSummary` to visualize the binning summary result.
 
 ```python
 from MOBPY.plot.MOB_PLOT import MOB_PLOT
 
 # plot the bin summary data.
 print('Bins Size Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = SizeBinning, var_name = 'Durationinmonth')
 
 print('Statisitcal Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = StatsBinning, var_name = 'Durationinmonth')
 ```
 
-<p align = 'center'><img src = 'doc/charts/Durationinmonth-Size.png' alt = 'Image' style = 'width: 1200px'/></p>
+<p align = 'center'><img src = 'https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Durationinmonth-Size.png' alt = 'Image' style = 'width: 1200px'/></p>
 
 
+<h2> <strong> Highlighted Features </strong></h2>
 
+**_User Preferences_**:
 
-Normally, the result of `Stats` (statistical base) and `Size` (bins size base) will be identical, but when the data appears to be quite extreme in the binning process, the `Size` method will prefer to make the population of each bin between the maximum and minimum limitation, while the `Stats` method will remain to conduct the algorithm through a stricter logic based on the testing hypothesis results.
+The MOB algorithm offers two user preference settings (**`mergeMethod`** argument):
+
+1. `Size`: This setting allows you to optimize the sample size of each bin within specified maximum and minimum limits while ensuring that the minimum number of bins constraint is maintained.
+
+2. `Stats`: With this setting, the algorithm applies a stricter approach based on hypothesis testing results.<br>
+
+
+Typically, the `'Stats'` (statistical-based) and `'Size'` (bin size-based) methods yield identical results. However, when dealing with data under certain scenarios where the `'Size'` method, employed by **MOB**, tends to prioritize maintaining the population of each bin within the maximum and minimum limits. In contrast, the `'Stats'` method adheres to a more rigorous logic based on the results of hypothesis testing.
 
 For example, 
 
 ```python
 # run the MOB algorithm to discretize the variable 'Creditamount'.
 MOB_ALGO = MOB(data = df, var = 'Creditamount', response = 'default', exclude_value = None) 
 # Set Binning Constraints (Must-Do!)
@@ -97,66 +107,67 @@
 # plot the bin summary data.
 print('Bins Size Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = SizeBinning, var_name = 'Durationinmonth')
 print('Statisitcal Base')
 MOB_PLOT.plotBinsSummary(monoOptBinTable = StatsBinning, var_name = 'Durationinmonth')
 ```
 
-<div style="width: 100%;">
-  <table style="width: 100%;">
+<div>
+  <table >
     <thead>
       <tr>
         <th style="text-align: center;">SizeBinning</th>
         <th style="text-align: center;">StatsBinning</th>
       </tr>
     </thead>
     <tbody>
       <tr>
-        <td style="text-align: center;">mergeMethod = 'Size' (bins size base)</td>
-        <td style="text-align: center;">mergeMethod = 'Stats' (statistical base)</td>
+        <td style="text-align: center;">runMOB(mergeMethod='Size') (bins size base)</td>
+        <td style="text-align: center;">runMOB(mergeMethod='Stats') (statistical base)</td>
+      </tr>
+      <tr>
+        <td>
+            <img src="https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Creditamount-Size.png" width="400" >
+        </td>
+        <td>
+           <img src="https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/charts/Creditamount-Stats.png" width="400">
+        </td>
       </tr>
     </tbody>
   </table>
-
-  <div style="display: flex; justify-content: center;">
-    <img src="doc/charts/Creditamount-Size.png" alt="Image 1" style="width: 50%;" />
-    <img src="doc/charts/Creditamount-Stats.png" alt="Image 2" style="width: 50%;" />
-  </div>
 </div>
-<br>
 
-The left side image is the result generated by **`mergeMethod = 'Size'`** (bins size base), and the right side is the result generated by **`mergeMethod = 'Stats'`** (statistical base).We can see that the **Size method** merge the bins that do not meet the minimum sample population and maintain the bins number in order to prevent from exceeding the minimum bins limitation.<br><br>
+The left side image is the result generated by **`mergeMethod = 'Size'`** (bin size-based), and the right side is the result generated by **`mergeMethod = 'Stats'`** (statistical-based). We can see that the `'Size'` method is designed to merge bins that fail to meet the minimum sample population requirement. This approach ensures that the number of bins remains within the specified limit, preventing it from exceeding the minimum bin limitation. By merging bins that fall short of the population threshold, the `'Size'` method effectively maintains a balanced distribution of data across the bins..<br><br>
 
 
+<h2><strong> Full Documentation </strong></h2>
+
+↪ [Full API Reference](https://github.com/ChenTaHung/Monotonic-Optimal-Binning/blob/main/doc/MOBPY-API-Ref.md)<br><br>
 
 <h2> <strong> Environment </strong></h2>
 
 ```bash
 OS : macOS Ventura
 
 IDE: Visual Studio Code 1.79.2 (Universal)
 
 Language : Python 3.9.7 
     - pandas 1.3.4
     - numpy 1.20.3
     - scipy 1.7.1
     - matplotlib 3.7.1
 ```
-<br>
-
-<h2><strong> Citation </strong></h2>
-
-- [Mironchyk, Pavel, and Viktor Tchistiakov. "Monotone optimal binning algorithm for credit risk modeling." Utr. Work. Pap (2017).](https://www.researchgate.net/profile/Viktor-Tchistiakov/publication/322520135_Monotone_optimal_binning_algorithm_for_credit_risk_modeling/links/5a5dd1a8458515c03edf9a97/Monotone-optimal-binning-algorithm-for-credit-risk-modeling.pdf)
-
 
 
 <h2><strong> Reference </strong></h2>
 
 - Testing Dataset : [German Credit Risk](https://www.kaggle.com/datasets/uciml/german-credit) from [Kaggle](https://www.kaggle.com/)
 
+- [Mironchyk, Pavel, and Viktor Tchistiakov. "Monotone optimal binning algorithm for credit risk modeling." Utr. Work. Pap (2017).](https://www.researchgate.net/profile/Viktor-Tchistiakov/publication/322520135_Monotone_optimal_binning_algorithm_for_credit_risk_modeling/links/5a5dd1a8458515c03edf9a97/Monotone-optimal-binning-algorithm-for-credit-risk-modeling.pdf)
+
 - GitHub Project : [Monotone Optimal Binning (SAS 9.4 version)](https://github.com/cdfq384903/MonotonicOptimalBinning)
 
 <h2><strong> Authors </strong></h2>
 
 
 1. Chen, Ta-Hung (Denny) <br>
     - LinkedIn Profile : https://www.linkedin.com/in/dennychen-tahung/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

