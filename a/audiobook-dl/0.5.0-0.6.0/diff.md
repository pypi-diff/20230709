# Comparing `tmp/audiobook-dl-0.5.0.tar.gz` & `tmp/audiobook-dl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-dl-0.5.0.tar", last modified: Mon Apr 10 11:40:48 2023, max compression
+gzip compressed data, was "audiobook-dl-0.6.0.tar", last modified: Sun Jul  9 17:36:37 2023, max compression
```

## Comparing `audiobook-dl-0.5.0.tar` & `audiobook-dl-0.6.0.tar`

### file list

```diff
@@ -1,77 +1,87 @@
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.200801 audiobook-dl-0.5.0/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.183801 audiobook-dl-0.5.0/.github/
--rw-r--r--   0 jo1gi     (1000) users      (100)       13 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/.github/FUNDING.yml
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.183801 audiobook-dl-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 jo1gi     (1000) users      (100)      349 2023-03-21 07:18:57.000000 audiobook-dl-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.184801 audiobook-dl-0.5.0/.github/workflows/
--rw-r--r--   0 jo1gi     (1000) users      (100)      315 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-01-19 22:18:06.000000 audiobook-dl-0.5.0/.github/workflows/pytest.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      539 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/.gitignore
--rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/LICENSE
--rw-r--r--   0 jo1gi     (1000) users      (100)     4902 2023-04-10 11:40:48.200801 audiobook-dl-0.5.0/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     4331 2023-04-07 08:43:53.000000 audiobook-dl-0.5.0/README.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.186801 audiobook-dl-0.5.0/audiobook_dl.egg-info/
--rw-r--r--   0 jo1gi     (1000) users      (100)     4902 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     1935 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/SOURCES.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/dependency_links.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       58 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/entry_points.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       82 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/requires.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-04-10 11:40:48.000000 audiobook-dl-0.5.0/audiobook_dl.egg-info/top_level.txt
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.188801 audiobook-dl-0.5.0/audiobookdl/
--rw-r--r--   0 jo1gi     (1000) users      (100)      167 2023-04-10 11:35:29.000000 audiobook-dl-0.5.0/audiobookdl/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3102 2023-04-06 21:14:29.000000 audiobook-dl-0.5.0/audiobookdl/__main__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2696 2023-04-05 19:24:53.000000 audiobook-dl-0.5.0/audiobookdl/args.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.188801 audiobook-dl-0.5.0/audiobookdl/assets/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.191801 audiobook-dl-0.5.0/audiobookdl/assets/errors/
--rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-02-05 08:49:39.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/book_access.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-02-16 19:20:53.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/chapters_add.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      468 2022-09-01 08:49:16.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/data_not_present.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       45 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/failed_combining.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-02-16 19:20:51.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/missing_dependency.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/no_files_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-02-02 07:28:40.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/no_source_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       55 2022-04-05 11:33:45.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/request_error.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-01-19 21:44:13.000000 audiobook-dl-0.5.0/audiobookdl/assets/errors/user_not_authorized.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-02-16 17:36:53.000000 audiobook-dl-0.5.0/audiobookdl/assets/ffmpeg_chapter_template.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      317 2022-03-16 08:34:25.000000 audiobook-dl-0.5.0/audiobookdl/assets/simple_help.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)     1254 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/exceptions.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1401 2023-04-10 11:35:15.000000 audiobook-dl-0.5.0/audiobookdl/logging.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.193801 audiobook-dl-0.5.0/audiobookdl/output/
--rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-01-19 21:44:13.000000 audiobook-dl-0.5.0/audiobookdl/output/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     6858 2023-04-06 21:10:31.000000 audiobook-dl-0.5.0/audiobookdl/output/download.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      641 2023-04-03 16:18:40.000000 audiobook-dl-0.5.0/audiobookdl/output/encryption.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1786 2023-04-05 18:17:14.000000 audiobook-dl-0.5.0/audiobookdl/output/formats.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.194801 audiobook-dl-0.5.0/audiobookdl/output/metadata/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1340 2023-04-09 10:25:30.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-02-16 20:23:47.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/ffmpeg.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2435 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/id3.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1476 2023-04-09 10:22:01.000000 audiobook-dl-0.5.0/audiobookdl/output/metadata/mp4.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2476 2023-04-02 15:33:26.000000 audiobook-dl-0.5.0/audiobookdl/output/output.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.198801 audiobook-dl-0.5.0/audiobookdl/sources/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1548 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1589 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/audiobooksdotcom.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4230 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/bookbeat.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4001 2023-04-05 12:31:35.000000 audiobook-dl-0.5.0/audiobookdl/sources/chirp.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3373 2023-04-06 11:50:10.000000 audiobook-dl-0.5.0/audiobookdl/sources/ereolen.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1067 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/librivox.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4750 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/nextory.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2914 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/overdrive.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      155 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/rss.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4078 2023-04-09 09:22:07.000000 audiobook-dl-0.5.0/audiobookdl/sources/saxo.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5187 2023-04-10 11:35:19.000000 audiobook-dl-0.5.0/audiobookdl/sources/scribd.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.198801 audiobook-dl-0.5.0/audiobookdl/sources/source/
--rw-r--r--   0 jo1gi     (1000) users      (100)     5146 2023-04-10 11:35:15.000000 audiobook-dl-0.5.0/audiobookdl/sources/source/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2374 2023-04-10 11:35:19.000000 audiobook-dl-0.5.0/audiobookdl/sources/source/networking.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4311 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/storytel.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4169 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/sources/yourcloudlibrary.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.199801 audiobook-dl-0.5.0/audiobookdl/utils/
--rw-r--r--   0 jo1gi     (1000) users      (100)      972 2023-03-24 11:47:59.000000 audiobook-dl-0.5.0/audiobookdl/utils/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2924 2023-04-03 15:48:37.000000 audiobook-dl-0.5.0/audiobookdl/utils/audiobook.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      655 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/audiobookdl/utils/dependencies.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1298 2023-04-03 15:54:34.000000 audiobook-dl-0.5.0/pyproject.toml
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-04-10 11:40:48.200801 audiobook-dl-0.5.0/setup.cfg
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-04-06 21:10:31.000000 audiobook-dl-0.5.0/setup.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      396 2023-04-10 11:35:15.000000 audiobook-dl-0.5.0/shell.nix
--rw-r--r--   0 jo1gi     (1000) users      (100)     1987 2023-04-02 15:07:08.000000 audiobook-dl-0.5.0/supported_sites.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-04-10 11:40:48.199801 audiobook-dl-0.5.0/tests/
--rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-02-13 07:19:44.000000 audiobook-dl-0.5.0/tests/test_urls.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.126743 audiobook-dl-0.6.0/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.098743 audiobook-dl-0.6.0/.github/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       13 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/FUNDING.yml
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.098743 audiobook-dl-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      349 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.099743 audiobook-dl-0.6.0/.github/workflows/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      315 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/workflows/pytest.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      539 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.gitignore
+-rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/LICENSE
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-09 17:36:37.126743 audiobook-dl-0.6.0/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4798 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/README.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.102743 audiobook-dl-0.6.0/audiobook_dl.egg-info/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2311 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       58 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/entry_points.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       88 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/requires.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/top_level.txt
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.104743 audiobook-dl-0.6.0/audiobookdl/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      191 2023-07-09 17:33:15.000000 audiobook-dl-0.6.0/audiobookdl/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5968 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/__main__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3495 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/args.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.105743 audiobook-dl-0.6.0/audiobookdl/assets/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.110743 audiobook-dl-0.6.0/audiobookdl/assets/errors/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/book_access.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/chapters_add.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       56 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/config_not_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      468 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/data_not_present.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       45 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/failed_combining.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/missing_dependency.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/no_files_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/no_source_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       55 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/request_error.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/user_not_authorized.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/ffmpeg_chapter_template.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      317 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/simple_help.txt
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.092743 audiobook-dl-0.6.0/audiobookdl/assets/sources/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.113743 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1010 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/book_info.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      108 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/files.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      270 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/login.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      185 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast_episode_file.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      866 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast_episodes.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1983 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/config.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1342 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/exceptions.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1407 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/logging.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.115743 audiobook-dl-0.6.0/audiobookdl/output/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     8073 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/output/download.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      641 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/encryption.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.117743 audiobook-dl-0.6.0/audiobookdl/output/metadata/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1363 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1524 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/ffmpeg.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2391 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/id3.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1476 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/mp4.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3473 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/output/output.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.123743 audiobook-dl-0.6.0/audiobookdl/sources/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1637 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2050 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/audiobooksdotcom.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4654 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/bookbeat.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4318 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/chirp.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3510 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/ereolen.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1325 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/librivox.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5289 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/nextory.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3308 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/overdrive.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     7927 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/podimo.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      155 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/sources/rss.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4413 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/saxo.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     6258 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/scribd.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.124743 audiobook-dl-0.6.0/audiobookdl/sources/source/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5125 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/source/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2404 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/sources/source/networking.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5819 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/storytel.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4717 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/yourcloudlibrary.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.124743 audiobook-dl-0.6.0/audiobookdl/utils/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1159 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/utils/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4028 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/utils/audiobook.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1317 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/pyproject.toml
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-09 17:36:37.126743 audiobook-dl-0.6.0/setup.cfg
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/setup.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      434 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/shell.nix
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2139 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/supported_sites.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.125743 audiobook-dl-0.6.0/tests/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1087 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/tests/test_output.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/tests/test_urls.py
```

### Comparing `audiobook-dl-0.5.0/.gitignore` & `audiobook-dl-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.5.0/LICENSE` & `audiobook-dl-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.5.0/PKG-INFO` & `audiobook-dl-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.5.0
+Version: 0.6.0
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -21,21 +21,22 @@
 CLI tool for downloading audiobooks from online sources.
 
 ## Supported Services
 audiobook-dl currently supports downloading from the following sources:
 - [audiobooks.com](https://audiobooks.com)
 - [BookBeat](https://www.bookbeat.com/)
 - [Chirp](https://www.chirpbooks.com/)
-- [eReolen (Danish Library)](https://ereolen.dk)
+- [eReolen](https://ereolen.dk)
 - [Librivox](https://librivox.org)
 - [Nextory](https://nextory.com)
-- [Overdrive (Library service)](https://www.overdrive.com/)
+- [Overdrive / Libby](https://www.overdrive.com/)
+- [Podimo](https://podimo.com)
 - [Saxo](https://saxo.com)
 - [Scribd](https://scribd.com)
-- [Storytel](https://www.storytel.com/)
+- [Storytel](https://www.storytel.com/) / [Mofibo](https://mofibo.com)
 - [YourCloudLibrary](https://www.yourcloudlibrary.com/)
 
 [More info](./supported_sites.md)
 
 ## Installation
 audiobook-dl can be installed from the repo itself or through pip.
 
@@ -115,7 +116,18 @@
 Issues, bug-reports, pull requests or ideas for features and improvements are
 **very welcome**.
 
 ## Donations
 If you like the project, please consider donating:
 - [Ko-fi](https://ko-fi.com/jo1gi)
 - [Buy me a Coffee](https://www.buymeacoffee.com/joakimholm)
+<details>
+<summary>Cryptocurrencies</summary>
+
+- Bitcoin: bc1qrh8hcnw0fd22y7rmljlmrztwrz2nd5tqckrt44
+- Bitcoin Cash: qp6rt9zx7tfyu9e4alxcn5yf4re5pfztvu8yx0rywh
+- Dash: XfgopGkj4BBpuzsUvrbj9jenXUZ6dXsr3J
+- Etherium: 0x8f5d2eb6d2a4d4615d2b9b1cfa28b4c5b9d18f9f
+- Litecoin: ltc1qfz2936a04m2h7t0srxftygjrq759auav7ndfd3
+- Monero: 853tLAbK5wQ93mdj884C31JGKBUEJCpM25gEjGGLnuVDc8PEDMJi6uC5Vcz9g37K2PeT8FY1bjEveUWqJXNPotFRLwLnn9a
+
+</details>
```

### Comparing `audiobook-dl-0.5.0/README.md` & `audiobook-dl-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 CLI tool for downloading audiobooks from online sources.
 
 ## Supported Services
 audiobook-dl currently supports downloading from the following sources:
 - [audiobooks.com](https://audiobooks.com)
 - [BookBeat](https://www.bookbeat.com/)
 - [Chirp](https://www.chirpbooks.com/)
-- [eReolen (Danish Library)](https://ereolen.dk)
+- [eReolen](https://ereolen.dk)
 - [Librivox](https://librivox.org)
 - [Nextory](https://nextory.com)
-- [Overdrive (Library service)](https://www.overdrive.com/)
+- [Overdrive / Libby](https://www.overdrive.com/)
+- [Podimo](https://podimo.com)
 - [Saxo](https://saxo.com)
 - [Scribd](https://scribd.com)
-- [Storytel](https://www.storytel.com/)
+- [Storytel](https://www.storytel.com/) / [Mofibo](https://mofibo.com)
 - [YourCloudLibrary](https://www.yourcloudlibrary.com/)
 
 [More info](./supported_sites.md)
 
 ## Installation
 audiobook-dl can be installed from the repo itself or through pip.
 
@@ -101,7 +102,18 @@
 Issues, bug-reports, pull requests or ideas for features and improvements are
 **very welcome**.
 
 ## Donations
 If you like the project, please consider donating:
 - [Ko-fi](https://ko-fi.com/jo1gi)
 - [Buy me a Coffee](https://www.buymeacoffee.com/joakimholm)
+<details>
+<summary>Cryptocurrencies</summary>
+
+- Bitcoin: bc1qrh8hcnw0fd22y7rmljlmrztwrz2nd5tqckrt44
+- Bitcoin Cash: qp6rt9zx7tfyu9e4alxcn5yf4re5pfztvu8yx0rywh
+- Dash: XfgopGkj4BBpuzsUvrbj9jenXUZ6dXsr3J
+- Etherium: 0x8f5d2eb6d2a4d4615d2b9b1cfa28b4c5b9d18f9f
+- Litecoin: ltc1qfz2936a04m2h7t0srxftygjrq759auav7ndfd3
+- Monero: 853tLAbK5wQ93mdj884C31JGKBUEJCpM25gEjGGLnuVDc8PEDMJi6uC5Vcz9g37K2PeT8FY1bjEveUWqJXNPotFRLwLnn9a
+
+</details>
```

### Comparing `audiobook-dl-0.5.0/audiobook_dl.egg-info/PKG-INFO` & `audiobook-dl-0.6.0/audiobook_dl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.5.0
+Version: 0.6.0
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
@@ -21,21 +21,22 @@
 CLI tool for downloading audiobooks from online sources.
 
 ## Supported Services
 audiobook-dl currently supports downloading from the following sources:
 - [audiobooks.com](https://audiobooks.com)
 - [BookBeat](https://www.bookbeat.com/)
 - [Chirp](https://www.chirpbooks.com/)
-- [eReolen (Danish Library)](https://ereolen.dk)
+- [eReolen](https://ereolen.dk)
 - [Librivox](https://librivox.org)
 - [Nextory](https://nextory.com)
-- [Overdrive (Library service)](https://www.overdrive.com/)
+- [Overdrive / Libby](https://www.overdrive.com/)
+- [Podimo](https://podimo.com)
 - [Saxo](https://saxo.com)
 - [Scribd](https://scribd.com)
-- [Storytel](https://www.storytel.com/)
+- [Storytel](https://www.storytel.com/) / [Mofibo](https://mofibo.com)
 - [YourCloudLibrary](https://www.yourcloudlibrary.com/)
 
 [More info](./supported_sites.md)
 
 ## Installation
 audiobook-dl can be installed from the repo itself or through pip.
 
@@ -115,7 +116,18 @@
 Issues, bug-reports, pull requests or ideas for features and improvements are
 **very welcome**.
 
 ## Donations
 If you like the project, please consider donating:
 - [Ko-fi](https://ko-fi.com/jo1gi)
 - [Buy me a Coffee](https://www.buymeacoffee.com/joakimholm)
+<details>
+<summary>Cryptocurrencies</summary>
+
+- Bitcoin: bc1qrh8hcnw0fd22y7rmljlmrztwrz2nd5tqckrt44
+- Bitcoin Cash: qp6rt9zx7tfyu9e4alxcn5yf4re5pfztvu8yx0rywh
+- Dash: XfgopGkj4BBpuzsUvrbj9jenXUZ6dXsr3J
+- Etherium: 0x8f5d2eb6d2a4d4615d2b9b1cfa28b4c5b9d18f9f
+- Litecoin: ltc1qfz2936a04m2h7t0srxftygjrq759auav7ndfd3
+- Monero: 853tLAbK5wQ93mdj884C31JGKBUEJCpM25gEjGGLnuVDc8PEDMJi6uC5Vcz9g37K2PeT8FY1bjEveUWqJXNPotFRLwLnn9a
+
+</details>
```

### Comparing `audiobook-dl-0.5.0/audiobook_dl.egg-info/SOURCES.txt` & `audiobook-dl-0.6.0/audiobook_dl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,48 +14,56 @@
 audiobook_dl.egg-info/dependency_links.txt
 audiobook_dl.egg-info/entry_points.txt
 audiobook_dl.egg-info/requires.txt
 audiobook_dl.egg-info/top_level.txt
 audiobookdl/__init__.py
 audiobookdl/__main__.py
 audiobookdl/args.py
+audiobookdl/config.py
 audiobookdl/exceptions.py
 audiobookdl/logging.py
 audiobookdl/assets/ffmpeg_chapter_template.txt
 audiobookdl/assets/simple_help.txt
 audiobookdl/assets/errors/book_access.txt
 audiobookdl/assets/errors/chapters_add.txt
+audiobookdl/assets/errors/config_not_found.txt
 audiobookdl/assets/errors/data_not_present.txt
 audiobookdl/assets/errors/failed_combining.txt
 audiobookdl/assets/errors/missing_dependency.txt
 audiobookdl/assets/errors/no_files_found.txt
 audiobookdl/assets/errors/no_source_found.txt
 audiobookdl/assets/errors/request_error.txt
 audiobookdl/assets/errors/user_not_authorized.txt
+audiobookdl/assets/sources/podimo/book_info.graphql
+audiobookdl/assets/sources/podimo/files.graphql
+audiobookdl/assets/sources/podimo/login.graphql
+audiobookdl/assets/sources/podimo/podcast.graphql
+audiobookdl/assets/sources/podimo/podcast_episode_file.graphql
+audiobookdl/assets/sources/podimo/podcast_episodes.graphql
 audiobookdl/output/__init__.py
 audiobookdl/output/download.py
 audiobookdl/output/encryption.py
-audiobookdl/output/formats.py
 audiobookdl/output/output.py
 audiobookdl/output/metadata/__init__.py
 audiobookdl/output/metadata/ffmpeg.py
 audiobookdl/output/metadata/id3.py
 audiobookdl/output/metadata/mp4.py
 audiobookdl/sources/__init__.py
 audiobookdl/sources/audiobooksdotcom.py
 audiobookdl/sources/bookbeat.py
 audiobookdl/sources/chirp.py
 audiobookdl/sources/ereolen.py
 audiobookdl/sources/librivox.py
 audiobookdl/sources/nextory.py
 audiobookdl/sources/overdrive.py
+audiobookdl/sources/podimo.py
 audiobookdl/sources/rss.py
 audiobookdl/sources/saxo.py
 audiobookdl/sources/scribd.py
 audiobookdl/sources/storytel.py
 audiobookdl/sources/yourcloudlibrary.py
 audiobookdl/sources/source/__init__.py
 audiobookdl/sources/source/networking.py
 audiobookdl/utils/__init__.py
 audiobookdl/utils/audiobook.py
-audiobookdl/utils/dependencies.py
+tests/test_output.py
 tests/test_urls.py
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/args.py` & `audiobook-dl-0.6.0/audiobookdl/args.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 from audiobookdl import __version__
-from typing import Any
+from typing import Any, List
 
 
 def parse_arguments() -> Any:
     parser = argparse.ArgumentParser(
         prog="audiobook-dl",
         description="Download audiobooks from websites",
     )
@@ -104,8 +104,38 @@
         help="Password for source",
     )
     parser.add_argument(
         '--library',
         dest="library",
         help="Library for source",
     )
+    parser.add_argument(
+        '--write-json-metadata',
+        dest = "write_json_metadata",
+        help = "Write metadata in a seperate json file",
+        action="store_true",
+    )
+    parser.add_argument(
+        '--config',
+        dest = "config_location",
+        help = "Alternative location of config file"
+    )
     return parser.parse_args()
+
+
+def get_urls(options) -> List[str]:
+    """
+    Creates a list of all urls in cli options.
+    Urls a found in `options.urls` and read from `options.input_file` if the
+    file exists
+
+    :param options: Cli options
+    :returns: Combined list of all urls
+    """
+    urls = []
+    # Args
+    urls.extend(options.urls)
+    # File
+    if options.input_file:
+        with open(options.input_file, "r") as f:
+            urls.extend(f.read().split())
+    return urls
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/exceptions.py` & `audiobook-dl-0.6.0/audiobookdl/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,7 +34,10 @@
     error_description = "request_error"
 
 class UserNotAuthorized(AudiobookDLException):
     error_description = "user_not_authorized"
 
 class MissingBookAccess(AudiobookDLException):
     error_description = "book_access"
+
+class ConfigNotFound(AudiobookDLException):
+    error_description = "config_not_found"
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/logging.py` & `audiobook-dl-0.6.0/audiobookdl/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rich.text import Text
 from rich.style import Style
 from rich.markup import render, escape
 from rich.console import Console
 from rich.progress import Progress, ProgressColumn
-from typing import Union
+from typing import Union, List
 from audiobookdl.utils import read_asset_file
 
 debug_mode = False
 quiet_mode = False
 ffmpeg_output = False
 console = Console(stderr=True)
 DEBUG_PREFIX = render("[yellow bold]DEBUG[/]")
@@ -44,9 +44,9 @@
     console.print(read_asset_file(path))
 
 
 def simple_help() -> None:
     """Print basic help information"""
     print_asset_file("assets/simple_help.txt")
 
-def progress(progress_format: list[Union[str, ProgressColumn]]) -> Progress:
+def progress(progress_format: List[Union[str, ProgressColumn]]) -> Progress:
     return Progress(*progress_format, console=console)
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/output/download.py` & `audiobook-dl-0.6.0/audiobookdl/output/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,166 @@
 from audiobookdl import AudiobookFile, Source, logging, Audiobook
 from audiobookdl.exceptions import UserNotAuthorized, NoFilesFound
 from . import metadata, output, encryption
 
 import os
 import shutil
 from functools import partial
-from typing import Any, Union, Optional
-from rich.progress import Progress, BarColumn, ProgressColumn
+from typing import Any, Iterable, List, Optional, Sequence, Tuple, Union
+from rich.progress import Progress, BarColumn, ProgressColumn, SpinnerColumn
 from rich.prompt import Confirm
 from multiprocessing.pool import ThreadPool
+from pathlib import Path
+import rich # TODO Remove
 
 
-DOWNLOAD_PROGRESS: list[Union[str, ProgressColumn]] = [
-    "{task.description}", BarColumn(), "[progress.percentage]{task.percentage:>3.0f}%"
+DOWNLOAD_PROGRESS: List[Union[str, ProgressColumn]] = [
+    SpinnerColumn(),
+    "{task.description}",
+    BarColumn(),
+    "[progress.percentage]{task.percentage:>3.0f}%"
 ]
 
 
-def download(source: Source, options):
-    """Downloads audiobook from source object"""
+def download(audiobook: Audiobook, options):
+    """
+    Download contents of audiobook
+
+    :param audiobook: Audiobook to download
+    :param options: Cli options
+    """
     try:
-        audiobook = create_audiobook(source)
-        output_dir = output.gen_output_location(options.output_template, audiobook.metadata, options.remove_chars)
+        output_dir = output.gen_output_location(
+            options.output_template,
+            audiobook.metadata,
+            options.remove_chars
+        )
         download_audiobook(audiobook, output_dir, options)
     except KeyboardInterrupt:
         logging.log("Stopped download")
         logging.log("Cleaning up files")
         shutil.rmtree(output_dir)
 
 
-def create_audiobook(source: Source) -> Audiobook:
-    """Creates a new `Audiobook` object from a `Source`"""
-    if source.requires_authentication and not source.authenticated:
-        raise UserNotAuthorized
-    source.prepare()
-    files = source.get_files()
-    if len(files) == 0:
-        raise NoFilesFound
-    return Audiobook(
-        session = source._session,
-        metadata = source.get_metadata(),
-        chapters = source.get_chapters(),
-        files = files,
-        cover = source.get_cover()
-    )
-
-
 def download_audiobook(audiobook: Audiobook, output_dir: str, options):
     """Download, convert, combine, and add metadata to files from `Audiobook` object"""
     # Downloading files
     filepaths = download_files_with_cli_output(audiobook, output_dir)
     # Converting files
     current_format, output_format = get_output_audio_format(options.output_format, filepaths)
     if current_format != output_format:
-        logging.log("Converting files")
+        logging.log("  Converting files")
         filepaths = output.convert_output(filepaths, output_format)
     # Combine files
-    if options.combine:
-        logging.log("Combining files")
+    if options.combine and len(filepaths) > 1:
+        logging.log("  Combining files")
         output_path = f"{output_dir}.{output_format}"
         output.combine_audiofiles(filepaths, output_dir, output_path)
         filepaths = [output_path]
     # Add metadata
     if len(filepaths) == 1:
         add_metadata_to_file(audiobook, filepaths[0], options)
     else:
         add_metadata_to_dir(audiobook, filepaths, output_dir, options)
 
 
 def add_metadata_to_file(audiobook: Audiobook, filepath: str, options):
-    """Embed metadata into a single file"""
+    """
+    Embed metadata into a single file
+
+    :param audiobook: Audiobook object. Stores metadata
+    :param filepath: Filepath of output file
+    :options: Cli options
+    """
+    # Chapters
     if audiobook.chapters and not options.no_chapters:
-        logging.log("Adding chapters")
+        logging.log("  Adding chapters")
         metadata.add_chapters(filepath, audiobook.chapters)
-    logging.log("Adding metadata")
+    # General metadata
+    logging.log("  Adding metadata")
     metadata.add_metadata(filepath, audiobook.metadata)
+    if options.write_json_metadata:
+        with open(f"{filepath}.json", "w") as f:
+            f.write(audiobook.metadata.as_json())
+    # Cover
     if audiobook.cover:
-        logging.log("Embedding cover")
+        logging.log("  Embedding cover")
         metadata.embed_cover(filepath, audiobook.cover)
 
 
-def add_metadata_to_dir(audiobook: Audiobook, filepaths: list[str], output_dir: str, options):
-    """Add metadata to a directory with audio files"""
+def add_metadata_to_dir(audiobook: Audiobook, filepaths: Iterable[str], output_dir: str, options):
+    """
+    Add metadata to a directory with audio files
+
+    :param audiobook: Audiobook object. Stores metadata
+    :param filepaths: Iterable over filepaths of output files
+    :param output_dir: Directory where files are stored
+    :param optiosn: Cli options
+    """
+    logging.log(" Addding metadata")
     for filepath in filepaths:
         metadata.add_metadata(filepath, audiobook.metadata)
+    if options.write_json_metadata:
+        metadata_file_path = os.path.join(output_dir, "metadata.json")
+        with open(metadata_file_path, "w") as f:
+            f.write(audiobook.metadata.as_json())
     if audiobook.cover:
-        logging.log("Adding cover")
+        logging.log("  Adding cover")
         cover_path = os.path.join(output_dir, f"cover.{audiobook.cover.extension}")
         with open(cover_path, "wb") as f:
             f.write(audiobook.cover.image)
 
 
-def download_files_with_cli_output(audiobook: Audiobook, output_dir: str) -> list[str]:
+def download_files_with_cli_output(audiobook: Audiobook, output_dir: str) -> List[str]:
     """
-    Download `audiobook` with cli output
-    Returns a list of paths of the downloaded files
+    Download `audiobook` with cli progress bar
+
+    :param audiobook: Audiobook to download
+    :param output_dir: Output directory where files are downloaded to
+    :returns: A list of paths of the downloaded files
     """
     if len(audiobook.files) > 1:
         setup_download_dir(output_dir)
+    else:
+        parent = Path(output_dir).parent
+        if not parent.exists():
+            os.makedirs(parent)
     with logging.progress(DOWNLOAD_PROGRESS) as progress:
         task = progress.add_task(
-            f"Downloading {len(audiobook.files)} files [blue]{audiobook.title}",
+            f"Downloading [blue]{audiobook.title}",
             total = len(audiobook.files)
         )
         update_progress = partial(progress.advance, task)
         filepaths = download_files(audiobook, output_dir, update_progress)
         # Make sure progress bar is at 100%
         remaining_progress: float = progress.tasks[0].remaining or 0
         update_progress(remaining_progress)
         # Return filenames of downloaded files
         return filepaths
 
 
 def create_filepath(audiobook: Audiobook, output_dir: str, index: int) -> str:
-    """Create output file path for file number `index` in `audibook`"""
+    """
+    Create output file path for file number `index` in `audibook`
+
+    :param audiobook: Currently downloading audiobook
+    :param output_dir: Directory where file should be stored
+    :param index: Index in audiobooks list of files
+    :returns: Filepath
+    """
     extension = audiobook.files[index].ext
     if len(audiobook.files) == 1:
         path = f"{output_dir}.{extension}"
     else:
         name = f"{audiobook.title} - Part {index}.{extension}"
         path = os.path.join(output_dir, name)
     return path
 
 
-def download_file(args: tuple[Audiobook, str, int, Any]) -> str:
+def download_file(args: Tuple[Audiobook, str, int, Any]) -> str:
     # Prepare download
     audiobook, output_dir, index, update_progress = args
     file = audiobook.files[index]
     filepath = create_filepath(audiobook, output_dir, index)
     logging.debug(f"Starting downloading file: {file.url}")
     request = audiobook.session.get(file.url, headers=file.headers, stream=True)
     total_filesize = int(request.headers["Content-length"])
@@ -139,44 +173,54 @@
     # Decrypt file if necessary
     if file.encryption_method:
         encryption.decrypt_file(filepath, file.encryption_method)
     # Return filepath
     return filepath
 
 
-def download_files(audiobook: Audiobook, output_dir: str, update_progress) -> list[str]:
+def download_files(audiobook: Audiobook, output_dir: str, update_progress) -> List[str]:
     """Download files from audiobook and return paths of the downloaded files"""
     filepaths = []
     with ThreadPool(processes=20) as pool:
         arguments = []
         for index in range(len(audiobook.files)):
             arguments.append((audiobook, output_dir, index, update_progress))
         for filepath in pool.imap(download_file, arguments):
             filepaths.append(filepath)
     return filepaths
 
 
-def get_output_audio_format(option: Optional[str], files: list[str]) -> tuple[str, str]:
+def get_output_audio_format(option: Optional[str], files: Sequence[str]) -> Tuple[str, str]:
     """
     Get output format for files
 
     `option` is used if specied; else it's based on the file extensions
+    :param option: User specified value
+    :param files: Audio file names
+    :returns: A tuple with current format and output format
     """
     current_format = os.path.splitext(files[0])[1][1:]
     if option:
         output_format = option
-    elif current_format == "ts":
-        output_format = "mp3"
     else:
         output_format = current_format
     return current_format, output_format
 
 
-def setup_download_dir(path: str):
-    """Creates output folder"""
+def setup_download_dir(path: str) -> None:
+    """
+    Creates output folder for the audiobook.
+    Will give a prompt if the folder already exists.
+
+    :param path: Path of output folder
+    :returns: Nothing
+    """
+    logging.log("Creating output dir")
     if os.path.isdir(path):
-        answer = Confirm.ask(f"The folder '[blue]{path}[/blue]' already exists. Do you want to override it?")
+        answer = Confirm.ask(
+            f"The folder '[blue]{path}[/blue]' already exists. Do you want to override it?"
+        )
         if answer:
             shutil.rmtree(path)
         else:
             exit()
     os.makedirs(path)
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/output/encryption.py` & `audiobook-dl-0.6.0/audiobookdl/output/encryption.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.5.0/audiobookdl/output/metadata/__init__.py` & `audiobook-dl-0.6.0/audiobookdl/output/metadata/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from audiobookdl import logging, Chapter, AudiobookMetadata, Cover
-from audiobookdl.utils import dependencies
 from . import id3, mp4, ffmpeg
+from audiobookdl import logging, Chapter, AudiobookMetadata, Cover
+from audiobookdl.utils import program_in_path
+
 import os
+from typing import Sequence
 
 def add_metadata(filepath: str, metadata: AudiobookMetadata):
     """Adds metadata to the given audio file"""
     if id3.is_id3_file(filepath):
         id3.add_id3_metadata(filepath, metadata)
     elif mp4.is_mp4_file(filepath):
         mp4.add_mp4_metadata(filepath, metadata)
@@ -19,19 +21,19 @@
         id3.embed_id3_cover(filepath, cover)
     elif mp4.is_mp4_file(filepath):
         mp4.embed_mp4_cover(filepath, cover)
     else:
         logging.debug("Could not embed cover")
 
 
-def add_chapters(filepath: str, chapters: list[Chapter]):
+def add_chapters(filepath: str, chapters: Sequence[Chapter]):
     """Adds chapters to the given audio file"""
     if id3.is_id3_file(filepath):
         id3.add_id3_chapters(filepath, chapters)
-    elif dependencies.program_in_path("ffmpeg"):
+    elif program_in_path("ffmpeg"):
         ffmpeg.add_chapters_ffmpeg(filepath, chapters)
     else:
         if logging.debug_mode:
             logging.debug("Could not add chapters")
         else:
             filetype = os.path.splitext(filepath)[1][1:]
             logging.print_error_file("chapters_add", filetype=filetype)
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/output/metadata/ffmpeg.py` & `audiobook-dl-0.6.0/audiobookdl/output/metadata/ffmpeg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from audiobookdl import Chapter, utils, logging
 from mutagen import File as MutagenFile
 import subprocess
 import os
+from typing import Sequence
 
 TMP_CHAPTER_FILE = "chapters.tmp.txt"
 TMP_MEDIA_FILE = "audiobook.tmp.mp4"
 
 def create_chapter_text(title: str, start: int, end: int) -> str:
     chapter_template = utils.read_asset_file("assets/ffmpeg_chapter_template.txt")
     return chapter_template.format(
         title = title,
         start = start,
         end = end
     )
 
 
-def create_tmp_chapter_file(filepath: str, chapters: list[Chapter]) -> str:
+def create_tmp_chapter_file(filepath: str, chapters: Sequence[Chapter]) -> str:
     result = ";FFMETADATA1\n"
     for i in range(len(chapters)-1):
         chapter = chapters[i]
         result += create_chapter_text(chapter.title, chapter.start, chapters[i+1].start)
     length = MutagenFile(filepath).info.length*1000
     last_chapter = chapters[-1]
     result += create_chapter_text(
         title = last_chapter.title,
         start = last_chapter.start,
         end = int(length)
     )
     return result
 
-def add_chapters_ffmpeg(filepath: str, chapters: list[Chapter]):
+def add_chapters_ffmpeg(filepath: str, chapters: Sequence[Chapter]):
     try:
         with open(TMP_CHAPTER_FILE, "w") as f:
             f.write(create_tmp_chapter_file(filepath, chapters))
         subprocess.run(
             ["ffmpeg", "-y", "-i", filepath, "-i", TMP_CHAPTER_FILE,
                 "-map_metadata", "1", "-c", "copy", TMP_MEDIA_FILE],
             capture_output = not logging.ffmpeg_output
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/output/metadata/id3.py` & `audiobook-dl-0.6.0/audiobookdl/output/metadata/id3.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from audiobookdl import logging, Chapter, AudiobookMetadata, Cover
 
 from mutagen import File as MutagenFile
 from mutagen.easyid3 import EasyID3
 from mutagen.mp3 import MP3
 from mutagen.id3 import ID3, APIC, CHAP, TIT2, CTOC, CTOCFlags, ID3NoHeaderError
 
+from typing import Sequence
+
 # Conversion table between metadata names and ID3 tags
 ID3_CONVERT = {
     "author": "artist",
     "series": "album",
     "title": "title",
     "narrator": "performer",
 }
@@ -25,47 +27,48 @@
 }
 
 def is_id3_file(filepath: str) -> bool:
     """Returns true if `filepath` points to an id3 file"""
     ext = re.search(r"(?<=(\.))\w+$", filepath)
     return ext is not None and ext.group(0) in ID3_FORMATS
 
+
 def add_id3_metadata(filepath: str, metadata: AudiobookMetadata):
     """Add ID3 metadata tags to the given audio file"""
     audio = MP3(filepath, ID3=EasyID3)
     # Adding tags
     for key, value in metadata.all_properties(allow_duplicate_keys=False):
         if key in ID3_CONVERT:
             audio[ID3_CONVERT[key]] = value
         elif key in EasyID3.valid_keys.keys():
             audio[key] = value
-        else:
-            logging.debug(f"Tried to add invalid id3 tag: {key}")
     audio.save(v2_version=3)
 
+
 def embed_id3_cover(filepath: str, cover: Cover):
     mimetype = EXTENSION_TO_MIMETYPE[cover.extension]
     try:
         audio = ID3(filepath)
     except ID3NoHeaderError:
         return
     audio.add(APIC(type=0, data=cover.image, mime=mimetype))
     audio.save()
 
+
 def add_id3_chapter(audio: ID3, start: int, end: int, title: str, index: int):
     """Adds a single chapter to the given audio file"""
     audio.add(CHAP(
         element_id=u"chp"+str(index),
         start_time=int(start),
         end_time=int(end),
         sub_frames=[TIT2(text=[title])]
     ))
 
 
-def add_id3_chapters(filepath: str, chapters: list[Chapter]):
+def add_id3_chapters(filepath: str, chapters: Sequence[Chapter]):
     """Adds chapters to the given audio file"""
     audio = ID3(filepath)
     for i in range(len(chapters)-1):
         add_id3_chapter(
             audio,
             start = chapters[i].start,
             end = chapters[i+1].start,
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/output/metadata/mp4.py` & `audiobook-dl-0.6.0/audiobookdl/output/metadata/mp4.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.5.0/audiobookdl/output/output.py` & `audiobook-dl-0.6.0/audiobookdl/output/output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,87 @@
 from audiobookdl import logging, AudiobookMetadata
 from audiobookdl.exceptions import FailedCombining
 
 import os
 import shutil
 import platform
 import subprocess
+from typing import Sequence, Mapping
 
 LOCATION_DEFAULTS = {
     'album': 'NA',
     'artist': 'NA',
 }
 
-def gen_output_filename(booktitle: str, file: dict[str, str], template: str) -> str:
+def gen_output_filename(booktitle: str, file: Mapping[str, str], template: str) -> str:
     """Generates an output filename based on different attributes of the
     file"""
     arguments = {**file, **{"booktitle": booktitle}}
     filename = template.format(**arguments)
     return _fix_output(filename)
 
 
-def combine_audiofiles(filenames: list[str], tmp_dir: str, output_path: str):
+def combine_audiofiles(filenames: Sequence[str], tmp_dir: str, output_path: str):
     """Combines the given audiofiles in `path` into a new file"""
     inputs = "|".join(filenames)
     subprocess.run(
-        ["ffmpeg", "-i", f"concat:{inputs}", "-safe", "0", "-c", "copy", output_path],
+        ["ffmpeg", "-i", f"concat:{inputs}", "-safe", "0", "-codec", "copy", output_path],
         capture_output=not logging.ffmpeg_output,
     )
     if not os.path.exists(output_path):
         raise FailedCombining
     shutil.rmtree(tmp_dir)
 
 
-def convert_output(filenames: list[str], output_format: str):
+def can_copy_codec(input_format: str, output_format: str) -> bool:
+    """
+    Checks whether the codec can be copies to the new output
+
+    :param input_format: Input file filetype
+    :param output_format: Output file filetype
+    :returns: True if the codec can be copied
+    """
+    # TODO Add better verification
+    return output_format == "mkv" \
+        or output_format == "mka" \
+        or (input_format == "ts" and output_format == "mp3")
+
+
+def convert_output(filenames: Sequence[str], output_format: str):
     """Converts a list of audio files into another format and return new
     files"""
     new_paths = []
     for old_path in filenames:
-        split_path = os.path.splitext(old_path)
-        new_path = f"{split_path[0]}.{output_format}"
-        if not output_format == split_path[1][1:]:
-            subprocess.run(
-                ["ffmpeg", "-i", old_path, new_path],
-                capture_output=not logging.ffmpeg_output
-            )
+        path_without_ext, old_ext = os.path.splitext(old_path)
+        new_path = f"{path_without_ext}.{output_format}"
+        if not output_format == old_ext:
+            if can_copy_codec(old_ext, output_format):
+                subprocess.run(
+                    ["ffmpeg", "-i", old_path, "-codec", "copy", new_path],
+                    capture_output=not logging.ffmpeg_output
+                )
+            else:
+                subprocess.run(
+                    ["ffmpeg", "-i", old_path, new_path],
+                    capture_output=not logging.ffmpeg_output
+                )
             os.remove(old_path)
-        new_paths.append(f"{os.path.splitext(old_path)[0]}.{output_format}")
+        new_paths.append(new_path)
     return new_paths
 
 
 def gen_output_location(template: str, metadata: AudiobookMetadata, remove_chars: str) -> str:
-    """Generates the location of the output based on attributes of the
-    audiobook"""
+    """
+    Generates the location of the output based on attributes of the audiobook.
+
+    :param template: Python string template audiobook metadata is put into
+    :param metadata: Audiobook metadata,
+    :param remove_chars: List of characters to be removed from the final path
+    :returns: `template` with metadata inserted
+    """
     if metadata is None:
         metadata = {}
     metadata.title = _fix_output(metadata.title)
     metadata_dict = {**LOCATION_DEFAULTS, **metadata.all_properties_dict()}
     formatted = template.format(**metadata_dict)
     formatted = _remove_chars(formatted, remove_chars)
     return formatted
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/__init__.py` & `audiobook-dl-0.6.0/audiobookdl/sources/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,50 +3,55 @@
 from .audiobooksdotcom import AudiobooksdotcomSource
 from .bookbeat import BookBeatSource
 from .chirp import ChirpSource
 from .ereolen import EreolenSource
 from .librivox import LibrivoxSource
 from .nextory import NextorySource
 from .overdrive import OverdriveSource
+from .podimo import PodimoSource
 from .saxo import SaxoSource
 from .scribd import ScribdSource
 from .storytel import StorytelSource
 from .yourcloudlibrary import YourCloudLibrarySource
 
 from ..exceptions import NoSourceFound
 import re
+from typing import Iterable, List
 
 def find_compatible_source(url: str) -> Source:
     """Finds the first source that supports the given url"""
     sources = get_source_classes()
     for source in sources:
         for n, m in enumerate(source.match):
             if not re.match(m, url) is None:
-                return source(url, n)
+                return source()
     raise NoSourceFound
 
+
 def get_source_classes():
     """Returns a list of all available sources"""
     return [
         AudiobooksdotcomSource,
         BookBeatSource,
         ChirpSource,
         EreolenSource,
         LibrivoxSource,
         NextorySource,
         OverdriveSource,
+        PodimoSource,
         SaxoSource,
         ScribdSource,
         StorytelSource,
         YourCloudLibrarySource,
     ]
 
-def get_source_names() -> list[str]:
+
+def get_source_names() -> Iterable[str]:
     """
     Returns the names of all sources available
     There are sometimes multiple names for the same source
     """
-    results: list[str] = []
+    results: List[str] = []
     for source in get_source_classes():
         for source_name in source.names:
             results.append(source_name)
     return sorted(results, key=lambda x: x.lower())
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/audiobooksdotcom.py` & `audiobook-dl-0.6.0/audiobookdl/sources/audiobooksdotcom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,67 @@
 from .source import Source
-from audiobookdl import AudiobookFile, logging, AudiobookMetadata, Cover
+from audiobookdl import AudiobookFile, logging, AudiobookMetadata, Cover, Audiobook
+from audiobookdl.exceptions import NoSourceFound
+
 import re
+from typing import List
 from urllib.parse import unquote
 from urllib3.util import parse_url
 
 BASEURL = "https://www.audiobooks.com/book/stream/"
 
 
 class AudiobooksdotcomSource(Source):
     match = [
         r"{}\d+(/\d)?".format(BASEURL)
     ]
     names = [ "audiobooks.com" ]
 
-    def prepare(self):
-        path = parse_url(self.url).path
-        book_id = path.split("/")[3] # Third part of path is book id
-        logging.debug(f"{book_id=}")
-        self.scrape_url = f"{BASEURL}{book_id}/1"
+    def download(self, url: str) -> Audiobook:
+        path = parse_url(url).path
+        if not path:
+            raise NoSourceFound
+        book_id = path.split("/")[3]
+        scrape_url = f"{BASEURL}{book_id}/1"
+        return Audiobook(
+            session = self._session,
+            metadata = self.get_metadata(scrape_url),
+            cover = self.get_cover(scrape_url),
+            files = self.get_files(scrape_url),
+        )
 
 
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.find_elem_in_page(self.scrape_url, "h2#bookTitle")
+    def get_metadata(self, scrape_url: str) -> AudiobookMetadata:
+        title = self.find_elem_in_page(scrape_url, "h2#bookTitle")
         return AudiobookMetadata(title)
 
-    def get_cover(self) -> Cover:
+
+    def get_cover(self, scrape_url: str) -> Cover:
         cover_url = "http:" + \
             self.find_elem_in_page(
-                self.scrape_url,
+                scrape_url,
                 "img.bookimage",
                 data="src"
             )
         return Cover(self.get(cover_url), "jpg")
 
-    def _get_user_agent(self) -> str:
-        """Returns user agent from cookies"""
+
+    def extract_useragent_from_cookies(self) -> str:
+        """
+        Extracts user agent from cookies in local session.
+
+        :returns: User-Agent string
+        """
         raw = self._session.cookies.get("ci_session", domain="www.audiobooks.com")
         return unquote(raw).split("\"")[11]
 
-    def get_files(self) -> list[AudiobookFile]:
-        # User agent has to match the one in the cookies
-        headers = { "User-Agent": self._get_user_agent() }
+
+    def get_files(self, scrape_url: str) -> List[AudiobookFile]:
         media_url = self.find_in_page(
-            self.scrape_url,
+            scrape_url,
             r"(?<=(mp3: \")).+(?=(&rs))",
-            headers=headers
+            headers = {
+                # User agent has to match the one in the cookies
+                "User-Agent": self.extract_useragent_from_cookies()
+            }
         )
         return [ AudiobookFile(url=media_url, ext="mp3") ]
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/bookbeat.py` & `audiobook-dl-0.6.0/audiobookdl/sources/bookbeat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,136 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover
-from typing import Any, Optional
+from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover, Audiobook
+from typing import Any, List, Optional, Dict
 import uuid
 from audiobookdl.exceptions import UserNotAuthorized, MissingBookAccess
 import base64
 import re
 
 
-def get_device_id() -> str:
-    return (
-        str(uuid.uuid3(uuid.NAMESPACE_DNS, "audiobook-dl"))
-        + " "
-        + base64.b64encode(b"Personal Computer").decode()
-    )
 
 
 class BookBeatSource(Source):
     match = [
         r"https?://(www.)?bookbeat.+",
     ]
     names = ["BookBeat"]
     _authentication_methods = [
         "login",
     ]
-
     saved_books: dict
     book_info: dict
 
-    def _login(self, username: str, password: str):
+    @staticmethod
+    def create_device_id() -> str:
+        """Create random device id"""
+        return (
+            str(uuid.uuid3(uuid.NAMESPACE_DNS, "audiobook-dl"))
+            + " "
+            + base64.b64encode(b"Personal Computer").decode()
+        )
+
+    def _login(self, url: str, username: str, password: str):
         headers = {
             "accept": "application/hal+json",
             "bb-client": "BookBeatApp",
-            "bb-device": get_device_id(),
+            "bb-device": self.create_device_id(),
         }
         self._session.headers = headers
-
         login_json = {"username": username, "password": password}
-
         tokens = self.post_json(
             "https://api.bookbeat.com/api/login",
             json=login_json
         )
-        self._session.headers.update({"authorization": "Bearer " + tokens["token"]})
+        token = tokens["token"]
+        self._session.headers.update({"authorization": f"Bearer {token}"})
         self.saved_books = self.get_json(
             "https://api.bookbeat.com/api/my/books/saved?offset=0&limit=100"
         )
 
 
-    def get_files(self) -> list[AudiobookFile]:
+    def download(self, url: str) -> Audiobook:
+        book_id_re = r"(\d+)$"
+        wanted_id_match = re.search(book_id_re, url)
+        if not wanted_id_match:
+            raise ValueError(f"Couldn't get bookid from url {url}")
+        wanted_id = wanted_id_match.group(1)
+        book_info = self.find_book_info(wanted_id)
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(book_info),
+            metadata = self.get_metadata(book_info),
+            cover = self.get_cover(book_info),
+            chapters = self.get_chapters(book_info),
+        )
+
+
+    def download_license_url(self, book_info):
         dl_info = self.get_json(
-            "https://api.bookbeat.com/api/downloadinfo/" + str(self.book_info["bookid"])
+            "https://api.bookbeat.com/api/downloadinfo/" + str(book_info["bookid"])
         )
-        # Find license_url
         if "_embedded" in dl_info:
             if "downloads" in dl_info["_embedded"]:
                 for dl in dl_info["_embedded"]["downloads"]:
                     if dl["format"] == "audioBook":
-                        license_url = dl["_links"]["license"]["href"]
-                        break
+                        return dl["_links"]["license"]["href"]
+        raise MissingBookAccess
+
 
-        if license_url is None:
-            raise MissingBookAccess
+    def get_files(self, book_info: Dict) -> List[AudiobookFile]:
+        license_url = self.download_license_url(book_info)
         lic = self.get_json(license_url)
-        self.book_info["license"] = lic
+        book_info["license"] = lic
         if "_links" in lic:
             return [
                 AudiobookFile(
                     url=lic["_links"]["download"]["href"],
                     headers=self._session.headers,
                     ext="mp4",
                 )
             ]
         raise MissingBookAccess
 
 
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.book_info["metadata"]["title"]
+    def get_metadata(self, book_info: Dict) -> AudiobookMetadata:
+        title = book_info["metadata"]["title"]
         metadata = AudiobookMetadata(title)
         try:
-            contributors = next(
-                iter(
-                    [
-                        e["contributors"]
-                        for e in self.book_info["metadata"]["editions"]
-                        if e["format"] == "audioBook"
-                    ]
-                ),
-                None,
-            )
+            contributors = [
+                e["contributors"] for e in book_info["metadata"]["editions"] if e["format"] == "audioBook"
+            ][0]
             if not contributors:
                 return metadata
             for contributor in contributors:
                 name = f"{contributor['firstname']} {contributor['lastname']}"
                 if "author" in contributor["role"]:
                     metadata.add_author(name)
                 if "narrator" in contributor["role"]:
                     metadata.add_narrator(name)
             return metadata
         except:
             return metadata
 
-    def get_chapters(self) -> list[Chapter]:
+
+    @staticmethod
+    def get_chapters(book_info: Dict) -> List[Chapter]:
         chapters = []
-        for chapter_number, track in enumerate(self.book_info["license"]["tracks"]):
+        for chapter_number, track in enumerate(book_info["license"]["tracks"]):
             chapters.append(Chapter(track["start"], f"Chapter {chapter_number+1}"))
         return chapters
 
-    def get_cover(self) -> Cover:
-        cover_url = self.book_info["metadata"]["cover"]
+
+    def get_cover(self, book_info: Dict) -> Cover:
+        cover_url = book_info["metadata"]["cover"]
         cover_data = self.get(cover_url)
         return Cover(cover_data, "jpg")
 
-    def prepare(self):
-        book_id_re = r"(\d+)$"
-        wanted_id_match = re.search(book_id_re, self.url)
-        if not wanted_id_match:
-            raise ValueError(f"Couldn't get bookid from url {self.url}")
-        wanted_id = wanted_id_match.group(1)
+
+    def find_book_info(self, book_id: str) -> Dict:
+        """Find book by id from owned books"""
         for book in self.saved_books["_embedded"]["savedBooks"]:
-            if str(book["bookid"]) == wanted_id:
-                self.book_info = book
-                self.book_info["metadata"] = self._session.get(
-                    self.book_info["_links"]["book"]["href"]
+            if str(book["bookid"]) == book_id:
+                book["metadata"] = self._session.get(
+                    book["_links"]["book"]["href"]
                 ).json()
-                return
+                return book
         raise MissingBookAccess
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/chirp.py` & `audiobook-dl-0.6.0/audiobookdl/sources/chirp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,115 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, logging, AudiobookMetadata, Cover
+from audiobookdl import AudiobookFile, Chapter, logging, AudiobookMetadata, Cover, Audiobook
 
-from typing import Optional
+from typing import List, Optional, Tuple
 import base64
 from Crypto.Cipher import AES
 
 LOGIN_URL = "https://www.chirpbooks.com/users/sign_in"
 
 class ChirpSource(Source):
     match = [
         r"https://www.chirpbooks.com/player/\d+"
     ]
-
     names = [ "Chirp" ]
-
     headers = {
         "content-type": "application/json"
     }
 
-    def _get_tracks(self, book_id):
-        response = self.post_json(
-            f"https://www.chirpbooks.com/api/graphql",
-            json = {
-                "operationName": "fetchAudiobookTracks",
-                "query": "query fetchAudiobookTracks($id:ID!){audiobook(id:$id){tracks{partNumber chapterNumber offsetFromBookStartMs durationMs displayName}}}",
-                "variables": {
-                    "id": book_id
-                }
-            },
-            headers = self.headers,
+
+    def download(self, url: str) -> Audiobook:
+        book_id = int(self.find_elem_in_page(url, "div.user-audiobook", "data-audiobook-id"))
+        user_id = int(self.find_in_page(url, r'"id":(\d+)', 1))
+        tracks = self._get_tracks(book_id)
+        key, iv = self._create_key(url, user_id)
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(book_id, key, iv, tracks),
+            metadata = self.get_metadata(url),
+            cover = self.get_cover(url),
+            chapters = self.get_chapters(tracks)
         )
-        return response["data"]["audiobook"]["tracks"]
 
 
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.find_elem_in_page(self.url, "title")
+    def get_metadata(self, url: str) -> AudiobookMetadata:
+        title = self.find_elem_in_page(url, "title")
         metadata = AudiobookMetadata(title)
-        for credit in self.find_elems_in_page(self.url, ".credit"):
+        for credit in self.find_elems_in_page(url, ".credit"):
             text = credit.text
             if text.startswith("Written by"):
                 metadata.add_author(text[11:])
             elif text.startswith("Narrated by"):
                 metadata.add_narrator(text[12:])
         return metadata
 
 
-    def get_cover(self) -> Cover:
-        cover_url = self.find_elem_in_page(self.url, "img.cover-image", data="src")
+    def get_cover(self, url: str) -> Cover:
+        cover_url = self.find_elem_in_page(url, "img.cover-image", data="src")
         cover_data = self.get(cover_url)
         return Cover(cover_data, "jpg")
 
 
-    def get_audio_url(self, track):
+    def get_audio_url(self, book_id: int, key: bytes, iv: bytes, track):
         url_resp = self.post_json(
             f"https://www.chirpbooks.com/api/graphql",
             json = {
                 "operationName": "fetchAudiobookTrackUrl",
                 "query": "query fetchAudiobookTrackUrl($id:ID!,$partNumber:Int!,$chapterNumber:Int!){audiobook(id:$id){track(partNumber:$partNumber,chapterNumber:$chapterNumber){webPlayerMediaUrl}}}",
                 "variables": {
-                    "id": self.book_id,
+                    "id": book_id,
                     "chapterNumber": track["chapterNumber"],
                     "partNumber": track["partNumber"]
                 }
             },
             headers = self.headers
         )
         webplayermediaurl = url_resp["data"]["audiobook"]["track"]["webPlayerMediaUrl"]
         ciphertext = base64.b64decode(webplayermediaurl)
-        cipher = AES.new(self.key, AES.MODE_CBC, self.iv)
+        cipher = AES.new(key, AES.MODE_CBC, iv)
         return cipher.decrypt(ciphertext).decode("utf8")[:-1]
 
 
-    def get_files(self) -> list[AudiobookFile]:
+    def get_files(self, book_id: int, key: bytes, iv: bytes, tracks) -> List[AudiobookFile]:
         files = []
-        for track in self.tracks:
+        for track in tracks:
             files.append(AudiobookFile(
-                url = self.get_audio_url(track),
+                url = self.get_audio_url(book_id, key, iv, track),
                 ext = "mp3",
                 title = track["displayName"],
             ))
         return files
 
 
-    def get_chapters(self) -> list[Chapter]:
+    def get_chapters(self, tracks) -> List[Chapter]:
         chapters = []
         start_time = 0
-        for track in self.tracks:
+        for track in tracks:
             title = track["displayName"]
             chapters.append(Chapter(start_time, title))
             start_time += track["durationMs"]
         return chapters
 
 
-    def _calc_iv(self):
-        """Creates IV based on `user_id` to decrypt audio url"""
-        padding = 'x'*(12-len(str(self.user_id)))
-        padded_user_id = f"{padding}{self.user_id}"
-        return base64.b64encode(bytes(padded_user_id, "UTF-8"))
-
-
-    def prepare(self):
-        self.book_id = int(self.find_elem_in_page(self.url, "div.user-audiobook", "data-audiobook-id"))
-        logging.debug(f"{self.book_id=}")
-        self.user_id = int(self.find_in_page(self.url, r'"id":(\d+)', 1))
-        logging.debug(f"{self.user_id=}")
-        self.tracks = self._get_tracks(self.book_id)
-        self.iv = self._calc_iv()
-        logging.debug(f"{self.iv=}")
-        self.key = bytes(self.find_elem_in_page(self.url, "div.user-audiobook", "data-dk"), "UTF-8")
-        logging.debug(f"{self.key=}")
+    def _create_key(self, url: str, user_id: int) -> Tuple[bytes, bytes]:
+        """Creates key and iv to decrypt audio url"""
+        key = bytes(self.find_elem_in_page(url, "div.user-audiobook", "data-dk"), "UTF-8")
+        # Creates IV based on `user_id`
+        padding = 'x'*(12-len(str(user_id)))
+        padded_user_id = f"{padding}{user_id}"
+        iv = base64.b64encode(bytes(padded_user_id, "UTF-8"))
+        return key, iv
+
+
+    def _get_tracks(self, book_id: int):
+        response = self.post_json(
+            f"https://www.chirpbooks.com/api/graphql",
+            json = {
+                "operationName": "fetchAudiobookTracks",
+                "query": "query fetchAudiobookTracks($id:ID!){audiobook(id:$id){tracks{partNumber chapterNumber offsetFromBookStartMs durationMs displayName}}}",
+                "variables": {
+                    "id": book_id
+                }
+            },
+            headers = self.headers
+        )
+        return response["data"]["audiobook"]["tracks"]
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/ereolen.py` & `audiobook-dl-0.6.0/audiobookdl/sources/ereolen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,29 @@
 from .source import Source
-from audiobookdl import  AudiobookFile, logging, utils, AudiobookMetadata, Cover
+from audiobookdl import  AudiobookFile, logging, utils, AudiobookMetadata, Cover, Audiobook
 from audiobookdl.exceptions import UserNotAuthorized, RequestError
 
-from typing import Optional
+from typing import List, Optional, Dict
 import re
 import json
 
 LOGIN_PAGE_URL = "https://ereolen.dk/adgangsplatformen/login?destination=/user"
 
 class EreolenSource(Source):
     _authentication_methods = [
         "cookies",
         "login"
     ]
-
     names = [ "eReolen" ]
-
     login_data = [ "username", "password", "library" ]
-
     match = [
         r"https?://ereolen.dk/ting/object/.+"
     ]
-    book_id: str
-
-
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.meta["title"]
-        metadata = AudiobookMetadata(title)
-        metadata.add_author(self.meta["artist"])
-        return metadata
-
-
-    def get_cover(self) -> Cover:
-        cover_data = self.get(self.meta["cover"])
-        return Cover(cover_data, "jpg")
-
-    def get_files(self) -> list[AudiobookFile]:
-        return self.get_stream_files(
-            f"https://audio.api.streaming.pubhub.dk/v1/stream/hls/{self.book_id}/playlist.m3u8"
-        )
-
-    def _get_libraries(self):
-        """Returns list of available libraries for login"""
-        libraries_raw = self.find_in_page(
-            LOGIN_PAGE_URL,
-            "libraries = ({.+})<",
-            group_index=1
-        )
-        libraries = {}
-        for library in json.loads(libraries_raw)["folk"]:
-            library_name = library["name"]
-            library_id = library["branchId"]
-            libraries[library_name] = library_id
-        return libraries
 
-    def _login(self, username: str, password: str, library: str): # type: ignore
+    def _login(self, url: str, username: str, password: str, library: str): # type: ignore
         login_path = self.find_elem_in_page(LOGIN_PAGE_URL, "#borchk-login-form", "action")
         library_attr_name = self.find_elem_in_page(LOGIN_PAGE_URL, "#borchk-login-form label", "for")
         libraries = self._get_libraries()
         logging.debug(f"{login_path=}")
         logging.debug(f"{library_attr_name=}")
         logging.debug(f"{libraries=}")
         if library not in libraries.keys():
@@ -71,26 +36,64 @@
                 library_attr_name: library,
                 "agency": libraries[library],
                 "userId": username,
                 "pincode": password
             }
         )
 
-    def prepare(self):
-        ajax: Optional[dict] = self.get_json(f"{self.url}/listen/ajax")
+
+    def download(self, url: str) -> Audiobook:
+        ajax: Optional[Dict] = self.get_json(f"{url}/listen/ajax")
         if not ajax:
             raise RequestError
-        logging.debug(f"{ajax=}")
         if ajax[1]["title"] != "Lyt":
             raise UserNotAuthorized
         id_match = re.search(r"(?<=(o=))[0-9a-f\-]+", ajax[1]["data"])
         if id_match and id_match.group():
-            self.book_id = id_match.group()
-            logging.debug(f"{self.book_id=}")
+            book_id = id_match.group()
+            logging.debug(f"{book_id=}")
         else:
             logging.debug("Could not find book id")
             raise UserNotAuthorized
-        meta: Optional[dict] = self.get_json(f"https://audio.api.streaming.pubhub.dk/v1/orders/{self.book_id}")
+        meta: Optional[dict] = self.get_json(f"https://audio.api.streaming.pubhub.dk/v1/orders/{book_id}")
         if meta is None:
             raise UserNotAuthorized
-        self.meta = meta
-        logging.debug(f"{self.meta=}")
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(book_id),
+            metadata = self.get_metadata(meta),
+            cover = self.get_cover(meta),
+        )
+
+
+    def get_metadata(self, meta) -> AudiobookMetadata:
+        title = meta["title"]
+        metadata = AudiobookMetadata(title)
+        metadata.add_author(meta["artist"])
+        return metadata
+
+
+    def get_cover(self, meta) -> Cover:
+        cover_data = self.get(meta["cover"])
+        return Cover(cover_data, "jpg")
+
+
+    def get_files(self, book_id: str) -> List[AudiobookFile]:
+        return self.get_stream_files(
+            f"https://audio.api.streaming.pubhub.dk/v1/stream/hls/{book_id}/playlist.m3u8"
+        )
+
+
+    def _get_libraries(self):
+        """Returns list of available libraries for login"""
+        libraries_raw = self.find_in_page(
+            LOGIN_PAGE_URL,
+            "libraries = ({.+})<",
+            group_index=1
+        )
+        libraries = {}
+        for library in json.loads(libraries_raw)["folk"]:
+            library_name = library["name"]
+            library_id = library["branchId"]
+            libraries[library_name] = library_id
+        return libraries
+
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/librivox.py` & `audiobook-dl-0.6.0/audiobookdl/sources/librivox.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from .source import Source
-from audiobookdl import AudiobookFile, AudiobookMetadata, Cover
+from audiobookdl import AudiobookFile, AudiobookMetadata, Cover, Audiobook
+from typing import List
 
 
 class LibrivoxSource(Source):
-    _authentication_methods: list[str] = []
+    _authentication_methods: List[str] = []
 
     names = [ "Librivox" ]
 
     match = [
         r"https?://librivox.org/.+"
     ]
+    def download(self, url: str) -> Audiobook:
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(url),
+            metadata = self.get_metadata(url),
+            cover = self.get_cover(url)
+        )
 
 
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.find_elem_in_page(self.url, ".content-wrap h1")
+    def get_metadata(self, url: str) -> AudiobookMetadata:
+        title = self.find_elem_in_page(url, ".content-wrap h1")
         return AudiobookMetadata(title)
 
-    def get_cover(self) -> Cover:
+    def get_cover(self, url: str) -> Cover:
         cover_url = self.find_elem_in_page(
-            self.url,
+            url,
             ".book-page-book-cover img",
             data="src"
         )
         cover_data = self.get(cover_url)
         return Cover(cover_data, "jpg")
 
-    def get_files(self) -> list[AudiobookFile]:
-        parts = self.find_elems_in_page(self.url,
-                                        ".chapter-download .chapter-name")
+    def get_files(self, url: str) -> List[AudiobookFile]:
+        parts = self.find_elems_in_page(url, ".chapter-download .chapter-name")
         files = []
         for part in parts:
             files.append(AudiobookFile(
                 url = part.get("href"),
                 title = part.text,
                 ext = "mp3"
             ))
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/nextory.py` & `audiobook-dl-0.6.0/audiobookdl/sources/nextory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover
-from typing import Any, Optional
+from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover, Audiobook
+from audiobookdl.exceptions import DataNotPresent
+from typing import Any, Optional, Dict
 import hashlib
 import uuid
 import platform
 
 
 def calculate_checksum(username: str, password: str, salt: str) -> str:
     return get_checksum(username + salt + password)
@@ -20,42 +21,66 @@
 
 def get_device_id() -> str:
     return str(uuid.uuid3(uuid.NAMESPACE_DNS, "audiobook-dl"))
 
 
 class NextorySource(Source):
     match = [
-        r"https?://(www.)?nextory.+",
+        r"https?://((www|catalog-\w\w).)?nextory.+",
     ]
     names = [ "Nextory" ]
     _authentication_methods = [
         "login",
     ]
 
     user_data: dict
     book_info: dict
 
+    def download(self, url) -> Audiobook:
+        book_id = url.split("-")[-1].replace("/", "")
+        book_info = self.find_book_info(book_id)
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(book_info),
+            metadata = self.get_metadata(book_info),
+            cover = self.get_cover(book_info),
+        )
+
+
+    def find_book_info(self, book_id: str) -> Dict:
+        """
+        Find metadata about book in list of active books
+
+        :param book_id: Book id
+        :returns: Book metadata
+        """
+        for book in self.user_data["active"]["data"]["books"]:
+            if str(book["id"]) == book_id:
+                return book
+        raise DataNotPresent
+
+
     def get_salt(self) -> str:
         url = "https://api.nextory.se/api/app/catalogue/7.5/salt"
         resp = self._session.get(url)
         if resp.status_code != 200:
             raise RuntimeError("Couldn't get salt from nextory.")
         return resp.json()["data"]["salt"]
 
-    def _login(self, username: str, password: str):
+
+    def _login(self, url: str, username: str, password: str):
         # Step one
         login_url = "https://api.nextory.se/api/app/user/7.5/login"
         headers = {
             "appid": "200",
             "model": "Personal Computer",
             "locale": "en_GB",
             "deviceid": get_device_id(),
             "osinfo": platform.platform(),
             "version": "4.34.6",
-            #"user-agent": "okhttp/4.9.3",
         }
 
         self._session.headers = headers
         salt = self.get_salt()
         files = {
             "username": (None, username),
             "password": (None, password),
@@ -71,17 +96,18 @@
         # Step two
         resp = self._session.get("https://api.nextory.se/api/app/user/7.5/accounts/list")
         if resp.status_code != 200:
             raise PermissionError("Error in NextorySource login step two")
         account_list = resp.json()
 
         # Step three
+        login_key = account_list["data"]["accounts"][0]["loginkey"]
         params = {
-            "loginkey": account_list["data"]["accounts"][0]["loginkey"],
-            "checksum": calculate_password_checksum(account_list["data"]["accounts"][0]["loginkey"], salt)
+            "loginkey": login_key,
+            "checksum": calculate_password_checksum(login_key, salt)
         }
 
         resp = self._session.get(login_url, params=params)
         if resp.status_code != 200:
             raise PermissionError("Error in NextorySource login step three")
 
         account_info = resp.json()
@@ -100,38 +126,40 @@
             "account_list": account_list,
             "account_info": account_info,
             "active": active,
         }
         self._session.headers.update({'apiver': "7.5"})
 
 
-    def get_files(self) -> list[AudiobookFile]:
-        return [AudiobookFile(url=self.book_info["file"]["url"], headers=self._session.headers, ext="mp3")]
+    def get_files(self, book_info) -> list[AudiobookFile]:
+        return [
+            AudiobookFile(
+                url=book_info["file"]["url"],
+                headers=self._session.headers,
+                ext="mp3"
+            )
+        ]
 
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.book_info["title"]
+
+    def get_metadata(self, book_info) -> AudiobookMetadata:
+        title = book_info["title"]
         metadata = AudiobookMetadata(title)
         try:
-            book_info = self._session.get("https://api.nextory.se/api/app/product/7.5/bookinfo",
-                                         params={"id": self.book_info["id"]}).json()
             metadata.add_authors(self.book_info["authors"])
-            metadata.add_narrators(book_info["data"]["books"]["narrators"])
+            narrators = self._session.get(
+                "https://api.nextory.se/api/app/product/7.5/bookinfo",
+                params={"id": self.book_info["id"]}
+            ).json()["data"]["books"]["narrators"]
+            metadata.add_narrators(narrators)
             return metadata
         except:
             return metadata
 
     def get_chapters(self) -> list[Chapter]:
         # Nextory has no chapters...?
         return []
 
-    def get_cover(self) -> Cover:
-        cover_url = self.book_info["imgurl"].replace("{$width}", "640")
+
+    def get_cover(self, book_info) -> Cover:
+        cover_url = book_info["imgurl"].replace("{$width}", "640")
         cover_data = self.get(cover_url)
         return Cover(cover_data, "jpg")
-
-    def prepare(self):
-        wanted_id = self.url.split("-")[-1].replace("/", "")
-        for book in self.user_data["active"]["data"]["books"]:
-            if str(book["id"]) == wanted_id:
-                self.book_info = book
-                return
-        raise PermissionError(f"Book with id {wanted_id} was not found in My Library.")
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/overdrive.py` & `audiobook-dl-0.6.0/audiobookdl/sources/overdrive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,92 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover
+from audiobookdl import AudiobookFile, Chapter, AudiobookMetadata, Cover, Audiobook
 from audiobookdl.exceptions import DataNotPresent, UserNotAuthorized
 
 import re
 import json
 from urllib3.util import parse_url
+from typing import List
 
 
 class OverdriveSource(Source):
     match = [
         r"https://.+\.listen\.overdrive\.com"
     ]
-
     names = [ "Overdrive", "Libby" ]
 
-    def prepare(self):
+
+    def download(self, url: str) -> Audiobook:
         # Parse url
-        parsed_url = parse_url(self.url)
+        parsed_url = parse_url(url)
         hostname = parsed_url.hostname
-        self.prefix = f"https://{hostname}"
+        prefix = f"https://{hostname}"
         # Extract json from javascript
-        raw = self.find_in_page(self.url, 'window.bData = {.+;')
+        raw = self.find_in_page(url, 'window.bData = {.+;')
         if raw is None:
             raise UserNotAuthorized
         raw_trimmed = raw[15:-1]
-        self.meta = json.loads(raw_trimmed)
-        # Table of contents
-        self.toc = []
-        for part in self.meta["nav"]["toc"]:
-            if "contents" in part:
-                self.toc = []
-                for _ in range(len(self.meta["spine"])):
-                    self.toc.append(self.meta["nav"]["toc"][0]["title"])
-                break
-            else:
-                self.toc.append(part["title"])
+        book_info = json.loads(raw_trimmed)
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(prefix, book_info),
+            metadata = self.get_metadata(book_info),
+            cover = self.get_cover(prefix, book_info),
+            chapters = self.get_chapters(book_info)
+        )
 
 
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.meta["title"]["main"]
+    def get_metadata(self, book_info) -> AudiobookMetadata:
+        title = book_info["title"]["main"]
         metadata = AudiobookMetadata(title)
-        for creator in self.meta["creator"]:
+        for creator in book_info["creator"]:
             if creator["role"] == "author":
                 metadata.add_author(creator["name"])
             if creator["role"] == "narrator":
                 metadata.add_narrator(creator["name"])
         return metadata
 
-    def get_cover(self) -> Cover:
-        cover_url = self.prefix + self.meta['-odread-furbish-uri']
+    def get_cover(self, prefix: str, book_info) -> Cover:
+        cover_url = f"{prefix}/{book_info['-odread-furbish-uri']}"
         cover_data = self.get(cover_url)
         return Cover(cover_data, "jpg")
 
-    def _get_previous_length(self, index) -> int:
+    def _get_previous_length(self, index: int, book_info) -> int:
         """Returns the ending point of the previous part"""
         if index == 0:
             return 0
-        return self._get_previous_length(index-1) + \
-            self.meta["spine"][index-1]["audio-duration"]
+        return self._get_previous_length(index-1, book_info) + \
+            book_info["spine"][index-1]["audio-duration"]
 
-    def get_chapters(self) -> list[Chapter]:
+    def get_chapters(self, book_info) -> List[Chapter]:
         chapters = []
-        for chapter in self.meta["nav"]["toc"]:
+        for chapter in book_info["nav"]["toc"]:
             timepoint = 0.
             if '#' in chapter["path"]:
                 timepoint = float(chapter["path"].split("#")[1])
             part_result = re.search(r"(?<=(Part))\d+", chapter["path"])
             if part_result is None:
                 continue
             part = int(part_result.group(0))-1
-            start = int((self._get_previous_length(part)+timepoint)*1000)
+            start = int((self._get_previous_length(part, book_info)+timepoint)*1000)
             chapters.append(Chapter(start, chapter["title"]))
         return chapters
 
-    def get_files(self) -> list[AudiobookFile]:
+
+    def get_files(self, prefix: str, book_info) -> List[AudiobookFile]:
+        toc: List[str] = []
+        for part in book_info["nav"]["toc"]:
+            if "contents" in part:
+                toc = []
+                for _ in range(len(book_info["spine"])):
+                    toc.append(book_info["nav"]["toc"][0]["title"])
+                break
+            else:
+                toc.append(part["title"])
         files = []
-        for num, part in enumerate(self.meta["spine"]):
+        for num, part in enumerate(book_info["spine"]):
             files.append(AudiobookFile(
-                url = f"{self.prefix}/{part['path']}",
-                title = self.toc[num],
+                url = f"{prefix}/{part['path']}",
+                title = toc[num],
                 ext = "mp3"
             ))
         return files
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/saxo.py` & `audiobook-dl-0.6.0/audiobookdl/sources/saxo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from .source import Source
-from audiobookdl import logging, AudiobookFile, AudiobookMetadata, Chapter, Cover
+from audiobookdl import logging, AudiobookFile, AudiobookMetadata, Chapter, Cover, Audiobook
 from audiobookdl.exceptions import NoSourceFound
 from audiobookdl.utils.audiobook import AESEncryption
 import re
+from typing import List
 
 class SaxoSource(Source):
     _authentication_methods = [
         "login"
     ]
     names = [ "Saxo" ]
     match = [
         r"https?://(www.)?saxo.(com|dk)/[^/]+/.+"
     ]
     _APP_OS = "android"
     _APP_VERSION = "6.2.4"
 
-    def _login(self, username: str, password: str) -> None:
+    def _login(self, url: str, username: str, password: str) -> None:
         resp = self.post_json(
             "https://auth-read.saxo.com/auth/token",
             data = {
                 "username": username,
                 "password": password,
                 "grant_type": "password",
             },
@@ -28,17 +29,31 @@
             }
         )
         self.bearer_token = resp["access_token"]
         self.user_id = resp["id"]
         logging.debug(f"{self.bearer_token=}")
         logging.debug(f"{self.user_id=}")
 
-    def _get_isbn(self) -> str:
+
+    def download(self, url: str) -> Audiobook:
+        isbn = self._extract_isbn(url)
+        book_id = self._search_for_book(isbn)
+        logging.debug(f"{book_id=}")
+        book_info = self._get_book_metadata(book_id)
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(book_info),
+            metadata = self.get_metadata(book_info),
+            cover = self.get_cover(book_info),
+        )
+
+
+    def _extract_isbn(self, url: str) -> str:
         """Extract isbn of book from url"""
-        isbn_match = re.search(f"\d+$", self.url)
+        isbn_match = re.search(r"\d+$", url)
         if isbn_match and isbn_match.group():
             return isbn_match.group()
         else:
             raise NoSourceFound
 
     def _search_for_book(self, isbn: str) -> str:
         """Search for internal book id by isbn number"""
@@ -63,20 +78,22 @@
                 "Appauthorization": f"bearer {self.bearer_token}",
                 "App-Os": self._APP_OS,
                 "App-Version": self._APP_VERSION,
             },
             json = [ book_id ]
         )["items"][0]
 
-    def get_files(self) -> list[AudiobookFile]:
+
+    def get_files(self, book_info) -> List[AudiobookFile]:
         result = []
-        for file in self.book_meta["techInfo"]["chapters"]:
+        book_id = book_info["bookId"]
+        for file in book_info["techInfo"]["chapters"]:
             filename = file["fileName"]
             link = self.get_json(
-                f"https://api-read.saxo.com/api/v1/book/{self.book_meta['bookId']}/content/encryptedstream/{filename}",
+                f"https://api-read.saxo.com/api/v1/book/{book_id}/content/encryptedstream/{filename}",
                 headers = {
                     "Appauthorization": f"bearer {self.bearer_token}",
                     "App-Os": self._APP_OS,
                     "App-Version": self._APP_VERSION,
                 },
             )["link"]
             result.append(AudiobookFile(
@@ -86,26 +103,21 @@
                 encryption_method = AESEncryption(
                     b"CD3E9D141D8EFC0886912E7A8F3652C4",
                     b"78CB354D377772F1",
                 )
             ))
         return result
 
-    def get_metadata(self) -> AudiobookMetadata:
-        metadata: dict = self.book_meta["bookMetadata"]
+    def get_metadata(self, book_info) -> AudiobookMetadata:
+        metadata: dict = book_info["bookMetadata"]
         title = metadata["title"]
         result = AudiobookMetadata(title)
         result.add_authors(metadata["authors"])
         result.add_narrators(metadata["readBy"])
         result.series = metadata.get("seriesName")
         return result
 
-    def get_cover(self) -> Cover:
-        cover_url = self.book_meta["bookMetadata"]["image"]["highQualityImageUrl"]
+
+    def get_cover(self, book_info) -> Cover:
+        cover_url = book_info["bookMetadata"]["image"]["highQualityImageUrl"]
         bytes = self.get(cover_url)
         return Cover(bytes, "jpg")
-
-    def prepare(self) -> None:
-        isbn = self._get_isbn()
-        book_id = self._search_for_book(isbn)
-        logging.debug(f"{book_id=}")
-        self.book_meta = self._get_book_metadata(book_id)
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/source/__init__.py` & `audiobook-dl-0.6.0/audiobookdl/sources/source/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,108 +1,114 @@
 # Internal imports
 from . import networking
-from audiobookdl import logging, AudiobookFile, Chapter, AudiobookMetadata, Cover
+from audiobookdl import logging, AudiobookFile, Chapter, AudiobookMetadata, Cover, Result, Audiobook, BookId
 from audiobookdl.exceptions import DataNotPresent
 
 # External imports
 import requests
 import lxml.html
 from lxml.cssselect import CSSSelector
 import re
 from http.cookiejar import MozillaCookieJar
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional, TypeVar, Generic
 
-class Source:
+T = TypeVar("T")
+
+class Source(Generic[T]):
     """An abstract class for downloading audiobooks from a specific
     online source."""
 
     # Data required for logging in
-    login_data: list[str] = [ "username", "password" ]
+    login_data: List[str] = [ "username", "password" ]
     # A list of regexes that indicates which website a sevice supports
-    match: list[str] = []
+    match: List[str] = []
     # list of names
-    names: list[str] = []
+    names: List[str] = []
     # Methods for authenticating
-    _authentication_methods: list[str] = [ "cookies" ]
+    _authentication_methods: List[str] = [ "cookies" ]
     # If cookies are loaded
     __authenticated = False
     # Cache of previously loaded pages
-    __pages: dict[str, bytes] = {}
+    __pages: Dict[str, bytes] = {}
+
 
-    def __init__(self, url, match_num):
-        self.url = url
-        self.match_num = match_num
+    def __init__(self):
         self._session = requests.Session()
 
+
+    @property
+    def name(self) -> str:
+        """Primary name of source"""
+        return self.names[0].lower()
+
+
     @property
     def requires_authentication(self):
         """Returns `True` if this source requires authentication to download books"""
         return len(self._authentication_methods) > 0
 
+
     @property
     def authenticated(self):
         """Returns `True` if the source has been authenticated"""
         return self.__authenticated
 
+
     @property
     def supports_cookies(self):
+        """Returns `True` if the source supports authentication with cookies"""
         return "cookies" in self._authentication_methods
 
+
     def load_cookie_file(self, cookie_file: str):
         """Loads cookies from a cookie file into session"""
         if self.supports_cookies:
+            logging.debug(f"Loading cookies from '{cookie_file}'")
             cookie_jar = MozillaCookieJar()
             cookie_jar.load(cookie_file, ignore_expires=True)
             self._session.cookies.update(cookie_jar)
             self.__authenticated = True
 
+
     @property
     def supports_login(self):
+        """Returns `True` if the source supports authentication with login"""
         return "login" in self._authentication_methods
 
-    def _login(self, username: str, password: str):
+
+    def _login(self, url: str, username: str, password: str):
         pass
 
-    def login(self, **kwargs) -> None:
+
+    def login(self, url: str, **kwargs) -> None:
         """Authenticate with source using username and password"""
         if self.supports_login:
-            self._login(**kwargs)
+            logging.debug("Logging in")
+            self._login(url, **kwargs)
             self.__authenticated = True
 
-    def prepare(self) -> None:
-        """Operations to be run before the audiobook is downloaded"""
-        pass
 
-    def get_metadata(self) -> AudiobookMetadata:
-        """Returns metadata of the audiobook"""
-        raise NotImplemented
+    def download_from_id(self, book_id: T) -> Audiobook:
+        """Download book specified by id"""
+        raise NotImplementedError
 
-    def get_cover(self) -> Optional[Cover]:
-        """Returns the image data for the audiobook"""
-        return None
 
-    def get_files(self) -> list[AudiobookFile]:
-        """Return a list of audio files for the audiobook"""
-        raise NotImplemented
-
-    def get_chapters(self) -> list[Chapter]:
-        """
-        Returns a list of tuples with the starting point of the chapter and
-        the title of the chapter
-        """
-        return []
+    def download(self, url: str) -> Result:
+        """Download book or series"""
+        raise NotImplementedError
 
 
     def _get_page(self, url: str, **kwargs) -> bytes:
         """Download a page and caches it"""
         if url not in self.__pages:
             resp = self.get(url, **kwargs)
             self.__pages[url] = resp
         return self.__pages[url]
 
+
     def find_elem_in_page(self, url: str, selector: str, data=None, **kwargs):
         """
         Find the first html element in page from `url` that matches `selector`.
         Will return the attribute specified in `data`. Will return element text
         if `data` is `None`.
         Will cache the page.
         """
@@ -111,38 +117,41 @@
             logging.debug(f"Could not find matching element from {url} with {selector}")
             raise DataNotPresent
         elem = results[0]
         if data is None:
             return elem.text
         return elem.get(data)
 
-    def find_elems_in_page(self, url: str, selector: str, **kwargs) -> list[Any]:
+
+    def find_elems_in_page(self, url: str, selector: str, **kwargs) -> list:
         """
         Find all html elements in the page from `url` thats matches `selector`.
         Will cache the page.
         """
         sel = CSSSelector(selector)
         page: bytes = self._get_page(url, **kwargs)
         tree = lxml.html.fromstring(page.decode("utf8"))
         results = sel(tree)
         return results
 
+
     def find_in_page(self, url: str, regex: str, group_index: int = 0, **kwargs) -> str:
         """
         Find some text in a page based on a regex.
         Will cache the page.
         """
         page = self._get_page(url, **kwargs).decode("utf8")
         m = re.search(regex, page)
         if m is None:
             logging.debug(f"Could not find match from {url} with {regex}")
             raise DataNotPresent
         return m.group(group_index)
 
-    def find_all_in_page(self, url: str, regex: str, **kwargs) -> list[Any]:
+
+    def find_all_in_page(self, url: str, regex: str, **kwargs) -> list:
         """
         Find all places in a page that matches the regex.
         Will cache the page.
         """
         return re.findall(regex, self._get_page(url, **kwargs).decode("utf8"))
 
     # Networking
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/source/networking.py` & `audiobook-dl-0.6.0/audiobookdl/sources/source/networking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from audiobookdl import AudiobookFile, exceptions, logging
 from audiobookdl.utils.audiobook import AESEncryption
 
+from typing import Dict, List
 import json
 import os
 import m3u8
 import requests
 
 
 def post(self, url: str, **kwargs) -> bytes:
@@ -40,15 +41,15 @@
 
 def get_json(self, url: str, **kwargs) -> dict:
     """Downloads data with the given url and converts it to json"""
     resp = self.get(url, **kwargs)
     return json.loads(resp.decode('utf8'))
 
 
-def get_stream_files(self, url: str, headers={}) -> list[AudiobookFile]:
+def get_stream_files(self, url: str, headers={}) -> List[AudiobookFile]:
     """Creates a list of audio files from an m3u8 file"""
     playlist = m3u8.load(url, headers=headers)
     files = []
     for _, seg in enumerate(playlist.segments):
         current = AudiobookFile(
             url = seg.absolute_uri,
             ext = os.path.splitext(seg.absolute_uri)[1][1:],
@@ -59,15 +60,15 @@
                 key = self._get_page(seg.key.absolute_uri, headers=headers),
                 iv = int(seg.key.iv, 0).to_bytes(16, byteorder='big')
             )
         files.append(current)
     return files
 
 
-def _get_all_cookies(session: requests.Session) -> dict[str, str]:
+def _get_all_cookies(session: requests.Session) -> Dict[str, str]:
     """
     Retrieves all cookies from session
 
     :returns: Dictionary of cookies
     """
     cookies = {}
     for cookie in session.cookies:
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/sources/storytel.py` & `audiobook-dl-0.6.0/audiobookdl/sources/yourcloudlibrary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,147 @@
 from .source import Source
-from audiobookdl import AudiobookFile, Chapter, logging, AudiobookMetadata, Cover
-from audiobookdl.exceptions import UserNotAuthorized, MissingBookAccess
-from Crypto.Cipher import AES
-from Crypto.Util.Padding import pad
-from typing import Any, Optional
+from audiobookdl import AudiobookFile, logging, AudiobookMetadata, Cover, Audiobook
+from audiobookdl.exceptions import UserNotAuthorized, RequestError
 
+import requests.utils
+import base64
+from typing import List
 
-class StorytelSource(Source):
+class YourCloudLibrarySource(Source):
     match = [
-        r"https?://(www.)?(storytel|mofibo).com/.+/books/.+",
+        r"https?://ebook.yourcloudlibrary.com/library/[^/]+/AudioPlayer/.+"
     ]
-    names = [ "Storytel", "Mofibo" ]
+    names = [ "YourCloudLibrary" ]
     _authentication_methods = [
-        "login",
+        "cookies",
+        "login"
     ]
 
-    user_data: dict
-    book_info: dict
+    def download(self, url: str) -> Audiobook:
+        fullfillment_token = self.download_fullfillment_token(url)
+        book_info = self.download_book_info(url)
+        library = self.extract_library_id(url)
+        audioplayer = self.post_json(
+            f"https://ebook.yourcloudlibrary.com/uisvc/{library}/AudioPlayer",
+            data = {
+                "url": f"{book_info['fullfillmentTokenUrl']}&token={fullfillment_token}"
+            }
+        )
+        fulfillment_id = audioplayer["fulfillmentId"]
+        account_id = audioplayer["accountId"]
+        session_key = audioplayer["sessionKey"]
+        headers = { "Session-Key": session_key }
+        meta = self.get_json(
+            f"https://api.findawayworld.com/v4/accounts/{account_id}/audiobooks/{fulfillment_id}",
+            headers=headers
+        )
+        playlist = self.post_json(
+            f"https://api.findawayworld.com/v4/audiobooks/{fulfillment_id}/playlists",
+            json = {
+                "license_id": audioplayer["licenseId"]
+            },
+            headers=headers
+        )
+        return Audiobook(
+            session = self._session,
+            files = self.get_files(playlist),
+            metadata = self.get_metadata(book_info, meta),
+            cover = self.download_cover(meta),
+        )
 
-    @staticmethod
-    def encrypt_password(password: str) -> str:
-        # Thanks to https://github.com/javsanpar/storytel-tui
-        key = b"VQZBJ6TD8M9WBUWT"
-        iv = b"joiwef08u23j341a"
-        msg = pad(password.encode(), AES.block_size)
-        cipher = AES.new(key, AES.MODE_CBC, iv)
-        cipher_text = cipher.encrypt(msg)
-        return cipher_text.hex()
-
-    def _login(self, username: str, password: str):
-        password = self.encrypt_password(password)
-        url = f"https://www.storytel.com/api/login.action?m=1&uid={username}&pwd={password}"
-        self._session.headers.update({
-            "content-type": "application/x-www-form-urlencoded",
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/109.0"
-        })
-        resp = self._session.get(url)
-        if resp.status_code != 200:
-            raise UserNotAuthorized
-        self._session.headers.update({"authorization": f"Bearer {resp.json()['accountInfo']['jwt']}"})
-        self.user_data = resp.json()
 
+    @staticmethod
+    def get_files(playlist) -> List[AudiobookFile]:
+        files = []
+        for f in playlist["playlist"]:
+            files.append(AudiobookFile(
+                url = f["url"],
+                ext = "mp3"
+            ))
+        return files
 
-    def get_files(self) -> list[AudiobookFile]:
-        aid = self.book_info["book"]["AId"]
-        url = f"https://www.storytel.com/mp3streamRangeReq?startposition=0&programId={aid}" \
-              f"&token={self.user_data['accountInfo']['singleSignToken']}"
-        return [AudiobookFile(url=url, headers=self._session.headers, ext="mp3")]
 
-    def get_metadata(self) -> AudiobookMetadata:
-        title = self.book_info["book"]["name"]
+    def get_metadata(self, book_info, meta) -> AudiobookMetadata:
+        title = book_info["Title"]
         metadata = AudiobookMetadata(title)
-        try:
-            for author in self.book_info["book"]["authors"]:
-                metadata.add_author(author["name"])
-            for narrator in self.book_info["abook"]["narrators"]:
-                metadata.add_narrator(narrator["name"])
-            if "series" in self.book_info["book"]:
-                if len(self.book_info["book"]["series"]) > 0:
-                    metadata.series = self.book_info["book"]["series"][0]["name"]
-            return metadata
-        except:
-            return metadata
-
-    def get_chapters(self) -> list[Chapter]:
-        url = f"https://api.storytel.net/playback-metadata/consumable/{self.book_info['book']['consumableId']}"
-        try:
-            chapters: list[Chapter] = []
-            storytel_metadata = self._session.get(url).json()
-            if "formats" in storytel_metadata and len(storytel_metadata["formats"]) > 0:
-                # Find audiobook format
-                for format in storytel_metadata["formats"]:
-                    if format["type"] == "abook":
-                        f = format
-                logging.debug(f"{f=}")
-                # Add chapters
-                if "chapters" in f and len(f["chapters"]) > 0:
-                    start_time = 0
-                    for c in f["chapters"]:
-                        chapters.append(Chapter(start_time, c["title"] if c["title"] else f"Chapter {c['number']}"))
-                        start_time += c["durationInMilliseconds"]
-            return chapters
-        except:
-            return []
+        if not meta is None:
+            audiobook = meta["audiobook"]
+            metadata.add_authors(audiobook["authors"])
+            metadata.add_narrators(audiobook["narrators"])
+            if audiobook["series"] is not None and len(audiobook["series"]) >= 1:
+                metadata.series = audiobook["series"][0]
+        return metadata
 
-    def get_cover(self) -> Cover:
-        cover_url = f"https://www.storytel.com/images/{self.book_info['abook']['isbn']}/640x640/cover.jpg"
+
+    def download_cover(self, meta) -> Cover:
+        cover_url = meta['audiobook']['cover_url']
         cover_data = self.get(cover_url)
         return Cover(cover_data, "jpg")
 
-    def prepare(self):
-        wanted_id = self.url.split("-")[-1]
-        bookshelf_url = f"https://www.storytel.com/api/getBookShelf.action" \
-                        f"?token={self.user_data['accountInfo']['singleSignToken']}"
-        self.user_data["bookshelf"] = self._session.get(bookshelf_url).json()
-        for book in self.user_data["bookshelf"]["books"]:
-            if book["book"]["consumableId"] == wanted_id:
-                self.book_info = book
-                return
-        raise MissingBookAccess
+
+    @staticmethod
+    def extract_library_id(url: str) -> str:
+        """
+        Extract library id from url
+
+        :param url: Url 
+        :returns: Library id
+        """
+        return url.split("/")[-3]
+
+
+    def download_fullfillment_token(self, url: str) -> str:
+        """
+        Download and extract fullfillment token
+
+        :param url: Book url
+        :returns: Fullfillment token
+        """
+        token_base64 = self.find_in_page(
+            url,
+            r"(?<=(\"Osi\":\"x-))[^\"]+",
+            force_cookies = True,
+        )
+        if token_base64 is None:
+            raise UserNotAuthorized
+        token = base64.b64decode(token_base64).decode('utf8')
+        logging.debug(f"{token=}")
+        return token
+
+
+    def download_book_info(self, url: str) -> dict:
+        """
+        Download metadata about book
+
+        :param url: Book url
+        :returns: Metadata about book
+        """
+        # Get list of borrowed books
+        library = self.extract_library_id(url)
+        borrowed = self.get_json(
+            f"https://ebook.yourcloudlibrary.com/uisvc/{library}/Patron/Borrowed",
+            force_cookies = True
+        )
+        if borrowed is None:
+            raise UserNotAuthorized
+        # Find the matching book in list of borrowed books
+        url_id = url.split("/")[-1]
+        book_info = None
+        for i in borrowed:
+            if i["Id"] == url_id:
+                book_info = i
+        if book_info is None:
+            raise UserNotAuthorized
+        return book_info
+
+
+    def _login(self, url: str, username: str, password: str):
+        library = self.extract_library_id(url)
+        resp = self.post(
+            f"https://ebook.yourcloudlibrary.com/uisvc/{library}/Patron/LoginPatron",
+            data = {
+                "UserId": username,
+                "Password": password
+            }
+        )
+        # TODO Validate authentication
+        logging.debug(f"Authentication response {resp.decode('utf8')}")
```

### Comparing `audiobook-dl-0.5.0/audiobookdl/utils/__init__.py` & `audiobook-dl-0.6.0/audiobookdl/utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import importlib.resources
+from typing import Sequence
+import shutil
 
 def levenstein_distance(a: str, b: str) -> int:
     """
     Calculates the levenstein distance between `a` and `b`
 
     https://en.wikipedia.org/wiki/Levenshtein_distance
     """
@@ -14,19 +16,24 @@
         return levenstein_distance(a[1:], b[1:])
     return 1 + min(
         levenstein_distance(a, b[1:]), # Character is inserted
         levenstein_distance(a[1:], b), # Character is deleted
         levenstein_distance(a[1:], b[1:]) # Character is replaced
     )
 
-def nearest_string(input: str, list: list[str]) -> str:
+def nearest_string(input: str, list: Sequence[str]) -> str:
     """
     Returns the closest element in `list` to `input` based on the levenstein
     distance
     """
     return sorted(list, key = lambda x: levenstein_distance(input, x))[0]
 
 
 def read_asset_file(path: str) -> str:
     return importlib.resources.files("audiobookdl") \
         .joinpath(path) \
         .read_text(encoding="utf8")
+
+
+def program_in_path(program: str) -> bool:
+    """Checks whethher `program` is in the path"""
+    return shutil.which(program) is not None
```

### Comparing `audiobook-dl-0.5.0/pyproject.toml` & `audiobook-dl-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -20,30 +20,31 @@
     "lxml",
     "rich",
     "mutagen",
     "pillow",
     "cssselect",
     "m3u8",
     "pycryptodome",
-    "importlib-resources"
+    "importlib-resources",
+    "attrs"
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/jo1gi/audiobook-dl"
 "Bugtracker" = "https://github.com/jo1gi/audiobook-dl/issues"
 
 [project.scripts]
 audiobook-dl = "audiobookdl.__main__:run"
 
 [tool.setuptools.dynamic]
 version = {attr = "audiobookdl.__version__"}
 
 [tool.setuptools.package-data]
-mypkg = ["*.txt"]
+audiobookdl = ["*.txt"]
 
 [tool.mypy]
 ignore_missing_imports = true
 allow_untyped_globals = false
 disallow_untyped_calls = true
 
 [[tool.mypy.overrides]]
```

### Comparing `audiobook-dl-0.5.0/supported_sites.md` & `audiobook-dl-0.6.0/supported_sites.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,11 +5,12 @@
 | audiobooks.com   |    ✓    |         ✗         |                                                                                                |
 | BookBeat         |    ✗    |         ✓         | Books must be saved to My Books <br> Not tested with multi-user account <br> No metadata (yet) |
 | Chirp            |    ✓    |         ✗         |                                                                                                |
 | eReolen          |    ✓    |         ✓         | Requires library for login                                                                     |
 | Librivox         |    ✗    |         ✗         | Authentication not required                                                                    |
 | Nextory          |    ✗    |         ✓         | Books must be in "Your Library" <br/>Only single (first) account supported                     |
 | Overdrive        |    ✓    |         ✗         |                                                                                                |
+| Podimo           |    ✗    |         ✓         |                                                                                                |
 | Saxo             |    ✗    |         ✓         |                                                                                                |
 | Scribd           |    ✓    |         ✗         |                                                                                                |
 | Storytel         |    ✗    |         ✓         | Books have to be in your bookshelf                                                             |
 | YourCloudLibrary |    ✓    |         ✓         |                                                                                                |
```

### Comparing `audiobook-dl-0.5.0/tests/test_urls.py` & `audiobook-dl-0.6.0/tests/test_urls.py`

 * *Files identical despite different names*

