# Comparing `tmp/vina2vi-0.0.6.tar.gz` & `tmp/vina2vi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vina2vi-0.0.6.tar", last modified: Sun Jul  9 09:24:29 2023, max compression
+gzip compressed data, was "vina2vi-0.0.7.tar", last modified: Sun Jul  9 10:51:42 2023, max compression
```

## Comparing `vina2vi-0.0.6.tar` & `vina2vi-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.803042 vina2vi-0.0.6/
--rw-r--r--   0 phunc20   (1000) wheel      (998)     1087 2022-10-24 16:41:33.000000 vina2vi-0.0.6/LICENSE
--rw-r--r--   0 phunc20   (1000) wheel      (998)     3969 2023-07-09 09:24:29.803042 vina2vi-0.0.6/PKG-INFO
--rw-r--r--   0 phunc20   (1000) wheel      (998)     3842 2023-07-09 09:20:59.000000 vina2vi-0.0.6/README.md
--rw-r--r--   0 phunc20   (1000) wheel      (998)      375 2023-07-09 09:24:13.000000 vina2vi-0.0.6/pyproject.toml
--rw-r--r--   0 phunc20   (1000) wheel      (998)       38 2023-07-09 09:24:29.803042 vina2vi-0.0.6/setup.cfg
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.796375 vina2vi-0.0.6/vina2vi/
--rw-r--r--   0 phunc20   (1000) wheel      (998)       43 2023-01-22 16:43:46.000000 vina2vi-0.0.6/vina2vi/__init__.py
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.803042 vina2vi-0.0.6/vina2vi/metrics/
--rw-r--r--   0 phunc20   (1000) wheel      (998)      483 2023-07-09 09:20:59.000000 vina2vi-0.0.6/vina2vi/metrics/__init__.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)     4992 2023-01-22 16:43:46.000000 vina2vi-0.0.6/vina2vi/metrics/edit_dist.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)     1070 2023-07-09 09:20:59.000000 vina2vi-0.0.6/vina2vi/metrics/levenshtein.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)     7073 2023-01-22 16:43:46.000000 vina2vi-0.0.6/vina2vi/metrics/tf_edit_dist.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)    11270 2023-07-09 09:21:17.000000 vina2vi-0.0.6/vina2vi/util.py
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 09:24:29.799709 vina2vi-0.0.6/vina2vi.egg-info/
--rw-r--r--   0 phunc20   (1000) wheel      (998)     3969 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/PKG-INFO
--rw-r--r--   0 phunc20   (1000) wheel      (998)      312 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/SOURCES.txt
--rw-r--r--   0 phunc20   (1000) wheel      (998)        1 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/dependency_links.txt
--rw-r--r--   0 phunc20   (1000) wheel      (998)        8 2023-07-09 09:24:29.000000 vina2vi-0.0.6/vina2vi.egg-info/top_level.txt
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.453312 vina2vi-0.0.7/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     1087 2022-09-23 18:32:00.000000 vina2vi-0.0.7/LICENSE
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3990 2023-07-09 10:51:42.453312 vina2vi-0.0.7/PKG-INFO
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3842 2023-03-12 06:52:25.000000 vina2vi-0.0.7/README.md
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      400 2023-07-09 10:51:03.000000 vina2vi-0.0.7/pyproject.toml
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       38 2023-07-09 10:51:42.453312 vina2vi-0.0.7/setup.cfg
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.449979 vina2vi-0.0.7/vina2vi/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       43 2023-03-12 06:52:03.000000 vina2vi-0.0.7/vina2vi/__init__.py
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.453312 vina2vi-0.0.7/vina2vi/metrics/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      483 2023-03-12 06:52:25.000000 vina2vi-0.0.7/vina2vi/metrics/__init__.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     4992 2023-03-12 06:52:03.000000 vina2vi-0.0.7/vina2vi/metrics/edit_dist.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     1070 2023-03-12 06:57:42.000000 vina2vi-0.0.7/vina2vi/metrics/levenshtein.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     7073 2023-03-12 06:52:03.000000 vina2vi-0.0.7/vina2vi/metrics/tf_edit_dist.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)    11495 2023-07-09 08:14:57.000000 vina2vi-0.0.7/vina2vi/util.py
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.449979 vina2vi-0.0.7/vina2vi.egg-info/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3990 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/PKG-INFO
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      342 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/SOURCES.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)        1 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/dependency_links.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       43 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/requires.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)        8 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/top_level.txt
```

### Comparing `vina2vi-0.0.6/LICENSE` & `vina2vi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.6/PKG-INFO` & `vina2vi-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: vina2vi
-Version: 0.0.6
+Version: 0.0.7
 License: MIT
 Description-Content-Type: text/markdown
