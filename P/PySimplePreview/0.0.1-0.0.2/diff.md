# Comparing `tmp/PySimplePreview-0.0.1.tar.gz` & `tmp/PySimplePreview-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySimplePreview-0.0.1.tar", last modified: Sun Jul  9 20:30:04 2023, max compression
+gzip compressed data, was "PySimplePreview-0.0.2.tar", last modified: Sun Jul  9 21:49:06 2023, max compression
```

## Comparing `PySimplePreview-0.0.1.tar` & `PySimplePreview-0.0.2.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.790001 PySimplePreview-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-09 20:30:04.790001 PySimplePreview-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-09 20:30:04.790001 PySimplePreview-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.786001 PySimplePreview-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.786001 PySimplePreview-0.0.1/src/PySimplePreview/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.786001 PySimplePreview-0.0.1/src/PySimplePreview/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/data/config_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/data/di.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/data/previews_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/di.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.786001 PySimplePreview-0.0.1/src/PySimplePreview/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/di.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.786001 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.786001 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/abc/files_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/abc/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/files_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/previews_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.790001 PySimplePreview-0.0.1/src/PySimplePreview/domain/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/model/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/model/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/model/log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/model/position.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/domain/model/preview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.790001 PySimplePreview-0.0.1/src/PySimplePreview/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.790001 PySimplePreview-0.0.1/src/PySimplePreview/view/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/api/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.790001 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/external_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/external_preview_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/preview_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/system_args_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/controller/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/di.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-09 20:29:55.000000 PySimplePreview-0.0.1/src/PySimplePreview/view/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:30:04.786001 PySimplePreview-0.0.1/src/PySimplePreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-09 20:30:04.000000 PySimplePreview-0.0.1/src/PySimplePreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-09 20:30:04.000000 PySimplePreview-0.0.1/src/PySimplePreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:30:04.000000 PySimplePreview-0.0.1/src/PySimplePreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 20:30:04.000000 PySimplePreview-0.0.1/src/PySimplePreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 20:30:04.000000 PySimplePreview-0.0.1/src/PySimplePreview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.786301 PySimplePreview-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-09 21:49:06.786301 PySimplePreview-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-09 21:49:06.786301 PySimplePreview-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.778300 PySimplePreview-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.778300 PySimplePreview-0.0.2/src/PySimplePreview/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.782301 PySimplePreview-0.0.2/src/PySimplePreview/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/data/config_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/data/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/data/previews_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/di.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.782301 PySimplePreview-0.0.2/src/PySimplePreview/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/di.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.782301 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.782301 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/abc/files_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/abc/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/files_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/previews_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.782301 PySimplePreview-0.0.2/src/PySimplePreview/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/model/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/model/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/model/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/model/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/domain/model/preview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.786301 PySimplePreview-0.0.2/src/PySimplePreview/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.786301 PySimplePreview-0.0.2/src/PySimplePreview/view/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/api/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.786301 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/external_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/external_preview_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/preview_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/system_args_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/controller/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-09 21:48:55.000000 PySimplePreview-0.0.2/src/PySimplePreview/view/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:49:06.782301 PySimplePreview-0.0.2/src/PySimplePreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-09 21:49:06.000000 PySimplePreview-0.0.2/src/PySimplePreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-09 21:49:06.000000 PySimplePreview-0.0.2/src/PySimplePreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:49:06.000000 PySimplePreview-0.0.2/src/PySimplePreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 21:49:06.000000 PySimplePreview-0.0.2/src/PySimplePreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-09 21:49:06.000000 PySimplePreview-0.0.2/src/PySimplePreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 21:49:06.000000 PySimplePreview-0.0.2/src/PySimplePreview.egg-info/top_level.txt
```

### Comparing `PySimplePreview-0.0.1/LICENSE.md` & `PySimplePreview-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/PKG-INFO` & `PySimplePreview-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 Metadata-Version: 2.1
 Name: PySimplePreview
