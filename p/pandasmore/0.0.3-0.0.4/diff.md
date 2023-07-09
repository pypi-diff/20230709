# Comparing `tmp/pandasmore-0.0.3.tar.gz` & `tmp/pandasmore-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasmore-0.0.3.tar", last modified: Sun Jun 25 13:22:18 2023, max compression
+gzip compressed data, was "pandasmore-0.0.4.tar", last modified: Sun Jul  9 14:43:27 2023, max compression
```

## Comparing `pandasmore-0.0.3.tar` & `pandasmore-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.673146 pandasmore-0.0.3/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.665146 pandasmore-0.0.3/.github/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/.github/workflows/
--rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 pandasmore-0.0.3/.github/workflows/deploy.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 pandasmore-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-04-27 10:12:58.000000 pandasmore-0.0.3/.gitignore
--rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 pandasmore-0.0.3/LICENSE
--rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 pandasmore-0.0.3/MANIFEST.in
--rw-rw-r--   0 imb       (1000) imb       (1000)     4779 2023-06-25 13:22:18.669146 pandasmore-0.0.3/PKG-INFO
--rw-rw-r--   0 imb       (1000) imb       (1000)     3958 2023-06-25 13:21:43.000000 pandasmore-0.0.3/README.md
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/nbs/
--rw-r--r--   0 imb       (1000) imb       (1000)    61779 2023-06-25 12:55:13.000000 pandasmore-0.0.3/nbs/00_core.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-23 19:18:59.000000 pandasmore-0.0.3/nbs/_quarto.yml
--rw-r--r--   0 imb       (1000) imb       (1000)    14681 2023-06-25 13:20:37.000000 pandasmore-0.0.3/nbs/index.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      279 2023-06-25 13:21:39.000000 pandasmore-0.0.3/nbs/nbdev.yml
--rw-rw-r--   0 imb       (1000) imb       (1000)       76 2023-06-24 20:54:34.000000 pandasmore-0.0.3/nbs/sidebar.yml
--rw-r--r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 pandasmore-0.0.3/nbs/styles.css
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/pandasmore/
--rw-r--r--   0 imb       (1000) imb       (1000)       41 2023-06-25 13:21:38.000000 pandasmore-0.0.3/pandasmore/__init__.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     1576 2023-06-25 13:21:38.000000 pandasmore-0.0.3/pandasmore/_modidx.py
--rw-r--r--   0 imb       (1000) imb       (1000)    12540 2023-06-25 13:21:38.000000 pandasmore-0.0.3/pandasmore/core.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:22:18.669146 pandasmore-0.0.3/pandasmore.egg-info/
--rw-r--r--   0 imb       (1000) imb       (1000)     4779 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/PKG-INFO
--rw-r--r--   0 imb       (1000) imb       (1000)      518 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/SOURCES.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/dependency_links.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       42 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/entry_points.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 19:24:31.000000 pandasmore-0.0.3/pandasmore.egg-info/not-zip-safe
--rw-r--r--   0 imb       (1000) imb       (1000)       23 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/requires.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       11 2023-06-25 13:22:18.000000 pandasmore-0.0.3/pandasmore.egg-info/top_level.txt
--rw-r--r--   0 imb       (1000) imb       (1000)      898 2023-06-25 13:21:28.000000 pandasmore-0.0.3/settings.ini
--rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-06-25 13:22:18.673146 pandasmore-0.0.3/setup.cfg
--rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 pandasmore-0.0.3/setup.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-09 14:43:27.909558 pandasmore-0.0.4/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-09 14:43:27.905558 pandasmore-0.0.4/.github/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-09 14:43:27.909558 pandasmore-0.0.4/.github/workflows/
+-rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 pandasmore-0.0.4/.github/workflows/deploy.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 pandasmore-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-07-07 17:20:36.000000 pandasmore-0.0.4/.gitignore
+-rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 pandasmore-0.0.4/LICENSE
+-rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 pandasmore-0.0.4/MANIFEST.in
+-rw-rw-r--   0 imb       (1000) imb       (1000)     4779 2023-07-09 14:43:27.909558 pandasmore-0.0.4/PKG-INFO
+-rw-rw-r--   0 imb       (1000) imb       (1000)     3958 2023-07-07 17:25:02.000000 pandasmore-0.0.4/README.md
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-09 14:43:27.909558 pandasmore-0.0.4/data/
+-rw-rw-r--   0 imb       (1000) imb       (1000)        0 2023-07-09 14:42:17.000000 pandasmore-0.0.4/data/.gitkeep
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-09 14:43:27.909558 pandasmore-0.0.4/nbs/
+-rw-r--r--   0 imb       (1000) imb       (1000)    65360 2023-07-09 14:42:17.000000 pandasmore-0.0.4/nbs/00_core.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-23 19:18:59.000000 pandasmore-0.0.4/nbs/_quarto.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)    14567 2023-07-07 17:23:05.000000 pandasmore-0.0.4/nbs/index.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      279 2023-07-09 14:42:17.000000 pandasmore-0.0.4/nbs/nbdev.yml
+-rw-rw-r--   0 imb       (1000) imb       (1000)       76 2023-06-24 20:54:34.000000 pandasmore-0.0.4/nbs/sidebar.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 pandasmore-0.0.4/nbs/styles.css
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-09 14:43:27.909558 pandasmore-0.0.4/pandasmore/
+-rw-r--r--   0 imb       (1000) imb       (1000)       41 2023-07-09 14:42:17.000000 pandasmore-0.0.4/pandasmore/__init__.py
+-rw-rw-r--   0 imb       (1000) imb       (1000)     1683 2023-07-09 14:42:17.000000 pandasmore-0.0.4/pandasmore/_modidx.py
+-rw-r--r--   0 imb       (1000) imb       (1000)    14200 2023-07-09 14:42:17.000000 pandasmore-0.0.4/pandasmore/core.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-09 14:43:27.909558 pandasmore-0.0.4/pandasmore.egg-info/
+-rw-r--r--   0 imb       (1000) imb       (1000)     4779 2023-07-09 14:43:27.000000 pandasmore-0.0.4/pandasmore.egg-info/PKG-INFO
+-rw-r--r--   0 imb       (1000) imb       (1000)      532 2023-07-09 14:43:27.000000 pandasmore-0.0.4/pandasmore.egg-info/SOURCES.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-07-09 14:43:27.000000 pandasmore-0.0.4/pandasmore.egg-info/dependency_links.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)       42 2023-07-09 14:43:27.000000 pandasmore-0.0.4/pandasmore.egg-info/entry_points.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 19:24:31.000000 pandasmore-0.0.4/pandasmore.egg-info/not-zip-safe
+-rw-r--r--   0 imb       (1000) imb       (1000)       23 2023-07-09 14:43:27.000000 pandasmore-0.0.4/pandasmore.egg-info/requires.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)       11 2023-07-09 14:43:27.000000 pandasmore-0.0.4/pandasmore.egg-info/top_level.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)      898 2023-07-09 14:38:12.000000 pandasmore-0.0.4/settings.ini
+-rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-07-09 14:43:27.909558 pandasmore-0.0.4/setup.cfg
+-rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 pandasmore-0.0.4/setup.py
```

### Comparing `pandasmore-0.0.3/.gitignore` & `pandasmore-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.3/LICENSE` & `pandasmore-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.3/PKG-INFO` & `pandasmore-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmore
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extends pandas with common functions used in finance and economics research
 Home-page: https://github.com/ionmihai/pandasmore
 Author: ionmihai
 Author-email: mihaiion@email.arizona.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmore-0.0.3/README.md` & `pandasmore-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.3/nbs/00_core.ipynb` & `pandasmore-0.0.4/nbs/00_core.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849480293134364%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(3, 'import os, glob \\n')]}}, 6: {'outputs': {0: {'data': "*

 * *            "{'text/html': {insert: [(29, '      <td>0.297133</td>\\n'), (30, '      "*

 * *            "<td>0.408554</td>\\n'), (36, '      <td>0.564141</td>\\n'), (37, '      "*

 * *            "<td>0.565167</td>\\n'), (43, '      <td>0.915189</td>\\n'), (44, '      "*

 * *            "<td>0.950576</td>\\n'), (50, '      <td>0.119610</td>\\n'), (51, '      "*

 * *            "<td>0.189224</td>\\n'), (57, '      <td>0.461875</td […]*

```diff
@@ -42,14 +42,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#|exports\n",
                 "from __future__ import annotations\n",
                 "from typing import List, Callable \n",
+                "import os, glob \n",
                 "import pandas as pd\n",
                 "import numpy as np"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -91,136 +92,136 @@
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.023895</td>\n",
-                            "      <td>0.144473</td>\n",
+                            "      <td>0.297133</td>\n",
+                            "      <td>0.408554</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.408212</td>\n",
-                            "      <td>0.184723</td>\n",
+                            "      <td>0.915189</td>\n",
+                            "      <td>0.950576</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.584678</td>\n",
-                            "      <td>0.432209</td>\n",
+                            "      <td>0.930075</td>\n",
+                            "      <td>0.628481</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.171717</td>\n",
-                            "      <td>0.017650</td>\n",
+                            "      <td>0.072018</td>\n",
+                            "      <td>0.343373</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.619073</td>\n",
-                            "      <td>0.220823</td>\n",
+                            "      <td>0.418783</td>\n",
+                            "      <td>0.383560</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.455055</td>\n",
-                            "      <td>0.675069</td>\n",
+                            "      <td>0.372503</td>\n",
+                            "      <td>0.528721</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
                             "      <td>2.0</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.194823</td>\n",
-                            "      <td>0.765347</td>\n",
+                            "      <td>0.098657</td>\n",
+                            "      <td>0.231477</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.126668</td>\n",
-                            "      <td>0.165793</td>\n",
+                            "      <td>0.202530</td>\n",
+                            "      <td>0.051602</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>11</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.112679</td>\n",
-                            "      <td>0.955364</td>\n",
+                            "      <td>0.748226</td>\n",
+                            "      <td>0.235425</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>12</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.489733</td>\n",
-                            "      <td>0.119378</td>\n",
+                            "      <td>0.039119</td>\n",
+                            "      <td>0.098717</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>13</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.661579</td>\n",
-                            "      <td>0.934074</td>\n",
+                            "      <td>0.263658</td>\n",
+                            "      <td>0.428772</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>14</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.477654</td>\n",
-                            "      <td>0.282844</td>\n",
+                            "      <td>0.912622</td>\n",
+                            "      <td>0.795038</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "    permno     date         A         B\n",
-                            "0      1.0      NaN  0.023895  0.144473\n",
-                            "1      1.0  2010-01  0.197353  0.724926\n",
-                            "2      1.0  2010-02  0.408212  0.184723\n",
-                            "3      1.0  2010-02  0.000676  0.062295\n",
-                            "4      1.0  2010-04  0.421966  0.193566\n",
-                            "5      2.0      NaN  0.584678  0.432209\n",
-                            "6      2.0  2010-01  0.171717  0.017650\n",
-                            "7      2.0  2010-02  0.619073  0.220823\n",
-                            "8      2.0  2010-02  0.455055  0.675069\n",
-                            "9      2.0  2010-04  0.194823  0.765347\n",
-                            "10     NaN      NaN  0.126668  0.165793\n",
-                            "11     NaN  2010-01  0.112679  0.955364\n",
-                            "12     NaN  2010-02  0.489733  0.119378\n",
-                            "13     NaN  2010-02  0.661579  0.934074\n",
-                            "14     NaN  2010-04  0.477654  0.282844"
+                            "0      1.0      NaN  0.297133  0.408554\n",
+                            "1      1.0  2010-01  0.564141  0.565167\n",
+                            "2      1.0  2010-02  0.915189  0.950576\n",
+                            "3      1.0  2010-02  0.119610  0.189224\n",
+                            "4      1.0  2010-04  0.461875  0.217378\n",
+                            "5      2.0      NaN  0.930075  0.628481\n",
+                            "6      2.0  2010-01  0.072018  0.343373\n",
+                            "7      2.0  2010-02  0.418783  0.383560\n",
+                            "8      2.0  2010-02  0.372503  0.528721\n",
+                            "9      2.0  2010-04  0.098657  0.231477\n",
+                            "10     NaN      NaN  0.202530  0.051602\n",
+                            "11     NaN  2010-01  0.748226  0.235425\n",
+                            "12     NaN  2010-02  0.039119  0.098717\n",
+                            "13     NaN  2010-02  0.263658  0.428772\n",
+                            "14     NaN  2010-04  0.912622  0.795038"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -287,58 +288,58 @@
                             "      <th>date</th>\n",
                             "      <th>A</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>0.144473</td>\n",
+                            "      <td>0.408554</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.023895</td>\n",
+                            "      <td>0.297133</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.565167</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.197353</td>\n",
+                            "      <td>0.564141</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>0.184723</td>\n",
+                            "      <td>0.950576</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.408212</td>\n",
+                            "      <td>0.915189</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.189224</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.000676</td>\n",
+                            "      <td>0.119610</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.217378</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.421966</td>\n",
+                            "      <td>0.461875</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "          B  permno     date         A\n",
-                            "0  0.144473     1.0      NaN  0.023895\n",
-                            "1  0.724926     1.0  2010-01  0.197353\n",
-                            "2  0.184723     1.0  2010-02  0.408212\n",
-                            "3  0.062295     1.0  2010-02  0.000676\n",
-                            "4  0.193566     1.0  2010-04  0.421966"
+                            "0  0.408554     1.0      NaN  0.297133\n",
+                            "1  0.565167     1.0  2010-01  0.564141\n",
+                            "2  0.950576     1.0  2010-02  0.915189\n",
+                            "3  0.189224     1.0  2010-02  0.119610\n",
+                            "4  0.217378     1.0  2010-04  0.461875"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -404,64 +405,64 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaT</td>\n",
                             "      <td>NaT</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.023895</td>\n",
-                            "      <td>0.144473</td>\n",
+                            "      <td>0.297133</td>\n",
+                            "      <td>0.408554</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.408212</td>\n",
-                            "      <td>0.184723</td>\n",
+                            "      <td>0.915189</td>\n",
+                            "      <td>0.950576</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "      date     dtdate    Mdate  permno         A         B\n",
-                            "0      NaN        NaT      NaT     1.0  0.023895  0.144473\n",
-                            "1  2010-01 2010-01-01  2010-01     1.0  0.197353  0.724926\n",
-                            "2  2010-02 2010-02-01  2010-02     1.0  0.408212  0.184723\n",
-                            "3  2010-02 2010-02-01  2010-02     1.0  0.000676  0.062295\n",
-                            "4  2010-04 2010-04-01  2010-04     1.0  0.421966  0.193566"
+                            "0      NaN        NaT      NaT     1.0  0.297133  0.408554\n",
+                            "1  2010-01 2010-01-01  2010-01     1.0  0.564141  0.565167\n",
+                            "2  2010-02 2010-02-01  2010-02     1.0  0.915189  0.950576\n",
+                            "3  2010-02 2010-02-01  2010-02     1.0  0.119610  0.189224\n",
+                            "4  2010-04 2010-04-01  2010-04     1.0  0.461875  0.217378"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -475,27 +476,29 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#|export\n",
                 "def setup_tseries(df: pd.Series|pd.DataFrame, # Input DataFrame; a copy is returned\n",
                 "# Params passed to `process_dates`\n",
+                "                dates_processed: bool=False, # If True, assumes dates are already processed with `process_dates`\n",
                 "                time_var: str='date', # This will be the date variable used to generate datetime var `dtdate_var`\n",
                 "                time_var_format: str='%Y-%m-%d', # Format of `time_var`; must be valid pandas `strftime`\n",
                 "                dtdate_var: str='dtdate', # Name of datetime var to be created from `time_var`\n",
                 "                freq: str=None, # Used to create `f'{freq}date'` period date; must be valid pandas offset string\n",
                 "# Params for cleaning dates                \n",
                 "                drop_missing_index_vals: bool=True, # What to do with missing `f'{freq}date'`\n",
                 "                drop_index_duplicates: bool=True, # What to do with duplicates in `f'{freq}date'` values\n",
                 "                duplicates_which_keep: str='last', # If duplicates in index, which to keep; must be 'first', 'last' or `False`\n",
                 "                ) -> pd.DataFrame:\n",
                 "    \"\"\"Applies `process_dates` to `df`; cleans up resulting `f'{freq}date'` period date and sets it as index.\"\"\"\n",
                 "\n",
                 "    if isinstance(df, pd.Series): df = df.to_frame()\n",
-                "    df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)\n",
+                "    if not dates_processed:\n",
+                "        df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)\n",
                 "\n",
                 "    if drop_missing_index_vals:\n",
                 "        df = df.dropna(subset=[time_var])\n",
                 "    df = df.sort_values([dtdate_var])\n",
                 "    if drop_index_duplicates:\n",
                 "        df = df.drop_duplicates(subset=[f'{freq}date'], keep=duplicates_which_keep)\n",
                 "    df = df.set_index([f'{freq}date']) \n",
@@ -535,56 +538,56 @@
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.023895</td>\n",
-                            "      <td>0.144473</td>\n",
+                            "      <td>0.297133</td>\n",
+                            "      <td>0.408554</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-01</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.408212</td>\n",
-                            "      <td>0.184723</td>\n",
+                            "      <td>0.915189</td>\n",
+                            "      <td>0.950576</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-02</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>2010-04</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "   permno     date         A         B\n",
-                            "0     1.0      NaN  0.023895  0.144473\n",
-                            "1     1.0  2010-01  0.197353  0.724926\n",
-                            "2     1.0  2010-02  0.408212  0.184723\n",
-                            "3     1.0  2010-02  0.000676  0.062295\n",
-                            "4     1.0  2010-04  0.421966  0.193566"
+                            "0     1.0      NaN  0.297133  0.408554\n",
+                            "1     1.0  2010-01  0.564141  0.565167\n",
+                            "2     1.0  2010-02  0.915189  0.950576\n",
+                            "3     1.0  2010-02  0.119610  0.189224\n",
+                            "4     1.0  2010-04  0.461875  0.217378"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -635,43 +638,43 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "            date     dtdate  permno         A         B\n",
                             "Mdate                                                  \n",
-                            "2010-01  2010-01 2010-01-01     1.0  0.197353  0.724926\n",
-                            "2010-02  2010-02 2010-02-01     1.0  0.000676  0.062295\n",
-                            "2010-04  2010-04 2010-04-01     1.0  0.421966  0.193566"
+                            "2010-01  2010-01 2010-01-01     1.0  0.564141  0.565167\n",
+                            "2010-02  2010-02 2010-02-01     1.0  0.119610  0.189224\n",
+                            "2010-04  2010-04 2010-04-01     1.0  0.461875  0.217378"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -688,27 +691,29 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "#|export\n",
                 "def setup_panel(df: pd.DataFrame, # Input DataFrame; a copy is returned\n",
                 "                panel_ids :str=None, # Name of variable that identifies panel entities\n",
                 "# Params passed to `process_dates`\n",
+                "                dates_processed: bool=False, # If True, assumes dates are already processed with `process_dates`\n",
                 "                time_var: str='date', # This will be the date variable used to generate datetime var `dtdate_var`\n",
                 "                time_var_format: str='%Y-%m-%d', # Format of `time_var`; must be valid pandas `strftime`\n",
                 "                dtdate_var: str='dtdate', # Name of datetime var to be created from `time_var`\n",
                 "                freq: str=None, # Used to create `f'{freq}date'` period date; must be valid pandas offset string\n",
                 "# Params for cleaning panel_ids and dates                \n",
                 "                drop_missing_index_vals: bool=True, # What to do with missing `panel_ids` or `f'{freq}date'`\n",
                 "                panel_ids_toint: str='Int64', # Converts `panel_ids` to int in place; use falsy value if not wanted\n",
                 "                drop_index_duplicates: bool=True, # What to do with duplicates in (`panel_ids`, `f'{freq}date'`) values\n",
                 "                duplicates_which_keep: str='last', # If duplicates in index, which to keep; must be 'first', 'last' or `False`\n",
                 "                ) -> pd.DataFrame:\n",
                 "    \"\"\"Applies `process_dates` to `df`; cleans up (`panel_ids` ,`f'{freq}date'`) and sets it as index.\"\"\"\n",
                 "\n",
-                "    df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)\n",
+                "    if not dates_processed:\n",
+                "        df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)\n",
                 "    if drop_missing_index_vals:\n",
                 "        df = df.dropna(subset=[panel_ids,time_var])\n",
                 "    if panel_ids_toint:\n",
                 "        df[panel_ids] = df[panel_ids].astype('Int64')\n",
                 "    df = df.sort_values([panel_ids, dtdate_var])\n",
                 "    if drop_index_duplicates:\n",
                 "        df = df.drop_duplicates(subset=[panel_ids, f'{freq}date'], keep=duplicates_which_keep)\n",
@@ -759,66 +764,66 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">1</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">2</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.171717</td>\n",
-                            "      <td>0.017650</td>\n",
+                            "      <td>0.072018</td>\n",
+                            "      <td>0.343373</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.455055</td>\n",
-                            "      <td>0.675069</td>\n",
+                            "      <td>0.372503</td>\n",
+                            "      <td>0.528721</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.194823</td>\n",
-                            "      <td>0.765347</td>\n",
+                            "      <td>0.098657</td>\n",
+                            "      <td>0.231477</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                   date     dtdate         A         B\n",
                             "permno Mdate                                          \n",
-                            "1      2010-01  2010-01 2010-01-01  0.197353  0.724926\n",
-                            "       2010-02  2010-02 2010-02-01  0.000676  0.062295\n",
-                            "       2010-04  2010-04 2010-04-01  0.421966  0.193566\n",
-                            "2      2010-01  2010-01 2010-01-01  0.171717  0.017650\n",
-                            "       2010-02  2010-02 2010-02-01  0.455055  0.675069\n",
-                            "       2010-04  2010-04 2010-04-01  0.194823  0.765347"
+                            "1      2010-01  2010-01 2010-01-01  0.564141  0.565167\n",
+                            "       2010-02  2010-02 2010-02-01  0.119610  0.189224\n",
+                            "       2010-04  2010-04 2010-04-01  0.461875  0.217378\n",
+                            "2      2010-01  2010-01 2010-01-01  0.072018  0.343373\n",
+                            "       2010-02  2010-02 2010-02-01  0.372503  0.528721\n",
+                            "       2010-04  2010-04 2010-04-01  0.098657  0.231477"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -942,18 +947,18 @@
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "permno  Mdate  \n",
                             "1       2010-01         NaN\n",
-                            "        2010-02    0.197353\n",
+                            "        2010-02    0.564141\n",
                             "        2010-04         NaN\n",
                             "2       2010-01         NaN\n",
-                            "        2010-02    0.171717\n",
+                            "        2010-02    0.072018\n",
                             "        2010-04         NaN\n",
                             "Name: A_lag1, dtype: float64"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -969,18 +974,18 @@
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "permno  Mdate  \n",
                             "1       2010-01         NaN\n",
-                            "        2010-02    0.197353\n",
+                            "        2010-02    0.564141\n",
                             "        2010-04         NaN\n",
                             "2       2010-01         NaN\n",
-                            "        2010-02    0.171717\n",
+                            "        2010-02    0.072018\n",
                             "        2010-04         NaN\n",
                             "Name: A_lag1, dtype: float64"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -1063,56 +1068,56 @@
                             "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">1</th>\n",
                             "      <th>2010-01</th>\n",
-                            "      <td>0.197353</td>\n",
+                            "      <td>0.564141</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.197353</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.564141</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
-                            "      <td>0.421966</td>\n",
+                            "      <td>0.461875</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">2</th>\n",
                             "      <th>2010-01</th>\n",
-                            "      <td>0.171717</td>\n",
+                            "      <td>0.072018</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
-                            "      <td>0.455055</td>\n",
-                            "      <td>0.171717</td>\n",
+                            "      <td>0.372503</td>\n",
+                            "      <td>0.072018</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
-                            "      <td>0.194823</td>\n",
+                            "      <td>0.098657</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                       A    A_lag1\n",
                             "permno Mdate                      \n",
-                            "1      2010-01  0.197353       NaN\n",
-                            "       2010-02  0.000676  0.197353\n",
-                            "       2010-04  0.421966       NaN\n",
-                            "2      2010-01  0.171717       NaN\n",
-                            "       2010-02  0.455055  0.171717\n",
-                            "       2010-04  0.194823       NaN"
+                            "1      2010-01  0.564141       NaN\n",
+                            "       2010-02  0.119610  0.564141\n",
+                            "       2010-04  0.461875       NaN\n",
+                            "2      2010-01  0.072018       NaN\n",
+                            "       2010-02  0.372503  0.072018\n",
+                            "       2010-04  0.098657       NaN"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1171,97 +1176,97 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">1</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.000676</td>\n",
+                            "      <td>0.119610</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.189224</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">2</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.171717</td>\n",
-                            "      <td>0.017650</td>\n",
+                            "      <td>0.072018</td>\n",
+                            "      <td>0.343373</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.455055</td>\n",
+                            "      <td>0.372503</td>\n",
                             "      <td>NaN</td>\n",
-                            "      <td>0.675069</td>\n",
+                            "      <td>0.528721</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.455055</td>\n",
-                            "      <td>0.675069</td>\n",
+                            "      <td>0.372503</td>\n",
+                            "      <td>0.528721</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.194823</td>\n",
-                            "      <td>0.765347</td>\n",
+                            "      <td>0.098657</td>\n",
+                            "      <td>0.231477</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                   date     dtdate         A         B  A_lag3   A_lead1  \\\n",
                             "permno Mdate                                                               \n",
-                            "1      2010-01  2010-01 2010-01-01  0.197353  0.724926     NaN  0.000676   \n",
-                            "       2010-02  2010-02 2010-02-01  0.000676  0.062295     NaN       NaN   \n",
-                            "       2010-04  2010-04 2010-04-01  0.421966  0.193566     NaN       NaN   \n",
-                            "2      2010-01  2010-01 2010-01-01  0.171717  0.017650     NaN  0.455055   \n",
-                            "       2010-02  2010-02 2010-02-01  0.455055  0.675069     NaN       NaN   \n",
-                            "       2010-04  2010-04 2010-04-01  0.194823  0.765347     NaN       NaN   \n",
+                            "1      2010-01  2010-01 2010-01-01  0.564141  0.565167     NaN  0.119610   \n",
+                            "       2010-02  2010-02 2010-02-01  0.119610  0.189224     NaN       NaN   \n",
+                            "       2010-04  2010-04 2010-04-01  0.461875  0.217378     NaN       NaN   \n",
+                            "2      2010-01  2010-01 2010-01-01  0.072018  0.343373     NaN  0.372503   \n",
+                            "       2010-02  2010-02 2010-02-01  0.372503  0.528721     NaN       NaN   \n",
+                            "       2010-04  2010-04 2010-04-01  0.098657  0.231477     NaN       NaN   \n",
                             "\n",
                             "                B_lag3   B_lead1  \n",
                             "permno Mdate                      \n",
-                            "1      2010-01     NaN  0.062295  \n",
+                            "1      2010-01     NaN  0.189224  \n",
                             "       2010-02     NaN       NaN  \n",
                             "       2010-04     NaN       NaN  \n",
-                            "2      2010-01     NaN  0.675069  \n",
+                            "2      2010-01     NaN  0.528721  \n",
                             "       2010-02     NaN       NaN  \n",
                             "       2010-04     NaN       NaN  "
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -1322,90 +1327,90 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">1</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">2</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.171717</td>\n",
-                            "      <td>0.017650</td>\n",
+                            "      <td>0.072018</td>\n",
+                            "      <td>0.343373</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.455055</td>\n",
-                            "      <td>0.675069</td>\n",
+                            "      <td>0.372503</td>\n",
+                            "      <td>0.528721</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.194823</td>\n",
-                            "      <td>0.765347</td>\n",
+                            "      <td>0.098657</td>\n",
+                            "      <td>0.231477</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                   date     dtdate         A         B  A_lg2  A_ld2  B_lg2  \\\n",
                             "permno Mdate                                                                  \n",
-                            "1      2010-01  2010-01 2010-01-01  0.197353  0.724926    NaN    NaN    NaN   \n",
-                            "       2010-02  2010-02 2010-02-01  0.000676  0.062295    NaN    NaN    NaN   \n",
-                            "       2010-04  2010-04 2010-04-01  0.421966  0.193566    NaN    NaN    NaN   \n",
-                            "2      2010-01  2010-01 2010-01-01  0.171717  0.017650    NaN    NaN    NaN   \n",
-                            "       2010-02  2010-02 2010-02-01  0.455055  0.675069    NaN    NaN    NaN   \n",
-                            "       2010-04  2010-04 2010-04-01  0.194823  0.765347    NaN    NaN    NaN   \n",
+                            "1      2010-01  2010-01 2010-01-01  0.564141  0.565167    NaN    NaN    NaN   \n",
+                            "       2010-02  2010-02 2010-02-01  0.119610  0.189224    NaN    NaN    NaN   \n",
+                            "       2010-04  2010-04 2010-04-01  0.461875  0.217378    NaN    NaN    NaN   \n",
+                            "2      2010-01  2010-01 2010-01-01  0.072018  0.343373    NaN    NaN    NaN   \n",
+                            "       2010-02  2010-02 2010-02-01  0.372503  0.528721    NaN    NaN    NaN   \n",
+                            "       2010-04  2010-04 2010-04-01  0.098657  0.231477    NaN    NaN    NaN   \n",
                             "\n",
                             "                B_ld2  \n",
                             "permno Mdate           \n",
                             "1      2010-01    NaN  \n",
                             "       2010-02    NaN  \n",
                             "       2010-04    NaN  \n",
                             "2      2010-01    NaN  \n",
@@ -1456,18 +1461,18 @@
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "permno  Mdate  \n",
                             "1       2010-01         NaN\n",
-                            "        2010-02   -0.996575\n",
+                            "        2010-02   -0.787978\n",
                             "        2010-04         NaN\n",
                             "2       2010-01         NaN\n",
-                            "        2010-02    1.650026\n",
+                            "        2010-02    4.172353\n",
                             "        2010-04         NaN\n",
                             "dtype: float64"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -1495,18 +1500,18 @@
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "permno  Mdate  \n",
                             "1       2010-01         NaN\n",
-                            "        2010-02   -0.196677\n",
+                            "        2010-02   -0.444531\n",
                             "        2010-04         NaN\n",
                             "2       2010-01         NaN\n",
-                            "        2010-02    0.283338\n",
+                            "        2010-02    0.300485\n",
                             "        2010-04         NaN\n",
                             "dtype: float64"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
@@ -1520,20 +1525,21 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#|export\n",
                 "def rrolling(df: pd.Series|pd.DataFrame, # Must have period date Index (if Series) or (panel_id, period_date) Multiindex (if DataFrame) \n",
-                "                        func: str, # Name of any pandas aggregation function (to applied to `df` data within each rolling window\n",
-                "                        window:int=None, # Rolling window length; if None, uses 'expanding' without fixing lags \n",
-                "                        skipna: bool|None=False, # Use None if `func` does not take `skipna` arg.\n",
-                "                        use_fast_lags: bool=True\n",
-                "                        ) -> pd.Series:\n",
-                "    \"\"\"Like `pd.DataFrame.rolling` but using robust `lag`s. Run `df = setup_tseries(df)` or `df = setup_panel(df)` prior to using.\"\"\"\n",
+                "            func: str, # Name of any pandas aggregation function (to applied to `df` data within each rolling window\n",
+                "            window:int=None, # Rolling window length; if None, uses 'expanding' without fixing lags \n",
+                "            skipna: bool|None=False, # Use None if `func` does not take `skipna` arg.\n",
+                "            use_fast_lags: bool=True\n",
+                "            ) -> pd.Series:\n",
+                "    \"\"\"Like `pd.DataFrame.rolling` but using robust `lag`s. \n",
+                "    Run `df = setup_tseries(df)` or `df = setup_panel(df)` prior to using.\"\"\"\n",
                 "\n",
                 "    if isinstance(df,pd.Series): df = df.to_frame()\n",
                 "    if len(df.columns) > 1: raise ValueError(\"`df` must have a single column\")\n",
                 "    varname = df.columns[0]\n",
                 "    out = df.copy()\n",
                 "\n",
                 "    if window:\n",
@@ -1595,72 +1601,72 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">1</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
-                            "      <td>0.197353</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
+                            "      <td>0.564141</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
-                            "      <td>0.099015</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
+                            "      <td>0.341876</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
-                            "      <td>0.421966</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
+                            "      <td>0.461875</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">2</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.171717</td>\n",
-                            "      <td>0.017650</td>\n",
-                            "      <td>0.171717</td>\n",
+                            "      <td>0.072018</td>\n",
+                            "      <td>0.343373</td>\n",
+                            "      <td>0.072018</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.455055</td>\n",
-                            "      <td>0.675069</td>\n",
-                            "      <td>0.313386</td>\n",
+                            "      <td>0.372503</td>\n",
+                            "      <td>0.528721</td>\n",
+                            "      <td>0.222261</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.194823</td>\n",
-                            "      <td>0.765347</td>\n",
-                            "      <td>0.194823</td>\n",
+                            "      <td>0.098657</td>\n",
+                            "      <td>0.231477</td>\n",
+                            "      <td>0.098657</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                   date     dtdate         A         B  rolling_A\n",
                             "permno Mdate                                                     \n",
-                            "1      2010-01  2010-01 2010-01-01  0.197353  0.724926   0.197353\n",
-                            "       2010-02  2010-02 2010-02-01  0.000676  0.062295   0.099015\n",
-                            "       2010-04  2010-04 2010-04-01  0.421966  0.193566   0.421966\n",
-                            "2      2010-01  2010-01 2010-01-01  0.171717  0.017650   0.171717\n",
-                            "       2010-02  2010-02 2010-02-01  0.455055  0.675069   0.313386\n",
-                            "       2010-04  2010-04 2010-04-01  0.194823  0.765347   0.194823"
+                            "1      2010-01  2010-01 2010-01-01  0.564141  0.565167   0.564141\n",
+                            "       2010-02  2010-02 2010-02-01  0.119610  0.189224   0.341876\n",
+                            "       2010-04  2010-04 2010-04-01  0.461875  0.217378   0.461875\n",
+                            "2      2010-01  2010-01 2010-01-01  0.072018  0.343373   0.072018\n",
+                            "       2010-02  2010-02 2010-02-01  0.372503  0.528721   0.222261\n",
+                            "       2010-04  2010-04 2010-04-01  0.098657  0.231477   0.098657"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1713,72 +1719,72 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">1</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.197353</td>\n",
-                            "      <td>0.724926</td>\n",
+                            "      <td>0.564141</td>\n",
+                            "      <td>0.565167</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.000676</td>\n",
-                            "      <td>0.062295</td>\n",
-                            "      <td>0.099015</td>\n",
+                            "      <td>0.119610</td>\n",
+                            "      <td>0.189224</td>\n",
+                            "      <td>0.341876</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.421966</td>\n",
-                            "      <td>0.193566</td>\n",
+                            "      <td>0.461875</td>\n",
+                            "      <td>0.217378</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th rowspan=\"3\" valign=\"top\">2</th>\n",
                             "      <th>2010-01</th>\n",
                             "      <td>2010-01</td>\n",
                             "      <td>2010-01-01</td>\n",
-                            "      <td>0.171717</td>\n",
-                            "      <td>0.017650</td>\n",
+                            "      <td>0.072018</td>\n",
+                            "      <td>0.343373</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-02</th>\n",
                             "      <td>2010-02</td>\n",
                             "      <td>2010-02-01</td>\n",
-                            "      <td>0.455055</td>\n",
-                            "      <td>0.675069</td>\n",
-                            "      <td>0.313386</td>\n",
+                            "      <td>0.372503</td>\n",
+                            "      <td>0.528721</td>\n",
+                            "      <td>0.222261</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2010-04</th>\n",
                             "      <td>2010-04</td>\n",
                             "      <td>2010-04-01</td>\n",
-                            "      <td>0.194823</td>\n",
-                            "      <td>0.765347</td>\n",
+                            "      <td>0.098657</td>\n",
+                            "      <td>0.231477</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                   date     dtdate         A         B  rolling_A\n",
                             "permno Mdate                                                     \n",
-                            "1      2010-01  2010-01 2010-01-01  0.197353  0.724926        NaN\n",
-                            "       2010-02  2010-02 2010-02-01  0.000676  0.062295   0.099015\n",
-                            "       2010-04  2010-04 2010-04-01  0.421966  0.193566        NaN\n",
-                            "2      2010-01  2010-01 2010-01-01  0.171717  0.017650        NaN\n",
-                            "       2010-02  2010-02 2010-02-01  0.455055  0.675069   0.313386\n",
-                            "       2010-04  2010-04 2010-04-01  0.194823  0.765347        NaN"
+                            "1      2010-01  2010-01 2010-01-01  0.564141  0.565167        NaN\n",
+                            "       2010-02  2010-02 2010-02-01  0.119610  0.189224   0.341876\n",
+                            "       2010-04  2010-04 2010-04-01  0.461875  0.217378        NaN\n",
+                            "2      2010-01  2010-01 2010-01-01  0.072018  0.343373        NaN\n",
+                            "       2010-02  2010-02 2010-02-01  0.372503  0.528721   0.222261\n",
+                            "       2010-04  2010-04 2010-04-01  0.098657  0.231477        NaN"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1799,17 +1805,17 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Mdate\n",
-                            "2010-01    0.197353\n",
-                            "2010-02    0.000676\n",
-                            "2010-04    0.421966\n",
+                            "2010-01    0.564141\n",
+                            "2010-02    0.119610\n",
+                            "2010-04    0.461875\n",
                             "Freq: M, Name: A, dtype: float64"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1823,17 +1829,17 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Mdate\n",
-                            "2010-01    0.197353\n",
-                            "2010-02    0.099015\n",
-                            "2010-04    0.421966\n",
+                            "2010-01    0.564141\n",
+                            "2010-02    0.341876\n",
+                            "2010-04    0.461875\n",
                             "Freq: M, dtype: float64"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1890,14 +1896,98 @@
                 "    if divide_by_mean:\n",
                 "        return (df.copy() - df.mean()) / df.mean()\n",
                 "    else:\n",
                 "        return (df.copy() - df.mean()) / df.std()"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Exporting"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#| export\n",
+                "def to_stata(df: pd.DataFrame=None,\n",
+                "             outfile: str=None, # Output file path; must include .dta extension\n",
+                "             obj_drop: bool=False, # Whether to drop all columns of `object` type\n",
+                "             obj_to_str: bool=False, # Whether to convert all columns of `object` type to `string` type\n",
+                "             **to_stata_kwargs # Other kwargs to pass to `pd.to_stata`\n",
+                "             ):\n",
+                "    \"\"\"Writes `df` to stata `outfile` \"\"\"\n",
+                "\n",
+                "    if df.index.equals(pd.RangeIndex(start=0, stop=len(df), step=1)): df = df.copy()\n",
+                "    else: df = df.reset_index().copy()\n",
+                "\n",
+                "    #Deal with `object` and `string` data types\n",
+                "    for v in list(df.columns):\n",
+                "        if df[v].dtype=='string': df[v] = df[v].fillna('').astype(str)\n",
+                "        if df[v].dtype=='object':\n",
+                "            if obj_drop: df = df.drop(v, axis=1)\n",
+                "            elif obj_to_str and df[v].dropna().apply(lambda x: isinstance(x, str)).all():\n",
+                "                df[v] = df[v].fillna('').astype(str)\n",
+                "\n",
+                "    #Deal with time data\n",
+                "    dates_to_td = {}\n",
+                "    for v in list(df.columns):\n",
+                "        if str(df[v].dtype).startswith('period'): df = df.drop(v, axis=1)\n",
+                "        elif df[v].dtype=='datetime64[ns]':\n",
+                "            if df[v].apply(lambda x: x.tz is not None).any(): df = df.drop(v, axis=1)\n",
+                "            else: dates_to_td[v] = 'td'\n",
+                "        pass\n",
+                "    \n",
+                "    df.to_stata(outfile, convert_dates=dates_to_td, write_index=False, **to_stata_kwargs)   "
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Index data is automatically included in the output, unless the index is the default range from 0 to len(df)."
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Columns of `object` data type are by default left to `pd.to_stata` to figure out how to convert. Note that columns of strings with missing data might cause an error in this default case. In this case, the best thing to do is for you convert it to `string` type before calling this function. If not, setting `obj_to_str` to True will deal with this internally but it will be slower.\n",
+                "\n",
+                "For time data, columns of `period` type and columns of `datetime64[ns]` type with time zone information will be dropped. All other `datetime64[ns]` variables will be converted to `td` dates in Stata. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "to_stata(df, outfile='../data/df.dta', version=117)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#| hide \n",
+                "for f in glob.glob('../data/*'): os.remove(f)\n",
+                "with open('../data/.gitkeep', 'w') as f: pass #empty file to force github to track the data folder"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#| hide\n",
                 "import nbdev; nbdev.nbdev_export()"
```

### Comparing `pandasmore-0.0.3/nbs/index.ipynb` & `pandasmore-0.0.4/nbs/index.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {"'cells'": '{delete: [12]}'}*

```diff
@@ -482,21 +482,14 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pdm.lag(df['A'])"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "python3",
             "language": "python",
             "name": "python3"
```

### Comparing `pandasmore-0.0.3/nbs/styles.css` & `pandasmore-0.0.4/nbs/styles.css`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.3/pandasmore/_modidx.py` & `pandasmore-0.0.4/pandasmore/_modidx.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,9 @@
                                  'pandasmore.core.order_columns': ('core.html#order_columns', 'pandasmore/core.py'),
                                  'pandasmore.core.process_dates': ('core.html#process_dates', 'pandasmore/core.py'),
                                  'pandasmore.core.rdiff': ('core.html#rdiff', 'pandasmore/core.py'),
                                  'pandasmore.core.rpct_change': ('core.html#rpct_change', 'pandasmore/core.py'),
                                  'pandasmore.core.rrolling': ('core.html#rrolling', 'pandasmore/core.py'),
                                  'pandasmore.core.setup_panel': ('core.html#setup_panel', 'pandasmore/core.py'),
                                  'pandasmore.core.setup_tseries': ('core.html#setup_tseries', 'pandasmore/core.py'),
+                                 'pandasmore.core.to_stata': ('core.html#to_stata', 'pandasmore/core.py'),
                                  'pandasmore.core.wins': ('core.html#wins', 'pandasmore/core.py')}}}
