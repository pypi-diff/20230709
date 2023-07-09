# Comparing `tmp/libcoveocds-0.8.0.tar.gz` & `tmp/libcoveocds-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libcoveocds-0.8.0.tar", last modified: Wed Aug 26 16:48:55 2020, max compression
+gzip compressed data, was "dist/libcoveocds-0.9.1.tar", last modified: Wed Oct  7 15:58:04 2020, max compression
```

## Comparing `libcoveocds-0.8.0.tar` & `libcoveocds-0.9.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     2941 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/CHANGELOG.md
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1269 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/README.rst
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1745 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/libcoveocds/config.py
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds/cli/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      697 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/libcoveocds/cli/__main__.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/libcoveocds/cli/__init__.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/libcoveocds/__init__.py
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds/lib/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     2986 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/libcoveocds/lib/additional_checks.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/libcoveocds/lib/__init__.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    18872 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/libcoveocds/lib/common_checks.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     2469 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/libcoveocds/lib/api.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    12754 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/libcoveocds/schema.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     8426 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/libcoveocds/common_checks.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     3639 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/libcoveocds/api.py
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1054 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/test_api.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     5958 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/test_schema.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/__init__.py
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/lib/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     7161 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/test_api.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/__init__.py
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/lib/fixtures/
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/lib/fixtures/common_checks/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    25816 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/fixtures/common_checks/badfile.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)  9120411 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/fixtures/common_checks/samplerubbish.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      523 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/fixtures/common_checks/record_check_ocids.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     6049 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/fixtures/common_checks/release_aggregate.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    21721 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/fixtures/common_checks/tenders_releases_7_releases_check_ocids.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     9864 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/lib/test_common_checks.py
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/fixtures/
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/fixtures/additional_checks/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     6909 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/fixtures/additional_checks/empty_fields_releases.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     7425 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/fixtures/additional_checks/basic_releases.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)   102968 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/fixtures/additional_checks/empty_fields_records.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)   103309 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/fixtures/additional_checks/full_record.json
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/fixtures/api/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     7425 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/fixtures/api/basic_1.json
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    28077 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/dupe_ids_1.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1169 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/records_non_unique.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      583 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/records_unique.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      511 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/records_non_unique_no_ocid.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      538 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/releases_unique.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     7425 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/basic_1.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      384 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/records_no_validation_errors.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      540 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/releases_non_unique_no_id.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1227 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/releases_non_unique.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1316 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/records_invalid_releases.json
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/1-0/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1377 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/1-0/records_invalid_releases.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      399 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/fixtures/common_checks/releases_no_validation_errors.json
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    24206 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/tests/test_common_checks.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     2542 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/tests/test_additional_checks.py
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      990 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/LICENSE
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      270 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/MAINTAINERS.md
-drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds.egg-info/
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)        1 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds.egg-info/dependency_links.txt
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       63 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds.egg-info/entry_points.txt
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      125 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds.egg-info/requires.txt
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       12 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds.egg-info/top_level.txt
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1971 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds.egg-info/SOURCES.txt
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1999 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/libcoveocds.egg-info/PKG-INFO
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       89 2020-08-06 16:33:30.000000 libcoveocds-0.8.0/MANIFEST.in
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1999 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/PKG-INFO
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       38 2020-08-26 16:48:54.000000 libcoveocds-0.8.0/setup.cfg
--rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1160 2020-08-26 16:48:21.000000 libcoveocds-0.8.0/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.912677 libcoveocds-0.9.1/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3274 2020-10-07 15:57:12.000000 libcoveocds-0.9.1/CHANGELOG.md
+-rw-rw-r--   0 rob       (1000) rob       (1000)      990 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)      270 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/MAINTAINERS.md
+-rw-rw-r--   0 rob       (1000) rob       (1000)       89 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/MANIFEST.in
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2865 2020-10-07 15:58:04.912677 libcoveocds-0.9.1/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2031 2020-10-07 07:27:09.000000 libcoveocds-0.9.1/README.rst
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.900677 libcoveocds-0.9.1/libcoveocds/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3639 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/api.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.900677 libcoveocds-0.9.1/libcoveocds/cli/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/cli/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2595 2020-10-07 07:27:09.000000 libcoveocds-0.9.1/libcoveocds/cli/__main__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     8426 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/common_checks.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1745 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/config.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.900677 libcoveocds-0.9.1/libcoveocds/lib/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/lib/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2986 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/lib/additional_checks.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2469 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/lib/api.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    19183 2020-10-07 15:57:12.000000 libcoveocds-0.9.1/libcoveocds/lib/common_checks.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    12754 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/libcoveocds/schema.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.900677 libcoveocds-0.9.1/libcoveocds.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2865 2020-10-07 15:58:04.000000 libcoveocds-0.9.1/libcoveocds.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1989 2020-10-07 15:58:04.000000 libcoveocds-0.9.1/libcoveocds.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2020-10-07 15:58:04.000000 libcoveocds-0.9.1/libcoveocds.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       63 2020-10-07 15:58:04.000000 libcoveocds-0.9.1/libcoveocds.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)      131 2020-10-07 15:58:04.000000 libcoveocds-0.9.1/libcoveocds.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       12 2020-10-07 15:58:04.000000 libcoveocds-0.9.1/libcoveocds.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2020-10-07 15:58:04.912677 libcoveocds-0.9.1/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1177 2020-10-07 15:57:12.000000 libcoveocds-0.9.1/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.904677 libcoveocds-0.9.1/tests/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.900677 libcoveocds-0.9.1/tests/fixtures/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.904677 libcoveocds-0.9.1/tests/fixtures/additional_checks/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     7425 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/additional_checks/basic_releases.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)   102968 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/additional_checks/empty_fields_records.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6909 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/additional_checks/empty_fields_releases.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)   103309 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/additional_checks/full_record.json
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.904677 libcoveocds-0.9.1/tests/fixtures/api/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     7425 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/api/basic_1.json
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.904677 libcoveocds-0.9.1/tests/fixtures/common_checks/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.904677 libcoveocds-0.9.1/tests/fixtures/common_checks/1-0/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1377 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/1-0/records_invalid_releases.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)     7425 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/basic_1.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)    28077 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/dupe_ids_1.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1316 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/records_invalid_releases.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)      384 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/records_no_validation_errors.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1169 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/records_non_unique.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)      511 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/records_non_unique_no_ocid.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)      583 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/records_unique.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)      399 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/releases_no_validation_errors.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1227 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/releases_non_unique.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)      540 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/releases_non_unique_no_id.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)      538 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/fixtures/common_checks/releases_unique.json
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.904677 libcoveocds-0.9.1/tests/lib/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        0 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/lib/__init__.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.900677 libcoveocds-0.9.1/tests/lib/fixtures/
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2020-10-07 15:58:04.912677 libcoveocds-0.9.1/tests/lib/fixtures/common_checks/
+-rw-rw-r--   0 rob       (1000) rob       (1000)    25816 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/lib/fixtures/common_checks/badfile.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)      523 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/lib/fixtures/common_checks/record_check_ocids.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6049 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/lib/fixtures/common_checks/release_aggregate.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)  9120411 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/lib/fixtures/common_checks/samplerubbish.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)    21721 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/lib/fixtures/common_checks/tenders_releases_7_releases_check_ocids.json
+-rw-rw-r--   0 rob       (1000) rob       (1000)     7161 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/lib/test_api.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     9963 2020-10-07 15:57:12.000000 libcoveocds-0.9.1/tests/lib/test_common_checks.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2542 2020-09-24 14:43:57.000000 libcoveocds-0.9.1/tests/test_additional_checks.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1258 2020-10-07 07:27:09.000000 libcoveocds-0.9.1/tests/test_api.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3703 2020-10-07 07:27:09.000000 libcoveocds-0.9.1/tests/test_cli.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)    24030 2020-10-07 07:27:09.000000 libcoveocds-0.9.1/tests/test_common_checks.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6105 2020-10-07 07:27:09.000000 libcoveocds-0.9.1/tests/test_schema.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libcoveocds-0.8.0/CHANGELOG.md` & `libcoveocds-0.9.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.9.1] - 2020-09-07
+
+### Fixed
+
+- Bump version number in setup.py
+
+## [0.9.0] - 2020-09-07
+
+### Added
+
+- Add Unique IDs count to aggregates
+- Added many options to CLI: convert, output-dir, schema-version, delete, exclude-file
+
+### Changed
+
+- Cache all requests in the tests https://github.com/OpenDataServices/lib-cove/pull/59
+
 ## [0.8.0] - 2020-08-26
 
 ### Changed
 
 - Move OCDS specific code here from lib-cove https://github.com/open-contracting/lib-cove-ocds/pull/44
 
 ## [0.7.6] - 2020-08-21
