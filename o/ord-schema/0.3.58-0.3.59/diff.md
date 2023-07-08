# Comparing `tmp/ord-schema-0.3.58.tar.gz` & `tmp/ord-schema-0.3.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.58.tar", last modified: Wed Jul  5 21:18:50 2023, max compression
+gzip compressed data, was "ord-schema-0.3.59.tar", last modified: Sat Jul  8 23:12:02 2023, max compression
```

## Comparing `ord-schema-0.3.58.tar` & `ord-schema-0.3.59.tar`

### file list

```diff
@@ -1,72 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.618902 ord-schema-0.3.58/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-05 21:18:21.000000 ord-schema-0.3.58/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 21:18:21.000000 ord-schema-0.3.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 21:18:21.000000 ord-schema-0.3.58/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-05 21:18:50.618902 ord-schema-0.3.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-05 21:18:21.000000 ord-schema-0.3.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.610901 ord-schema-0.3.58/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.614902 ord-schema-0.3.58/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.614902 ord-schema-0.3.58/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/add_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/add_datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.614902 ord-schema-0.3.58/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49139 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.618902 ord-schema-0.3.58/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45196 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-05 21:18:21.000000 ord-schema-0.3.58/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.610901 ord-schema-0.3.58/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-05 21:18:50.000000 ord-schema-0.3.58/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-05 21:18:50.000000 ord-schema-0.3.58/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:18:50.000000 ord-schema-0.3.58/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-05 21:18:50.000000 ord-schema-0.3.58/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 21:18:50.000000 ord-schema-0.3.58/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:50.618902 ord-schema-0.3.58/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-05 21:18:21.000000 ord-schema-0.3.58/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (123)    46287 2023-07-05 21:18:21.000000 ord-schema-0.3.58/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-05 21:18:21.000000 ord-schema-0.3.58/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 21:18:21.000000 ord-schema-0.3.58/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:18:50.618902 ord-schema-0.3.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-05 21:18:30.000000 ord-schema-0.3.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.889325 ord-schema-0.3.59/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-08 23:11:37.000000 ord-schema-0.3.59/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 23:11:37.000000 ord-schema-0.3.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 23:11:37.000000 ord-schema-0.3.59/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-08 23:12:02.889325 ord-schema-0.3.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 23:11:37.000000 ord-schema-0.3.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.877325 ord-schema-0.3.59/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.881325 ord-schema-0.3.59/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.881325 ord-schema-0.3.59/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.881325 ord-schema-0.3.59/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49139 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.889325 ord-schema-0.3.59/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45196 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.877325 ord-schema-0.3.59/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.889325 ord-schema-0.3.59/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-08 23:11:37.000000 ord-schema-0.3.59/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46287 2023-07-08 23:11:37.000000 ord-schema-0.3.59/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-08 23:11:37.000000 ord-schema-0.3.59/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-08 23:11:37.000000 ord-schema-0.3.59/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:12:02.889325 ord-schema-0.3.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-08 23:11:41.000000 ord-schema-0.3.59/setup.py
```

### Comparing `ord-schema-0.3.58/LICENSE` & `ord-schema-0.3.59/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/PKG-INFO` & `ord-schema-0.3.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.58
+Version: 0.3.59
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.58/README.md` & `ord-schema-0.3.59/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/__init__.py` & `ord-schema-0.3.59/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/frozen_message.py` & `ord-schema-0.3.59/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/frozen_message_test.py` & `ord-schema-0.3.59/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/logging.py` & `ord-schema-0.3.59/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/macros/__init__.py` & `ord-schema-0.3.59/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/macros/solutions.py` & `ord-schema-0.3.59/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.59/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/macros/workups.py` & `ord-schema-0.3.59/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/message_helpers.py` & `ord-schema-0.3.59/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/message_helpers_test.py` & `ord-schema-0.3.59/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/orm/__init__.py` & `ord-schema-0.3.59/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/orm/add_datasets_test.py` & `ord-schema-0.3.59/ord_schema/orm/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-# Copyright 2022 Open Reaction Database Project Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""Tests for ord_schema.orm.add_datasets."""
-import os
-
-import docopt
-import pytest
-from sqlalchemy import create_engine
-from sqlalchemy.exc import IntegrityError
-from testing.postgresql import Postgresql
-
-from ord_schema.orm import add_datasets
-from ord_schema.orm.database import prepare_database
-
-
-def test_main():
-    with Postgresql() as postgres:
-        engine = create_engine(postgres.url(), future=True)
-        assert prepare_database(engine)  # Requires RDKit.
-        argv = [
-            "--url",
-            postgres.url(),
-            "--pattern",
-            os.path.join(os.path.dirname(__file__), "testdata", "ord-nielsen-example.pbtxt"),
-        ]
-        add_datasets.main(**docopt.docopt(add_datasets.__doc__, argv))
-        with pytest.raises(IntegrityError, match="violates unique constraint"):
-            add_datasets.main(**docopt.docopt(add_datasets.__doc__, argv))
-        argv.append("--overwrite")
-        add_datasets.main(**docopt.docopt(add_datasets.__doc__, argv))
+# Copyright 2022 Open Reaction Database Project Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Pytest fixtures."""
+import os
+from typing import Iterator
+
+import pytest
+from sqlalchemy import create_engine
+from sqlalchemy.orm import Session
+from testing.postgresql import Postgresql
+
+from ord_schema.message_helpers import load_message
+from ord_schema.orm.database import add_dataset, add_rdkit, prepare_database
+from ord_schema.proto import dataset_pb2
+
+
+@pytest.fixture
+def test_session() -> Iterator[Session]:
+    dataset = load_message(
+        os.path.join(os.path.dirname(__file__), "testdata", "ord-nielsen-example.pbtxt"), dataset_pb2.Dataset
+    )
+    with Postgresql() as postgres:
+        engine = create_engine(postgres.url(), future=True, echo=True)
+        rdkit_cartridge = prepare_database(engine)
+        with Session(engine) as session:
+            add_dataset(dataset, session)
+            session.flush()
+            if rdkit_cartridge:
+                add_rdkit(session)
+            session.commit()
+        with Session(engine) as session:
+            yield session
```

### Comparing `ord-schema-0.3.58/ord_schema/orm/conftest.py` & `ord-schema-0.3.59/ord_schema/orm/mappers_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,37 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Pytest fixtures."""
+"""Tests for ord_schema.orm.mappers."""
 import os
-from typing import Iterator
-
 import pytest
-from sqlalchemy import create_engine
-from sqlalchemy.orm import Session
-from testing.postgresql import Postgresql
 
 from ord_schema.message_helpers import load_message
-from ord_schema.orm.database import add_dataset, add_rdkit, prepare_database
-from ord_schema.proto import dataset_pb2
+from ord_schema.orm.mappers import from_proto, to_proto
+from ord_schema.proto.dataset_pb2 import Dataset
 
 
-@pytest.fixture
-def test_session() -> Iterator[Session]:
-    dataset = load_message(
-        os.path.join(os.path.dirname(__file__), "testdata", "ord-nielsen-example.pbtxt"), dataset_pb2.Dataset
-    )
-    with Postgresql() as postgres:
-        engine = create_engine(postgres.url(), future=True, echo=True)
-        rdkit_cartridge = prepare_database(engine)
-        with Session(engine) as session:
-            add_dataset(dataset, session)
-            session.flush()
-            if rdkit_cartridge:
-                add_rdkit(session)
-            session.commit()
-        with Session(engine) as session:
-            yield session
+@pytest.mark.parametrize(
+    "filename",
+    (
+        os.path.join(os.path.dirname(__file__), "testdata", "empty.pbtxt"),
+        os.path.join(os.path.dirname(__file__), "testdata", "full.pbtxt"),
+        os.path.join(os.path.dirname(__file__), "testdata", "ord-nielsen-example.pbtxt"),
+    ),
+)
+def test_round_trip(filename):
+    dataset = load_message(filename, Dataset)
+    assert dataset == to_proto(from_proto(dataset))
```

### Comparing `ord-schema-0.3.58/ord_schema/orm/database.py` & `ord-schema-0.3.59/ord_schema/orm/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Functions for creating/managing the PostgreSQL database."""
 import time
 import os
 from unittest.mock import patch
 