```

### Comparing `pandasmore-0.0.3/pandasmore/core.py` & `pandasmore-0.0.4/pandasmore/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% ../nbs/00_core.ipynb 4
 from __future__ import annotations
 from typing import List, Callable 
+import os, glob 
 import pandas as pd
 import numpy as np
 
 # %% auto 0
 __all__ = ['order_columns', 'process_dates', 'setup_tseries', 'setup_panel', 'fast_lag', 'lag', 'add_lags', 'rpct_change',
-           'rdiff', 'rrolling', 'wins', 'norm']
+           'rdiff', 'rrolling', 'wins', 'norm', 'to_stata']
 
 # %% ../nbs/00_core.ipynb 8
 def order_columns(df: pd.DataFrame, these_first: List[str]) -> pd.DataFrame:
     """Returns `df` with reordered columns. Use as `df = order_columns(df,_)`"""
     
     remaining = [x for x in df.columns if x not in these_first]
     return df[these_first + remaining]
@@ -30,53 +31,57 @@
     df[dtdate_var] = pd.to_datetime(df[time_var], format=time_var_format)
     df[f'{freq}date'] = df['dtdate'].dt.to_period(freq)
     return order_columns(df, [time_var,dtdate_var,f'{freq}date'])
 
 # %% ../nbs/00_core.ipynb 12
 def setup_tseries(df: pd.Series|pd.DataFrame, # Input DataFrame; a copy is returned
 # Params passed to `process_dates`
+                dates_processed: bool=False, # If True, assumes dates are already processed with `process_dates`
                 time_var: str='date', # This will be the date variable used to generate datetime var `dtdate_var`
                 time_var_format: str='%Y-%m-%d', # Format of `time_var`; must be valid pandas `strftime`
                 dtdate_var: str='dtdate', # Name of datetime var to be created from `time_var`
                 freq: str=None, # Used to create `f'{freq}date'` period date; must be valid pandas offset string
 # Params for cleaning dates                
                 drop_missing_index_vals: bool=True, # What to do with missing `f'{freq}date'`
                 drop_index_duplicates: bool=True, # What to do with duplicates in `f'{freq}date'` values
                 duplicates_which_keep: str='last', # If duplicates in index, which to keep; must be 'first', 'last' or `False`
                 ) -> pd.DataFrame:
     """Applies `process_dates` to `df`; cleans up resulting `f'{freq}date'` period date and sets it as index."""
 
     if isinstance(df, pd.Series): df = df.to_frame()