+Provides-Extra: eval
 License-File: LICENSE
 
 # vina2vi
 `vina2vi` stands for _**Vi**etnamese **n**o **a**ccent **to** **Vi**etnamese_,  
 which is a Python package aiming at helping foreigners **decrypt** messages
 in Vietnamese.  
 (More precisely, foreigners who already know the basics of the language.)
```

### Comparing `vina2vi-0.0.6/README.md` & `vina2vi-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.6/vina2vi/metrics/edit_dist.py` & `vina2vi-0.0.7/vina2vi/metrics/edit_dist.py`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.6/vina2vi/metrics/levenshtein.py` & `vina2vi-0.0.7/vina2vi/metrics/levenshtein.py`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.6/vina2vi/metrics/tf_edit_dist.py` & `vina2vi-0.0.7/vina2vi/metrics/tf_edit_dist.py`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.6/vina2vi/util.py` & `vina2vi-0.0.7/vina2vi/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import string
 import unicodedata
 from dataclasses import dataclass, field
 
 import unidecode
 import torch
+from datasets import Dataset, DatasetDict
 
 
 @dataclass(frozen=True)
 class Vietnamese:
     ambiguous_chars = {
         "a": "aáảãàạâấẩẫầậăắẳẵằặ",
         "d": "dđ",
         "e": "eéẻẽèẹêếểễềệ",
         "i": "iíỉĩìị",
-        "o": "oóỏõòọôôốổỗồộơớởỡờợ",
+        "o": "oóỏõòôọôốổỗồộơớởỡờợ",
         "u": "uúủũùụưứửữừự",
         "y": "yýỷỹỳỵ",
     }
     for k, v in ambiguous_chars.items():
         ambiguous_chars[k] = unicodedata.normalize("NFC", v)
     lowers = "".join(ambiguous_chars.values()) + string.ascii_lowercase
     uppers = lowers.upper()
@@ -177,18 +178,25 @@
     *,
     topk: int = 5,
     device=torch.device("cpu"),
     tokenizer,
     model,
     data_collator,
 ):
-    if "test" in datasets:
-        ds = datasets["test"]
-    else:
-        ds = datasets["train"]
+    """
+    args
+        data_collator, aka collate_fn
+    """
+    if isinstance(datasets, DatasetDict):
+        if "test" in datasets:
+            ds = datasets["test"]
+        else:
+            ds = datasets["train"]
+    elif isinstance(datasets, Dataset):
+        ds = datasets
     sample = ds.shuffle().select([0])[0]
     #print(f'tokenizer.decode(sample["labels"]) = "{tokenizer.decode(sample["labels"])}"')
     collated = data_collator([sample])
     # Put on the same assigned device
     collated = {k: v.to(device) for k, v in collated.items()}
     masked_text = tokenizer.decode(collated["input_ids"][0])
     mask_token_indices = torch.where(collated["input_ids"] == tokenizer.mask_token_id)[1]
```

### Comparing `vina2vi-0.0.6/vina2vi.egg-info/PKG-INFO` & `vina2vi-0.0.7/vina2vi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: vina2vi
-Version: 0.0.6
+Version: 0.0.7
 License: MIT
 Description-Content-Type: text/markdown
+Provides-Extra: eval
 License-File: LICENSE
 
 # vina2vi
 `vina2vi` stands for _**Vi**etnamese **n**o **a**ccent **to** **Vi**etnamese_,  
 which is a Python package aiming at helping foreigners **decrypt** messages
 in Vietnamese.  
 (More precisely, foreigners who already know the basics of the language.)
```

