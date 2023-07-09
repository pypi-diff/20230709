# Comparing `tmp/PythonCA-1.23.3.2.tar.gz` & `tmp/PythonCA-1.23.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonCA-1.23.3.2.tar", last modified: Tue Jun  7 01:08:33 2022, max compression
+gzip compressed data, was "PythonCA-1.23.3.7.tar", last modified: Sun Jul  9 02:41:44 2023, max compression
```

## Comparing `PythonCA-1.23.3.2.tar` & `PythonCA-1.23.3.7.tar`

### file list

```diff
@@ -1,181 +1,139 @@
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.503808 PythonCA-1.23.3.2/
--rw-r--r--   0 noboru     (501) admin       (80)    10244 2020-03-27 02:37:26.000000 PythonCA-1.23.3.2/.DS_Store
--rw-r--r--   0 noboru     (501) admin       (80)      371 2020-11-18 04:01:46.000000 PythonCA-1.23.3.2/.hgignore
--rw-r--r--   0 noboru     (501) admin       (80)      692 2022-06-07 00:48:05.000000 PythonCA-1.23.3.2/.hgtags
--rwxr-xr-x   0 noboru     (501) admin       (80)    24225 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/CaChannel.py
--rw-r--r--   0 noboru     (501) admin       (80)     1120 2022-05-09 02:01:34.000000 PythonCA-1.23.3.2/EPICS_config_Darwin.py
--rw-r--r--   0 noboru     (501) admin       (80)     1133 2022-05-09 03:43:19.000000 PythonCA-1.23.3.2/EPICS_config_Darwin.pyc
--rw-r--r--   0 noboru     (501) admin       (80)      364 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/EPICS_config_Linux.py
--rw-r--r--   0 noboru     (501) admin       (80)      197 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/EPICS_config_Win32.py
--rw-r--r--   0 noboru     (501) admin       (80)     1475 2022-02-15 05:43:19.000000 PythonCA-1.23.3.2/EPICS_config_common.py
--rw-r--r--   0 noboru     (501) admin       (80)     2075 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/EPICS_config_local_sample.py
--rw-r--r--   0 noboru     (501) admin       (80)     1725 2022-05-06 08:59:00.000000 PythonCA-1.23.3.2/MANIFEST
--rw-r--r--   0 noboru     (501) admin       (80)      851 2022-02-15 00:13:27.000000 PythonCA-1.23.3.2/MANIFEST.in
--rw-r--r--   0 noboru     (501) admin       (80)     1365 2022-05-24 06:54:44.000000 PythonCA-1.23.3.2/Makefile
--rw-r--r--   0 noboru     (501) admin       (80)       31 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/Numeric.py
--rw-r--r--   0 noboru     (501) admin       (80)     2665 2022-06-07 01:08:33.980294 PythonCA-1.23.3.2/PKG-INFO
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.505000 PythonCA-1.23.3.2/PythonCA.egg-info/
--rw-r--r--   0 noboru     (501) admin       (80)     2665 2022-06-07 01:08:32.000000 PythonCA-1.23.3.2/PythonCA.egg-info/PKG-INFO
--rw-r--r--   0 noboru     (501) admin       (80)     3756 2022-06-07 01:08:33.000000 PythonCA-1.23.3.2/PythonCA.egg-info/SOURCES.txt
--rw-r--r--   0 noboru     (501) admin       (80)        1 2022-06-07 01:08:32.000000 PythonCA-1.23.3.2/PythonCA.egg-info/dependency_links.txt
--rw-r--r--   0 noboru     (501) admin       (80)       76 2022-06-07 01:08:32.000000 PythonCA-1.23.3.2/PythonCA.egg-info/top_level.txt
--rw-r--r--   0 noboru     (501) admin       (80)      520 2009-03-03 07:31:51.000000 PythonCA-1.23.3.2/README
--rw-r--r--   0 noboru     (501) admin       (80)     2452 2022-06-07 00:49:24.000000 PythonCA-1.23.3.2/README.html
--rw-r--r--   0 noboru     (501) admin       (80)     2164 2022-06-07 00:49:24.000000 PythonCA-1.23.3.2/README.md
--rw-r--r--   0 noboru     (501) admin       (80)     2367 2020-11-19 13:23:49.000000 PythonCA-1.23.3.2/README.rst
--rw-r--r--   0 noboru     (501) admin       (80)    45625 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/_ca.c
--rw-r--r--   0 noboru     (501) admin       (80)    69008 2022-05-24 07:51:02.000000 PythonCA-1.23.3.2/_ca314.cpp
--rwxr-xr-x   0 noboru     (501) admin       (80)     1507 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/_ca_fnal.py
--rw-r--r--   0 noboru     (501) admin       (80)    18742 2022-05-06 08:44:55.000000 PythonCA-1.23.3.2/_ca_kek.py
--rwxr-xr-x   0 noboru     (501) admin       (80)    15544 2011-01-19 23:26:35.000000 PythonCA-1.23.3.2/_conv_helper.cpp
--rw-r--r--   0 noboru     (501) admin       (80)     1987 2022-05-06 08:44:55.000000 PythonCA-1.23.3.2/ca.py
--rw-r--r--   0 noboru     (501) admin       (80)    10293 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/caError.py
--rw-r--r--   0 noboru     (501) admin       (80)     3786 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/cadefs.py
--rw-r--r--   0 noboru     (501) admin       (80)     2115 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/caerr.py
--rw-r--r--   0 noboru     (501) admin       (80)    99543 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/caerr_wrap.c
--rw-r--r--   0 noboru     (501) admin       (80)     6883 2019-04-13 05:36:42.000000 PythonCA-1.23.3.2/calib.pxd
--rw-r--r--   0 noboru     (501) admin       (80)     1804 2019-12-12 06:33:34.000000 PythonCA-1.23.3.2/calib.pyx
--rw-r--r--   0 noboru     (501) admin       (80)   225604 2020-04-07 01:25:28.000000 PythonCA-1.23.3.2/calib3.cpp
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.505758 PythonCA-1.23.3.2/cas/
--rw-r--r--   0 noboru     (501) admin       (80)     3491 2019-11-20 07:24:43.000000 PythonCA-1.23.3.2/cas/caq.py
--rw-r--r--   0 noboru     (501) admin       (80)     7747 2019-11-20 08:52:22.000000 PythonCA-1.23.3.2/cas/cas.py
--rw-r--r--   0 noboru     (501) admin       (80)     8306 2019-11-20 07:59:12.000000 PythonCA-1.23.3.2/cas/xca.py
--rw-r--r--   0 noboru     (501) admin       (80)     2024 2019-04-13 05:37:07.000000 PythonCA-1.23.3.2/db_access.pxd
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.694407 PythonCA-1.23.3.2/dist/
--rw-r--r--   0 noboru     (501) admin       (80)     6148 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/.DS_Store
--rw-r--r--   0 noboru     (501) admin       (80)    41272 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.16.1.4.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    42645 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.16.1.5.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    39939 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.16.1.5beta.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    39961 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.16.1.5beta2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    41914 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.16.1.5beta3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    43228 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.1.beta1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    45765 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.1.beta2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    46759 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.1.beta3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    46928 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.1.rc1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    51422 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.1.rc3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    52826 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    53638 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.2.1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    52835 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    43236 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.20.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    56640 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.21.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    56649 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.21d2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    57831 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.21d3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    58690 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.22d.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    58460 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.22d1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    58708 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/PythonCA-1.22d2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    41277 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.16.1.4.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    42649 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.16.1.5.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    39948 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.16.1.5beta.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    39960 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.16.1.5beta2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    41914 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.16.1.5beta3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    43237 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.1.beta1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    45774 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.1.beta2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    46777 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.1.beta3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    46933 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.1.rc1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    51429 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.1.rc3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    52828 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    53648 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.2.1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    52836 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    43248 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.20.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    56641 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.21.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    56653 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.21d2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    57836 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.21d3.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    58978 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.22d.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    58465 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.22d1.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    58713 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/cas-1.22d2.tar.gz
--rw-r--r--   0 noboru     (501) admin       (80)    18360 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/dist/products.html
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.698237 PythonCA-1.23.3.2/doc/
--rwx------   0 noboru     (501) admin       (80)     2437 2019-04-13 03:15:58.000000 PythonCA-1.23.3.2/doc/InstallationMemo.html
--rw-r--r--   0 noboru     (501) admin       (80)     2044 2019-04-13 03:39:28.000000 PythonCA-1.23.3.2/doc/InstallationMemo.md
--rw-r--r--   0 noboru     (501) admin       (80)     2043 2019-04-13 03:15:56.000000 PythonCA-1.23.3.2/doc/InstallationMemo.rst
--rw-r--r--   0 noboru     (501) admin       (80)     1675 2019-04-13 03:09:37.000000 PythonCA-1.23.3.2/doc/InstallationMemo.rst~
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.699197 PythonCA-1.23.3.2/doc/sphinx/
--rw-r--r--   0 noboru     (501) admin       (80)      641 2022-05-24 06:02:40.000000 PythonCA-1.23.3.2/doc/sphinx/Makefile
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.382873 PythonCA-1.23.3.2/doc/sphinx/build/
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.701809 PythonCA-1.23.3.2/doc/sphinx/build/html/
--rw-r--r--   0 noboru     (501) admin       (80)     7682 2022-05-24 06:01:04.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/InstallationMemo.html
--rw-r--r--   0 noboru     (501) admin       (80)     4248 2022-05-24 08:35:39.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/ReleaseMemo-1.23.2.2.1.html
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.766618 PythonCA-1.23.3.2/doc/sphinx/build/html/_sources/
--rw-r--r--   0 noboru     (501) admin       (80)     2096 2022-05-24 05:56:33.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/_sources/InstallationMemo.rst.txt
--rw-r--r--   0 noboru     (501) admin       (80)     1160 2022-05-24 08:35:17.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/_sources/ReleaseMemo-1.23.2.2.1.rst.txt
--rw-r--r--   0 noboru     (501) admin       (80)      590 2022-05-24 09:13:03.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/_sources/index.rst.txt
--rw-r--r--   0 noboru     (501) admin       (80)     2363 2022-05-24 09:13:14.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/genindex.html
--rw-r--r--   0 noboru     (501) admin       (80)     4125 2022-05-24 09:13:14.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/index.html
--rw-r--r--   0 noboru     (501) admin       (80)     2706 2022-05-24 09:13:14.000000 PythonCA-1.23.3.2/doc/sphinx/build/html/search.html
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.767882 PythonCA-1.23.3.2/doc/sphinx/build/latex/
--rw-r--r--   0 noboru     (501) admin       (80)     1633 2022-05-24 09:13:10.000000 PythonCA-1.23.3.2/doc/sphinx/build/latex/Makefile
--rw-r--r--   0 noboru     (501) admin       (80)     7363 2022-05-24 09:13:10.000000 PythonCA-1.23.3.2/doc/sphinx/build/latex/PythonCAPythonmoduleforEPICSCAlibrary.tex
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.770437 PythonCA-1.23.3.2/doc/sphinx/source/
--rw-r--r--   0 noboru     (501) admin       (80)     2096 2022-05-24 05:56:33.000000 PythonCA-1.23.3.2/doc/sphinx/source/InstallationMemo.rst
--rw-r--r--   0 noboru     (501) admin       (80)       50 2022-05-24 06:01:00.000000 PythonCA-1.23.3.2/doc/sphinx/source/Makefile
--rw-r--r--   0 noboru     (501) admin       (80)     1160 2022-05-24 08:35:17.000000 PythonCA-1.23.3.2/doc/sphinx/source/ReleaseMemo-1.23.2.2.1.rst
--rw-r--r--   0 noboru     (501) admin       (80)     5993 2022-05-24 06:04:17.000000 PythonCA-1.23.3.2/doc/sphinx/source/conf.py
--rw-r--r--   0 noboru     (501) admin       (80)      590 2022-05-24 09:13:03.000000 PythonCA-1.23.3.2/doc/sphinx/source/index.rst
--rw-r--r--   0 noboru     (501) admin       (80)      444 2022-06-07 01:08:30.000000 PythonCA-1.23.3.2/epicsVersion.py
--rw-r--r--   0 noboru     (501) admin       (80)       97 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/foo.py
--rw-r--r--   0 noboru     (501) admin       (80)     6773 2007-03-27 15:11:00.000000 PythonCA-1.23.3.2/gen_caerrpy.c
--rw-r--r--   0 noboru     (501) admin       (80)      291 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/generate_caError.py
--rw-r--r--   0 noboru     (501) admin       (80)       24 2022-06-07 00:48:57.000000 PythonCA-1.23.3.2/hgstamp.py
--rw-r--r--   0 noboru     (501) admin       (80)     3567 2020-04-07 01:01:03.000000 PythonCA-1.23.3.2/makeEpicsVersion.py
--rw-r--r--   0 noboru     (501) admin       (80)      276 2019-04-17 09:51:39.000000 PythonCA-1.23.3.2/printfn.py
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.974933 PythonCA-1.23.3.2/sample/
--rw-r--r--   0 noboru     (501) admin       (80)     7971 2020-11-19 07:40:24.000000 PythonCA-1.23.3.2/sample/CaSimple.py
--rw-r--r--   0 noboru     (501) admin       (80)     4257 2020-11-19 07:03:01.000000 PythonCA-1.23.3.2/sample/CaSimple_usingQueue.py
--rw-r--r--   0 noboru     (501) admin       (80)     4655 2020-11-19 07:03:10.000000 PythonCA-1.23.3.2/sample/DummySimple.py
--rw-r--r--   0 noboru     (501) admin       (80)     4137 2020-11-19 07:03:27.000000 PythonCA-1.23.3.2/sample/QtSample1.py
--rw-r--r--   0 noboru     (501) admin       (80)      975 2020-11-19 07:03:38.000000 PythonCA-1.23.3.2/sample/SyncGroupSample.py
--rw-r--r--   0 noboru     (501) admin       (80)     1895 2020-11-19 07:03:46.000000 PythonCA-1.23.3.2/sample/TkMinimal.py
--rw-r--r--   0 noboru     (501) admin       (80)      146 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/sample/TkMinimal.tcl
--rw-r--r--   0 noboru     (501) admin       (80)     4000 2020-11-19 07:34:54.000000 PythonCA-1.23.3.2/sample/TkRandom.py
--rw-r--r--   0 noboru     (501) admin       (80)     3025 2020-11-19 07:04:16.000000 PythonCA-1.23.3.2/sample/TkRandom2.py
--rw-r--r--   0 noboru     (501) admin       (80)     3934 2020-11-19 07:04:29.000000 PythonCA-1.23.3.2/sample/TkSample1.1.py
--rw-r--r--   0 noboru     (501) admin       (80)     3892 2020-11-19 06:14:11.000000 PythonCA-1.23.3.2/sample/TkSample1.py
--rw-r--r--   0 noboru     (501) admin       (80)     3009 2020-11-19 07:04:40.000000 PythonCA-1.23.3.2/sample/TkSample2.py
--rw-r--r--   0 noboru     (501) admin       (80)     3452 2020-11-19 07:04:50.000000 PythonCA-1.23.3.2/sample/TkSample3.py
--rw-r--r--   0 noboru     (501) admin       (80)     2313 2020-11-19 07:04:59.000000 PythonCA-1.23.3.2/sample/TkSimple2.py
--rw-r--r--   0 noboru     (501) admin       (80)      302 2020-11-19 07:05:24.000000 PythonCA-1.23.3.2/sample/TkTest.py
--rw-r--r--   0 noboru     (501) admin       (80)     2088 2020-11-19 07:05:47.000000 PythonCA-1.23.3.2/sample/WxMinimal.py
--rw-r--r--   0 noboru     (501) admin       (80)     3922 2020-11-19 07:06:20.000000 PythonCA-1.23.3.2/sample/WxRandom.py
--rw-r--r--   0 noboru     (501) admin       (80)     4040 2020-11-19 07:06:35.000000 PythonCA-1.23.3.2/sample/WxSample1.py
--rw-r--r--   0 noboru     (501) admin       (80)     4956 2020-11-19 07:06:46.000000 PythonCA-1.23.3.2/sample/WxSample2.py
--rw-r--r--   0 noboru     (501) admin       (80)     3244 2020-11-19 07:06:55.000000 PythonCA-1.23.3.2/sample/WxSimple.py
--rw-r--r--   0 noboru     (501) admin       (80)     3429 2020-11-19 07:07:03.000000 PythonCA-1.23.3.2/sample/WxSimple2.py
--rw-r--r--   0 noboru     (501) admin       (80)        0 2007-05-03 13:51:37.000000 PythonCA-1.23.3.2/sample/__init__.py
--rw-r--r--   0 noboru     (501) admin       (80)     1278 2020-11-19 07:07:08.000000 PythonCA-1.23.3.2/sample/caAlarmSeverity.py
--rw-r--r--   0 noboru     (501) admin       (80)     1590 2020-11-19 07:07:19.000000 PythonCA-1.23.3.2/sample/caBadSample2.py
--rw-r--r--   0 noboru     (501) admin       (80)      812 2020-11-19 07:07:24.000000 PythonCA-1.23.3.2/sample/caBadSample3.py
--rw-r--r--   0 noboru     (501) admin       (80)     6427 2020-11-19 07:07:31.000000 PythonCA-1.23.3.2/sample/caBadSampleChannels.py
--rw-r--r--   0 noboru     (501) admin       (80)     2036 2020-11-19 07:07:42.000000 PythonCA-1.23.3.2/sample/caBadSampleThreadLock.py
--rw-r--r--   0 noboru     (501) admin       (80)     1021 2020-11-19 07:07:46.000000 PythonCA-1.23.3.2/sample/epicsQt.py
--rw-r--r--   0 noboru     (501) admin       (80)     3114 2020-11-19 07:27:15.000000 PythonCA-1.23.3.2/sample/ex_tk4.py
--rw-r--r--   0 noboru     (501) admin       (80)     3056 2020-11-19 07:08:32.000000 PythonCA-1.23.3.2/sample/ex_tk4n.py
--rw-r--r--   0 noboru     (501) admin       (80)      845 2020-11-19 07:08:38.000000 PythonCA-1.23.3.2/sample/ezca.py
--rw-r--r--   0 noboru     (501) admin       (80)     1323 2020-11-19 07:08:44.000000 PythonCA-1.23.3.2/sample/fakeca.py
--rw-r--r--   0 noboru     (501) admin       (80)     1023 2020-11-19 07:20:35.000000 PythonCA-1.23.3.2/sample/fd_reg_test.py
--rw-r--r--   0 noboru     (501) admin       (80)      865 2020-11-19 07:08:53.000000 PythonCA-1.23.3.2/sample/fd_register_example.py
--rw-r--r--   0 noboru     (501) admin       (80)      873 2020-11-18 13:49:18.000000 PythonCA-1.23.3.2/sample/simplecb.py
--rw-r--r--   0 noboru     (501) admin       (80)     1295 2020-11-18 13:48:03.000000 PythonCA-1.23.3.2/sample/simplecb2.py
--rw-r--r--   0 noboru     (501) admin       (80)     1352 2020-11-19 07:09:05.000000 PythonCA-1.23.3.2/sample/t5ca.py
--rw-r--r--   0 noboru     (501) admin       (80)     2565 2020-11-19 07:09:24.000000 PythonCA-1.23.3.2/sample/tamura.py
--rw-r--r--   0 noboru     (501) admin       (80)     2907 2020-11-19 07:09:46.000000 PythonCA-1.23.3.2/sample/tamura2.py
--rwxr-xr-x   0 noboru     (501) admin       (80)     4280 2020-11-19 07:09:59.000000 PythonCA-1.23.3.2/sample/thread_test.py
--rwxr-xr-x   0 noboru     (501) admin       (80)     3843 2020-11-19 07:10:14.000000 PythonCA-1.23.3.2/sample/thread_test2.py
--rw-r--r--   0 noboru     (501) admin       (80)     4009 2020-11-19 07:10:24.000000 PythonCA-1.23.3.2/sample/thread_test2C.py
--rw-r--r--   0 noboru     (501) admin       (80)     4445 2020-11-19 07:10:38.000000 PythonCA-1.23.3.2/sample/thread_test3.py
--rw-r--r--   0 noboru     (501) admin       (80)     4197 2020-11-19 07:11:14.000000 PythonCA-1.23.3.2/sample/thread_testC.py
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.975354 PythonCA-1.23.3.2/sample/wf_put_test/
--rw-r--r--   0 noboru     (501) admin       (80)     1030 2022-05-24 07:25:39.000000 PythonCA-1.23.3.2/sample/wf_put_test/wf_put_test.py
--rw-r--r--   0 noboru     (501) admin       (80)       68 2022-06-07 01:08:33.981070 PythonCA-1.23.3.2/setup.cfg
--rw-r--r--   0 noboru     (501) admin       (80)     9792 2022-06-07 01:08:20.000000 PythonCA-1.23.3.2/setup.py
-drwxr-xr-x   0 noboru     (501) admin       (80)        0 2022-06-07 01:08:33.979744 PythonCA-1.23.3.2/test/
--rwxr-xr-x   0 noboru     (501) admin       (80)      393 2020-12-16 06:32:10.000000 PythonCA-1.23.3.2/test/SoftEcas.command
--rw-r--r--   0 noboru     (501) admin       (80)     1675 2018-01-04 08:49:21.000000 PythonCA-1.23.3.2/test/WFmemleakCheck.py
--rwxr-xr-x   0 noboru     (501) admin       (80)     2001 2018-01-05 07:48:43.000000 PythonCA-1.23.3.2/test/excas.db
--rw-r--r--   0 noboru     (501) admin       (80)      588 2020-12-11 05:50:14.000000 PythonCA-1.23.3.2/test/excas.substitutions
--rwxrwxr--   0 noboru     (501) admin       (80)      864 2008-05-17 10:20:46.000000 PythonCA-1.23.3.2/test/excas2.db
--rwxrwxr--   0 noboru     (501) admin       (80)      493 2020-12-11 08:58:43.000000 PythonCA-1.23.3.2/test/excasw.db
--rw-r--r--   0 noboru     (501) admin       (80)      842 2009-02-16 15:06:43.000000 PythonCA-1.23.3.2/test/randomTest.py
--rwxr-xr-x   0 noboru     (501) admin       (80)      300 2020-12-28 04:11:17.000000 PythonCA-1.23.3.2/test/st.cmd
--rwxr-xr-x   0 noboru     (501) admin       (80)     1488 2020-12-28 04:03:09.000000 PythonCA-1.23.3.2/test/test.db
--rw-r--r--   0 noboru     (501) admin       (80)     1256 2020-12-10 21:00:25.000000 PythonCA-1.23.3.2/test/testPythonCA.py
--rw-r--r--   0 noboru     (501) admin       (80)      393 2007-09-23 11:25:04.000000 PythonCA-1.23.3.2/test/testTemplate.py
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.322818 PythonCA-1.23.3.7/
+-rw-r--r--   0 noboru     (501) admin       (80)    10244 2020-03-27 02:37:26.000000 PythonCA-1.23.3.7/.DS_Store
+-rw-r--r--   0 noboru     (501) admin       (80)      432 2023-07-08 22:56:28.000000 PythonCA-1.23.3.7/.hgignore
+-rw-r--r--   0 noboru     (501) admin       (80)      692 2022-06-07 00:48:05.000000 PythonCA-1.23.3.7/.hgtags
+-rwxr-xr-x   0 noboru     (501) admin       (80)    24225 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/CaChannel.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1120 2023-07-08 22:38:29.000000 PythonCA-1.23.3.7/EPICS_config_Darwin.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1133 2023-07-08 22:39:05.000000 PythonCA-1.23.3.7/EPICS_config_Darwin.pyc
+-rw-r--r--   0 noboru     (501) admin       (80)      364 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/EPICS_config_Linux.py
+-rw-r--r--   0 noboru     (501) admin       (80)      197 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/EPICS_config_Win32.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1475 2023-07-08 22:38:12.000000 PythonCA-1.23.3.7/EPICS_config_common.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2075 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/EPICS_config_local_sample.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1725 2022-05-06 08:59:00.000000 PythonCA-1.23.3.7/MANIFEST
+-rw-r--r--   0 noboru     (501) admin       (80)      862 2023-07-08 22:58:26.000000 PythonCA-1.23.3.7/MANIFEST.in
+-rw-r--r--   0 noboru     (501) admin       (80)     1532 2023-07-07 07:19:32.000000 PythonCA-1.23.3.7/Makefile
+-rw-r--r--   0 noboru     (501) admin       (80)       31 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/Numeric.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2666 2023-07-09 02:41:44.648810 PythonCA-1.23.3.7/PKG-INFO
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.323598 PythonCA-1.23.3.7/PythonCA.egg-info/
+-rw-r--r--   0 noboru     (501) admin       (80)     2666 2023-07-09 02:41:43.000000 PythonCA-1.23.3.7/PythonCA.egg-info/PKG-INFO
+-rw-r--r--   0 noboru     (501) admin       (80)     2624 2023-07-09 02:41:44.000000 PythonCA-1.23.3.7/PythonCA.egg-info/SOURCES.txt
+-rw-r--r--   0 noboru     (501) admin       (80)        1 2023-07-09 02:41:43.000000 PythonCA-1.23.3.7/PythonCA.egg-info/dependency_links.txt
+-rw-r--r--   0 noboru     (501) admin       (80)       80 2023-07-09 02:41:43.000000 PythonCA-1.23.3.7/PythonCA.egg-info/top_level.txt
+-rw-r--r--   0 noboru     (501) admin       (80)      520 2009-03-03 07:31:51.000000 PythonCA-1.23.3.7/README
+-rw-r--r--   0 noboru     (501) admin       (80)     2452 2023-07-09 02:41:41.000000 PythonCA-1.23.3.7/README.html
+-rw-r--r--   0 noboru     (501) admin       (80)     2165 2023-07-09 02:41:42.000000 PythonCA-1.23.3.7/README.md
+-rw-r--r--   0 noboru     (501) admin       (80)     2367 2020-11-19 13:23:49.000000 PythonCA-1.23.3.7/README.rst
+-rw-r--r--   0 noboru     (501) admin       (80)    45625 2018-01-05 07:48:43.000000 PythonCA-1.23.3.7/_ca.c
+-rw-r--r--   0 noboru     (501) admin       (80)    69083 2023-07-08 22:55:33.000000 PythonCA-1.23.3.7/_ca314.cpp
+-rwxr-xr-x   0 noboru     (501) admin       (80)     1507 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/_ca_fnal.py
+-rw-r--r--   0 noboru     (501) admin       (80)    18794 2023-07-07 23:47:59.000000 PythonCA-1.23.3.7/_ca_kek.py
+-rwxr-xr-x   0 noboru     (501) admin       (80)    15544 2011-01-19 23:26:35.000000 PythonCA-1.23.3.7/_conv_helper.cpp
+-rw-r--r--   0 noboru     (501) admin       (80)     1987 2023-07-07 23:47:59.000000 PythonCA-1.23.3.7/ca.py
+-rw-r--r--   0 noboru     (501) admin       (80)    10293 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/caError.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3786 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/cadefs.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2115 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/caerr.py
+-rw-r--r--   0 noboru     (501) admin       (80)    99543 2018-01-05 07:48:43.000000 PythonCA-1.23.3.7/caerr_wrap.c
+-rw-r--r--   0 noboru     (501) admin       (80)     6883 2019-04-13 05:36:42.000000 PythonCA-1.23.3.7/calib.pxd
+-rw-r--r--   0 noboru     (501) admin       (80)     1819 2023-07-09 02:39:59.000000 PythonCA-1.23.3.7/calib.pyx
+-rw-r--r--   0 noboru     (501) admin       (80)   237698 2023-07-09 02:40:11.000000 PythonCA-1.23.3.7/calib3.cpp
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.324741 PythonCA-1.23.3.7/cas/
+-rw-r--r--   0 noboru     (501) admin       (80)       30 2023-07-09 02:00:11.000000 PythonCA-1.23.3.7/cas/__init__.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3491 2019-11-20 07:24:43.000000 PythonCA-1.23.3.7/cas/caq.py
+-rw-r--r--   0 noboru     (501) admin       (80)     7778 2023-07-09 01:59:47.000000 PythonCA-1.23.3.7/cas/cas.py
+-rw-r--r--   0 noboru     (501) admin       (80)     8313 2023-07-09 02:00:38.000000 PythonCA-1.23.3.7/cas/xca.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2024 2019-04-13 05:37:07.000000 PythonCA-1.23.3.7/db_access.pxd
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.387899 PythonCA-1.23.3.7/doc/
+-rwx------   0 noboru     (501) admin       (80)     2437 2019-04-13 03:15:58.000000 PythonCA-1.23.3.7/doc/InstallationMemo.html
+-rw-r--r--   0 noboru     (501) admin       (80)     2044 2019-04-13 03:39:28.000000 PythonCA-1.23.3.7/doc/InstallationMemo.md
+-rw-r--r--   0 noboru     (501) admin       (80)     2043 2019-04-13 03:15:56.000000 PythonCA-1.23.3.7/doc/InstallationMemo.rst
+-rw-r--r--   0 noboru     (501) admin       (80)     1675 2019-04-13 03:09:37.000000 PythonCA-1.23.3.7/doc/InstallationMemo.rst~
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.388378 PythonCA-1.23.3.7/doc/sphinx/
+-rw-r--r--   0 noboru     (501) admin       (80)      641 2022-05-24 06:02:40.000000 PythonCA-1.23.3.7/doc/sphinx/Makefile
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.205544 PythonCA-1.23.3.7/doc/sphinx/build/
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.390497 PythonCA-1.23.3.7/doc/sphinx/build/html/
+-rw-r--r--   0 noboru     (501) admin       (80)     7682 2022-05-24 06:01:04.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/InstallationMemo.html
+-rw-r--r--   0 noboru     (501) admin       (80)     4248 2022-05-24 08:35:39.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/ReleaseMemo-1.23.2.2.1.html
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.391683 PythonCA-1.23.3.7/doc/sphinx/build/html/_sources/
+-rw-r--r--   0 noboru     (501) admin       (80)     2096 2022-05-24 05:56:33.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/_sources/InstallationMemo.rst.txt
+-rw-r--r--   0 noboru     (501) admin       (80)     1160 2022-05-24 08:35:17.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/_sources/ReleaseMemo-1.23.2.2.1.rst.txt
+-rw-r--r--   0 noboru     (501) admin       (80)      590 2022-05-24 09:13:03.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/_sources/index.rst.txt
+-rw-r--r--   0 noboru     (501) admin       (80)     2363 2022-05-24 09:13:14.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/genindex.html
+-rw-r--r--   0 noboru     (501) admin       (80)     4125 2022-05-24 09:13:14.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/index.html
+-rw-r--r--   0 noboru     (501) admin       (80)     2706 2022-05-24 09:13:14.000000 PythonCA-1.23.3.7/doc/sphinx/build/html/search.html
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.457086 PythonCA-1.23.3.7/doc/sphinx/build/latex/
+-rw-r--r--   0 noboru     (501) admin       (80)     1633 2022-05-24 09:13:10.000000 PythonCA-1.23.3.7/doc/sphinx/build/latex/Makefile
+-rw-r--r--   0 noboru     (501) admin       (80)     7363 2022-05-24 09:13:10.000000 PythonCA-1.23.3.7/doc/sphinx/build/latex/PythonCAPythonmoduleforEPICSCAlibrary.tex
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.459679 PythonCA-1.23.3.7/doc/sphinx/source/
+-rw-r--r--   0 noboru     (501) admin       (80)     2096 2022-05-24 05:56:33.000000 PythonCA-1.23.3.7/doc/sphinx/source/InstallationMemo.rst
+-rw-r--r--   0 noboru     (501) admin       (80)       50 2022-05-24 06:01:00.000000 PythonCA-1.23.3.7/doc/sphinx/source/Makefile
+-rw-r--r--   0 noboru     (501) admin       (80)     1160 2022-05-24 08:35:17.000000 PythonCA-1.23.3.7/doc/sphinx/source/ReleaseMemo-1.23.2.2.1.rst
+-rw-r--r--   0 noboru     (501) admin       (80)     5993 2022-05-24 06:04:17.000000 PythonCA-1.23.3.7/doc/sphinx/source/conf.py
+-rw-r--r--   0 noboru     (501) admin       (80)      590 2022-05-24 09:13:03.000000 PythonCA-1.23.3.7/doc/sphinx/source/index.rst
+-rw-r--r--   0 noboru     (501) admin       (80)      436 2023-07-09 02:41:42.000000 PythonCA-1.23.3.7/epicsVersion.py
+-rw-r--r--   0 noboru     (501) admin       (80)       97 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/foo.py
+-rw-r--r--   0 noboru     (501) admin       (80)     6773 2007-03-27 15:11:00.000000 PythonCA-1.23.3.7/gen_caerrpy.c
+-rw-r--r--   0 noboru     (501) admin       (80)      291 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/generate_caError.py
+-rw-r--r--   0 noboru     (501) admin       (80)       24 2023-07-07 23:48:00.000000 PythonCA-1.23.3.7/hgstamp.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3567 2020-04-07 01:01:03.000000 PythonCA-1.23.3.7/makeEpicsVersion.py
+-rw-r--r--   0 noboru     (501) admin       (80)      276 2019-04-17 09:51:39.000000 PythonCA-1.23.3.7/printfn.py
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.575627 PythonCA-1.23.3.7/sample/
+-rw-r--r--   0 noboru     (501) admin       (80)     7971 2020-11-19 07:40:24.000000 PythonCA-1.23.3.7/sample/CaSimple.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4257 2020-11-19 07:03:01.000000 PythonCA-1.23.3.7/sample/CaSimple_usingQueue.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4655 2020-11-19 07:03:10.000000 PythonCA-1.23.3.7/sample/DummySimple.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4137 2020-11-19 07:03:27.000000 PythonCA-1.23.3.7/sample/QtSample1.py
+-rw-r--r--   0 noboru     (501) admin       (80)      975 2020-11-19 07:03:38.000000 PythonCA-1.23.3.7/sample/SyncGroupSample.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1895 2020-11-19 07:03:46.000000 PythonCA-1.23.3.7/sample/TkMinimal.py
+-rw-r--r--   0 noboru     (501) admin       (80)      146 2018-01-05 07:48:43.000000 PythonCA-1.23.3.7/sample/TkMinimal.tcl
+-rw-r--r--   0 noboru     (501) admin       (80)     4000 2020-11-19 07:34:54.000000 PythonCA-1.23.3.7/sample/TkRandom.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3025 2020-11-19 07:04:16.000000 PythonCA-1.23.3.7/sample/TkRandom2.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3934 2020-11-19 07:04:29.000000 PythonCA-1.23.3.7/sample/TkSample1.1.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3892 2020-11-19 06:14:11.000000 PythonCA-1.23.3.7/sample/TkSample1.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3009 2020-11-19 07:04:40.000000 PythonCA-1.23.3.7/sample/TkSample2.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3452 2020-11-19 07:04:50.000000 PythonCA-1.23.3.7/sample/TkSample3.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2313 2020-11-19 07:04:59.000000 PythonCA-1.23.3.7/sample/TkSimple2.py
+-rw-r--r--   0 noboru     (501) admin       (80)      302 2020-11-19 07:05:24.000000 PythonCA-1.23.3.7/sample/TkTest.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2088 2020-11-19 07:05:47.000000 PythonCA-1.23.3.7/sample/WxMinimal.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3922 2020-11-19 07:06:20.000000 PythonCA-1.23.3.7/sample/WxRandom.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4040 2020-11-19 07:06:35.000000 PythonCA-1.23.3.7/sample/WxSample1.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4956 2020-11-19 07:06:46.000000 PythonCA-1.23.3.7/sample/WxSample2.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3244 2020-11-19 07:06:55.000000 PythonCA-1.23.3.7/sample/WxSimple.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3429 2020-11-19 07:07:03.000000 PythonCA-1.23.3.7/sample/WxSimple2.py
+-rw-r--r--   0 noboru     (501) admin       (80)        0 2007-05-03 13:51:37.000000 PythonCA-1.23.3.7/sample/__init__.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1278 2020-11-19 07:07:08.000000 PythonCA-1.23.3.7/sample/caAlarmSeverity.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1590 2020-11-19 07:07:19.000000 PythonCA-1.23.3.7/sample/caBadSample2.py
+-rw-r--r--   0 noboru     (501) admin       (80)      812 2020-11-19 07:07:24.000000 PythonCA-1.23.3.7/sample/caBadSample3.py
+-rw-r--r--   0 noboru     (501) admin       (80)     6427 2020-11-19 07:07:31.000000 PythonCA-1.23.3.7/sample/caBadSampleChannels.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2036 2020-11-19 07:07:42.000000 PythonCA-1.23.3.7/sample/caBadSampleThreadLock.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1021 2020-11-19 07:07:46.000000 PythonCA-1.23.3.7/sample/epicsQt.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3114 2020-11-19 07:27:15.000000 PythonCA-1.23.3.7/sample/ex_tk4.py
+-rw-r--r--   0 noboru     (501) admin       (80)     3056 2020-11-19 07:08:32.000000 PythonCA-1.23.3.7/sample/ex_tk4n.py
+-rw-r--r--   0 noboru     (501) admin       (80)      845 2020-11-19 07:08:38.000000 PythonCA-1.23.3.7/sample/ezca.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1323 2020-11-19 07:08:44.000000 PythonCA-1.23.3.7/sample/fakeca.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1023 2020-11-19 07:20:35.000000 PythonCA-1.23.3.7/sample/fd_reg_test.py
+-rw-r--r--   0 noboru     (501) admin       (80)      865 2020-11-19 07:08:53.000000 PythonCA-1.23.3.7/sample/fd_register_example.py
+-rw-r--r--   0 noboru     (501) admin       (80)      873 2020-11-18 13:49:18.000000 PythonCA-1.23.3.7/sample/simplecb.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1295 2020-11-18 13:48:03.000000 PythonCA-1.23.3.7/sample/simplecb2.py
+-rw-r--r--   0 noboru     (501) admin       (80)     1352 2020-11-19 07:09:05.000000 PythonCA-1.23.3.7/sample/t5ca.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2565 2020-11-19 07:09:24.000000 PythonCA-1.23.3.7/sample/tamura.py
+-rw-r--r--   0 noboru     (501) admin       (80)     2907 2020-11-19 07:09:46.000000 PythonCA-1.23.3.7/sample/tamura2.py
+-rwxr-xr-x   0 noboru     (501) admin       (80)     4280 2020-11-19 07:09:59.000000 PythonCA-1.23.3.7/sample/thread_test.py
+-rwxr-xr-x   0 noboru     (501) admin       (80)     3843 2020-11-19 07:10:14.000000 PythonCA-1.23.3.7/sample/thread_test2.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4009 2020-11-19 07:10:24.000000 PythonCA-1.23.3.7/sample/thread_test2C.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4445 2020-11-19 07:10:38.000000 PythonCA-1.23.3.7/sample/thread_test3.py
+-rw-r--r--   0 noboru     (501) admin       (80)     4197 2020-11-19 07:11:14.000000 PythonCA-1.23.3.7/sample/thread_testC.py
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.643469 PythonCA-1.23.3.7/sample/wf_put_test/
+-rw-r--r--   0 noboru     (501) admin       (80)     1030 2022-05-24 07:25:39.000000 PythonCA-1.23.3.7/sample/wf_put_test/wf_put_test.py
+-rw-r--r--   0 noboru     (501) admin       (80)       68 2023-07-09 02:41:44.649415 PythonCA-1.23.3.7/setup.cfg
+-rw-r--r--   0 noboru     (501) admin       (80)    10024 2023-07-09 01:43:50.000000 PythonCA-1.23.3.7/setup.py
+drwxr-xr-x   0 noboru     (501) admin       (80)        0 2023-07-09 02:41:44.648293 PythonCA-1.23.3.7/test/
+-rwxr-xr-x   0 noboru     (501) admin       (80)      393 2020-12-16 06:32:10.000000 PythonCA-1.23.3.7/test/SoftEcas.command
+-rw-r--r--   0 noboru     (501) admin       (80)     1675 2018-01-04 08:49:21.000000 PythonCA-1.23.3.7/test/WFmemleakCheck.py
+-rwxr-xr-x   0 noboru     (501) admin       (80)     2001 2018-01-05 07:48:43.000000 PythonCA-1.23.3.7/test/excas.db
+-rw-r--r--   0 noboru     (501) admin       (80)      588 2020-12-11 05:50:14.000000 PythonCA-1.23.3.7/test/excas.substitutions
+-rwxrwxr--   0 noboru     (501) admin       (80)      864 2008-05-17 10:20:46.000000 PythonCA-1.23.3.7/test/excas2.db
+-rwxrwxr--   0 noboru     (501) admin       (80)      493 2020-12-11 08:58:43.000000 PythonCA-1.23.3.7/test/excasw.db
+-rw-r--r--   0 noboru     (501) admin       (80)      842 2009-02-16 15:06:43.000000 PythonCA-1.23.3.7/test/randomTest.py
+-rwxr-xr-x   0 noboru     (501) admin       (80)      300 2020-12-28 04:11:17.000000 PythonCA-1.23.3.7/test/st.cmd
+-rwxr-xr-x   0 noboru     (501) admin       (80)     1488 2020-12-28 04:03:09.000000 PythonCA-1.23.3.7/test/test.db
+-rw-r--r--   0 noboru     (501) admin       (80)     1256 2020-12-10 21:00:25.000000 PythonCA-1.23.3.7/test/testPythonCA.py
+-rw-r--r--   0 noboru     (501) admin       (80)      393 2007-09-23 11:25:04.000000 PythonCA-1.23.3.7/test/testTemplate.py
```

### Comparing `PythonCA-1.23.3.2/.DS_Store` & `PythonCA-1.23.3.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/.hgtags` & `PythonCA-1.23.3.7/.hgtags`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/CaChannel.py` & `PythonCA-1.23.3.7/CaChannel.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/EPICS_config_Darwin.py` & `PythonCA-1.23.3.7/EPICS_config_Darwin.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/EPICS_config_Darwin.pyc` & `PythonCA-1.23.3.7/EPICS_config_Darwin.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a fe75 7862 6300 0000 0000 0000  .....uxbc.......
+00000000: 03f3 0d0a 65e5 a964 6300 0000 0000 0000  ....e..dc.......
 00000010: 0004 0000 0040 0000 0073 0b01 0000 6400  .....@...s....d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0100  .d..l..Z..d..d..
 00000030: 6c01 005a 0100 6400 0064 0100 6c02 005a  l..Z..d..d..l..Z
 00000040: 0200 6400 0064 0200 6c03 0054 6504 0064  ..d..d..l..Te..d
 00000050: 0300 6b02 0072 4300 6404 005a 0400 6e15  ..k..rC.d..Z..n.
 00000060: 0065 0400 6405 006b 0200 7258 0064 0600  .e..d..k..rX.d..
 00000070: 5a04 006e 0000 6505 005a 0600 6506 0072  Z..n..e..Z..e..r
```