-from sqlalchemy import cast, delete, func, text, update
+from sqlalchemy import cast, delete, func, select, text, update
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import Session
 
 from ord_schema.logging import get_logger
 from ord_schema.orm.mappers import Base, Mappers, from_proto
 from ord_schema.orm.rdkit_mappers import CString, FingerprintType, RDKitMol, RDKitReaction
@@ -72,14 +72,21 @@
     mapped_dataset = from_proto(dataset)
     logger.info(f"from_proto() took {time.time() - start}s")
     start = time.time()
     session.add(mapped_dataset)
     logger.info(f"session.add() took {time.time() - start}s")
 
 
+def get_dataset_md5(dataset_id: str, session: Session) -> str | None:
+    """The MD5 hash of the current version of a dataset, if it exists in the database."""
+    result = session.execute(select(Mappers.Dataset.md5).where(Mappers.Dataset.dataset_id == dataset_id))
+    row = result.first()
+    return row[0] if row else None
+
+
 def delete_dataset(dataset_id: str, session: Session) -> None:
     """Deletes a dataset from the database."""
     logger.info(f"Deleting dataset {dataset_id}")
     start = time.time()
     session.execute(delete(Mappers.Dataset).where(Mappers.Dataset.dataset_id == dataset_id))
     logger.info(f"delete took {time.time() - start}s")