```

### Comparing `libcoveocds-0.8.0/libcoveocds/config.py` & `libcoveocds-0.9.1/libcoveocds/config.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/libcoveocds/lib/additional_checks.py` & `libcoveocds-0.9.1/libcoveocds/lib/additional_checks.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/libcoveocds/lib/common_checks.py` & `libcoveocds-0.9.1/libcoveocds/lib/common_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     organisation_identifier_contact_point = set()
     organisation_name_no_id_contact_point = set()
 
     release_tender_item_ids = set()
     release_award_item_ids = set()
     release_contract_item_ids = set()
     item_identifier_schemes = set()
+    unique_item_ids = set()
 
     unique_currency = set()
 
     planning_doctype = collections.Counter()
     planning_doc_count = 0
     tender_doctype = collections.Counter()
     tender_doc_count = 0
@@ -149,14 +150,16 @@
                 process_org(procuring_entity, unique_procuring_identifier, unique_procuring_name_no_id)
             tenderers = tender.get('tenderers', [])
             for tenderer in tenderers:
                 process_org(tenderer, unique_tenderers_identifier, unique_tenderers_name_no_id)
             tender_items = tender.get('items', [])
             for item in tender_items:
                 item_id = item.get('id')
+                if item_id:
+                    unique_item_ids.add(item_id)
                 if item_id and release_id:
                     release_tender_item_ids.add((ocid, release_id, item_id))
                 get_item_scheme(item)
             milestones = tender.get('milestones')
             if milestones:
                 for milestone in milestones:
                     tender_milestones_doc_count += tools.update_docs(milestone, tender_milestones_doctype)