### Comparing `PythonCA-1.23.3.2/EPICS_config_common.py` & `PythonCA-1.23.3.7/EPICS_config_common.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/EPICS_config_local_sample.py` & `PythonCA-1.23.3.7/EPICS_config_local_sample.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/MANIFEST` & `PythonCA-1.23.3.7/MANIFEST`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/MANIFEST.in` & `PythonCA-1.23.3.7/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 prune RCS/*
 prune */build
+prune dist/
+prune dist/*
 prune ._*
 prune sample/._*
 prune test/._*
 prune doc/._*
 prune doc/sphinx/build/*
 prune cas/._*
-prune */build
 prune ._*
 prune \#*
 prune *~
 prune .#*
 prune *.pyc
 prune sample/._*
 prune test/._*
```

### Comparing `PythonCA-1.23.3.2/Makefile` & `PythonCA-1.23.3.7/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -2,60 +2,72 @@
 # -*- coding:utf-8 -*-
 #
 .PHONY: update_hgstamp
 .phony:distclean checkin release build  all clean readme install
 
 all:build install
 
-CC=/usr/bin/clang
-CXX=/usr/bin/clang++
+CC  ?=/usr/bin/clang
+CXX ?=/usr/bin/clang++
+PYTHON3 ?=$(shell which python3)
+PYTHON2 ?=$(shell which python2)
 
 # from https://www.mercurial-scm.org/wiki/VersioningWithMake
 #HGVERSION:= $(shell hg parents --template 'hgid: {node|short}')
 HGVERSION:= $(shell hg parents --template 'HGTagShort = \\\"{latesttag}.{latesttagdistance}\\\"')
 VERSION:= $(shell hg parents --template '{latesttag}.{latesttagdistance}')
 
 hgstamp.py: update_hgstamp
 	[ -f $@ ] || touch $@
 	echo $(HGVERSION) | cmp -s $@ - || echo $(HGVERSION) > $@
 #
 