```

### Comparing `ord-schema-0.3.58/ord_schema/orm/database_test.py` & `ord-schema-0.3.59/ord_schema/orm/database_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for ord_schema.orm.database."""
 from sqlalchemy import select
 
-from ord_schema.orm.database import delete_dataset
+from ord_schema.orm.database import delete_dataset, get_dataset_md5
 from ord_schema.orm.mappers import Mappers
 from ord_schema.proto import reaction_pb2
 
 
 def test_orm(test_session):
     query = (
         select(Mappers.Reaction)
@@ -34,7 +34,12 @@
     assert len(reactions) == 12
 
 
 def test_delete_dataset(test_session):
     assert test_session.query(Mappers.Reaction).count() == 80
     delete_dataset("test_dataset", test_session)
     assert test_session.query(Mappers.Reaction).count() == 0
+
+
+def test_get_dataset_md5(test_session):
+    assert get_dataset_md5("test_dataset", test_session) == "42c687cafd247fd72d2a78c550b0b054"
+    assert get_dataset_md5("other_dataset", test_session) is None
```

### Comparing `ord-schema-0.3.58/ord_schema/orm/mappers.py` & `ord-schema-0.3.59/ord_schema/orm/mappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,22 @@
         - Some messages can be repeated, while others are unique to their parent. These uniqueness constraints force
           the use of joined table inheritance since they are specific to their polymorphic type.
       For convenience and consistency, we use single table inheritance for *all* message types, regardless of whether
       they are used in one context or more than one context. This means that we do not enforce the second constraint in
       the database.
 """
 from collections import defaultdict
+from hashlib import md5
 from operator import attrgetter
 from typing import Any, Mapping, Optional, Type
 
 from google.protobuf.descriptor import Descriptor, FieldDescriptor
 from google.protobuf.message import Message
 from inflection import underscore
-from sqlalchemy import Boolean, Column, Enum, Float, Integer, ForeignKey, LargeBinary, Text
+from sqlalchemy import Boolean, Column, Enum, Float, Integer, ForeignKey, LargeBinary, String, Text
 from sqlalchemy.dialects.postgresql import ARRAY
 from sqlalchemy.orm import relationship
 
 import ord_schema.orm.rdkit_mappers  # pylint: disable=unused-import
 from ord_schema import message_helpers
 from ord_schema.logging import get_logger
 from ord_schema.orm import Base
@@ -162,14 +163,16 @@
         elif field.type == FieldDescriptor.TYPE_ENUM:
             attrs[field.name] = Column(Enum(*field.enum_type.values_by_name.keys(), name=field.enum_type.name))
         else:
             attrs[field.name] = Column(_FIELD_TYPES[field.type])
     if message_type == dataset_pb2.Dataset:
         # Make dataset IDs globally unique.
         attrs["dataset_id"] = Column(Text, nullable=False, unique=True)
