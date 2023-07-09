# Comparing `tmp/vina2vi-0.0.5.tar.gz` & `tmp/vina2vi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vina2vi-0.0.5.tar", last modified: Mon Dec  5 04:50:47 2022, max compression
+gzip compressed data, was "vina2vi-0.0.6.tar", last modified: Sun Jul  9 09:24:29 2023, max compression
```

## Comparing `vina2vi-0.0.5.tar` & `vina2vi-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 wucf     (425715701) 290727152        0 2022-12-05 04:50:47.487209 vina2vi-0.0.5/
--rw-r--r--   0 wucf     (425715701) 290727152     1087 2022-09-26 16:49:48.000000 vina2vi-0.0.5/LICENSE
--rw-r--r--   0 wucf     (425715701) 290727152     3939 2022-12-05 04:50:47.486868 vina2vi-0.0.5/PKG-INFO
--rw-r--r--   0 wucf     (425715701) 290727152     3825 2022-12-05 04:48:53.000000 vina2vi-0.0.5/README.md
--rw-r--r--   0 wucf     (425715701) 290727152      279 2022-12-05 04:49:25.000000 vina2vi-0.0.5/pyproject.toml
--rw-r--r--   0 wucf     (425715701) 290727152       38 2022-12-05 04:50:47.487297 vina2vi-0.0.5/setup.cfg
-drwxr-xr-x   0 wucf     (425715701) 290727152        0 2022-12-05 04:50:47.480448 vina2vi-0.0.5/vina2vi/
--rw-r--r--   0 wucf     (425715701) 290727152       44 2022-09-26 16:49:48.000000 vina2vi-0.0.5/vina2vi/__init__.py
-drwxr-xr-x   0 wucf     (425715701) 290727152        0 2022-12-05 04:50:47.485672 vina2vi-0.0.5/vina2vi/metrics/
--rw-r--r--   0 wucf     (425715701) 290727152      420 2022-11-15 04:32:19.000000 vina2vi-0.0.5/vina2vi/metrics/__init__.py
--rw-r--r--   0 wucf     (425715701) 290727152     4205 2022-11-01 06:34:46.000000 vina2vi-0.0.5/vina2vi/metrics/edit_dist.py
--rw-r--r--   0 wucf     (425715701) 290727152     7377 2022-11-01 06:34:46.000000 vina2vi-0.0.5/vina2vi/metrics/tf_edit_dist.py
--rw-r--r--   0 wucf     (425715701) 290727152     1402 2022-11-15 04:32:19.000000 vina2vi-0.0.5/vina2vi/utils.py
-drwxr-xr-x   0 wucf     (425715701) 290727152        0 2022-12-05 04:50:47.482869 vina2vi-0.0.5/vina2vi.egg-info/
--rw-r--r--   0 wucf     (425715701) 290727152     3939 2022-12-05 04:50:47.000000 vina2vi-0.0.5/vina2vi.egg-info/PKG-INFO
--rw-r--r--   0 wucf     (425715701) 290727152      282 2022-12-05 04:50:47.000000 vina2vi-0.0.5/vina2vi.egg-info/SOURCES.txt
--rw-r--r--   0 wucf     (425715701) 290727152        1 2022-12-05 04:50:47.000000 vina2vi-0.0.5/vina2vi.egg-info/dependency_links.txt
--rw-r--r--   0 wucf     (425715701) 290727152        8 2022-12-05 04:50:47.000000 vina2vi-0.0.5/vina2vi.egg-info/top_level.txt
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.803042 vina2vi-0.0.6/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     1087 2022-10-24 16:41:33.000000 vina2vi-0.0.6/LICENSE
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3969 2023-07-09 09:24:29.803042 vina2vi-0.0.6/PKG-INFO
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3842 2023-07-09 09:20:59.000000 vina2vi-0.0.6/README.md
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      375 2023-07-09 09:24:13.000000 vina2vi-0.0.6/pyproject.toml
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       38 2023-07-09 09:24:29.803042 vina2vi-0.0.6/setup.cfg
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.796375 vina2vi-0.0.6/vina2vi/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       43 2023-01-22 16:43:46.000000 vina2vi-0.0.6/vina2vi/__init__.py
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.803042 vina2vi-0.0.6/vina2vi/metrics/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      483 2023-07-09 09:20:59.000000 vina2vi-0.0.6/vina2vi/metrics/__init__.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     4992 2023-01-22 16:43:46.000000 vina2vi-0.0.6/vina2vi/metrics/edit_dist.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     1070 2023-07-09 09:20:59.000000 vina2vi-0.0.6/vina2vi/metrics/levenshtein.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     7073 2023-01-22 16:43:46.000000 vina2vi-0.0.6/vina2vi/metrics/tf_edit_dist.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)    11270 2023-07-09 09:21:17.000000 vina2vi-0.0.6/vina2vi/util.py
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.799709 vina2vi-0.0.6/vina2vi.egg-info/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3969 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/PKG-INFO
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      312 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/SOURCES.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)        1 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/dependency_links.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)        8 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/top_level.txt
```

### Comparing `vina2vi-0.0.5/LICENSE` & `vina2vi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.5/PKG-INFO` & `vina2vi-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: vina2vi
-Version: 0.0.5
+Version: 0.0.6
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vina2vi
 `vina2vi` stands for _**Vi**etnamese **n**o **a**ccent **to** **Vi**etnamese_,  
 which is a Python package aiming at helping foreigners **decrypt** messages
 in Vietnamese.  
 (More precisely, foreigners who already know the basics of the language.)
 