+
 distclean:
 	-rm ./build/bdist.*
 
+
 checkin :
 	-hg ci -m "before release $(VERSION)"
 	-hg kwexpand
 	make hgstamp.py
 
+
 release: distclean
 	make readme
 	make hgstamp.py
 	-hg bookmark -i "release $(VERSION)"
-	python3 setup.py sdist
+	$(PYTHON3) setup.py sdist
+
 
 upload:
-	python3 -m twine upload  dist/PythonCA-$(VERSION).tar.gz
+	$(PYTHON3) -m twine upload  dist/PythonCA-$(VERSION).tar.gz
 
 
 pythonca: setup.py hgstamp.py
-	python setup.py clean
-	-python3 setup.py clean
-	python setup.py build
-	-python3 setup.py build
+	$(PYTHON3) setup.py clean
+	$(PYTHON3) setup.py build
+	-$(PYTHON2) setup.py clean
+	-$(PYTHON2) setup.py build
+
 
 install:
 	-rm -r ./build/bdist.*
-	python3 setup.py install
+	#$(PYTHON3) setup.py install
+	$(PYTHON3) -m pip install ./
 	-rm -r ./build/bdist.*
-	python2 setup.py install
+	#python2 setup.py install
+	$(PYTHON2) -m pip install ./
+
 
 build: pythonca
 