-    df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)
+    if not dates_processed:
+        df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)
 
     if drop_missing_index_vals:
         df = df.dropna(subset=[time_var])
     df = df.sort_values([dtdate_var])
     if drop_index_duplicates:
         df = df.drop_duplicates(subset=[f'{freq}date'], keep=duplicates_which_keep)
     df = df.set_index([f'{freq}date']) 
     return order_columns(df,[time_var,dtdate_var]) 
 
 # %% ../nbs/00_core.ipynb 15
 def setup_panel(df: pd.DataFrame, # Input DataFrame; a copy is returned
                 panel_ids :str=None, # Name of variable that identifies panel entities
 # Params passed to `process_dates`
+                dates_processed: bool=False, # If True, assumes dates are already processed with `process_dates`
                 time_var: str='date', # This will be the date variable used to generate datetime var `dtdate_var`
                 time_var_format: str='%Y-%m-%d', # Format of `time_var`; must be valid pandas `strftime`
                 dtdate_var: str='dtdate', # Name of datetime var to be created from `time_var`
                 freq: str=None, # Used to create `f'{freq}date'` period date; must be valid pandas offset string
 # Params for cleaning panel_ids and dates                
                 drop_missing_index_vals: bool=True, # What to do with missing `panel_ids` or `f'{freq}date'`
                 panel_ids_toint: str='Int64', # Converts `panel_ids` to int in place; use falsy value if not wanted
                 drop_index_duplicates: bool=True, # What to do with duplicates in (`panel_ids`, `f'{freq}date'`) values
                 duplicates_which_keep: str='last', # If duplicates in index, which to keep; must be 'first', 'last' or `False`
                 ) -> pd.DataFrame:
     """Applies `process_dates` to `df`; cleans up (`panel_ids` ,`f'{freq}date'`) and sets it as index."""
 