@@ -173,14 +176,16 @@
                 awardid_ocids.add((award_id, ocid))
             award_date = award.get('date', '')
             if award_date:
                 award_dates.append(str(award_date))
             award_items = award.get('items', [])
             for item in award_items:
                 item_id = item.get('id')
+                if item_id:
+                    unique_item_ids.add(item_id)
                 if item_id and release_id and award_id:
                     release_award_item_ids.add((ocid, release_id, award_id, item_id))
                 get_item_scheme(item)
             suppliers = award.get('suppliers', [])
             for supplier in suppliers:
                 process_org(supplier, unique_suppliers_identifier, unique_suppliers_name_no_id)
             award_doc_count += tools.update_docs(award, award_doctype)
@@ -196,14 +201,16 @@
             if period:
                 start_date = period.get('startDate', '')
                 if start_date:
                     contract_dates.append(start_date)
             contract_items = contract.get('items', [])
             for item in contract_items:
                 item_id = item.get('id')
+                if item_id:
+                    unique_item_ids.add(item_id)
                 if item_id and release_id and contract_id:
                     release_contract_item_ids.add((ocid, release_id, contract_id, item_id))
                 get_item_scheme(item)
             contract_doc_count += tools.update_docs(contract, contract_doctype)
             implementation = contract.get('implementation')
             if implementation:
                 implementation_ocids.add(ocid)
@@ -311,14 +318,15 @@
         organisations_with_address=len(organisation_identifier_address) + len(organisation_name_no_id_address),
         organisations_with_contact_point=len(organisation_identifier_contact_point) + len(organisation_name_no_id_contact_point), # noqa
 
         total_item_count=len(release_tender_item_ids) + len(release_award_item_ids) + len(release_contract_item_ids),
         tender_item_count=len(release_tender_item_ids),
         award_item_count=len(release_award_item_ids),
         contract_item_count=len(release_contract_item_ids),
+        unique_item_ids_count=len(unique_item_ids),
 
         item_identifier_schemes=sorted(item_identifier_schemes, key=lambda x: str(x)),
         unique_currency=sorted(unique_currency, key=lambda x: str(x)),
 
         planning_doc_count=planning_doc_count,
         tender_doc_count=tender_doc_count,
         tender_milestones_doc_count=tender_milestones_doc_count,
