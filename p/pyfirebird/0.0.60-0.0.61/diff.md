# Comparing `tmp/pyfirebird-0.0.60.tar.gz` & `tmp/pyfirebird-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.60.tar", last modified: Sun Jul  9 05:01:54 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.61.tar", last modified: Sun Jul  9 05:43:43 2023, max compression
```

## Comparing `pyfirebird-0.0.60.tar` & `pyfirebird-0.0.61.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.60/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1364 2023-07-07 07:50:00.000000 pyfirebird-0.0.60/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-06-26 09:30:30.000000 pyfirebird-0.0.60/src/firebird/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.60/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.60/src/firebird/cmd_tools/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2515 2023-07-07 07:05:58.000000 pyfirebird-0.0.60/src/firebird/cmd_tools/executor.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3061 2023-07-07 07:41:30.000000 pyfirebird-0.0.60/src/firebird/cmd_tools/executor_impl.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.60/src/firebird/cmd_tools/fbconsole.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3505 2023-06-28 09:30:24.000000 pyfirebird-0.0.60/src/firebird/cmd_tools/pipeline.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4078 2023-07-07 07:44:15.000000 pyfirebird-0.0.60/src/firebird/cmd_tools/pipeline_impl.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebird/libs/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       37 2023-07-07 05:29:05.000000 pyfirebird-0.0.60/src/firebird/libs/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      447 2023-07-07 05:34:51.000000 pyfirebird-0.0.60/src/firebird/libs/template.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.60/src/firebird/rabbitmq.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.557348 pyfirebird-0.0.60/src/firebird/resources/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebird/resources/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2088 2023-07-07 06:42:18.000000 pyfirebird-0.0.60/src/firebird/resources/templates/pipeline.yaml
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebird/utils/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.60/src/firebird/utils/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.60/src/firebird/utils/checkpoint.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5896 2023-07-07 07:40:43.000000 pyfirebird-0.0.60/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/asgi.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/settings.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/wsgi.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebirdconsole/ui/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/admin.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/apps.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebirdconsole/ui/migrations/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/migrations/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-28 08:49:46.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/models.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebirdconsole/ui/static/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.561348 pyfirebird-0.0.60/src/firebirdconsole/ui/static/images/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/static/images/logo.jpeg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1554034 2023-06-28 09:41:29.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/home.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1671249 2023-07-09 05:01:47.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/pipeline.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/src/firebirdconsole/ui/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/templates/application.html
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/templates/index.html
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/src/firebirdconsole/ui/templatetags/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/templatetags/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/templatetags/app_filters.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/tests.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      372 2023-06-28 00:42:35.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/view_tools.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/src/firebirdconsole/ui/views/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/views/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/src/firebirdconsole/ui/views/apis/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       47 2023-06-28 00:42:11.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/views/apis/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3666 2023-06-28 00:42:19.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/views/apis/main.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/views/home.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.60/src/firebirdconsole/ui/views/pipeline.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:01:54.565348 pyfirebird-0.0.60/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 05:01:54.000000 pyfirebird-0.0.60/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1940 2023-07-09 05:01:54.000000 pyfirebird-0.0.60/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-09 05:01:54.000000 pyfirebird-0.0.60/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-07-09 05:01:54.000000 pyfirebird-0.0.60/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       72 2023-07-09 05:01:54.000000 pyfirebird-0.0.60/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-07-09 05:01:54.000000 pyfirebird-0.0.60/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.61/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1364 2023-07-09 05:43:18.000000 pyfirebird-0.0.61/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-06-26 09:30:30.000000 pyfirebird-0.0.61/src/firebird/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.61/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.61/src/firebird/cmd_tools/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2515 2023-07-07 07:05:58.000000 pyfirebird-0.0.61/src/firebird/cmd_tools/executor.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3061 2023-07-07 07:41:30.000000 pyfirebird-0.0.61/src/firebird/cmd_tools/executor_impl.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.61/src/firebird/cmd_tools/fbconsole.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3505 2023-06-28 09:30:24.000000 pyfirebird-0.0.61/src/firebird/cmd_tools/pipeline.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4095 2023-07-09 05:26:02.000000 pyfirebird-0.0.61/src/firebird/cmd_tools/pipeline_impl.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebird/libs/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       37 2023-07-07 05:29:05.000000 pyfirebird-0.0.61/src/firebird/libs/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      448 2023-07-09 05:28:06.000000 pyfirebird-0.0.61/src/firebird/libs/template.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.61/src/firebird/rabbitmq.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebird/resources/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebird/resources/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2105 2023-07-09 05:31:20.000000 pyfirebird-0.0.61/src/firebird/resources/templates/pipeline.yaml
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebird/utils/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.61/src/firebird/utils/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.61/src/firebird/utils/checkpoint.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5793 2023-07-09 05:43:12.000000 pyfirebird-0.0.61/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/asgi.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/settings.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/wsgi.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/admin.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/apps.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/migrations/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/migrations/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-28 08:49:46.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/models.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.013037 pyfirebird-0.0.61/src/firebirdconsole/ui/static/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/static/images/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/static/images/logo.jpeg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1554034 2023-06-28 09:41:29.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/home.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1671249 2023-07-09 05:01:47.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/pipeline.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/templates/application.html
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/templates/index.html
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/templatetags/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/templatetags/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/templatetags/app_filters.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/tests.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      372 2023-06-28 00:42:35.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/view_tools.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/views/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/views/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/firebirdconsole/ui/views/apis/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       47 2023-06-28 00:42:11.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/views/apis/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3666 2023-06-28 00:42:19.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/views/apis/main.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/views/home.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.61/src/firebirdconsole/ui/views/pipeline.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 05:43:43.017037 pyfirebird-0.0.61/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 05:43:42.000000 pyfirebird-0.0.61/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1940 2023-07-09 05:43:43.000000 pyfirebird-0.0.61/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-09 05:43:42.000000 pyfirebird-0.0.61/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-07-09 05:43:42.000000 pyfirebird-0.0.61/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       72 2023-07-09 05:43:42.000000 pyfirebird-0.0.61/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-07-09 05:43:42.000000 pyfirebird-0.0.61/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.60/setup.py` & `pyfirebird-0.0.61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.60",
+    version="0.0.61",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.60/src/firebird/base.py` & `pyfirebird-0.0.61/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.61/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebird/cmd_tools/executor_impl.py` & `pyfirebird-0.0.61/src/firebird/cmd_tools/executor_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebird/cmd_tools/fbconsole.py` & `pyfirebird-0.0.61/src/firebird/cmd_tools/fbconsole.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.61/src/firebird/cmd_tools/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.61/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import importlib
 from uuid import uuid4
 from firebird.rabbitmq import get_connection, RabbitMQ
 from firebird import zkdb
 import tempfile
 import os
 import jinja2