-    df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)
+    if not dates_processed:
+        df = process_dates(df, time_var=time_var, time_var_format=time_var_format, dtdate_var=dtdate_var, freq=freq)
     if drop_missing_index_vals:
         df = df.dropna(subset=[panel_ids,time_var])
     if panel_ids_toint:
         df[panel_ids] = df[panel_ids].astype('Int64')
     df = df.sort_values([panel_ids, dtdate_var])
     if drop_index_duplicates:
         df = df.drop_duplicates(subset=[panel_ids, f'{freq}date'], keep=duplicates_which_keep)
@@ -176,20 +181,21 @@
 # %% ../nbs/00_core.ipynb 33
 def rdiff(df: pd.Series, n: int=1, use_fast_lags=True):
     """Difference using robust `lag()` or `fast_lag()` function."""
     return df - lag(df, n, use_fast_lags)
 
 # %% ../nbs/00_core.ipynb 35
 def rrolling(df: pd.Series|pd.DataFrame, # Must have period date Index (if Series) or (panel_id, period_date) Multiindex (if DataFrame) 
-                        func: str, # Name of any pandas aggregation function (to applied to `df` data within each rolling window
-                        window:int=None, # Rolling window length; if None, uses 'expanding' without fixing lags 
-                        skipna: bool|None=False, # Use None if `func` does not take `skipna` arg.
-                        use_fast_lags: bool=True
-                        ) -> pd.Series:
-    """Like `pd.DataFrame.rolling` but using robust `lag`s. Run `df = setup_tseries(df)` or `df = setup_panel(df)` prior to using."""
+            func: str, # Name of any pandas aggregation function (to applied to `df` data within each rolling window
+            window:int=None, # Rolling window length; if None, uses 'expanding' without fixing lags 
+            skipna: bool|None=False, # Use None if `func` does not take `skipna` arg.
+            use_fast_lags: bool=True
+            ) -> pd.Series:
+    """Like `pd.DataFrame.rolling` but using robust `lag`s. 
+    Run `df = setup_tseries(df)` or `df = setup_panel(df)` prior to using."""
 
     if isinstance(df,pd.Series): df = df.to_frame()
     if len(df.columns) > 1: raise ValueError("`df` must have a single column")
     varname = df.columns[0]
     out = df.copy()
 
     if window:
