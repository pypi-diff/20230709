# Comparing `tmp/aura-cli-0.2.tar.gz` & `tmp/aura-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura-cli-0.2.tar", last modified: Sat Jul  8 10:25:53 2023, max compression
+gzip compressed data, was "aura-cli-0.2.1.tar", last modified: Sun Jul  9 15:57:39 2023, max compression
```

## Comparing `aura-cli-0.2.tar` & `aura-cli-0.2.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2023-06-20 10:41:04.000000 aura-cli-0.2/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       72 2023-07-08 10:25:53.736949 aura-cli-0.2/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2566 2023-06-26 19:07:36.000000 aura-cli-0.2/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.732949 aura-cli-0.2/aura/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 18:27:12.000000 aura-cli-0.2/aura/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2081 2023-07-08 08:28:00.000000 aura-cli-0.2/aura/api_command.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2379 2023-07-08 08:28:05.000000 aura-cli-0.2/aura/api_repository.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      471 2023-06-24 14:36:06.000000 aura-cli-0.2/aura/aura.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.732949 aura-cli-0.2/aura/config/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      494 2023-07-08 09:46:09.000000 aura-cli-0.2/aura/config/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      800 2023-07-08 08:43:04.000000 aura-cli-0.2/aura/config/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      516 2023-07-08 09:03:13.000000 aura-cli-0.2/aura/config/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      927 2023-07-08 09:04:25.000000 aura-cli-0.2/aura/config/set.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      716 2023-07-08 09:15:27.000000 aura-cli-0.2/aura/config/unset.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      133 2023-06-24 14:37:07.000000 aura-cli-0.2/aura/config/valid_options.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5121 2023-06-26 18:49:34.000000 aura-cli-0.2/aura/config_repository.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.732949 aura-cli-0.2/aura/credentials/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      545 2023-07-08 10:09:22.000000 aura-cli-0.2/aura/credentials/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      870 2023-06-21 12:33:43.000000 aura-cli-0.2/aura/credentials/add.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      561 2023-06-21 12:34:21.000000 aura-cli-0.2/aura/credentials/current.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      401 2023-06-21 12:34:40.000000 aura-cli-0.2/aura/credentials/delete.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      738 2023-07-08 07:46:57.000000 aura-cli-0.2/aura/credentials/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      416 2023-06-21 12:35:14.000000 aura-cli-0.2/aura/credentials/use.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      238 2023-06-21 12:36:06.000000 aura-cli-0.2/aura/decorators.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1819 2023-07-08 08:09:16.000000 aura-cli-0.2/aura/error_handler.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1542 2023-07-03 14:02:40.000000 aura-cli-0.2/aura/format.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/aura/instances/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      535 2023-05-19 12:30:19.000000 aura-cli-0.2/aura/instances/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1348 2023-07-03 14:07:45.000000 aura-cli-0.2/aura/instances/create.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      784 2023-06-17 10:39:44.000000 aura-cli-0.2/aura/instances/delete.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      511 2023-06-17 10:45:40.000000 aura-cli-0.2/aura/instances/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      595 2023-06-24 15:32:01.000000 aura-cli-0.2/aura/instances/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      722 2023-07-03 14:35:54.000000 aura-cli-0.2/aura/instances/overwrite.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      522 2023-06-17 11:09:34.000000 aura-cli-0.2/aura/instances/pause.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      521 2023-06-17 11:11:13.000000 aura-cli-0.2/aura/instances/resume.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      836 2023-06-17 11:14:28.000000 aura-cli-0.2/aura/instances/update.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/aura/snapshots/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      304 2023-07-06 10:21:04.000000 aura-cli-0.2/aura/snapshots/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      561 2023-06-15 20:54:01.000000 aura-cli-0.2/aura/snapshots/create.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      709 2023-07-06 10:20:44.000000 aura-cli-0.2/aura/snapshots/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      738 2023-06-16 07:56:52.000000 aura-cli-0.2/aura/snapshots/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      734 2023-06-16 08:05:10.000000 aura-cli-0.2/aura/snapshots/restore.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/aura/tenants/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      175 2023-06-10 11:35:15.000000 aura-cli-0.2/aura/tenants/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      583 2023-06-26 18:40:12.000000 aura-cli-0.2/aura/tenants/get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2023-06-15 19:18:24.000000 aura-cli-0.2/aura/tenants/list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1151 2023-07-06 10:06:00.000000 aura-cli-0.2/aura/token_repository.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/aura/util/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-20 11:11:37.000000 aura-cli-0.2/aura/util/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1398 2023-06-26 18:28:03.000000 aura-cli-0.2/aura/util/get_instance_id.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/aura_cli.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       72 2023-07-08 10:25:53.000000 aura-cli-0.2/aura_cli.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2006 2023-07-08 10:25:53.000000 aura-cli-0.2/aura_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-08 10:25:53.000000 aura-cli-0.2/aura_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       39 2023-07-08 10:25:53.000000 aura-cli-0.2/aura_cli.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2023-07-08 10:25:53.000000 aura-cli-0.2/aura_cli.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-08 10:25:53.000000 aura-cli-0.2/aura_cli.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-08 10:25:53.736949 aura-cli-0.2/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      281 2023-07-08 10:07:23.000000 aura-cli-0.2/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2/tests/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/tests/config/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-08 08:43:49.000000 aura-cli-0.2/tests/config/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1399 2023-07-08 08:56:56.000000 aura-cli-0.2/tests/config/test_get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      717 2023-07-08 09:02:21.000000 aura-cli-0.2/tests/config/test_list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1006 2023-07-08 09:12:13.000000 aura-cli-0.2/tests/config/test_set.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      966 2023-07-08 09:16:52.000000 aura-cli-0.2/tests/config/test_unset.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      789 2023-07-08 09:25:40.000000 aura-cli-0.2/tests/conftest.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/tests/credentials/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-21 12:53:58.000000 aura-cli-0.2/tests/credentials/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      672 2023-06-21 13:45:07.000000 aura-cli-0.2/tests/credentials/test_add.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1070 2023-06-21 13:54:02.000000 aura-cli-0.2/tests/credentials/test_current.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2023-06-21 13:56:52.000000 aura-cli-0.2/tests/credentials/test_delete.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      907 2023-07-08 09:40:07.000000 aura-cli-0.2/tests/credentials/test_list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1060 2023-06-21 14:22:47.000000 aura-cli-0.2/tests/credentials/test_use.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/tests/instances/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2/tests/instances/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3355 2023-07-08 09:29:58.000000 aura-cli-0.2/tests/instances/test_create.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1608 2023-07-08 09:30:29.000000 aura-cli-0.2/tests/instances/test_delete.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1761 2023-07-08 09:31:13.000000 aura-cli-0.2/tests/instances/test_get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1549 2023-07-08 09:34:25.000000 aura-cli-0.2/tests/instances/test_list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1803 2023-07-08 09:35:11.000000 aura-cli-0.2/tests/instances/test_overwrite.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1603 2023-07-08 09:36:01.000000 aura-cli-0.2/tests/instances/test_pause.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1611 2023-07-08 09:36:27.000000 aura-cli-0.2/tests/instances/test_resume.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3010 2023-07-08 09:37:26.000000 aura-cli-0.2/tests/instances/test_update.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/tests/snapshots/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2/tests/snapshots/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1614 2023-07-08 09:27:31.000000 aura-cli-0.2/tests/snapshots/test_create.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2873 2023-07-08 09:28:20.000000 aura-cli-0.2/tests/snapshots/test_list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1853 2023-07-08 09:28:53.000000 aura-cli-0.2/tests/snapshots/test_restore.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-08 10:25:53.736949 aura-cli-0.2/tests/tenants/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2/tests/tenants/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      878 2023-07-08 09:26:35.000000 aura-cli-0.2/tests/tenants/test_get.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      865 2023-07-08 09:26:46.000000 aura-cli-0.2/tests/tenants/test_list.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:43.000000 aura-cli-0.2/tests/test_api_repository.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1072 2023-06-20 10:41:04.000000 aura-cli-0.2.1/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2023-07-09 15:57:39.709227 aura-cli-0.2.1/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2566 2023-06-26 19:07:36.000000 aura-cli-0.2.1/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.705227 aura-cli-0.2.1/aura/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 18:27:12.000000 aura-cli-0.2.1/aura/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2081 2023-07-08 08:28:00.000000 aura-cli-0.2.1/aura/api_command.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2379 2023-07-08 08:28:05.000000 aura-cli-0.2.1/aura/api_repository.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      531 2023-07-09 15:53:06.000000 aura-cli-0.2.1/aura/aura.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.705227 aura-cli-0.2.1/aura/config/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      494 2023-07-08 09:46:09.000000 aura-cli-0.2.1/aura/config/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      800 2023-07-08 08:43:04.000000 aura-cli-0.2.1/aura/config/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      516 2023-07-08 09:03:13.000000 aura-cli-0.2.1/aura/config/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      927 2023-07-08 09:04:25.000000 aura-cli-0.2.1/aura/config/set.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      716 2023-07-08 09:15:27.000000 aura-cli-0.2.1/aura/config/unset.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      133 2023-06-24 14:37:07.000000 aura-cli-0.2.1/aura/config/valid_options.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5121 2023-06-26 18:49:34.000000 aura-cli-0.2.1/aura/config_repository.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.705227 aura-cli-0.2.1/aura/credentials/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      545 2023-07-08 10:09:22.000000 aura-cli-0.2.1/aura/credentials/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      870 2023-06-21 12:33:43.000000 aura-cli-0.2.1/aura/credentials/add.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      561 2023-06-21 12:34:21.000000 aura-cli-0.2.1/aura/credentials/current.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      401 2023-06-21 12:34:40.000000 aura-cli-0.2.1/aura/credentials/delete.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      738 2023-07-08 07:46:57.000000 aura-cli-0.2.1/aura/credentials/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      416 2023-06-21 12:35:14.000000 aura-cli-0.2.1/aura/credentials/use.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      238 2023-06-21 12:36:06.000000 aura-cli-0.2.1/aura/decorators.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1819 2023-07-08 08:09:16.000000 aura-cli-0.2.1/aura/error_handler.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1542 2023-07-03 14:02:40.000000 aura-cli-0.2.1/aura/format.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.705227 aura-cli-0.2.1/aura/instances/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      535 2023-05-19 12:30:19.000000 aura-cli-0.2.1/aura/instances/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1348 2023-07-03 14:07:45.000000 aura-cli-0.2.1/aura/instances/create.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      784 2023-06-17 10:39:44.000000 aura-cli-0.2.1/aura/instances/delete.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      511 2023-06-17 10:45:40.000000 aura-cli-0.2.1/aura/instances/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      595 2023-06-24 15:32:01.000000 aura-cli-0.2.1/aura/instances/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      722 2023-07-03 14:35:54.000000 aura-cli-0.2.1/aura/instances/overwrite.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      522 2023-06-17 11:09:34.000000 aura-cli-0.2.1/aura/instances/pause.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      521 2023-06-17 11:11:13.000000 aura-cli-0.2.1/aura/instances/resume.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      836 2023-06-17 11:14:28.000000 aura-cli-0.2.1/aura/instances/update.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.705227 aura-cli-0.2.1/aura/snapshots/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      304 2023-07-06 10:21:04.000000 aura-cli-0.2.1/aura/snapshots/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      561 2023-06-15 20:54:01.000000 aura-cli-0.2.1/aura/snapshots/create.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      709 2023-07-06 10:20:44.000000 aura-cli-0.2.1/aura/snapshots/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      738 2023-06-16 07:56:52.000000 aura-cli-0.2.1/aura/snapshots/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      734 2023-06-16 08:05:10.000000 aura-cli-0.2.1/aura/snapshots/restore.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.705227 aura-cli-0.2.1/aura/tenants/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      175 2023-06-10 11:35:15.000000 aura-cli-0.2.1/aura/tenants/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      583 2023-06-26 18:40:12.000000 aura-cli-0.2.1/aura/tenants/get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2023-06-15 19:18:24.000000 aura-cli-0.2.1/aura/tenants/list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1151 2023-07-06 10:06:00.000000 aura-cli-0.2.1/aura/token_repository.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.705227 aura-cli-0.2.1/aura/util/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-20 11:11:37.000000 aura-cli-0.2.1/aura/util/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1398 2023-06-26 18:28:03.000000 aura-cli-0.2.1/aura/util/get_instance_id.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/aura_cli.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2023-07-09 15:57:39.000000 aura-cli-0.2.1/aura_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2006 2023-07-09 15:57:39.000000 aura-cli-0.2.1/aura_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-09 15:57:39.000000 aura-cli-0.2.1/aura_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       39 2023-07-09 15:57:39.000000 aura-cli-0.2.1/aura_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2023-07-09 15:57:39.000000 aura-cli-0.2.1/aura_cli.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-09 15:57:39.000000 aura-cli-0.2.1/aura_cli.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-09 15:57:39.709227 aura-cli-0.2.1/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      283 2023-07-09 15:51:03.000000 aura-cli-0.2.1/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2.1/tests/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/tests/config/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-08 08:43:49.000000 aura-cli-0.2.1/tests/config/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1399 2023-07-08 08:56:56.000000 aura-cli-0.2.1/tests/config/test_get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      717 2023-07-08 09:02:21.000000 aura-cli-0.2.1/tests/config/test_list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1006 2023-07-08 09:12:13.000000 aura-cli-0.2.1/tests/config/test_set.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      966 2023-07-08 09:16:52.000000 aura-cli-0.2.1/tests/config/test_unset.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      789 2023-07-08 09:25:40.000000 aura-cli-0.2.1/tests/conftest.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/tests/credentials/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-21 12:53:58.000000 aura-cli-0.2.1/tests/credentials/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      672 2023-06-21 13:45:07.000000 aura-cli-0.2.1/tests/credentials/test_add.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1070 2023-06-21 13:54:02.000000 aura-cli-0.2.1/tests/credentials/test_current.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      563 2023-06-21 13:56:52.000000 aura-cli-0.2.1/tests/credentials/test_delete.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      907 2023-07-08 09:40:07.000000 aura-cli-0.2.1/tests/credentials/test_list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1060 2023-06-21 14:22:47.000000 aura-cli-0.2.1/tests/credentials/test_use.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/tests/instances/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2.1/tests/instances/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3355 2023-07-08 09:29:58.000000 aura-cli-0.2.1/tests/instances/test_create.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1608 2023-07-08 09:30:29.000000 aura-cli-0.2.1/tests/instances/test_delete.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1761 2023-07-08 09:31:13.000000 aura-cli-0.2.1/tests/instances/test_get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1549 2023-07-08 09:34:25.000000 aura-cli-0.2.1/tests/instances/test_list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1803 2023-07-08 09:35:11.000000 aura-cli-0.2.1/tests/instances/test_overwrite.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1603 2023-07-08 09:36:01.000000 aura-cli-0.2.1/tests/instances/test_pause.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1611 2023-07-08 09:36:27.000000 aura-cli-0.2.1/tests/instances/test_resume.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3010 2023-07-08 09:37:26.000000 aura-cli-0.2.1/tests/instances/test_update.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/tests/snapshots/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2.1/tests/snapshots/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1614 2023-07-08 09:27:31.000000 aura-cli-0.2.1/tests/snapshots/test_create.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2873 2023-07-08 09:28:20.000000 aura-cli-0.2.1/tests/snapshots/test_list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1853 2023-07-08 09:28:53.000000 aura-cli-0.2.1/tests/snapshots/test_restore.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-09 15:57:39.709227 aura-cli-0.2.1/tests/tenants/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:44.000000 aura-cli-0.2.1/tests/tenants/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      878 2023-07-08 09:26:35.000000 aura-cli-0.2.1/tests/tenants/test_get.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      865 2023-07-08 09:26:46.000000 aura-cli-0.2.1/tests/tenants/test_list.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-13 16:55:43.000000 aura-cli-0.2.1/tests/test_api_repository.py
```

### Comparing `aura-cli-0.2/LICENSE` & `aura-cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/README.md` & `aura-cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/api_command.py` & `aura-cli-0.2.1/aura/api_command.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/api_repository.py` & `aura-cli-0.2.1/aura/api_repository.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/config/get.py` & `aura-cli-0.2.1/aura/config/get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/config/list.py` & `aura-cli-0.2.1/aura/config/list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/config/set.py` & `aura-cli-0.2.1/aura/config/set.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/config/unset.py` & `aura-cli-0.2.1/aura/config/unset.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/config_repository.py` & `aura-cli-0.2.1/aura/config_repository.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/credentials/__init__.py` & `aura-cli-0.2.1/aura/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/credentials/add.py` & `aura-cli-0.2.1/aura/credentials/add.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/credentials/current.py` & `aura-cli-0.2.1/aura/credentials/current.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/credentials/list.py` & `aura-cli-0.2.1/aura/credentials/list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/error_handler.py` & `aura-cli-0.2.1/aura/error_handler.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/format.py` & `aura-cli-0.2.1/aura/format.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/__init__.py` & `aura-cli-0.2.1/aura/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/create.py` & `aura-cli-0.2.1/aura/instances/create.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/delete.py` & `aura-cli-0.2.1/aura/instances/delete.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/list.py` & `aura-cli-0.2.1/aura/instances/list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/overwrite.py` & `aura-cli-0.2.1/aura/instances/overwrite.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/pause.py` & `aura-cli-0.2.1/aura/instances/pause.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/resume.py` & `aura-cli-0.2.1/aura/instances/resume.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/instances/update.py` & `aura-cli-0.2.1/aura/instances/update.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/snapshots/create.py` & `aura-cli-0.2.1/aura/snapshots/create.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/snapshots/get.py` & `aura-cli-0.2.1/aura/snapshots/get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/snapshots/list.py` & `aura-cli-0.2.1/aura/snapshots/list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/snapshots/restore.py` & `aura-cli-0.2.1/aura/snapshots/restore.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/tenants/get.py` & `aura-cli-0.2.1/aura/tenants/get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/token_repository.py` & `aura-cli-0.2.1/aura/token_repository.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura/util/get_instance_id.py` & `aura-cli-0.2.1/aura/util/get_instance_id.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/aura_cli.egg-info/SOURCES.txt` & `aura-cli-0.2.1/aura_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/config/test_get.py` & `aura-cli-0.2.1/tests/config/test_get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/config/test_list.py` & `aura-cli-0.2.1/tests/config/test_list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/config/test_set.py` & `aura-cli-0.2.1/tests/config/test_set.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/config/test_unset.py` & `aura-cli-0.2.1/tests/config/test_unset.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/conftest.py` & `aura-cli-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/credentials/test_add.py` & `aura-cli-0.2.1/tests/credentials/test_add.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/credentials/test_current.py` & `aura-cli-0.2.1/tests/credentials/test_current.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/credentials/test_delete.py` & `aura-cli-0.2.1/tests/credentials/test_delete.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/credentials/test_list.py` & `aura-cli-0.2.1/tests/credentials/test_list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/credentials/test_use.py` & `aura-cli-0.2.1/tests/credentials/test_use.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_create.py` & `aura-cli-0.2.1/tests/instances/test_create.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_delete.py` & `aura-cli-0.2.1/tests/instances/test_delete.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_get.py` & `aura-cli-0.2.1/tests/instances/test_get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_list.py` & `aura-cli-0.2.1/tests/instances/test_list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_overwrite.py` & `aura-cli-0.2.1/tests/instances/test_overwrite.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_pause.py` & `aura-cli-0.2.1/tests/instances/test_pause.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_resume.py` & `aura-cli-0.2.1/tests/instances/test_resume.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/instances/test_update.py` & `aura-cli-0.2.1/tests/instances/test_update.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/snapshots/test_create.py` & `aura-cli-0.2.1/tests/snapshots/test_create.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/snapshots/test_list.py` & `aura-cli-0.2.1/tests/snapshots/test_list.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/snapshots/test_restore.py` & `aura-cli-0.2.1/tests/snapshots/test_restore.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/tenants/test_get.py` & `aura-cli-0.2.1/tests/tenants/test_get.py`

 * *Files identical despite different names*

### Comparing `aura-cli-0.2/tests/tenants/test_list.py` & `aura-cli-0.2.1/tests/tenants/test_list.py`

 * *Files identical despite different names*

