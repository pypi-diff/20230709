# Comparing `tmp/vina2vi-0.0.7.tar.gz` & `tmp/vina2vi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vina2vi-0.0.7.tar", last modified: Sun Jul  9 10:51:42 2023, max compression
+gzip compressed data, was "vina2vi-0.0.8.tar", last modified: Sun Jul  9 14:09:27 2023, max compression
```

## Comparing `vina2vi-0.0.7.tar` & `vina2vi-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.453312 vina2vi-0.0.7/
--rw-r--r--   0 phunc20   (1000) wheel      (998)     1087 2022-09-23 18:32:00.000000 vina2vi-0.0.7/LICENSE
--rw-r--r--   0 phunc20   (1000) wheel      (998)     3990 2023-07-09 10:51:42.453312 vina2vi-0.0.7/PKG-INFO
--rw-r--r--   0 phunc20   (1000) wheel      (998)     3842 2023-03-12 06:52:25.000000 vina2vi-0.0.7/README.md
--rw-r--r--   0 phunc20   (1000) wheel      (998)      400 2023-07-09 10:51:03.000000 vina2vi-0.0.7/pyproject.toml
--rw-r--r--   0 phunc20   (1000) wheel      (998)       38 2023-07-09 10:51:42.453312 vina2vi-0.0.7/setup.cfg
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.449979 vina2vi-0.0.7/vina2vi/
--rw-r--r--   0 phunc20   (1000) wheel      (998)       43 2023-03-12 06:52:03.000000 vina2vi-0.0.7/vina2vi/__init__.py
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.453312 vina2vi-0.0.7/vina2vi/metrics/
--rw-r--r--   0 phunc20   (1000) wheel      (998)      483 2023-03-12 06:52:25.000000 vina2vi-0.0.7/vina2vi/metrics/__init__.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)     4992 2023-03-12 06:52:03.000000 vina2vi-0.0.7/vina2vi/metrics/edit_dist.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)     1070 2023-03-12 06:57:42.000000 vina2vi-0.0.7/vina2vi/metrics/levenshtein.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)     7073 2023-03-12 06:52:03.000000 vina2vi-0.0.7/vina2vi/metrics/tf_edit_dist.py
--rw-r--r--   0 phunc20   (1000) wheel      (998)    11495 2023-07-09 08:14:57.000000 vina2vi-0.0.7/vina2vi/util.py
-drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 10:51:42.449979 vina2vi-0.0.7/vina2vi.egg-info/
--rw-r--r--   0 phunc20   (1000) wheel      (998)     3990 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/PKG-INFO
--rw-r--r--   0 phunc20   (1000) wheel      (998)      342 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/SOURCES.txt
--rw-r--r--   0 phunc20   (1000) wheel      (998)        1 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/dependency_links.txt
--rw-r--r--   0 phunc20   (1000) wheel      (998)       43 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/requires.txt
--rw-r--r--   0 phunc20   (1000) wheel      (998)        8 2023-07-09 10:51:42.000000 vina2vi-0.0.7/vina2vi.egg-info/top_level.txt
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 14:09:27.141857 vina2vi-0.0.8/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     1087 2022-09-23 18:32:00.000000 vina2vi-0.0.8/LICENSE
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3969 2023-07-09 14:09:27.138523 vina2vi-0.0.8/PKG-INFO
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3842 2023-03-12 06:52:25.000000 vina2vi-0.0.8/README.md
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      455 2023-07-09 12:25:29.000000 vina2vi-0.0.8/pyproject.toml
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       38 2023-07-09 14:09:27.141857 vina2vi-0.0.8/setup.cfg
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 14:09:27.138523 vina2vi-0.0.8/vina2vi/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       43 2023-03-12 06:52:03.000000 vina2vi-0.0.8/vina2vi/__init__.py
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 14:09:27.138523 vina2vi-0.0.8/vina2vi/metrics/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      483 2023-03-12 06:52:25.000000 vina2vi-0.0.8/vina2vi/metrics/__init__.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     4992 2023-03-12 06:52:03.000000 vina2vi-0.0.8/vina2vi/metrics/edit_dist.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     1070 2023-03-12 06:57:42.000000 vina2vi-0.0.8/vina2vi/metrics/levenshtein.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     7073 2023-03-12 06:52:03.000000 vina2vi-0.0.8/vina2vi/metrics/tf_edit_dist.py
+-rw-r--r--   0 phunc20   (1000) wheel      (998)    11663 2023-07-09 14:07:59.000000 vina2vi-0.0.8/vina2vi/util.py
+drwxr-xr-x   0 phunc20   (1000) wheel      (998)        0 2023-07-09 14:09:27.138523 vina2vi-0.0.8/vina2vi.egg-info/
+-rw-r--r--   0 phunc20   (1000) wheel      (998)     3969 2023-07-09 14:09:27.000000 vina2vi-0.0.8/vina2vi.egg-info/PKG-INFO
+-rw-r--r--   0 phunc20   (1000) wheel      (998)      342 2023-07-09 14:09:27.000000 vina2vi-0.0.8/vina2vi.egg-info/SOURCES.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)        1 2023-07-09 14:09:27.000000 vina2vi-0.0.8/vina2vi.egg-info/dependency_links.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)       35 2023-07-09 14:09:27.000000 vina2vi-0.0.8/vina2vi.egg-info/requires.txt
+-rw-r--r--   0 phunc20   (1000) wheel      (998)        8 2023-07-09 14:09:27.000000 vina2vi-0.0.8/vina2vi.egg-info/top_level.txt
```

### Comparing `vina2vi-0.0.7/LICENSE` & `vina2vi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.7/PKG-INFO` & `vina2vi-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: vina2vi
-Version: 0.0.7
+Version: 0.0.8
 License: MIT
 Description-Content-Type: text/markdown
