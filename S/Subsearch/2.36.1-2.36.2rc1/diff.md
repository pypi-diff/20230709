# Comparing `tmp/Subsearch-2.36.1.tar.gz` & `tmp/Subsearch-2.36.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.36.1.tar", last modified: Sat Jul  8 17:59:54 2023, max compression
+gzip compressed data, was "Subsearch-2.36.2rc1.tar", last modified: Sat Jul  8 21:38:21 2023, max compression
```

## Comparing `Subsearch-2.36.1.tar` & `Subsearch-2.36.2rc1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.064437 Subsearch-2.36.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 17:59:36.000000 Subsearch-2.36.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-08 17:59:36.000000 Subsearch-2.36.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-08 17:59:54.064437 Subsearch-2.36.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-08 17:59:36.000000 Subsearch-2.36.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-08 17:59:36.000000 Subsearch-2.36.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:59:54.064437 Subsearch-2.36.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-08 17:59:36.000000 Subsearch-2.36.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.052436 Subsearch-2.36.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.056436 Subsearch-2.36.1/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 17:59:53.000000 Subsearch-2.36.1/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 17:59:54.000000 Subsearch-2.36.1/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.056436 Subsearch-2.36.1/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.056436 Subsearch-2.36.1/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/data_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/app_theme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/spritesheet_data.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/assets/spritesheet.png
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/assets/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/gui_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/gui/tabs/settings_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.060436 Subsearch-2.36.1/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 17:59:54.064437 Subsearch-2.36.1/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/app_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-08 17:59:36.000000 Subsearch-2.36.1/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.544102 Subsearch-2.36.2rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.544102 Subsearch-2.36.2rc1/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-08 21:38:21.000000 Subsearch-2.36.2rc1/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-08 21:38:21.000000 Subsearch-2.36.2rc1/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:38:21.000000 Subsearch-2.36.2rc1/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 21:38:21.000000 Subsearch-2.36.2rc1/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:38:21.000000 Subsearch-2.36.2rc1/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-08 21:38:21.000000 Subsearch-2.36.2rc1/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-08 21:38:21.000000 Subsearch-2.36.2rc1/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.544102 Subsearch-2.36.2rc1/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.544102 Subsearch-2.36.2rc1/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/data/data_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.544102 Subsearch-2.36.2rc1/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/spritesheet_data.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/src/subsearch/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/assets/spritesheet.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/assets/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/gui_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/gui/tabs/settings_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:38:21.548102 Subsearch-2.36.2rc1/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/app_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-08 21:38:02.000000 Subsearch-2.36.2rc1/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.36.1/LICENSE` & `Subsearch-2.36.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/PKG-INFO` & `Subsearch-2.36.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.36.1
+Version: 2.36.2rc1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.36.1/README.md` & `Subsearch-2.36.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/pyproject.toml` & `Subsearch-2.36.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/setup.py` & `Subsearch-2.36.2rc1/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.36.2rc1/src/Subsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.36.1
+Version: 2.36.2rc1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.36.1/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.36.2rc1/src/Subsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/__init__.py` & `Subsearch-2.36.2rc1/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/core.py` & `Subsearch-2.36.2rc1/src/subsearch/core.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/data/data_initializer.py` & `Subsearch-2.36.2rc1/src/subsearch/data/data_initializer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/data/data_objects.py` & `Subsearch-2.36.2rc1/src/subsearch/data/data_objects.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/data/languages.json` & `Subsearch-2.36.2rc1/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/__init__.py` & `Subsearch-2.36.2rc1/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/app_theme/spritesheet_data.tcl` & `Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/spritesheet_data.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl` & `Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/ttk_subsearch_theme.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl` & `Subsearch-2.36.2rc1/src/subsearch/gui/app_theme/ttk_theme_initializer.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/assets/spritesheet.png` & `Subsearch-2.36.2rc1/src/subsearch/gui/assets/spritesheet.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/assets/subsearch.ico` & `Subsearch-2.36.2rc1/src/subsearch/gui/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/gui_toolkit.py` & `Subsearch-2.36.2rc1/src/subsearch/gui/gui_toolkit.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/tab_manager.py` & `Subsearch-2.36.2rc1/src/subsearch/gui/tab_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.36.2rc1/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.36.2rc1/src/subsearch/gui/tabs/language_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.36.2rc1/src/subsearch/gui/tabs/search_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.36.2rc1/src/subsearch/gui/tabs/settings_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/providers/generic.py` & `Subsearch-2.36.2rc1/src/subsearch/providers/generic.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.36.2rc1/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/providers/subscene.py` & `Subsearch-2.36.2rc1/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.36.2rc1/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/app_integrity.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/app_integrity.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/exceptions.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/file_manager.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/io_json.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/io_json.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/io_winreg.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/log.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/log.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/mutex_synchronizer.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/mutex_synchronizer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/state_machine.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/state_machine.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/string_parser.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.36.1/src/subsearch/utils/update.py` & `Subsearch-2.36.2rc1/src/subsearch/utils/update.py`

 * *Files identical despite different names*