+
 readme: README.rst
 	/usr/local/bin/pandoc -t plain -o README.txt README.rst
 	/usr/local/bin/pandoc -t html -o README.html README.rst
 	/usr/local/bin/pandoc -t markdown -o README.md README.rst
 
+
 sdist:
-	python3 setup.py sdist
+	$(PYTHON3) setup.py sdist
```

### Comparing `PythonCA-1.23.3.2/PKG-INFO` & `PythonCA-1.23.3.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonCA
-Version: 1.23.3.2
+Version: 1.23.3.7
 Summary: EPICS CA library interface module
 Home-page: http://www-acc.kek.jp/EPICS_Gr/products.html
 Download-URL: https://pypi.org/project/PythonCA/
 Author: Noboru Yamamoto, KEK, JAPAN
 Author-email: Noboru.YAMAMOTO@kek.jp
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 2.7
@@ -46,15 +46,15 @@
 3.  goto this directory and run
 
     env EPICS_ROOT=/your/epics/root python3 setup.py build clean install
 
 ### memo:2019.4.19
 
 This module is updated so that it is now compatible with both Python2.x
-(x>6) and Python3.y. (I just tested with Python2.7 and Python3.7).
+(x\>6) and Python3.y. (I just tested with Python2.7 and Python3.7).
 
 This module also include calib module which is developed with Cython. It
 is still under development. Once this module is completed, ca314.cpp
 will be obsoleted and will be replaced by python module based on calib.
 
 ### memo:2020.11.17