```

### Comparing `libcoveocds-0.8.0/libcoveocds/lib/api.py` & `libcoveocds-0.9.1/libcoveocds/lib/api.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/libcoveocds/schema.py` & `libcoveocds-0.9.1/libcoveocds/schema.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/libcoveocds/common_checks.py` & `libcoveocds-0.9.1/libcoveocds/common_checks.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/libcoveocds/api.py` & `libcoveocds-0.9.1/libcoveocds/api.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/test_api.py` & `libcoveocds-0.9.1/tests/test_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import os
 import shutil
 import tempfile
 
 import pytest
 
+import libcoveocds.config
 from libcoveocds.api import APIException, ocds_json_output
 
+# Cache for faster tests.
+config = libcoveocds.config.LibCoveOCDSConfig()
+config.config['cache_all_requests'] = True
+
 
 def test_basic_1():
 
     cove_temp_folder = tempfile.mkdtemp(prefix='lib-cove-ocds-tests-', dir=tempfile.gettempdir())
     json_filename = os.path.join(os.path.dirname(
         os.path.realpath(__file__)), 'fixtures', 'api', 'basic_1.json'
     )
 
-    results = ocds_json_output(cove_temp_folder, json_filename, schema_version='', convert=False)
+    results = ocds_json_output(cove_temp_folder, json_filename, schema_version='', convert=False,
+                               lib_cove_ocds_config=config)
 
     assert results['version_used'] == '1.1'
 
 
 @pytest.mark.parametrize('json_data', ['{[,]}', '{"version": "1.bad"}'])
 def test_ocds_json_output_bad_data(json_data):
```

### Comparing `libcoveocds-0.8.0/tests/test_schema.py` & `libcoveocds-0.9.1/tests/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import copy
 
 import pytest
 
 import libcoveocds.config
 import libcoveocds.schema
 
+# Cache for faster tests.
+config = libcoveocds.config.LibCoveOCDSConfig()
+config.config['cache_all_requests'] = True
+
 DEFAULT_OCDS_VERSION = libcoveocds.config.LIB_COVE_OCDS_CONFIG_DEFAULT['schema_version']
 METRICS_EXT = 'https://raw.githubusercontent.com/open-contracting/ocds_metrics_extension/master/extension.json'
 CODELIST_EXT = 'https://raw.githubusercontent.com/INAImexico/ocds_extendedProcurementCategory_extension/0ed54770c85500cf21f46e88fb06a30a5a2132b1/extension.json' # noqa
 UNKNOWN_URL_EXT = 'http://bad-url-for-extensions.com/extension.json'
 NOT_FOUND_URL_EXT = 'https://standard.open-contracting.org/this-file-is-not-found-404.json/en'
 
 
@@ -97,15 +101,15 @@
      {UNKNOWN_URL_EXT: 'fetching failed'}, False, False),
     ({'version': '1.1', 'extensions': [METRICS_EXT]}, {METRICS_EXT: ()}, {}, True, True),
     ({'version': '1.1', 'extensions': [CODELIST_EXT]}, {CODELIST_EXT: ()}, {}, True, False),
     ({'version': '1.1', 'extensions': [UNKNOWN_URL_EXT, METRICS_EXT]}, {UNKNOWN_URL_EXT: (), METRICS_EXT: ()},
      {UNKNOWN_URL_EXT: 'fetching failed'}, True, True),
 ])
 def test_schema_ocds_extensions(release_data, extensions, invalid_extension, extended, extends_schema):
-    schema = libcoveocds.schema.SchemaOCDS(release_data=release_data)
+    schema = libcoveocds.schema.SchemaOCDS(release_data=release_data, lib_cove_ocds_config=config)
     assert schema.extensions == extensions
     assert not schema.extended
 
     schema_obj = schema.get_schema_obj()
     assert schema.invalid_extension == invalid_extension
     assert schema.extended == extended