-Version: 0.0.1
-Summary: "Realtime (live/hot) preview of PySimpleGUI layouts"
+Version: 0.0.2
+Summary: Realtime (live/hot) preview of PySimpleGUI layouts
 Author: MaxBQb
 License: MIT License
 Project-URL: Homepage, https://github.com/MaxBQb/PySimplePreview
 Project-URL: Bug Tracker, https://github.com/MaxBQb/PySimplePreview/issues
 Keywords: PySimpleGUI,preview,live-preview,realtime-preview,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Quick Overview
-This is python tool which provide realtime/live/hot preview of [PySimpleGUI](https://pypi.org/project/PySimpleGUI/) layouts
+# PySimplePreview
+[![PyPI version shields.io](https://img.shields.io/pypi/v/PySimplePreview.svg)](https://pypi.org/project/PySimplePreview/)
+[![GitHub license](https://img.shields.io/github/license/MaxBQb/WinMagnification.svg)](https://github.com/MaxBQb/PySimplePreview/blob/master/LICENSE.md)
+---
+
+This is python tool which provide realtime/live/hot preview of [PySimpleGUI](https://pypi.org/project/PySimpleGUI/) layouts.
 This tool assumes that developer writes layouts as separate method/function(-s).
-Note: Layout is simply list of lists of PySimpleGUI elements
+> Note: Layout is simply list of lists of PySimpleGUI elements.
 ## Usage
+### Installation
+Simply use pip:
+```sh
+pip install PySimplePreview
+```
 ### Prepare your project
 This tool is development-only dependency, so before you start using it, lets help python resolve it as optional dependency:
 1. First, if you store dependencies in `requirements.txt`, add separate file e.g. `requirements-dev.txt`
-  (you will be able to install all requirement with `pip install -r requirements.txt -r requirements-dev.txt`)
-2. Then I suggest create new module (you may also inline it's content in your code which is bad, but possible)
+  (you will be able to install all requirement with `pip install -r requirements.txt -r requirements-dev.txt`).
+2. Then I suggest create new module (you may also inline it's content in your code which is bad, but possible).
 With this content:
 ```py
 #  Use this to not couple with develop-only dependency
 try:  # Used when package installed
     # noinspection PyUnresolvedReferences
     from PySimplePreview import *
 except ImportError:  # Used when no dependency found
@@ -46,94 +55,97 @@
     def params(*args, **kwargs):
         return args, kwargs
 
     group_previews = preview
     method_previews = preview
 ```
 
-3. If you've created separate module, then you can simply import anything from it instead of PySimplePreview
-Note: You can always use custom technique to manage optional python dependencies, this is just example
-Now your app can work with and without PySimplePreview
+3. If you've created separate module, then you can simply import anything from it instead of PySimplePreview.
+> Note: You can always use custom technique to manage optional python dependencies, this is just example.
+
+Now your app can work with and without PySimplePreview!
 
 ### Examples
 1. First you need to import `preview` decorator from PySimplePreview (or yours custom module which tries to import it).
 ```py
 import PySimpleGUI as sg
 import PySimplePreview as psp
 # ... or custom module name, e.g. _PySimplePreview
 import _PySimplePreview as psp
 ```
-2. Then you can decorate any callable that returns layout with `preview`
+2. Then you can decorate any callable that returns layout with `preview`.
 Example:
 ```py
 @psp.preview
 def get_layout():
     return [
         [sg.Text("Hello, world!")]
     ]
 ```
-3. Now you can run PySimplePreview with `python -m PySimplePreview`
-4. Select path to your project's root and choose preview to be shown
-5. Edit your layout without closing PySimplePreview
+3. Now you can run PySimplePreview with `python -m PySimplePreview`.
+4. Select path to your project's root and choose preview to be shown.
+5. Edit your layout without closing PySimplePreview.
 Example:
 ```py
 @psp.preview
 def get_layout():
     return [
         [sg.Text("Hello, world!")],
         [sg.Text("Previews are cool!")],
     ]
 ```
 6. Remember to save your changes and *magic happens*: it's reflected in preview window.
 
-For more complex cases see [examples](examples/)
+For more complex cases see [examples](examples/).
 
 ## Features 
 ### PySimplePreview API
-1. `@preview` without params for functions and static methods
-  1.0 `@preview()` for parameters:
-  1.1 Custom name of preview
-  1.2 Parameters for function to be called with (can be evaluated lazily)
-  1.3 Custom group name (use for ease of searching, and maybe for something special later on)
-  1.4 Custom window (Use own PySimpleGUI windows to preview own layouts)
-3. `@method_preview` same as `@preview` but for class methods and properties
-  3.1 Have same parameters as `@preview()`, additionally have optional `instance_provider` parameter to provide `self` for methods
-    3.1.1 `instance_provider` can use cls parameter to create class instance
-    3.1.2 `instance_provider` can have no parameters to provide class instance from some other place
-    3.1.3 `instance_provider` can be omitted, then no-args constructor of class will be used
-4. Multiple previews may be applied to same callable
-5. `@group_previews` can be used to set group_name for multiple previews of same callable
-  5.0 `@group_previews()` name can be set as parameter
-6. In case when preview_name omitted, fully-qualified callable name will be used (`package.module.function_name` or `module.function_name`)
-7. Same goes for `group_previews` no-param form
+1. `@preview` without params for functions and static methods.
+    1. `@preview()` for parameters:
+    2. Custom name of preview.
+    3. Parameters for function to be called with (can be evaluated lazily).
+    4. Custom group name (use for ease of searching, and maybe for something special later on).
+    5. Custom window (Use own PySimpleGUI windows to preview own layouts).
+3. `@method_preview` same as `@preview` but for class methods and properties.
+    1. Have same parameters as `@preview()`, additionally have optional `instance_provider` parameter to provide `self` for methods.
+    2. `instance_provider` can use cls parameter to create class instance.
+    3. `instance_provider` can have no parameters to provide class instance from some other place.
+    4. `instance_provider` can be omitted, then no-args constructor of class will be used.
+4. Multiple previews may be applied to same callable.
+5. `@group_previews` can be used to set group_name for multiple previews of same callable.
+    1. `@group_previews()` name can be set as parameter.
+6. In case when preview_name omitted, fully-qualified callable name will be used (`package.module.function_name` or `module.function_name`).
+7. Same goes for `group_previews` no-param form.
 
 ### PySimplePreview App
-1. Preview Theme can be customised
-2. App remembers its position and size (toggleable)
-3. App stays on top of other windows (toggleable)
-4. Preview window can be separated from main app window
-5. Previews can be filtered by groups
-6. App supports execution params see `python -m PySimplePreview -h`
-7. See app logs for more info (it also contains handled user-defined events from layout previewed)
-8. If you want to see update on any module edited (when layout depends on other module), you may toggle Reload All option
-9. App supports observing single module, package with `__init__.py` file and just flat-layout (folder with `.py` files)
+1. Preview Theme can be customised.
+2. App remembers its position and size (toggleable).
+3. App stays on top of other windows (toggleable).
+4. Preview window can be separated from main app window.
+5. Previews can be filtered by groups.
+6. App supports execution params see `python -m PySimplePreview -h`.
+7. See app logs for more info (it also contains handled user-defined events from layout previewed).
+8. If you want to see update on any module edited (when layout depends on other module), you may toggle Reload All option.
+9. App supports observing single module, package with `__init__.py` file and just flat-layout (folder with `.py` files).
 
 # Docs
-There is no readthedocs page for this project for now (it may be changed soon)
-But public API well-documented in code and covered with typehints (supported by PyCharm)
-All features using can be found in [examples](examples/)
+There is no readthedocs page for this project for now (it may be changed soon).
+But public API well-documented in code and covered with typehints (supported by PyCharm).
+All features using can be found in [examples](examples/).
 
 # Compatability
 ## Python versions support
 For now only Python 3.11 tested, but older versions support planned.
 
 ## PySimpleGUI versions support
 Currently tested on PySimpleGUI 4.60.5, 
-I'll think about adding support for older versions later, better use latest releases anyway :)
+I'll think about adding support for older versions later,
+better use latest releases anyway :)
 
 ## Different PySimpleGUI backends
-Currently tested only with tkinter backend, I have plans for framework-agnostic version.
+Currently tested only with tkinter backend, 
+I have plans for framework-agnostic version.
 
 # Contribution
 Feel free to [open issues](https://github.com/MaxBQb/PySimplePreview/issues/new), but be careful with PR's (small fixes are OK, but this is MVP project, 
 it's implementation can be changed in any way).
 Also note that I may have not enough free time, so have patience.
```

### Comparing `PySimplePreview-0.0.1/README.md` & `PySimplePreview-0.0.2/src/PySimplePreview.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,44 @@
-# Quick Overview
-This is python tool which provide realtime/live/hot preview of [PySimpleGUI](https://pypi.org/project/PySimpleGUI/) layouts
+Metadata-Version: 2.1
+Name: PySimplePreview
+Version: 0.0.2
+Summary: Realtime (live/hot) preview of PySimpleGUI layouts
+Author: MaxBQb
+License: MIT License
+Project-URL: Homepage, https://github.com/MaxBQb/PySimplePreview
+Project-URL: Bug Tracker, https://github.com/MaxBQb/PySimplePreview/issues
+Keywords: PySimpleGUI,preview,live-preview,realtime-preview,GUI
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# PySimplePreview
+[![PyPI version shields.io](https://img.shields.io/pypi/v/PySimplePreview.svg)](https://pypi.org/project/PySimplePreview/)
+[![GitHub license](https://img.shields.io/github/license/MaxBQb/WinMagnification.svg)](https://github.com/MaxBQb/PySimplePreview/blob/master/LICENSE.md)
+---
+
+This is python tool which provide realtime/live/hot preview of [PySimpleGUI](https://pypi.org/project/PySimpleGUI/) layouts.
 This tool assumes that developer writes layouts as separate method/function(-s).
-Note: Layout is simply list of lists of PySimpleGUI elements
+> Note: Layout is simply list of lists of PySimpleGUI elements.
 ## Usage
+### Installation
+Simply use pip:
+```sh
+pip install PySimplePreview
+```
 ### Prepare your project
 This tool is development-only dependency, so before you start using it, lets help python resolve it as optional dependency:
 1. First, if you store dependencies in `requirements.txt`, add separate file e.g. `requirements-dev.txt`
-  (you will be able to install all requirement with `pip install -r requirements.txt -r requirements-dev.txt`)
-2. Then I suggest create new module (you may also inline it's content in your code which is bad, but possible)
+  (you will be able to install all requirement with `pip install -r requirements.txt -r requirements-dev.txt`).
+2. Then I suggest create new module (you may also inline it's content in your code which is bad, but possible).
 With this content:
 ```py
 #  Use this to not couple with develop-only dependency
 try:  # Used when package installed
     # noinspection PyUnresolvedReferences
     from PySimplePreview import *
 except ImportError:  # Used when no dependency found
@@ -28,94 +55,97 @@
     def params(*args, **kwargs):
         return args, kwargs
 
     group_previews = preview
     method_previews = preview
 ```
 
-3. If you've created separate module, then you can simply import anything from it instead of PySimplePreview
-Note: You can always use custom technique to manage optional python dependencies, this is just example
-Now your app can work with and without PySimplePreview
+3. If you've created separate module, then you can simply import anything from it instead of PySimplePreview.
+> Note: You can always use custom technique to manage optional python dependencies, this is just example.
+
+Now your app can work with and without PySimplePreview!
 
 ### Examples
 1. First you need to import `preview` decorator from PySimplePreview (or yours custom module which tries to import it).
 ```py
 import PySimpleGUI as sg
 import PySimplePreview as psp
 # ... or custom module name, e.g. _PySimplePreview
 import _PySimplePreview as psp
 ```
-2. Then you can decorate any callable that returns layout with `preview`
+2. Then you can decorate any callable that returns layout with `preview`.
 Example:
 ```py
 @psp.preview
 def get_layout():
     return [
         [sg.Text("Hello, world!")]
     ]
 ```
-3. Now you can run PySimplePreview with `python -m PySimplePreview`
-4. Select path to your project's root and choose preview to be shown
-5. Edit your layout without closing PySimplePreview
+3. Now you can run PySimplePreview with `python -m PySimplePreview`.
+4. Select path to your project's root and choose preview to be shown.
+5. Edit your layout without closing PySimplePreview.
 Example:
 ```py
 @psp.preview
 def get_layout():
     return [
         [sg.Text("Hello, world!")],
         [sg.Text("Previews are cool!")],
     ]
 ```
 6. Remember to save your changes and *magic happens*: it's reflected in preview window.
 
-For more complex cases see [examples](examples/)
+For more complex cases see [examples](examples/).
 
 ## Features 
 ### PySimplePreview API
-1. `@preview` without params for functions and static methods
-  1.0 `@preview()` for parameters:
-  1.1 Custom name of preview
-  1.2 Parameters for function to be called with (can be evaluated lazily)
-  1.3 Custom group name (use for ease of searching, and maybe for something special later on)
-  1.4 Custom window (Use own PySimpleGUI windows to preview own layouts)
-3. `@method_preview` same as `@preview` but for class methods and properties
-  3.1 Have same parameters as `@preview()`, additionally have optional `instance_provider` parameter to provide `self` for methods
-    3.1.1 `instance_provider` can use cls parameter to create class instance
-    3.1.2 `instance_provider` can have no parameters to provide class instance from some other place
-    3.1.3 `instance_provider` can be omitted, then no-args constructor of class will be used
-4. Multiple previews may be applied to same callable
-5. `@group_previews` can be used to set group_name for multiple previews of same callable
-  5.0 `@group_previews()` name can be set as parameter
-6. In case when preview_name omitted, fully-qualified callable name will be used (`package.module.function_name` or `module.function_name`)
-7. Same goes for `group_previews` no-param form
+1. `@preview` without params for functions and static methods.
+    1. `@preview()` for parameters:
+    2. Custom name of preview.
+    3. Parameters for function to be called with (can be evaluated lazily).
+    4. Custom group name (use for ease of searching, and maybe for something special later on).
+    5. Custom window (Use own PySimpleGUI windows to preview own layouts).
+3. `@method_preview` same as `@preview` but for class methods and properties.
+    1. Have same parameters as `@preview()`, additionally have optional `instance_provider` parameter to provide `self` for methods.
+    2. `instance_provider` can use cls parameter to create class instance.
+    3. `instance_provider` can have no parameters to provide class instance from some other place.
+    4. `instance_provider` can be omitted, then no-args constructor of class will be used.
+4. Multiple previews may be applied to same callable.
+5. `@group_previews` can be used to set group_name for multiple previews of same callable.
+    1. `@group_previews()` name can be set as parameter.
+6. In case when preview_name omitted, fully-qualified callable name will be used (`package.module.function_name` or `module.function_name`).
+7. Same goes for `group_previews` no-param form.
 
 ### PySimplePreview App
-1. Preview Theme can be customised
-2. App remembers its position and size (toggleable)
-3. App stays on top of other windows (toggleable)
-4. Preview window can be separated from main app window
-5. Previews can be filtered by groups
-6. App supports execution params see `python -m PySimplePreview -h`
-7. See app logs for more info (it also contains handled user-defined events from layout previewed)
-8. If you want to see update on any module edited (when layout depends on other module), you may toggle Reload All option
-9. App supports observing single module, package with `__init__.py` file and just flat-layout (folder with `.py` files)
+1. Preview Theme can be customised.
+2. App remembers its position and size (toggleable).
+3. App stays on top of other windows (toggleable).
+4. Preview window can be separated from main app window.
+5. Previews can be filtered by groups.
+6. App supports execution params see `python -m PySimplePreview -h`.
+7. See app logs for more info (it also contains handled user-defined events from layout previewed).
+8. If you want to see update on any module edited (when layout depends on other module), you may toggle Reload All option.
+9. App supports observing single module, package with `__init__.py` file and just flat-layout (folder with `.py` files).
 
 # Docs
-There is no readthedocs page for this project for now (it may be changed soon)
-But public API well-documented in code and covered with typehints (supported by PyCharm)
-All features using can be found in [examples](examples/)
+There is no readthedocs page for this project for now (it may be changed soon).
+But public API well-documented in code and covered with typehints (supported by PyCharm).
+All features using can be found in [examples](examples/).
 
 # Compatability
 ## Python versions support
 For now only Python 3.11 tested, but older versions support planned.
 
 ## PySimpleGUI versions support
 Currently tested on PySimpleGUI 4.60.5, 
-I'll think about adding support for older versions later, better use latest releases anyway :)
+I'll think about adding support for older versions later,
+better use latest releases anyway :)
 
 ## Different PySimpleGUI backends
-Currently tested only with tkinter backend, I have plans for framework-agnostic version.
+Currently tested only with tkinter backend, 
+I have plans for framework-agnostic version.
 
 # Contribution
 Feel free to [open issues](https://github.com/MaxBQb/PySimplePreview/issues/new), but be careful with PR's (small fixes are OK, but this is MVP project, 
 it's implementation can be changed in any way).
 Also note that I may have not enough free time, so have patience.
```

### Comparing `PySimplePreview-0.0.1/setup.cfg` & `PySimplePreview-0.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = PySimplePreview
 version = attr: PySimplePreview.__version__
 author = MaxBQb
-description = "Realtime (live/hot) preview of PySimpleGUI layouts"
+description = Realtime (live/hot) preview of PySimpleGUI layouts
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = PySimpleGUI, preview, live-preview, realtime-preview, GUI
 license = MIT License
 license_files = 
 	LICENSE.md
 project_urls = 
@@ -21,25 +21,22 @@
 
 [options.package_data]
 * = *.md
 
 [options]
 packages = find:
 python_requires = >=3.11
-dynamic = ["dependencies"]
+install_requires = file: requirements.txt
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	PySimplePreview = PySimplePreview:main
 
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/data/config_storage.py` & `PySimplePreview-0.0.2/src/PySimplePreview/data/config_storage.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/di.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/di.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/abc/module_loader.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/abc/module_loader.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/files_observer.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/files_observer.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/module_loader.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/module_loader.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/interactor/previews_manager.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/interactor/previews_manager.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/model/config.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/model/config.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/model/event.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/model/event.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/model/log_config.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/model/log_config.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/model/position.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/model/position.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/domain/model/preview.py` & `PySimplePreview-0.0.2/src/PySimplePreview/domain/model/preview.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/api/_types.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/api/_types.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/api/_utils.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/api/_utils.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/api/core.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/api/core.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/app.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/app.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/controller/base.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/controller/base.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/controller/external_preview.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/controller/external_preview.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/controller/external_preview_factory.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/controller/external_preview_factory.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/controller/preview_settings.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/controller/preview_settings.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/controller/system_args_handler.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/controller/system_args_handler.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/controller/utils.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/controller/utils.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/di.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/di.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/layouts.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/layouts.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/log.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/log.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview/view/models.py` & `PySimplePreview-0.0.2/src/PySimplePreview/view/models.py`

 * *Files identical despite different names*

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview.egg-info/PKG-INFO` & `PySimplePreview-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-Metadata-Version: 2.1
-Name: PySimplePreview
-Version: 0.0.1
-Summary: "Realtime (live/hot) preview of PySimpleGUI layouts"
-Author: MaxBQb
-License: MIT License
-Project-URL: Homepage, https://github.com/MaxBQb/PySimplePreview
-Project-URL: Bug Tracker, https://github.com/MaxBQb/PySimplePreview/issues
-Keywords: PySimpleGUI,preview,live-preview,realtime-preview,GUI
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
+# PySimplePreview
+[![PyPI version shields.io](https://img.shields.io/pypi/v/PySimplePreview.svg)](https://pypi.org/project/PySimplePreview/)
+[![GitHub license](https://img.shields.io/github/license/MaxBQb/WinMagnification.svg)](https://github.com/MaxBQb/PySimplePreview/blob/master/LICENSE.md)
+---
 
-# Quick Overview
-This is python tool which provide realtime/live/hot preview of [PySimpleGUI](https://pypi.org/project/PySimpleGUI/) layouts
+This is python tool which provide realtime/live/hot preview of [PySimpleGUI](https://pypi.org/project/PySimpleGUI/) layouts.
 This tool assumes that developer writes layouts as separate method/function(-s).
-Note: Layout is simply list of lists of PySimpleGUI elements
+> Note: Layout is simply list of lists of PySimpleGUI elements.
 ## Usage
+### Installation
+Simply use pip:
+```sh
+pip install PySimplePreview
+```
 ### Prepare your project
 This tool is development-only dependency, so before you start using it, lets help python resolve it as optional dependency:
 1. First, if you store dependencies in `requirements.txt`, add separate file e.g. `requirements-dev.txt`
-  (you will be able to install all requirement with `pip install -r requirements.txt -r requirements-dev.txt`)
-2. Then I suggest create new module (you may also inline it's content in your code which is bad, but possible)
+  (you will be able to install all requirement with `pip install -r requirements.txt -r requirements-dev.txt`).
+2. Then I suggest create new module (you may also inline it's content in your code which is bad, but possible).
 With this content:
 ```py
 #  Use this to not couple with develop-only dependency
 try:  # Used when package installed
     # noinspection PyUnresolvedReferences
     from PySimplePreview import *
 except ImportError:  # Used when no dependency found
@@ -46,94 +37,97 @@
     def params(*args, **kwargs):
         return args, kwargs
 
     group_previews = preview
     method_previews = preview
 ```
 
-3. If you've created separate module, then you can simply import anything from it instead of PySimplePreview
-Note: You can always use custom technique to manage optional python dependencies, this is just example
-Now your app can work with and without PySimplePreview
+3. If you've created separate module, then you can simply import anything from it instead of PySimplePreview.
+> Note: You can always use custom technique to manage optional python dependencies, this is just example.
+
+Now your app can work with and without PySimplePreview!
 
 ### Examples
 1. First you need to import `preview` decorator from PySimplePreview (or yours custom module which tries to import it).
 ```py
 import PySimpleGUI as sg
 import PySimplePreview as psp
 # ... or custom module name, e.g. _PySimplePreview
 import _PySimplePreview as psp
 ```
-2. Then you can decorate any callable that returns layout with `preview`
+2. Then you can decorate any callable that returns layout with `preview`.
 Example:
 ```py
 @psp.preview
 def get_layout():
     return [
         [sg.Text("Hello, world!")]
     ]
 ```
-3. Now you can run PySimplePreview with `python -m PySimplePreview`
-4. Select path to your project's root and choose preview to be shown
-5. Edit your layout without closing PySimplePreview
+3. Now you can run PySimplePreview with `python -m PySimplePreview`.
+4. Select path to your project's root and choose preview to be shown.
+5. Edit your layout without closing PySimplePreview.
 Example:
 ```py
 @psp.preview
 def get_layout():
     return [
         [sg.Text("Hello, world!")],
         [sg.Text("Previews are cool!")],
     ]
 ```
 6. Remember to save your changes and *magic happens*: it's reflected in preview window.
 
-For more complex cases see [examples](examples/)
+For more complex cases see [examples](examples/).
 
 ## Features 
 ### PySimplePreview API
-1. `@preview` without params for functions and static methods
-  1.0 `@preview()` for parameters:
-  1.1 Custom name of preview
-  1.2 Parameters for function to be called with (can be evaluated lazily)
-  1.3 Custom group name (use for ease of searching, and maybe for something special later on)
-  1.4 Custom window (Use own PySimpleGUI windows to preview own layouts)
-3. `@method_preview` same as `@preview` but for class methods and properties
-  3.1 Have same parameters as `@preview()`, additionally have optional `instance_provider` parameter to provide `self` for methods
-    3.1.1 `instance_provider` can use cls parameter to create class instance
-    3.1.2 `instance_provider` can have no parameters to provide class instance from some other place
-    3.1.3 `instance_provider` can be omitted, then no-args constructor of class will be used
-4. Multiple previews may be applied to same callable
-5. `@group_previews` can be used to set group_name for multiple previews of same callable
-  5.0 `@group_previews()` name can be set as parameter
-6. In case when preview_name omitted, fully-qualified callable name will be used (`package.module.function_name` or `module.function_name`)
-7. Same goes for `group_previews` no-param form
+1. `@preview` without params for functions and static methods.
+    1. `@preview()` for parameters:
+    2. Custom name of preview.
+    3. Parameters for function to be called with (can be evaluated lazily).
+    4. Custom group name (use for ease of searching, and maybe for something special later on).
+    5. Custom window (Use own PySimpleGUI windows to preview own layouts).
+3. `@method_preview` same as `@preview` but for class methods and properties.
+    1. Have same parameters as `@preview()`, additionally have optional `instance_provider` parameter to provide `self` for methods.
+    2. `instance_provider` can use cls parameter to create class instance.
+    3. `instance_provider` can have no parameters to provide class instance from some other place.
+    4. `instance_provider` can be omitted, then no-args constructor of class will be used.
+4. Multiple previews may be applied to same callable.
+5. `@group_previews` can be used to set group_name for multiple previews of same callable.
+    1. `@group_previews()` name can be set as parameter.
+6. In case when preview_name omitted, fully-qualified callable name will be used (`package.module.function_name` or `module.function_name`).
+7. Same goes for `group_previews` no-param form.
 
 ### PySimplePreview App
-1. Preview Theme can be customised
-2. App remembers its position and size (toggleable)
-3. App stays on top of other windows (toggleable)
-4. Preview window can be separated from main app window
-5. Previews can be filtered by groups
-6. App supports execution params see `python -m PySimplePreview -h`
-7. See app logs for more info (it also contains handled user-defined events from layout previewed)
-8. If you want to see update on any module edited (when layout depends on other module), you may toggle Reload All option
-9. App supports observing single module, package with `__init__.py` file and just flat-layout (folder with `.py` files)
+1. Preview Theme can be customised.
+2. App remembers its position and size (toggleable).
+3. App stays on top of other windows (toggleable).
+4. Preview window can be separated from main app window.
+5. Previews can be filtered by groups.
+6. App supports execution params see `python -m PySimplePreview -h`.
+7. See app logs for more info (it also contains handled user-defined events from layout previewed).
+8. If you want to see update on any module edited (when layout depends on other module), you may toggle Reload All option.
+9. App supports observing single module, package with `__init__.py` file and just flat-layout (folder with `.py` files).
 
 # Docs
-There is no readthedocs page for this project for now (it may be changed soon)
-But public API well-documented in code and covered with typehints (supported by PyCharm)
-All features using can be found in [examples](examples/)
+There is no readthedocs page for this project for now (it may be changed soon).
+But public API well-documented in code and covered with typehints (supported by PyCharm).
+All features using can be found in [examples](examples/).
 
 # Compatability
 ## Python versions support
 For now only Python 3.11 tested, but older versions support planned.
 
 ## PySimpleGUI versions support
 Currently tested on PySimpleGUI 4.60.5, 
-I'll think about adding support for older versions later, better use latest releases anyway :)
+I'll think about adding support for older versions later,
+better use latest releases anyway :)
 
 ## Different PySimpleGUI backends
-Currently tested only with tkinter backend, I have plans for framework-agnostic version.
+Currently tested only with tkinter backend, 
+I have plans for framework-agnostic version.
 
 # Contribution
 Feel free to [open issues](https://github.com/MaxBQb/PySimplePreview/issues/new), but be careful with PR's (small fixes are OK, but this is MVP project, 
 it's implementation can be changed in any way).
 Also note that I may have not enough free time, so have patience.
```

### Comparing `PySimplePreview-0.0.1/src/PySimplePreview.egg-info/SOURCES.txt` & `PySimplePreview-0.0.2/src/PySimplePreview.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE.md
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 src/PySimplePreview/__init__.py
 src/PySimplePreview/__main__.py
 src/PySimplePreview/di.py
 src/PySimplePreview.egg-info/PKG-INFO
 src/PySimplePreview.egg-info/SOURCES.txt
 src/PySimplePreview.egg-info/dependency_links.txt
 src/PySimplePreview.egg-info/entry_points.txt
+src/PySimplePreview.egg-info/requires.txt
 src/PySimplePreview.egg-info/top_level.txt
 src/PySimplePreview/data/__init__.py
 src/PySimplePreview/data/config_storage.py
 src/PySimplePreview/data/di.py
 src/PySimplePreview/data/previews_storage.py
 src/PySimplePreview/domain/__init__.py
 src/PySimplePreview/domain/di.py
```