```

### Comparing `PythonCA-1.23.3.2/PythonCA.egg-info/PKG-INFO` & `PythonCA-1.23.3.7/PythonCA.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonCA
-Version: 1.23.3.2
+Version: 1.23.3.7
 Summary: EPICS CA library interface module
 Home-page: http://www-acc.kek.jp/EPICS_Gr/products.html
 Download-URL: https://pypi.org/project/PythonCA/
 Author: Noboru Yamamoto, KEK, JAPAN
 Author-email: Noboru.YAMAMOTO@kek.jp
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 2.7
@@ -46,15 +46,15 @@
 3.  goto this directory and run
 
     env EPICS_ROOT=/your/epics/root python3 setup.py build clean install
 
 ### memo:2019.4.19
 
 This module is updated so that it is now compatible with both Python2.x
-(x>6) and Python3.y. (I just tested with Python2.7 and Python3.7).
+(x\>6) and Python3.y. (I just tested with Python2.7 and Python3.7).
 
 This module also include calib module which is developed with Cython. It
 is still under development. Once this module is completed, ca314.cpp
 will be obsoleted and will be replaced by python module based on calib.
 
 ### memo:2020.11.17
```

### Comparing `PythonCA-1.23.3.2/README` & `PythonCA-1.23.3.7/README`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/README.html` & `PythonCA-1.23.3.7/README.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,49 @@
-<h1 id="epics-ca-library-interface-module-kek-japan">EPICS CA library interface module (KEK, Japan)</h1>
+<h1 id="epics-ca-library-interface-module-kek-japan">EPICS CA library
+interface module (KEK, Japan)</h1>
 <h2 id="overview">Overview</h2>
-<p>This is a distribution of Python extension module for EPICS/CA libarary. It allow you to access EPICS runtime database or CA server through CA library. Now it support multi-threaded EPICS CA library in Release 3.14 or later of EPICS.</p>
+<p>This is a distribution of Python extension module for EPICS/CA
+libarary. It allow you to access EPICS runtime database or CA server
+through CA library. Now it support multi-threaded EPICS CA library in
+Release 3.14 or later of EPICS.</p>
 <p>Please read doc/InstallationMemo.html for installation proceduce.</p>
 <p>Thank you,</p>
 <p>2007/5/7</p>
 <p>Noboru Yamamoto EPICS group, Accelerator Lab. KEK, JAPAN</p>
-<p>* contributors: Takashi Obina PF-AR/KEK Tatsuro Nakamura KEKB/KEK Wang Xiaoqiang PSI</p>
+<p>* contributors: Takashi Obina PF-AR/KEK Tatsuro Nakamura KEKB/KEK
+Wang Xiaoqiang PSI</p>
 <p>* Special Thanks: to All users who gave us comments.</p>
 <h3 id="installation">installation</h3>
-<p>A setup script of this module need to know the location of your EPICS installation. Please EPICSROOT environment variable as the path where your EPICS base is.</p>
+<p>A setup script of this module need to know the location of your EPICS
+installation. Please EPICSROOT environment variable as the path where
+your EPICS base is.</p>
 <ol>
 <li><p>download source package from PyPI site.</p></li>
 <li><p>exapnd the file at appropriate directory</p></li>
 <li><p>goto this directory and run</p>
-<p>env EPICS_ROOT=/your/epics/root python3 setup.py build clean install</p></li>
+<p>env EPICS_ROOT=/your/epics/root python3 setup.py build clean
+install</p></li>
 </ol>
 <h3 id="memo2019.4.19">memo:2019.4.19</h3>
-<p>This module is updated so that it is now compatible with both Python2.x (x&gt;6) and Python3.y. (I just tested with Python2.7 and Python3.7).</p>
-<p>This module also include calib module which is developed with Cython. It is still under development. Once this module is completed, ca314.cpp will be obsoleted and will be replaced by python module based on calib.</p>
+<p>This module is updated so that it is now compatible with both
+Python2.x (x&gt;6) and Python3.y. (I just tested with Python2.7 and
+Python3.7).</p>
+<p>This module also include calib module which is developed with Cython.
+It is still under development. Once this module is completed, ca314.cpp
+will be obsoleted and will be replaced by python module based on
+calib.</p>
 <h3 id="memo2020.11.17">memo:2020.11.17</h3>
-<p>_ca_kek.py and _ca314.cpp are tweaked to support "SyncGroup" function.</p>
+<p>_ca_kek.py and _ca314.cpp are tweaked to support "SyncGroup"
+function.</p>
 <p>_ca_kek.py is also clean-upped with 2to3 and pylint.</p>
 <h3 id="memo2020.11.19">memo:2020.11.19</h3>
-<p>A crash on centOS was caused by incorrect data conversion format in PyArg_ParseTuple in _ca314.cpp. A size of data specified by the fromat should be matched with the size of the correspondig argument. Functions, sg_test/sg_reset/sg_state, were affected by this incorrect format characters.</p>
-<p>Most of python scripts in sample/ directory now works on both python2 and python3. I don't have PyQt, wxPython in the current test platform, so scripts using PyQt or wxPython are not tested( but converted with 2to3 anyway). You may need to install future module (not __future__ module) into your python2 enviroment, to test sicripts using tkinter module.</p>
+<p>A crash on centOS was caused by incorrect data conversion format in
+PyArg_ParseTuple in _ca314.cpp. A size of data specified by the fromat
+should be matched with the size of the correspondig argument. Functions,
+sg_test/sg_reset/sg_state, were affected by this incorrect format
+characters.</p>
+<p>Most of python scripts in sample/ directory now works on both python2
+and python3. I don't have PyQt, wxPython in the current test platform,
+so scripts using PyQt or wxPython are not tested( but converted with
+2to3 anyway). You may need to install future module (not __future__
+module) into your python2 enviroment, to test sicripts using tkinter
+module.</p>
```

### Comparing `PythonCA-1.23.3.2/README.md` & `PythonCA-1.23.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 3.  goto this directory and run
 
     env EPICS_ROOT=/your/epics/root python3 setup.py build clean install
 
 ### memo:2019.4.19
 
 This module is updated so that it is now compatible with both Python2.x
-(x>6) and Python3.y. (I just tested with Python2.7 and Python3.7).
+(x\>6) and Python3.y. (I just tested with Python2.7 and Python3.7).
 
 This module also include calib module which is developed with Cython. It
 is still under development. Once this module is completed, ca314.cpp
 will be obsoleted and will be replaced by python module based on calib.
 
 ### memo:2020.11.17
```

### Comparing `PythonCA-1.23.3.2/README.rst` & `PythonCA-1.23.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/_ca.c` & `PythonCA-1.23.3.7/_ca.c`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/_ca314.cpp` & `PythonCA-1.23.3.7/_ca314.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 #endif
 
 #if PY_VERSION_HEX > 0x03000000
 #define PyString_FromString(str) PyUnicode_FromString(str)
 #endif
 
 #if PY_VERSION_HEX > 0x030A0000
-#define PyEval_ThreadsInitialized() {True;}
+#define PyEval_ThreadsInitialized() (True)
 #endif
 
 #define False 0
 #define True 1
 
 #define DEBUG False
 
@@ -530,18 +530,20 @@
   chid ch_id;
   int status=-1;
   _ca_frame *pframe=NULL;
   
   unsigned long nc;
   PyObject *pcallback;
   
-  if(!PyArg_ParseTuple(args, "z#O", &name, &nc, &pcallback))
+  // if(!PyArg_ParseTuple(args, "z#O", &name, &nc, &pcallback))
+  if(!PyArg_ParseTuple(args, "zO", &name, &pcallback))
     return NULL;
   
-  if (!name || !nc ) {
+  //if (!name || !nc ) {
+  if (!name ) {
     PyErr_SetString(CaError, "Empty channel Name");
     return NULL; /* NULL triggers Exception */
   }
 
   Py_XINCREF(pcallback);
   {
     if (! PyCallable_Check(pcallback) ){
```

### Comparing `PythonCA-1.23.3.2/_ca_fnal.py` & `PythonCA-1.23.3.7/_ca_fnal.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/_ca_kek.py` & `PythonCA-1.23.3.7/_ca_kek.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 ## @package ca: EPICS-CA interface module for Python.
 """
 CA modlue : EPICS-CA interface module for Python.
 This module provide a  version of EPICS-CA and Python interface.
 It users C module _ca. _ca module basically maps C-API in EPICS ca library into python. Interface between ca.py and _ca module is  subject for change. You should not depend on it. API in ca.py will be preserved in future releases as much as possible.
 Author: Noboru Yamamoto, KEK, JAPAN. -2007.
-$Revision: b4d07ff54edb $
+$Revision: 9c57b570a211 $
 """