```

### Comparing `libcoveocds-0.8.0/tests/lib/test_api.py` & `libcoveocds-0.9.1/tests/lib/test_api.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/lib/fixtures/common_checks/badfile.json` & `libcoveocds-0.9.1/tests/lib/fixtures/common_checks/badfile.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/lib/fixtures/common_checks/samplerubbish.json` & `libcoveocds-0.9.1/tests/lib/fixtures/common_checks/samplerubbish.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/lib/fixtures/common_checks/record_check_ocids.json` & `libcoveocds-0.9.1/tests/lib/fixtures/common_checks/record_check_ocids.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/lib/fixtures/common_checks/release_aggregate.json` & `libcoveocds-0.9.1/tests/lib/fixtures/common_checks/release_aggregate.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/lib/fixtures/common_checks/tenders_releases_7_releases_check_ocids.json` & `libcoveocds-0.9.1/tests/lib/fixtures/common_checks/tenders_releases_7_releases_check_ocids.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/lib/test_common_checks.py` & `libcoveocds-0.9.1/tests/lib/test_common_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     'tender_count': 0,
     'unique_award_id': [],
     'unique_buyers_count': 0,
     'unique_buyers_identifier': {},
     'unique_buyers_name_no_id': [],
     'unique_currency': [],
     'unique_initation_type': [],
+    'unique_item_ids_count': 0,
     'unique_lang': [],
     'unique_ocids': [],
     'unique_org_count': 0,
     'unique_org_identifier_count': 0,
     'unique_org_name_count': 0,
     'unique_organisation_schemes': [],
     'unique_procuring_count': 0,
@@ -118,14 +119,15 @@
     'tender_milestones_doctype': {'doctype1': 2, 'doctype2': 1},
     'unique_award_id': ['1', '2'],
     'unique_buyers_count': 1,
     'unique_buyers_identifier': {'1': 'Gov'},
     'unique_buyers_name_no_id': [],
     'unique_currency': ['EUR', 'GBP', 'USD', 'YEN'],
     'unique_initation_type': ['tender'],
+    'unique_item_ids_count': 2,
     'unique_lang': ['English'],
     'unique_ocids': ['1'],
     'unique_org_count': 4,
     'unique_org_identifier_count': 2,
     'unique_org_name_count': 2,
     'unique_organisation_schemes': ['a', 'b'],
     'unique_procuring_count': 1,
@@ -171,14 +173,15 @@
     'planning_doc_count': 738,
     'release_count': 1005,
     'tender_count': 467,
     'tender_doc_count': 799,
     'tender_item_count': 770,
     'tender_milestones_doc_count': 1163,
     'unique_buyers_count': 169,
+    'unique_item_ids_count': 4698,
     'unique_org_count': 1339,
     'unique_org_identifier_count': 625,
     'unique_org_name_count': 714,
     'unique_procuring_count': 94,
     'unique_suppliers_count': 812,
     'unique_tenderers_count': 286,
     'processes_award_count': 466,