-Among other things, this Python package tries to
-- Restore Vietnamese diacrytics
+Among other things, this Python package aims to
+- Restore Vietnamese diacritics
 - Translate acronyms, **đổi vần**, etc.
+- Spell correction
 
 
 ## Installation
 Run the following to install:
 
 ```bash
 pip install vina2vi
@@ -40,15 +42,15 @@
   then `is_foreign` returns `True`
 - If the string consists exclusively of characters of modern Vietnamese alphabets,
   then `is_foreign` returns `False`
     - Languages whose alphabets are a subset of Vietnamese's are thus considered as Vietnamese
     - Currently, we do not consider chữ Nôm as Vietnamese; maybe we will in the future
 
 ```python
-In [1]: from vina2vi.utils import Vietnamese
+In [1]: from vina2vi.util import Vietnamese
 
 In [2]: Vietnamese.is_foreign("Российская Федерация\tRossiyskaya Federatsiya")
 Out[2]: True
 
 In [3]: Vietnamese.is_foreign("\n\tRossiyskaya Federatsiya")
 Out[3]: False
```

### Comparing `vina2vi-0.0.5/README.md` & `vina2vi-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # vina2vi
 `vina2vi` stands for _**Vi**etnamese **n**o **a**ccent **to** **Vi**etnamese_,  
 which is a Python package aiming at helping foreigners **decrypt** messages
 in Vietnamese.  
 (More precisely, foreigners who already know the basics of the language.)
 
-Among other things, this Python package tries to
-- Restore Vietnamese diacrytics
+Among other things, this Python package aims to
+- Restore Vietnamese diacritics
 - Translate acronyms, **đổi vần**, etc.
+- Spell correction
 
 
 ## Installation
 Run the following to install:
 
 ```bash
 pip install vina2vi
@@ -34,15 +35,15 @@
   then `is_foreign` returns `True`
 - If the string consists exclusively of characters of modern Vietnamese alphabets,
   then `is_foreign` returns `False`
     - Languages whose alphabets are a subset of Vietnamese's are thus considered as Vietnamese
     - Currently, we do not consider chữ Nôm as Vietnamese; maybe we will in the future
 
 ```python
-In [1]: from vina2vi.utils import Vietnamese
+In [1]: from vina2vi.util import Vietnamese
 
 In [2]: Vietnamese.is_foreign("Российская Федерация\tRossiyskaya Federatsiya")
 Out[2]: True
 
 In [3]: Vietnamese.is_foreign("\n\tRossiyskaya Federatsiya")
 Out[3]: False
```

### Comparing `vina2vi-0.0.5/vina2vi/metrics/tf_edit_dist.py` & `vina2vi-0.0.6/vina2vi/metrics/tf_edit_dist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-source_batch = <tf.Tensor 'source_batch:0' shape=(None,) dtype=string>
+pred_batch = <tf.Tensor 'pred_batch:0' shape=(None,) dtype=string>
 sim = <tf.Tensor 'while/StatefulPartitionedCall:0' shape=<unknown> dtype=float32>
-source_batch[i] = <tf.Tensor 'while/strided_slice_3:0' shape=() dtype=string>
+pred_batch[i] = <tf.Tensor 'while/strided_slice_3:0' shape=() dtype=string>
 
 """
 
 import tensorflow as tf
 import tensorflow_text as tf_text
 
 
@@ -15,40 +15,40 @@
     tf.TensorSpec([None], tf.int32),
     tf.TensorSpec([None], tf.int32),
     tf.TensorSpec(None, tf.int32),
     tf.TensorSpec(None, tf.int32),
     tf.TensorSpec(None, tf.int32),
 ])
 def tf_codepoint_lev(
-        source,
-        target,
-        delete=tf.constant(1),
-        insert=tf.constant(1),
-        substitute=tf.constant(2),
-    ):
+    pred,
+    gt,
+    delete=tf.constant(1),
+    insert=tf.constant(1),
+    substitute=tf.constant(2),
+):
     """
