# Comparing `tmp/katalytic-0.1.1.tar.gz` & `tmp/katalytic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-0.1.1.tar", last modified: Fri Apr 14 18:32:44 2023, max compression
+gzip compressed data, was "katalytic-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic-0.1.1.tar` & `katalytic-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0      132 2023-04-14 18:31:54.747619 katalytic-0.1.1/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-14 18:31:54.747619 katalytic-0.1.1/.gitignore
--rw-r--r--   0        0        0      841 2023-04-14 18:31:54.747619 katalytic-0.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      486 2023-04-14 18:31:54.747619 katalytic-0.1.1/.travis.yml
--rw-r--r--   0        0        0      745 2023-04-14 18:32:40.164900 katalytic-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-14 18:31:54.747619 katalytic-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2212 2023-04-14 18:31:54.747619 katalytic-0.1.1/README.md
--rw-r--r--   0        0        0     1779 2023-04-14 18:32:39.709128 katalytic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/pytest.sh
--rw-r--r--   0        0        0     3107 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-14 18:31:54.747619 katalytic-0.1.1/scripts/venv.sh
--rw-r--r--   0        0        0      106 2023-04-14 18:31:54.747619 katalytic-0.1.1/src/katalytic/katalytic.py
--rw-r--r--   0        0        0      284 2023-04-14 18:31:54.747619 katalytic-0.1.1/tests/test_collection.py
--rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 katalytic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2023-07-09 19:30:05.161864 katalytic-0.2.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-07-09 19:30:05.161864 katalytic-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3256 2023-07-09 19:30:05.161864 katalytic-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1513 2023-07-09 19:37:21.597758 katalytic-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5489 2023-07-09 19:30:05.161864 katalytic-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-07-09 19:30:05.161864 katalytic-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4416 2023-07-09 19:30:05.161864 katalytic-0.2.0/README.md
+-rw-r--r--   0        0        0     1478 2023-07-09 19:37:21.597758 katalytic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6303 2023-07-09 19:30:05.161864 katalytic-0.2.0/src/katalytic/_pkg.py
+-rw-r--r--   0        0        0    58606 2023-07-09 19:30:05.161864 katalytic-0.2.0/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0    22696 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    51483 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/files.py
+-rw-r--r--   0        0        0      130 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/katalytic.py
+-rw-r--r--   0        0        0     5838 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/maths/__init__.py
+-rw-r--r--   0        0        0    22812 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/maths/bboxes.py
+-rw-r--r--   0        0        0     4238 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/meta.py
+-rw-r--r--   0        0        0    13200 2023-07-09 19:30:05.165864 katalytic-0.2.0/tests/test_bboxes.py
+-rw-r--r--   0        0        0    19288 2023-07-09 19:30:05.165864 katalytic-0.2.0/tests/test_checks.py
+-rw-r--r--   0        0        0    52443 2023-07-09 19:30:05.165864 katalytic-0.2.0/tests/test_data.py
+-rw-r--r--   0        0        0    67110 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_files.py
+-rw-r--r--   0        0        0     3868 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_maths.py
+-rw-r--r--   0        0        0     3054 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_meta.py
+-rw-r--r--   0        0        0     2903 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_pkg.py
+-rw-r--r--   0        0        0     5761 1970-01-01 00:00:00.000000 katalytic-0.2.0/PKG-INFO
```

### Comparing `katalytic-0.1.1/.gitignore` & `katalytic-0.2.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 __pycache__/*
 .cache/*
 .*.swp
 */.ipynb_checkpoints/*
 .DS_Store
 data/
 logs/
+*sandbox*
 
 # Project files
 .ropeproject
 .project
 .pydevproject
 .settings
 .idea
```

### Comparing `katalytic-0.1.1/LICENSE.txt` & `katalytic-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