@@ -230,7 +236,38 @@
     """Subtract means from all columns of `df` and divide by their std. deviations, unless `divide_by_mean` is True"""
 
     if isinstance(df,pd.Series): df = df.to_frame()
     if divide_by_mean:
         return (df.copy() - df.mean()) / df.mean()
     else:
         return (df.copy() - df.mean()) / df.std()
+
+# %% ../nbs/00_core.ipynb 45
+def to_stata(df: pd.DataFrame=None,
+             outfile: str=None, # Output file path; must include .dta extension
+             obj_drop: bool=False, # Whether to drop all columns of `object` type
+             obj_to_str: bool=False, # Whether to convert all columns of `object` type to `string` type
+             **to_stata_kwargs # Other kwargs to pass to `pd.to_stata`
+             ):
+    """Writes `df` to stata `outfile` """
+
+    if df.index.equals(pd.RangeIndex(start=0, stop=len(df), step=1)): df = df.copy()
+    else: df = df.reset_index().copy()
+
+    #Deal with `object` and `string` data types
+    for v in list(df.columns):
+        if df[v].dtype=='string': df[v] = df[v].fillna('').astype(str)
+        if df[v].dtype=='object':
+            if obj_drop: df = df.drop(v, axis=1)
+            elif obj_to_str and df[v].dropna().apply(lambda x: isinstance(x, str)).all():
+                df[v] = df[v].fillna('').astype(str)
+
+    #Deal with time data
+    dates_to_td = {}
+    for v in list(df.columns):
+        if str(df[v].dtype).startswith('period'): df = df.drop(v, axis=1)
+        elif df[v].dtype=='datetime64[ns]':
+            if df[v].apply(lambda x: x.tz is not None).any(): df = df.drop(v, axis=1)
+            else: dates_to_td[v] = 'td'
+        pass
+    
+    df.to_stata(outfile, convert_dates=dates_to_td, write_index=False, **to_stata_kwargs)
```

### Comparing `pandasmore-0.0.3/pandasmore.egg-info/PKG-INFO` & `pandasmore-0.0.4/pandasmore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmore
-Version: 0.0.3
+Version: 0.0.4
 Summary: Extends pandas with common functions used in finance and economics research
 Home-page: https://github.com/ionmihai/pandasmore
 Author: ionmihai
 Author-email: mihaiion@email.arizona.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmore-0.0.3/pandasmore.egg-info/SOURCES.txt` & `pandasmore-0.0.4/pandasmore.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 .github/workflows/deploy.yaml
 .github/workflows/test.yaml
+data/.gitkeep
 nbs/00_core.ipynb
 nbs/_quarto.yml
 nbs/index.ipynb
 nbs/nbdev.yml
 nbs/sidebar.yml
 nbs/styles.css
 pandasmore/__init__.py
```

### Comparing `pandasmore-0.0.3/settings.ini` & `pandasmore-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pandasmore
 lib_name = pandasmore
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pandasmore
 nbs_path = nbs
 recursive = True
```

### Comparing `pandasmore-0.0.3/setup.py` & `pandasmore-0.0.4/setup.py`

 * *Files identical despite different names*