-from libs import render_template
+from firebird.libs import render_template
 from kubernetes import client,config as k8_config,utils
 
 logger = logging.getLogger(__name__)
 
 def register_command(config:dict, pipeline_namespace_name:str, pipeline_image_name:str, pipeline_module_name:str):
     pipeline = importlib.import_module(pipeline_module_name).get_pipeline(None)
     pipeline_info = pipeline.to_json()
@@ -82,15 +82,15 @@
 
 def start_command(config, pipeline_id, replicas):
     to_apply = ""
     with zkdb(**config['zookeeper']) as db:
         pipeline = db.get_pipeline(pipeline_id)
 
         generator_ids = []
-        for node in pipeline["nodes"]:
+        for node in pipeline["info"]["nodes"]:
             input_port_count = 0
             for port in node["ports"]:
               if port["type"] == "INPUT": # hack, better use PortType enum
                 input_port_count += 1
             if input_port_count == 0:
                 generator_ids.append(node["id"])
```

### Comparing `pyfirebird-0.0.60/src/firebird/rabbitmq.py` & `pyfirebird-0.0.61/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebird/resources/templates/pipeline.yaml` & `pyfirebird-0.0.61/src/firebird/resources/templates/pipeline.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
           - '-gid'
           - '{{generator_id}}'
         volumeMounts:
           - name: checkpoint-{{generator_id}}
             mountPath: /checkpoint
   volumeClaimTemplates:
     - metadata:
-        name: checkpoint
+        name: checkpoint-{{generator_id}}
       spec:
         accessModes: [ "ReadWriteOnce" ]
         resources:
           requests:
             storage: 20Mi
 {% endfor %}
 ---
```

### Comparing `pyfirebird-0.0.60/src/firebird/utils/checkpoint.py` & `pyfirebird-0.0.61/src/firebird/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebird/zkdb.py` & `pyfirebird-0.0.61/src/firebird/zkdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,19 +68,16 @@
         """
         executor_path = f"/pipelines/{pipeline_id}/executors/{executor_id}"
         if not self.zk.exists(executor_path):
             return None
         v, _ = self.zk.get(f"{executor_path}/info")
         executor_info = json.loads(v.decode("utf-8"))
         executor_info['id'] = executor_id
-        v, _ = self.zk.get(f"{executor_path}/stop")
-        stop = v == b'1'
         return {
-            "info": executor_info,
-            "stop": stop
+            "info": executor_info
         }
 
     def get_executor_stop(self, pipeline_id:str, executor_id:str) -> bool:
         """
         Check if stop is requested for an executor
         """
         executor_path = f"/pipelines/{pipeline_id}/executors/{executor_id}"
```

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/settings.py` & `pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/settings.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/firebirdconsole/urls.py` & `pyfirebird-0.0.61/src/firebirdconsole/firebirdconsole/urls.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/static/images/logo.jpeg` & `pyfirebird-0.0.61/src/firebirdconsole/ui/static/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/home.js` & `pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/home.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/pipeline.js` & `pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/pipeline.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt` & `pyfirebird-0.0.61/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/templates/application.html` & `pyfirebird-0.0.61/src/firebirdconsole/ui/templates/application.html`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/templatetags/app_filters.py` & `pyfirebird-0.0.61/src/firebirdconsole/ui/templatetags/app_filters.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/view_tools.py` & `pyfirebird-0.0.61/src/firebirdconsole/ui/view_tools.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/firebirdconsole/ui/views/apis/main.py` & `pyfirebird-0.0.61/src/firebirdconsole/ui/views/apis/main.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.60/src/pyfirebird.egg-info/SOURCES.txt` & `pyfirebird-0.0.61/src/pyfirebird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