-Provides-Extra: eval
 License-File: LICENSE
 
 # vina2vi
 `vina2vi` stands for _**Vi**etnamese **n**o **a**ccent **to** **Vi**etnamese_,  
 which is a Python package aiming at helping foreigners **decrypt** messages
 in Vietnamese.  
 (More precisely, foreigners who already know the basics of the language.)
```

### Comparing `vina2vi-0.0.7/README.md` & `vina2vi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.7/vina2vi/metrics/edit_dist.py` & `vina2vi-0.0.8/vina2vi/metrics/edit_dist.py`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.7/vina2vi/metrics/levenshtein.py` & `vina2vi-0.0.8/vina2vi/metrics/levenshtein.py`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.7/vina2vi/metrics/tf_edit_dist.py` & `vina2vi-0.0.8/vina2vi/metrics/tf_edit_dist.py`

 * *Files identical despite different names*

### Comparing `vina2vi-0.0.7/vina2vi/util.py` & `vina2vi-0.0.8/vina2vi/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 @dataclass(frozen=True)
 class Vietnamese:
     ambiguous_chars = {
         "a": "aáảãàạâấẩẫầậăắẳẵằặ",
         "d": "dđ",
         "e": "eéẻẽèẹêếểễềệ",
         "i": "iíỉĩìị",
-        "o": "oóỏõòôọôốổỗồộơớởỡờợ",
+        "o": "oóỏõòọôôốổỗồộơớởỡờợ",
         "u": "uúủũùụưứửữừự",
         "y": "yýỷỹỳỵ",
     }
     for k, v in ambiguous_chars.items():
         ambiguous_chars[k] = unicodedata.normalize("NFC", v)
     lowers = "".join(ambiguous_chars.values()) + string.ascii_lowercase
     uppers = lowers.upper()
@@ -221,25 +221,27 @@
     #gt_text = " ".join(
     #    t for t in gt_tokens if t not in tokenizer.special_tokens_map.values())
 
     model.to(device)
     token_logits = model(**collated).logits
     mask_token_logits = token_logits[0, mask_token_indices, :]
     # Pick the <mask> candidates with the highest logits
-    top_k_token_ids = torch.topk(mask_token_logits, topk, dim=1).indices.numpy()
+    #top_k_token_ids = torch.topk(mask_token_logits, topk, dim=1).indices.numpy()
+    top_k_token_ids = torch.topk(mask_token_logits, topk, dim=1).indices.cpu().numpy()
+    #top_k_token_ids = torch.topk(mask_token_logits, topk, dim=1).indices
 
 
     #print("(masked)")
     #print(f'"{masked_text}"', end="\n\n")
 
     #print("(gt)")
     #print(f'"{gt_text}"', end="\n\n")
 
     for kk in range(topk):
-        pred_ids = collated["input_ids"][0].numpy()
+        pred_ids = collated["input_ids"][0].cpu().numpy()
         infer_token_ids = top_k_token_ids[:, kk]
         pred_ids[mask_token_indices] = infer_token_ids
         pred_tokens = tokenizer.convert_ids_to_tokens(
             pred_ids, skip_special_tokens=False,)
         #print(f'{pred_tokens = }')
         for i, token in enumerate(pred_tokens):
             if i in mask_token_indices:
```

### Comparing `vina2vi-0.0.7/vina2vi.egg-info/PKG-INFO` & `vina2vi-0.0.8/vina2vi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: vina2vi
-Version: 0.0.7
+Version: 0.0.8
 License: MIT
 Description-Content-Type: text/markdown
-Provides-Extra: eval
 License-File: LICENSE
 
 # vina2vi
 `vina2vi` stands for _**Vi**etnamese **n**o **a**ccent **to** **Vi**etnamese_,  
 which is a Python package aiming at helping foreigners **decrypt** messages
 in Vietnamese.  
 (More precisely, foreigners who already know the basics of the language.)
```