```

### Comparing `libcoveocds-0.8.0/tests/fixtures/additional_checks/empty_fields_releases.json` & `libcoveocds-0.9.1/tests/fixtures/additional_checks/empty_fields_releases.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/additional_checks/basic_releases.json` & `libcoveocds-0.9.1/tests/fixtures/additional_checks/basic_releases.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/additional_checks/empty_fields_records.json` & `libcoveocds-0.9.1/tests/fixtures/additional_checks/empty_fields_records.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/additional_checks/full_record.json` & `libcoveocds-0.9.1/tests/fixtures/additional_checks/full_record.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/api/basic_1.json` & `libcoveocds-0.9.1/tests/fixtures/api/basic_1.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/dupe_ids_1.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/dupe_ids_1.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/records_non_unique.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/records_non_unique.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/records_unique.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/records_unique.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/releases_unique.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/releases_unique.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/basic_1.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/basic_1.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/releases_non_unique_no_id.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/releases_non_unique_no_id.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/releases_non_unique.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/releases_non_unique.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/records_invalid_releases.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/records_invalid_releases.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/fixtures/common_checks/1-0/records_invalid_releases.json` & `libcoveocds-0.9.1/tests/fixtures/common_checks/1-0/records_invalid_releases.json`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/tests/test_common_checks.py` & `libcoveocds-0.9.1/tests/test_common_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 import os
 import shutil
 import tempfile
 
 import pytest
 
 import libcoveocds.common_checks
+import libcoveocds.config
 import libcoveocds.schema
 
+# Cache for faster tests.
+config = libcoveocds.config.LibCoveOCDSConfig()
+config.config['cache_all_requests'] = True
+
 
 def test_basic_1():
 
     cove_temp_folder = tempfile.mkdtemp(prefix='libcoveocds-tests-', dir=tempfile.gettempdir())
-    schema = libcoveocds.schema.SchemaOCDS()
+    schema = libcoveocds.schema.SchemaOCDS(lib_cove_ocds_config=config)
     json_filename = os.path.join(os.path.dirname(
         os.path.realpath(__file__)), 'fixtures', 'common_checks', 'basic_1.json'
     )
     with open(json_filename) as fp:
         json_data = json.load(fp)
 
     context = {
@@ -37,15 +42,15 @@
 
     assert results['version_used'] == '1.1'
 
 
 def test_dupe_ids_1():
 
     cove_temp_folder = tempfile.mkdtemp(prefix='libcoveocds-tests-', dir=tempfile.gettempdir())
-    schema = libcoveocds.schema.SchemaOCDS()
+    schema = libcoveocds.schema.SchemaOCDS(lib_cove_ocds_config=config)
     json_filename = os.path.join(os.path.dirname(
         os.path.realpath(__file__)), 'fixtures', 'common_checks', 'dupe_ids_1.json'
     )
     with open(json_filename) as fp:
         json_data = json.load(fp)
 
     context = {
@@ -77,20 +82,20 @@
     ]
     values.sort()
     assert values[0] == 'ocds-213czf-000-00001-01-planning'
     assert values[1] == 'ocds-213czf-000-00001-02-planning'
 
 
 @pytest.mark.parametrize(
-    "package_schema_filename,filename,schema_subdir,validation_error_jsons_expected",
+    "record_pkg,filename,schema_subdir,validation_error_jsons_expected",
     [
-        ("release-package-schema.json", "releases_no_validation_errors.json", "", []),
-        ("record-package-schema.json", "records_no_validation_errors.json", "", []),
+        (False, "releases_no_validation_errors.json", "", []),
+        (True, "records_no_validation_errors.json", "", []),
         (
-            "record-package-schema.json",
+            True,
             "records_invalid_releases.json",
             "",
             [
                 {
                     "message": "'date' is missing but required within 'releases'",
                     "message_safe": "<code>date</code> is missing but required within <code>releases</code>",
                     "validator": "required",
@@ -216,15 +221,15 @@
                     "null_clause": "",
                     "error_id": None,
                     "values": [{"path": "records/0/releases"}],
                 },
             ],
         ),
         (
-            "record-package-schema.json",
+            True,
             "records_invalid_releases.json",
             "1-0",
             [
                 {
                     "message": "'date' is missing but required within 'releases'",
                     "message_safe": "<code>date</code> is missing but required within <code>releases</code>",
                     "validator": "required",
@@ -350,15 +355,15 @@
                     "null_clause": "",
                     "error_id": None,
                     "values": [{"path": "records/0/releases"}],
                 },
             ],
         ),
         (
-            "release-package-schema.json",
+            False,
             "releases_non_unique.json",
             "",
             [
                 {
                     "message": "Non-unique id values",
                     "message_safe": "Non-unique id values",
                     "validator": "uniqueItems",
@@ -373,15 +378,15 @@
                         {"path": "releases", "value": "EXAMPLE-1-1"},
                         {"path": "releases", "value": "EXAMPLE-1-2"},
                     ],
                 }
             ],
         ),
         (
-            "record-package-schema.json",
+            True,
             "records_non_unique.json",
             "",
             [
                 {
                     "message": "Non-unique ocid values",
                     "message_safe": "Non-unique ocid values",
                     "validator": "uniqueItems",
@@ -396,15 +401,15 @@
                         {"path": "records", "value": "EXAMPLE-1"},
                         {"path": "records", "value": "EXAMPLE-2"},
                     ],
                 }
             ],
         ),
         (
-            "release-package-schema.json",
+            False,
             "releases_non_unique_no_id.json",
             "",
             [
                 {
                     "message": "'id' is missing but required",
                     "message_safe": "<code>id</code> is missing but required",
                     "validator": "required",
@@ -429,15 +434,15 @@
                     "null_clause": "",
                     "error_id": "uniqueItems_no_ids",
                     "values": [{"path": "releases"}],
                 },
             ],
         ),
         (
-            "record-package-schema.json",
+            True,
             "records_non_unique_no_ocid.json",
             "",
             [
                 {
                     "message": "'ocid' is missing but required",
                     "message_safe": "<code>ocid</code> is missing but required",
                     "validator": "required",
@@ -464,15 +469,15 @@
                     "values": [{"path": "records"}],
                 },
             ],
         ),
         # Check that we handle unique arrays correctly also
         # (e.g. that we don't incorrectly claim they are not unique)
         (
-            "release-package-schema.json",
+            False,
             "releases_unique.json",
             "",
             [
                 {
                     "message": "'id' is missing but required",
                     "message_safe": "<code>id</code> is missing but required",
                     "validator": "required",
@@ -484,15 +489,15 @@
                     "null_clause": "",
                     "error_id": None,
                     "values": [{"path": "releases/0"}, {"path": "releases/1"}],
                 }
             ],
         ),
         (
-            "record-package-schema.json",
+            True,
             "records_unique.json",
             "",
             [
                 {
                     "message": "'ocid' is missing but required",
                     "message_safe": "<code>ocid</code> is missing but required",
                     "validator": "required",
@@ -506,31 +511,28 @@
                     "values": [{"path": "records/0"}, {"path": "records/1"}],
                 }
             ],
         ),
     ],
 )
 def test_validation_release_or_record_package(
-    package_schema_filename, filename, validation_error_jsons_expected, schema_subdir
+    record_pkg, filename, validation_error_jsons_expected, schema_subdir
 ):
     schema_host = os.path.join(
         os.path.dirname(os.path.realpath(__file__)),
         "fixtures",
         "common_checks",
         schema_subdir,
         "",
     )
     with open(os.path.join(schema_host, filename)) as fp:
         json_data = json.load(fp)
 
     cove_temp_folder = tempfile.mkdtemp(prefix='libcoveocds-tests-', dir=tempfile.gettempdir())
-    if package_schema_filename == 'record-package-schema.json':
-        schema = libcoveocds.schema.SchemaOCDS(record_pkg=True)
-    else:
-        schema = libcoveocds.schema.SchemaOCDS(record_pkg=False)
+    schema = libcoveocds.schema.SchemaOCDS(lib_cove_ocds_config=config, record_pkg=record_pkg)
     context = {
         'file_type': 'json',
     }
 
     results = libcoveocds.common_checks.common_checks_ocds(
         context,
         cove_temp_folder,
```