-__version__ = "$Revision: b4d07ff54edb $"
+__version__ = "$Revision: 9c57b570a211 $"
 # $Source: /opt/epics/R314/modules/soft/kekb/python/PythonCA-dev/_ca_kek.py $
 #
 try:
     import signal
 except:
     print ("signal module is not avaialble")
 
@@ -87,15 +87,15 @@
         DBR_CTRL_CHAR, DBR_CTRL_LONG,
         DBR_CTRL_ENUM, DBR_CTRL_DOUBLE
         )
 
     def __init__(self, name, cb=None,noflush=False):
         if not cb : cb=self.update_info
         if name == "":
-            raise ValueError( name)
+            raise ValueError(name)
         self.name=name
         self.field_type = None
         self.element_count = None
         self.puser = None
         self.conn_state = -1
         self.hostname = None
         self.raccess = None
@@ -394,14 +394,16 @@
     if isinstance(name,(bytes,str)):
         if ((name in __ca_dict)):
             ch=__ca_dict[name]
         else:
             try:
                 ch=channel(name)
                 ch.wait_conn()
+            except ValueError:
+                raise
             except:
                 raise ECA_BADCHID(name)
             tmo=20*tmo
             __ca_dict_lock.acquire()
             try:
                 __ca_dict[name]=ch
             finally:
```

### Comparing `PythonCA-1.23.3.2/_conv_helper.cpp` & `PythonCA-1.23.3.7/_conv_helper.cpp`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/ca.py` & `PythonCA-1.23.3.7/ca.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/caError.py` & `PythonCA-1.23.3.7/caError.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/cadefs.py` & `PythonCA-1.23.3.7/cadefs.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/caerr.py` & `PythonCA-1.23.3.7/caerr.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/caerr_wrap.c` & `PythonCA-1.23.3.7/caerr_wrap.c`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/calib.pxd` & `PythonCA-1.23.3.7/calib.pxd`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/calib.pyx` & `PythonCA-1.23.3.7/calib.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     else:
         return -1
 
 # cdef search_and_connect(    char *pChanName,    chid *pChanID    ):
 #     pchid=calib.ca_search_and_connect(name, pChanID, NULL, NULL)
 #     return pchid
 
-def search(name, nc, pcallback, args):
+def search(name:str, nc=None, pcallback=None, *args):
     # cdef chid *pchid=NULL;
     # pchid=calib.ca_search_and_connect(name, pchid, None,None)
     # return chid
     raise RuntimeError("not implemeted yet")
 
 def clear(ch_id):
      calib.ca_clear_channel(<calib.chid> ch_id)
```

### Comparing `PythonCA-1.23.3.2/calib3.cpp` & `PythonCA-1.23.3.7/calib3.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.14 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "PYCA_VERSION",
-                "\"1.23.1.7\""
+                "\"1.23.3.7\""
             ],
             [
                 "PYCA_HG_RELEASE",
-                "\"$HGTag: 1.23.1.7-fc9f97a7c027 $\""
+                "\"1.23.3.7\""
             ],
             [
                 "WITH_THREAD",
                 null
             ],
             [
                 "WITH_TK",
@@ -53,38 +53,40 @@
         "libraries": [
             "ca",
             "Com",
             "tkstub8.5",
             "tclstub8.5"
         ],
         "library_dirs": [
-            "/opt/epics/R7/base/lib/darwin-x86"
+            "/opt/epics/R7/base/lib/darwin-aarch64"
         ],
         "name": "calib",
         "runtime_library_dirs": [
-            "/opt/epics/R7/base/lib/darwin-x86"
+            "/opt/epics/R7/base/lib/darwin-aarch64"
         ],
         "sources": [
             "calib3.pyx"
         ],
         "undef_macros": "CFLAGS"
     },
     "module_name": "calib"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_14"