+        # Track the MD5 hash so we can quickly identify changes.
+        attrs["md5"] = Column(String(32), nullable=False)
     elif message_type == reaction_pb2.Reaction:
         # Make reaction IDs globally unique.
         attrs["reaction_id"] = Column(Text, nullable=False, unique=True)
         # Serialize and store the entire Reaction proto.
         attrs["proto"] = Column(LargeBinary, nullable=False)
         attrs["rdkit"] = relationship(f"_{message_type.DESCRIPTOR.name}RDKit", uselist=False)
     elif message_type in {reaction_pb2.Compound, reaction_pb2.ProductCompound}:
@@ -239,30 +242,31 @@
         ORM object.
     """
     if mapper is None:
         mapper = _MESSAGE_TO_MAPPER[type(message)]
     kwargs = {}
     if key is not None:
         kwargs["key"] = key
-    if isinstance(message, reaction_pb2.Reaction):
-        kwargs["proto"] = message.SerializeToString()
     for field, value in message.ListFields():
         if field.type == FieldDescriptor.TYPE_MESSAGE:
             field_mapper = getattr(mapper, field.name).mapper.class_
             if isinstance(value, Mapping):
                 kwargs[field.name] = [from_proto(v, mapper=field_mapper, key=k) for k, v in value.items()]
             elif field.label == FieldDescriptor.LABEL_REPEATED:
                 kwargs[field.name] = [from_proto(v, mapper=field_mapper) for v in value]
             else:
                 kwargs[field.name] = from_proto(value, mapper=field_mapper)
         elif field.type == FieldDescriptor.TYPE_ENUM:
             kwargs[field.name] = field.enum_type.values_by_number[value].name
         else:
             kwargs[field.name] = value
-    if isinstance(message, reaction_pb2.Reaction):
+    if isinstance(message, dataset_pb2.Dataset):
+        kwargs["md5"] = md5(message.SerializeToString(deterministic=True)).hexdigest()
+    elif isinstance(message, reaction_pb2.Reaction):
+        kwargs["proto"] = message.SerializeToString(deterministic=True)
         field_mapper = getattr(mapper, "rdkit").mapper.class_
         try:
             reaction_smiles = message_helpers.get_reaction_smiles(message, generate_if_missing=True)
             assert reaction_smiles is not None  # Type hint.
             reaction_smiles = reaction_smiles.split()[0]  # Handle CXSMILES.
             kwargs["rdkit"] = field_mapper(reaction_smiles=reaction_smiles)
         except ValueError:
```

### Comparing `ord-schema-0.3.58/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.59/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.59/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/proto/__init__.py` & `ord-schema-0.3.59/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.59/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.59/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.59/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.59/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.59/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/resolvers.py` & `ord-schema-0.3.59/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/resolvers_test.py` & `ord-schema-0.3.59/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/__init__.py` & `ord-schema-0.3.59/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.59/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.59/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.59/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.59/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.59/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.59/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.59/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.59/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.59/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/templating.py` & `ord-schema-0.3.59/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/templating_test.py` & `ord-schema-0.3.59/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/units.py` & `ord-schema-0.3.59/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/units_test.py` & `ord-schema-0.3.59/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/updates.py` & `ord-schema-0.3.59/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/updates_test.py` & `ord-schema-0.3.59/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/validations.py` & `ord-schema-0.3.59/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema/validations_test.py` & `ord-schema-0.3.59/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.59/ord_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.58
+Version: 0.3.59
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.58/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.59/ord_schema.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 ord_schema.egg-info/requires.txt
 ord_schema.egg-info/top_level.txt
 ord_schema/macros/__init__.py
 ord_schema/macros/solutions.py
 ord_schema/macros/solutions_test.py
 ord_schema/macros/workups.py
 ord_schema/orm/__init__.py
-ord_schema/orm/add_datasets.py
-ord_schema/orm/add_datasets_test.py
 ord_schema/orm/conftest.py
 ord_schema/orm/database.py
 ord_schema/orm/database_test.py
 ord_schema/orm/mappers.py
 ord_schema/orm/mappers_test.py
 ord_schema/orm/rdkit_mappers.py
 ord_schema/orm/rdkit_mappers_test.py
```

### Comparing `ord-schema-0.3.58/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.59/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/proto/dataset.proto` & `ord-schema-0.3.59/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/proto/reaction.proto` & `ord-schema-0.3.59/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/proto/test.proto` & `ord-schema-0.3.59/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.58/setup.py` & `ord-schema-0.3.59/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.58",
+    version="0.3.59",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

