# Comparing `tmp/rules_validations-0.4.1.tar.gz` & `tmp/rules_validations-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rules_validations-0.4.1.tar", max compression
+gzip compressed data, was "rules_validations-0.5.0.tar", max compression
```

## Comparing `rules_validations-0.4.1.tar` & `rules_validations-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-07-07 19:37:10.825817 rules_validations-0.4.1/README.md
--rw-r--r--   0        0        0      347 2023-07-07 19:37:27.273934 rules_validations-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2321 2023-07-07 19:37:10.825817 rules_validations-0.4.1/rules_validations/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-07 19:37:10.825817 rules_validations-0.4.1/rules_validations/baseEnum.py
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 rules_validations-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-07-09 16:01:36.958416 rules_validations-0.5.0/README.md
+-rw-r--r--   0        0        0      337 2023-07-09 16:01:47.938591 rules_validations-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2321 2023-07-09 16:01:36.958416 rules_validations-0.5.0/rules_validations/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-09 16:01:36.958416 rules_validations-0.5.0/rules_validations/baseEnum.py
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 rules_validations-0.5.0/PKG-INFO
```

### Comparing `rules_validations-0.4.1/rules_validations/__init__.py` & `rules_validations-0.5.0/rules_validations/__init__.py`

 * *Files identical despite different names*

### Comparing `rules_validations-0.4.1/rules_validations/baseEnum.py` & `rules_validations-0.5.0/rules_validations/baseEnum.py`

 * *Files identical despite different names*