-#define CYTHON_HEX_VERSION 0x001D0EF0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,14 +117,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -143,26 +146,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -192,18 +203,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -215,61 +275,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -392,17 +463,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -508,24 +638,36 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #else
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -566,26 +708,35 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
+#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
+#if PY_VERSION_HEX >= 0x030900A4
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
+#else
+  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
+  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
+#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -611,21 +762,21 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -639,16 +790,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -658,19 +811,18 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-
+#define __PYX_MARK_ERR_POS(f_index, lineno) \
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-{ \
-  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
-}
+    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -776,14 +928,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -995,26 +1148,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1099,21 +1252,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1134,26 +1295,32 @@
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
 
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
-
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
@@ -1203,14 +1370,19 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
@@ -1406,14 +1578,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("alarmSeverityString", 0);
 
   /* "calib3.pyx":10
  * 
  * def alarmSeverityString(sevr):
  *     try:             # <<<<<<<<<<<<<<
  *         return AlarmSeverity.Strings[sevr]
@@ -1565,14 +1740,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("alarmStatusString", 0);
 
   /* "calib3.pyx":16
  * 
  * def alarmStatusString(status):
  *     try:             # <<<<<<<<<<<<<<
  *         return AlarmStatus.Strings[status]
@@ -1725,14 +1903,17 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("message", 0);
 
   /* "calib3.pyx":22
  * 
  * def message(status):
  *     try:             # <<<<<<<<<<<<<<
  *         return caError._caErrorMsg[caError.CA_EXTRACT_MSG_NO(status)]
@@ -1908,14 +2089,17 @@
 static PyObject *__pyx_pf_5calib_6dbf_type_is_valid(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dbftype) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dbf_type_is_valid", 0);
 
   /* "calib3.pyx":28
  * 
  * def dbf_type_is_valid(dbftype):
  *     return dbftype >= 0 and dbftype <= LAST_TYPE             # <<<<<<<<<<<<<<
  * 
@@ -1990,14 +2174,17 @@
 static PyObject *__pyx_pf_5calib_8dbr_type_is_valid(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dbrtype) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dbr_type_is_valid", 0);
 
   /* "calib3.pyx":31
  * 
  * def dbr_type_is_valid(dbrtype):
  *     return dbrtype >= 0 and dbrtype <= LAST_BUFFER_TYPE             # <<<<<<<<<<<<<<
  * 
@@ -2072,14 +2259,17 @@
 static PyObject *__pyx_pf_5calib_10dbf_type_to_DBR(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dbftype) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dbf_type_to_DBR", 0);
 
   /* "calib3.pyx":34
  * 
  * def dbf_type_to_DBR(dbftype):
  *     if dbftype>=0 and dbftype <= LAST_TYPE:             # <<<<<<<<<<<<<<
  *         return dbftype
@@ -2183,14 +2373,17 @@
 static PyObject *__pyx_pf_5calib_12dbf_type_to_DBR_STS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dbftype) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dbf_type_to_DBR_STS", 0);
 
   /* "calib3.pyx":40
  * 
  * def dbf_type_to_DBR_STS(dbftype):
  *     if dbftype>=0 and dbftype <= LAST_TYPE:             # <<<<<<<<<<<<<<
  *         return dbftype + LAST_TYPE+1
@@ -2302,14 +2495,17 @@
 static PyObject *__pyx_pf_5calib_14dbf_type_to_DBR_TIME(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dbftype) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dbf_type_to_DBR_TIME", 0);
 
   /* "calib3.pyx":46
  * 
  * def dbf_type_to_DBR_TIME(dbftype):
  *     if dbftype>=0 and dbftype <= LAST_TYPE:             # <<<<<<<<<<<<<<
  *         return dbftype + (LAST_TYPE+1)*2
@@ -2424,14 +2620,17 @@
 static PyObject *__pyx_pf_5calib_16dbf_type_to_DBR_GR(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dbftype) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dbf_type_to_DBR_GR", 0);
 
   /* "calib3.pyx":51
  *         return -1
  * def dbf_type_to_DBR_GR(dbftype):
  *     if dbftype>=0 and dbftype <= LAST_TYPE:             # <<<<<<<<<<<<<<
  *         return dbftype + (LAST_TYPE+1)*3
@@ -2546,14 +2745,17 @@
 static PyObject *__pyx_pf_5calib_18dbf_type_to_DBR_CTRL(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_dbftype) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dbf_type_to_DBR_CTRL", 0);
 
   /* "calib3.pyx":57
  * 
  * def dbf_type_to_DBR_CTRL(dbftype):
  *     if dbftype>=0 and dbftype <= LAST_TYPE:             # <<<<<<<<<<<<<<
  *         return dbftype + (LAST_TYPE+1)*4
@@ -2642,107 +2844,129 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "calib3.pyx":66
  * #     return pchid
  * 
- * def search(name, nc, pcallback, args):             # <<<<<<<<<<<<<<
+ * def search(name:str, nc=None, pcallback=None, *args):             # <<<<<<<<<<<<<<
  *     # cdef chid *pchid=NULL;
  *     # pchid=calib.ca_search_and_connect(name, pchid, None,None)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5calib_21search(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_5calib_21search = {"search", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5calib_21search, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_5calib_21search(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_nc = 0;
   CYTHON_UNUSED PyObject *__pyx_v_pcallback = 0;
   CYTHON_UNUSED PyObject *__pyx_v_args = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("search (wrapper)", 0);
+  if (PyTuple_GET_SIZE(__pyx_args) > 3) {
+    __pyx_v_args = PyTuple_GetSlice(__pyx_args, 3, PyTuple_GET_SIZE(__pyx_args));
+    if (unlikely(!__pyx_v_args)) {
+      __Pyx_RefNannyFinishContext();
+      return NULL;
+    }
+    __Pyx_GOTREF(__pyx_v_args);
+  } else {
+    __pyx_v_args = __pyx_empty_tuple; __Pyx_INCREF(__pyx_empty_tuple);
+  }
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_nc,&__pyx_n_s_pcallback,&__pyx_n_s_args,0};
-    PyObject* values[4] = {0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_nc,&__pyx_n_s_pcallback,0};
+    PyObject* values[3] = {0,0,0};
+    values[1] = ((PyObject *)Py_None);
+    values[2] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
+        default:
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
-        default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_nc)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("search", 1, 4, 4, 1); __PYX_ERR(0, 66, __pyx_L3_error)
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_nc);
+          if (value) { values[1] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pcallback)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("search", 1, 4, 4, 2); __PYX_ERR(0, 66, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("search", 1, 4, 4, 3); __PYX_ERR(0, 66, __pyx_L3_error)
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pcallback);
+          if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 66, __pyx_L3_error)
+        const Py_ssize_t used_pos_args = (pos_args < 3) ? pos_args : 3;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, used_pos_args, "search") < 0)) __PYX_ERR(0, 66, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        default:
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        case  0:
+        goto __pyx_L5_argtuple_error;
+      }
     }
-    __pyx_v_name = values[0];
+    __pyx_v_name = ((PyObject*)values[0]);
     __pyx_v_nc = values[1];
     __pyx_v_pcallback = values[2];
-    __pyx_v_args = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("search", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 66, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("search", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 66, __pyx_L3_error)
   __pyx_L3_error:;
+  __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
   __Pyx_AddTraceback("calib.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyString_Type), 1, "name", 1))) __PYX_ERR(0, 66, __pyx_L1_error)
   __pyx_r = __pyx_pf_5calib_20search(__pyx_self, __pyx_v_name, __pyx_v_nc, __pyx_v_pcallback, __pyx_v_args);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_args);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5calib_20search(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_name, CYTHON_UNUSED PyObject *__pyx_v_nc, CYTHON_UNUSED PyObject *__pyx_v_pcallback, CYTHON_UNUSED PyObject *__pyx_v_args) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
 
   /* "calib3.pyx":70
  *     # pchid=calib.ca_search_and_connect(name, pchid, None,None)
  *     # return chid
  *     raise RuntimeError("not implemeted yet")             # <<<<<<<<<<<<<<
  * 
@@ -2753,15 +2977,15 @@
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 70, __pyx_L1_error)
 
   /* "calib3.pyx":66
  * #     return pchid
  * 
- * def search(name, nc, pcallback, args):             # <<<<<<<<<<<<<<
+ * def search(name:str, nc=None, pcallback=None, *args):             # <<<<<<<<<<<<<<
  *     # cdef chid *pchid=NULL;
  *     # pchid=calib.ca_search_and_connect(name, pchid, None,None)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2908,19 +3132,20 @@
                 err = -1;
             else
                 PyErr_Clear();
             break;
         }
         if (skip_leading_underscores &&
 #if PY_MAJOR_VERSION < 3
-            PyString_Check(name) &&
+            likely(PyString_Check(name)) &&
             PyString_AS_STRING(name)[0] == '_')
 #else
-            PyUnicode_Check(name) &&
-            PyUnicode_AS_UNICODE(name)[0] == '_')
+            likely(PyUnicode_Check(name)) &&
+            likely(__Pyx_PyUnicode_GET_LENGTH(name)) &&
+            __Pyx_PyUnicode_READ_CHAR(name, 0) == '_')
 #endif
         {
             Py_DECREF(name);
             continue;
         }
         value = PyObject_GetAttr(v, name);
         if (value == NULL)
@@ -3205,22 +3430,22 @@
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
   __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_calib3_pyx, __pyx_n_s_dbf_type_to_DBR_CTRL, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 56, __pyx_L1_error)
 
   /* "calib3.pyx":66
  * #     return pchid
  * 
- * def search(name, nc, pcallback, args):             # <<<<<<<<<<<<<<
+ * def search(name:str, nc=None, pcallback=None, *args):             # <<<<<<<<<<<<<<
  *     # cdef chid *pchid=NULL;
  *     # pchid=calib.ca_search_and_connect(name, pchid, None,None)
  */
   __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_name, __pyx_n_s_nc, __pyx_n_s_pcallback, __pyx_n_s_args); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_calib3_pyx, __pyx_n_s_search, 66, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_calib3_pyx, __pyx_n_s_search, 66, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 66, __pyx_L1_error)
 
   /* "calib3.pyx":72
  *     raise RuntimeError("not implemeted yet")
  * 
  * def clear(ch_id):             # <<<<<<<<<<<<<<
  *      calib.ca_clear_channel(<calib.chid> ch_id)
  * 
@@ -3233,15 +3458,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -3310,25 +3535,27 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION < 3
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC void
-#else
+#ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#elif PY_MAJOR_VERSION < 3
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" void
+#else
+#define __Pyx_PyMODINIT_FUNC void
 #endif
 #else
-#ifdef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyObject *
+#ifdef __cplusplus
+#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
 #else
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initcalib(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initcalib(void)
@@ -3403,14 +3630,17 @@
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_calib(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'calib' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -3450,19 +3680,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("calib", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -3473,15 +3701,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_calib) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3491,17 +3719,17 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "calib")) {
       if (unlikely(PyDict_SetItemString(modules, "calib", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
+  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
@@ -3666,15 +3894,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_dbf_type_to_DBR_CTRL, __pyx_t_1) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "calib3.pyx":66
  * #     return pchid
  * 
- * def search(name, nc, pcallback, args):             # <<<<<<<<<<<<<<
+ * def search(name:str, nc=None, pcallback=None, *args):             # <<<<<<<<<<<<<<
  *     # cdef chid *pchid=NULL;
  *     # pchid=calib.ca_search_and_connect(name, pchid, None,None)
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5calib_21search, NULL, __pyx_n_s_calib); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_search, __pyx_t_1) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -3919,15 +4147,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -4221,15 +4449,15 @@
 #endif
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -4308,15 +4536,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -4450,40 +4678,14 @@
             PyFPE_END_PROTECT(result)
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
-/* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
-{
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
-    } else {
-        num_expected = num_max;
-        more_or_less = "at most";
-    }
-    if (exact) {
-        more_or_less = "exactly";
-    }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
-}
-
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
@@ -4512,15 +4714,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
+        if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -4539,15 +4741,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
+                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -4555,15 +4757,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
+                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -4592,14 +4794,61 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
+{
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
+    }
+    if (exact) {
+        more_or_less = "exactly";
+    }
+    PyErr_Format(PyExc_TypeError,
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
+}
+
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    }
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    return 0;
+}
+
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
@@ -4753,28 +5002,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -4805,15 +5054,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.')) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -4842,15 +5091,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -4872,15 +5121,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -4946,15 +5195,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
@@ -4966,41 +5215,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -5011,34 +5267,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -5049,15 +5320,22 @@
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
@@ -5102,15 +5380,22 @@
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -5153,15 +5438,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5291,15 +5576,22 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -5342,15 +5634,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5586,19 +5878,41 @@
 static CYTHON_INLINE int __Pyx_StrEq(const char *s1, const char *s2) {
     while (*s1 != '\0' && *s1 == *s2) { s1++; s2++; }
     return *s1 == *s2;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -5848,14 +6162,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `PythonCA-1.23.3.2/cas/caq.py` & `PythonCA-1.23.3.7/cas/caq.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/cas/cas.py` & `PythonCA-1.23.3.7/cas/cas.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 # 2001.12.13 revised
 # 2011.11.14 replace ca.pend_event() --> xca.pend_event()
 # 2012.5.18  use xput instead of put
 # 2016.1.25  bug fixed
 # 2019.11.20 modify for python3 (apply, print, raise, map)
 #
 import ca
-import xca
+#import cas.xca as xca
+from  . import xca
 
 try :
     apply
 except NameError :
     exec('def apply(f,a,k={}) : return f(*a,**k)')
                 
 capollint = 0.02
```

### Comparing `PythonCA-1.23.3.2/cas/xca.py` & `PythonCA-1.23.3.7/cas/xca.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 #   addccb : when conn_state changed, cb(ch)
 #
 # This module depends on ca.py (with _ca_kek.py) and caq.py
 #
 
 import time
 import ca
-import caq  ##Q
+from . import caq  ##Q
 
 try :
     apply
 except NameError :
     exec('def apply(f,a,k={}) : return f(*a,**k)')
                 
 class xcaError(ca.caError) :
```

### Comparing `PythonCA-1.23.3.2/db_access.pxd` & `PythonCA-1.23.3.7/db_access.pxd`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/InstallationMemo.html` & `PythonCA-1.23.3.7/doc/InstallationMemo.html`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/InstallationMemo.md` & `PythonCA-1.23.3.7/doc/InstallationMemo.md`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/InstallationMemo.rst` & `PythonCA-1.23.3.7/doc/InstallationMemo.rst`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/InstallationMemo.rst~` & `PythonCA-1.23.3.7/doc/InstallationMemo.rst~`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/Makefile` & `PythonCA-1.23.3.7/doc/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/InstallationMemo.html` & `PythonCA-1.23.3.7/doc/sphinx/build/html/InstallationMemo.html`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/ReleaseMemo-1.23.2.2.1.html` & `PythonCA-1.23.3.7/doc/sphinx/build/html/ReleaseMemo-1.23.2.2.1.html`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/_sources/InstallationMemo.rst.txt` & `PythonCA-1.23.3.7/doc/sphinx/build/html/_sources/InstallationMemo.rst.txt`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/_sources/ReleaseMemo-1.23.2.2.1.rst.txt` & `PythonCA-1.23.3.7/doc/sphinx/build/html/_sources/ReleaseMemo-1.23.2.2.1.rst.txt`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/_sources/index.rst.txt` & `PythonCA-1.23.3.7/doc/sphinx/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/genindex.html` & `PythonCA-1.23.3.7/doc/sphinx/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/index.html` & `PythonCA-1.23.3.7/doc/sphinx/build/html/index.html`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/html/search.html` & `PythonCA-1.23.3.7/doc/sphinx/build/html/search.html`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/latex/Makefile` & `PythonCA-1.23.3.7/doc/sphinx/build/latex/Makefile`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/build/latex/PythonCAPythonmoduleforEPICSCAlibrary.tex` & `PythonCA-1.23.3.7/doc/sphinx/build/latex/PythonCAPythonmoduleforEPICSCAlibrary.tex`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/source/InstallationMemo.rst` & `PythonCA-1.23.3.7/doc/sphinx/source/InstallationMemo.rst`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/source/ReleaseMemo-1.23.2.2.1.rst` & `PythonCA-1.23.3.7/doc/sphinx/source/ReleaseMemo-1.23.2.2.1.rst`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/source/conf.py` & `PythonCA-1.23.3.7/doc/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/doc/sphinx/source/index.rst` & `PythonCA-1.23.3.7/doc/sphinx/source/index.rst`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/gen_caerrpy.c` & `PythonCA-1.23.3.7/gen_caerrpy.c`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/makeEpicsVersion.py` & `PythonCA-1.23.3.7/makeEpicsVersion.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/CaSimple.py` & `PythonCA-1.23.3.7/sample/CaSimple.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/CaSimple_usingQueue.py` & `PythonCA-1.23.3.7/sample/CaSimple_usingQueue.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/DummySimple.py` & `PythonCA-1.23.3.7/sample/DummySimple.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/QtSample1.py` & `PythonCA-1.23.3.7/sample/QtSample1.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/SyncGroupSample.py` & `PythonCA-1.23.3.7/sample/SyncGroupSample.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkMinimal.py` & `PythonCA-1.23.3.7/sample/TkMinimal.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkRandom.py` & `PythonCA-1.23.3.7/sample/TkRandom.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkRandom2.py` & `PythonCA-1.23.3.7/sample/TkRandom2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkSample1.1.py` & `PythonCA-1.23.3.7/sample/TkSample1.1.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkSample1.py` & `PythonCA-1.23.3.7/sample/TkSample1.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkSample2.py` & `PythonCA-1.23.3.7/sample/TkSample2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkSample3.py` & `PythonCA-1.23.3.7/sample/TkSample3.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/TkSimple2.py` & `PythonCA-1.23.3.7/sample/TkSimple2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/WxMinimal.py` & `PythonCA-1.23.3.7/sample/WxMinimal.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/WxRandom.py` & `PythonCA-1.23.3.7/sample/WxRandom.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/WxSample1.py` & `PythonCA-1.23.3.7/sample/WxSample1.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/WxSample2.py` & `PythonCA-1.23.3.7/sample/WxSample2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/WxSimple.py` & `PythonCA-1.23.3.7/sample/WxSimple.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/WxSimple2.py` & `PythonCA-1.23.3.7/sample/WxSimple2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/caAlarmSeverity.py` & `PythonCA-1.23.3.7/sample/caAlarmSeverity.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/caBadSample2.py` & `PythonCA-1.23.3.7/sample/caBadSample2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/caBadSample3.py` & `PythonCA-1.23.3.7/sample/caBadSample3.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/caBadSampleChannels.py` & `PythonCA-1.23.3.7/sample/caBadSampleChannels.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/caBadSampleThreadLock.py` & `PythonCA-1.23.3.7/sample/caBadSampleThreadLock.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/epicsQt.py` & `PythonCA-1.23.3.7/sample/epicsQt.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/ex_tk4.py` & `PythonCA-1.23.3.7/sample/ex_tk4.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/ex_tk4n.py` & `PythonCA-1.23.3.7/sample/ex_tk4n.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/ezca.py` & `PythonCA-1.23.3.7/sample/ezca.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/fakeca.py` & `PythonCA-1.23.3.7/sample/fakeca.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/fd_reg_test.py` & `PythonCA-1.23.3.7/sample/fd_reg_test.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/fd_register_example.py` & `PythonCA-1.23.3.7/sample/fd_register_example.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/simplecb.py` & `PythonCA-1.23.3.7/sample/simplecb.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/simplecb2.py` & `PythonCA-1.23.3.7/sample/simplecb2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/t5ca.py` & `PythonCA-1.23.3.7/sample/t5ca.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/tamura.py` & `PythonCA-1.23.3.7/sample/tamura.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/tamura2.py` & `PythonCA-1.23.3.7/sample/tamura2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/thread_test.py` & `PythonCA-1.23.3.7/sample/thread_test.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/thread_test2.py` & `PythonCA-1.23.3.7/sample/thread_test2.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/thread_test2C.py` & `PythonCA-1.23.3.7/sample/thread_test2C.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/thread_test3.py` & `PythonCA-1.23.3.7/sample/thread_test3.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/thread_testC.py` & `PythonCA-1.23.3.7/sample/thread_testC.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/sample/wf_put_test/wf_put_test.py` & `PythonCA-1.23.3.7/sample/wf_put_test/wf_put_test.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/setup.py` & `PythonCA-1.23.3.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """
 Setup file for Ca-Python using distutils package.
 Python2.4 or later should be used.
 
 Version Info: (before 1.22)
-  $HGTagShort: 1.23.3.2 $
-  $lastlog: start tag 1.23.3 $
+  $HGTagShort: 1.23.3.5 $
+  $lastlog: before release 1.23.3.4 $
 
   Revision 1.22  2010/08/18 06:46:32  noboru
   support python3
 
   Revision 1.6  2007/03/20 11:48:56  noboru
   Add RCS keywords to setup.py
 """
@@ -31,34 +31,34 @@
 except:
     UNAME="Unknowon"
 
 # macros managedd by mercurial keyword extension
 # mercurial keyword. use 'hg ci' and 'hg kwexpand' to update the following keywords
 #
 CVSAuthor="$Author: noboru $"
-CVSDate="$Date: 2022/06/07 00:48:19 $"
-CVSRev="$Revision: f9ca6aedd9c8 $"
-CVSSource="$Header: /opt/epics/R314/modules/soft/kekb/python/PythonCA-dev/setup.py f9ca6aedd9c8 2022/06/07 00:48:19 noboru $"
+CVSDate="$Date: 2023/07/07 09:59:27 $"
+CVSRev="$Revision: 9c57b570a211 $"
+CVSSource="$Header: /opt/epics/R314/modules/soft/kekb/python/PythonCA-dev/setup.py 9c57b570a211 2023/07/07 09:59:27 noboru $"
 CVSFile="$Source: /opt/epics/R314/modules/soft/kekb/python/PythonCA-dev/setup.py $"
-CVSId="$Id: setup.py f9ca6aedd9c8 2022/06/07 00:48:19 noboru $"
+CVSId="$Id: setup.py 9c57b570a211 2023/07/07 09:59:27 noboru $"
 #
-HGTag="$HGTag: 1.23.3.2-f9ca6aedd9c8 $"
-HGdate="$HGdate: Tue, 07 Jun 2022 09:48:19 +0900 $"
-HGTagShort="$HGTagShort: 1.23.3.2 $"
-HGlastlog="$lastlog: start tag 1.23.3 $"
+HGTag="$HGTag: 1.23.3.5-9c57b570a211 $"
+HGdate="$HGdate: Fri, 07 Jul 2023 18:59:27 +0900 $"
+HGTagShort="$HGTagShort: 1.23.3.5 $"
+HGlastlog="$lastlog: before release 1.23.3.4 $"
 #
 try:
     from hgstamp import HGTagShort as rev
 except:    
     rev=HGTag[HGTag.index(":")+1:HGTag.index("-")].strip()
 
 #release = os.popen("hg log -r tip --template '{latesttag}.{latesttagdistance}-{node|short}'").read()
 #release=HGTag
 release=rev
-
+print("rev:",rev)
 # compile options
 from Cython.Build.BuildExecutable import dump_config
 from Cython.Build import BuildExecutable 
 #dump_config()
 print("CFLAGS:",BuildExecutable.CFLAGS)
 
 try:
@@ -185,37 +185,37 @@
     libraries=libraries,
     library_dirs=[os.path.join(EPICSBASE,"lib",HOSTARCH),
     ] + [os.path.join(path,"") for path in (TKLIB,TCLLIB) if path],
     extra_compile_args=["-O"], # Can we set it to -O1 ?
     runtime_library_dirs=[os.path.join(EPICSBASE,"lib",HOSTARCH),],
 )
 
-setup(name="PythonEPICS-CA",
-      version=rev,
-      author="Noboru Yamamoto, KEK, JAPAN",
-      author_email = "Noboru.YAMAMOTO@kek.jp",
-      description="EPICS CA library interface module with Cython",
-      long_description="""
-      EPICS CA library interface module (KEK, Japan)
-      """,
-      url="http://www-acc.kek.jp/EPICS_Gr/products.html",
-      download_url="http://www-acc.kek.jp/EPICS_Gr/products.html",
-      classifiers=['Programming Language :: C++',
-                   'Programming Language :: Python :: 2.7',
-                   'Programming Language :: Python :: 3.7',
-                   'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
-                   ],
-      py_modules=[],
-      ext_modules=cythonize(calib_ext,
-                            exclude=[],
-                            nthreads=4,
-                            annotate=True,
-                            compiler_directives={"language_level":"3" if PY3 else "2"}, # "2","3","3str"
-                            ),
-      )
+# setup(name="PythonEPICS-CA",
+#       version=rev,
+#       author="Noboru Yamamoto, KEK, JAPAN",
+#       author_email = "Noboru.YAMAMOTO@kek.jp",
+#       description="EPICS CA library interface module with Cython",
+#       long_description="""
+#       EPICS CA library interface module (KEK, Japan)
+#       """,
+#       url="http://www-acc.kek.jp/EPICS_Gr/products.html",
+#       download_url="http://www-acc.kek.jp/EPICS_Gr/products.html",
+#       classifiers=['Programming Language :: C++',
+#                    'Programming Language :: Python :: 2.7',
+#                    'Programming Language :: Python :: 3.7',
+#                    'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
+#                    ],
+#       py_modules=[],
+#       ext_modules=cythonize(calib_ext,
+#                             exclude=[],
+#                             nthreads=4,
+#                             annotate=True,
+#                             compiler_directives={"language_level":"3" if PY3 else "2"}, # "2","3","3str"
+#                             ),
+#       )
 
 ca_ext= Extension(
     "_ca", [CA_SOURCE, ],
     depends=["setup.py",],
     include_dirs=tk_include_dir+[
         os.path.join(EPICSBASE,"include"),
         os.path.join(EPICSBASE,"include/os",UNAME),
@@ -245,15 +245,15 @@
                       nthreads=4,
                       annotate=True,
                       compiler_directives={"language_level":"3" if PY3 else "2"}, # "2","3","3str"
                       )
 #
 with open("README.md", "r") as fh:
    long_description = fh.read()
-#
+
 setup(name="PythonCA",
       version=rev,
       author="Noboru Yamamoto, KEK, JAPAN",
       author_email = "Noboru.YAMAMOTO@kek.jp",
       description="EPICS CA library interface module",
       long_description=long_description,
       url="http://www-acc.kek.jp/EPICS_Gr/products.html",
@@ -261,31 +261,34 @@
       classifiers=['Programming Language :: C++',
                    'Programming Language :: Python :: 2.7',
                    'Programming Language :: Python :: 3.6',
                    'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
                    #'Topic :: EPICS CA',
                    #'Topic :: Controls'
                    ],
-      py_modules=["ca", "caError", "cadefs","_ca_kek","_ca_fnal","CaChannel","printfn","epicsVersion"],
+      package_dir={"ca":"", "cas":"cas"},
+      py_modules=["ca", "caError", "cadefs","_ca_kek","_ca_fnal","CaChannel","printfn","epicsVersion",
+                  "cas.cas", "cas.xca", "cas.caq"
+                  ],
       ext_modules=ext_modules,
       **extra
 )
 
-setup(name="cas",
-      version=rev,
-      author="Tatsuro Nakamura, KEK, JAPAN",
-      author_email = "Tatsuro.nakamura@kek.jp",
-      description="EPICS CA library interface module",
-      long_description="""
-      Simple EPICS CA library interface module (KEK,Japan)
-      """,
-      url="http://www-acc.kek.jp/EPICS_Gr/products.html",
-      download_url="http://www-acc.kek.jp/EPICS_Gr/products.html",
-      classifiers=['Programming Language :: Python :: 2.7',
-                   'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
-                   #'Topic :: EPICS CA',
-                   #'Topic :: Controls'
-                   ],
-      package_dir={"":"cas"},
-      py_modules=["cas","xca"],
-      **extra
-)
+# setup(name="cas",
+#       version=rev,
+#       author="Tatsuro Nakamura, KEK, JAPAN",
+#       author_email = "Tatsuro.nakamura@kek.jp",
+#       description="EPICS CA library interface module",
+#       long_description="""
+#       Simple EPICS CA library interface module (KEK,Japan)
+#       """,
+#       url="http://www-acc.kek.jp/EPICS_Gr/products.html",
+#       download_url="http://www-acc.kek.jp/EPICS_Gr/products.html",
+#       classifiers=['Programming Language :: Python :: 2.7',
+#                    'Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator',
+#                    #'Topic :: EPICS CA',
+#                    #'Topic :: Controls'
+#                    ],
+#       package_dir={"":"cas"},
+#       py_modules=["cas","xca","caq"],
+#       **extra
+# )
```

### Comparing `PythonCA-1.23.3.2/test/WFmemleakCheck.py` & `PythonCA-1.23.3.7/test/WFmemleakCheck.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/test/excas.db` & `PythonCA-1.23.3.7/test/excas.db`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/test/excas.substitutions` & `PythonCA-1.23.3.7/test/excas.substitutions`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/test/excas2.db` & `PythonCA-1.23.3.7/test/excas2.db`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/test/randomTest.py` & `PythonCA-1.23.3.7/test/randomTest.py`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/test/test.db` & `PythonCA-1.23.3.7/test/test.db`

 * *Files identical despite different names*

### Comparing `PythonCA-1.23.3.2/test/testPythonCA.py` & `PythonCA-1.23.3.7/test/testPythonCA.py`

 * *Files identical despite different names*