### Comparing `libcoveocds-0.8.0/tests/test_additional_checks.py` & `libcoveocds-0.9.1/tests/test_additional_checks.py`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/LICENSE` & `libcoveocds-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libcoveocds-0.8.0/libcoveocds.egg-info/SOURCES.txt` & `libcoveocds-0.9.1/libcoveocds.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 libcoveocds/lib/__init__.py
 libcoveocds/lib/additional_checks.py
 libcoveocds/lib/api.py
 libcoveocds/lib/common_checks.py
 tests/__init__.py
 tests/test_additional_checks.py
 tests/test_api.py
+tests/test_cli.py
 tests/test_common_checks.py
 tests/test_schema.py
 tests/fixtures/additional_checks/basic_releases.json
 tests/fixtures/additional_checks/empty_fields_records.json
 tests/fixtures/additional_checks/empty_fields_releases.json
 tests/fixtures/additional_checks/full_record.json
 tests/fixtures/api/basic_1.json
```

### Comparing `libcoveocds-0.8.0/setup.py` & `libcoveocds-0.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from setuptools import find_packages, setup
 
 with open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='libcoveocds',
-    version='0.8.0',
+    version='0.9.1',
     author='Open Data Services',
     author_email='data@open-contracting.org',
     url='https://github.com/open-contracting/lib-cove-ocds',
     description='A data review library for the Open Contracting Data Standard (OCDS)',
     license='AGPLv3',
     packages=find_packages(exclude=['tests', 'tests.*']),
     long_description=long_description,
     install_requires=[
-        'libcove>=0.18.0',
+        'libcove>=0.19.0',
         'bleach',
         'cached-property',
         'CommonMark',
         'Django',
         'json-merge-patch',
         'requests',
+        'click',
     ],
     extras_require={
         'test': [
             'coveralls',
             'pytest',
             'pytest-cov',
             'isort',
```