-    source, target: an array of codepoints
+    pred, gt: an array of codepoints
     """
-    m = tf.shape(source)[0]
-    n = tf.shape(target)[0]
+    m = tf.shape(pred)[0]
+    n = tf.shape(gt)[0]
     distance_matrix[:m+1, :n+1].assign(tf.zeros([m+1, n+1], tf.int32))
 
     start = delete
     delta = delete
     limit = (m+1) * delete
     distance_matrix[1:m+1, 0].assign(tf.range(start, limit, delta))
 
     start = insert
     step = insert
     limit = (n+1) * insert
     distance_matrix[0, 1:n+1].assign(tf.range(start, limit, delta))
 
     for i in tf.range(1, m+1):
         for j in tf.range(1, n+1):
-            cond = source[i-1] == target[j-1]
+            cond = pred[i-1] == gt[j-1]
             candidates = [
                 distance_matrix[i-1, j-1] + tf.cond(
                     cond,
                     lambda: tf.constant(0),
                     lambda: substitute,
                 ),
                 distance_matrix[i-1, j] + delete,
@@ -73,27 +73,27 @@
     tf.TensorSpec([], tf.string),
     tf.TensorSpec([], tf.string),
     tf.TensorSpec(None, tf.int32),
     tf.TensorSpec(None, tf.int32),
     tf.TensorSpec(None, tf.int32),
 ])
 def tf_byte_lev(
-        source,
-        target,
-        delete=tf.constant(1),
-        insert=tf.constant(1),
-        substitute=tf.constant(2),
-    ):
-    source = tf_text.normalize_utf8(source, "NFKD")
-    target = tf_text.normalize_utf8(target, "NFKD")
-    source = tf.strings.unicode_decode(source, "UTF-8")
-    target = tf.strings.unicode_decode(target, "UTF-8")
+    pred,
+    gt,
+    delete=tf.constant(1),
+    insert=tf.constant(1),
+    substitute=tf.constant(2),
+):
+    pred = tf_text.normalize_utf8(pred, "NFKD")
+    gt = tf_text.normalize_utf8(gt, "NFKD")
+    pred = tf.strings.unicode_decode(pred, "UTF-8")
+    gt = tf.strings.unicode_decode(gt, "UTF-8")
     return tf_codepoint_lev(
-                source,
-                target,
+                pred,
+                gt,
                 delete,
                 insert,
                 substitute,
             )
 
 
 @tf.function(
@@ -102,26 +102,26 @@
         tf.TensorSpec([None], tf.string),
         tf.TensorSpec(None, tf.int32),
         tf.TensorSpec(None, tf.int32),
         tf.TensorSpec(None, tf.int32),
     ],
 )
 def tf_batch_lev(
-        source_batch,
-        target_batch,
-        delete=tf.constant(1),
-        insert=tf.constant(1),
-        substitute=tf.constant(2),
-    ):
-    batch_size = tf.shape(source_batch)[0]
+    pred_batch,
+    gt_batch,
+    delete=tf.constant(1),
+    insert=tf.constant(1),
+    substitute=tf.constant(2),
+):
+    batch_size = tf.shape(pred_batch)[0]
     somme = tf.constant(0.)
     for i in tf.range(batch_size):
         dist = tf_byte_lev(
-            source_batch[i],
-            target_batch[i],
+            pred_batch[i],
+            gt_batch[i],
             delete,
             insert,
             substitute,
         )
         somme += tf.cast(dist, tf.float32)
 
     avg = somme / tf.cast(batch_size, tf.float32)
@@ -137,44 +137,44 @@
         tf.TensorSpec(None, tf.int32),
         tf.TensorSpec(None, tf.bool),
         tf.TensorSpec(None, tf.float32),
     ],
     autograph=True,
 )
 def tf_byte_sim(
-        source,
-        target,
-        delete=tf.constant(1),
-        insert=tf.constant(1),
-        substitute=tf.constant(2),
-        proportional=tf.constant(True),
-        alpha=tf.constant(1/3),
-    ):
-    source = tf_text.normalize_utf8(source, "NFKD")
-    target = tf_text.normalize_utf8(target, "NFKD")
-    source = tf.strings.unicode_decode(source, "UTF-8")
-    target = tf.strings.unicode_decode(target, "UTF-8")
+    pred,
+    gt,
+    delete=tf.constant(1),
+    insert=tf.constant(1),
+    substitute=tf.constant(2),
+    proportional=tf.constant(True),
+    alpha=tf.constant(1/3),
+):
+    pred = tf_text.normalize_utf8(pred, "NFKD")
+    gt = tf_text.normalize_utf8(gt, "NFKD")
+    pred = tf.strings.unicode_decode(pred, "UTF-8")
+    gt = tf.strings.unicode_decode(gt, "UTF-8")
 
-    dist = tf_codepoint_lev(source, target, delete,
+    dist = tf_codepoint_lev(pred, gt, delete,
                             insert, substitute)
     dist = tf.cast(dist, tf.float32)
-    len_target = tf.shape(target)[0]
-    len_target = tf.cast(len_target, tf.float32)
+    len_gt = tf.shape(gt)[0]
+    len_gt = tf.cast(len_gt, tf.float32)
     substitute_float32 = tf.cast(substitute, tf.float32)
     if proportional:
         #proportion = dist / (
         #    substitute_float32 * tf.maximum(
         #        tf.constant(1.),
-        #        len_target
+        #        len_gt
         #))
         proportion = tf.math.divide(
             dist,
             substitute_float32 * tf.maximum(
                 tf.constant(1.),
-                len_target
+                len_gt
             )
         )
         #similarity = (
         #    tf.constant(1.)
         #    - tf.minimum(
         #          tf.constant(1.),
         #          proportion
@@ -184,15 +184,15 @@
             tf.constant(1.),
             tf.minimum(
                 tf.constant(1.),
                 proportion
             )
         )
     else:
-        if dist > len_target*substitute_float32:
+        if dist > len_gt*substitute_float32:
             similarity = tf.constant(0.)
         else:
             similarity = (
                 tf.constant(1.)
                 / (alpha*dist + tf.constant(1.))
             )
     similarity = tf.ensure_shape(similarity, [])
@@ -209,47 +209,47 @@
         tf.TensorSpec(None, tf.int32),
         tf.TensorSpec(None, tf.bool),
         tf.TensorSpec(None, tf.float32),
     ],
     #autograph=True,
 )
 def tf_batch_sim(
-        source_batch,
-        target_batch,
-        delete=tf.constant(1),
-        insert=tf.constant(1),
-        substitute=tf.constant(2),
-        proportional=tf.constant(True),
-        alpha=tf.constant(1/3),
-    ):
-    batch_size = tf.shape(source_batch)[0]
-    #batch_size = source_batch.shape[0]
-    #print(f"\n{source_batch = }")
+    pred_batch,
+    gt_batch,
+    delete=tf.constant(1),
+    insert=tf.constant(1),
+    substitute=tf.constant(2),
+    proportional=tf.constant(True),
+    alpha=tf.constant(1/3),
+):
+    batch_size = tf.shape(pred_batch)[0]
+    #batch_size = pred_batch.shape[0]
+    #print(f"\n{pred_batch = }")
     somme = tf.constant(0.)
     for i in tf.range(batch_size):
         #tf.autograph.experimental.set_loop_options(
         #    shape_invariants=[
         #        (somme, tf.TensorShape(()))
         #    ]
         #)
         #tf.autograph.experimental.set_loop_options(maximum_iterations=128)
 
         #somme = somme + tf_byte_sim(
-        #        source_batch[i],
-        #        target_batch[i],
+        #        pred_batch[i],
+        #        gt_batch[i],
         #        delete,
         #        insert,
         #        substitute,
         #        proportional,
         #        alpha,
         #    )
 
         sim = tf_byte_sim(
-            source_batch[i],
-            target_batch[i],
+            pred_batch[i],
+            gt_batch[i],
             delete,
             insert,
             substitute,
             proportional,
             alpha,
         )
         # TODO: tf.add() and +=, diff?
```

### Comparing `vina2vi-0.0.5/vina2vi.egg-info/PKG-INFO` & `vina2vi-0.0.6/vina2vi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: vina2vi
-Version: 0.0.5
+Version: 0.0.6
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vina2vi
 `vina2vi` stands for _**Vi**etnamese **n**o **a**ccent **to** **Vi**etnamese_,  
 which is a Python package aiming at helping foreigners **decrypt** messages
 in Vietnamese.  
 (More precisely, foreigners who already know the basics of the language.)
 
-Among other things, this Python package tries to
-- Restore Vietnamese diacrytics
+Among other things, this Python package aims to
+- Restore Vietnamese diacritics
 - Translate acronyms, **đổi vần**, etc.
+- Spell correction
 
 
 ## Installation
 Run the following to install:
 
 ```bash
 pip install vina2vi
@@ -40,15 +42,15 @@
   then `is_foreign` returns `True`
 - If the string consists exclusively of characters of modern Vietnamese alphabets,
   then `is_foreign` returns `False`
     - Languages whose alphabets are a subset of Vietnamese's are thus considered as Vietnamese
     - Currently, we do not consider chữ Nôm as Vietnamese; maybe we will in the future
 
 ```python
-In [1]: from vina2vi.utils import Vietnamese
+In [1]: from vina2vi.util import Vietnamese
 
 In [2]: Vietnamese.is_foreign("Российская Федерация\tRossiyskaya Federatsiya")
 Out[2]: True
 
 In [3]: Vietnamese.is_foreign("\n\tRossiyskaya Federatsiya")
 Out[3]: False
```

