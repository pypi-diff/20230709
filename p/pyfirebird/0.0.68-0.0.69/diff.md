# Comparing `tmp/pyfirebird-0.0.68.tar.gz` & `tmp/pyfirebird-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.68.tar", last modified: Sun Jul  9 21:00:52 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.69.tar", last modified: Sun Jul  9 21:08:36 2023, max compression
```

## Comparing `pyfirebird-0.0.68.tar` & `pyfirebird-0.0.69.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.702823 pyfirebird-0.0.68/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 21:00:52.702823 pyfirebird-0.0.68/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.68/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-09 21:00:52.702823 pyfirebird-0.0.68/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1364 2023-07-09 20:57:27.000000 pyfirebird-0.0.68/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.694822 pyfirebird-0.0.68/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.694822 pyfirebird-0.0.68/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      178 2023-07-09 20:16:41.000000 pyfirebird-0.0.68/src/firebird/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.68/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.694822 pyfirebird-0.0.68/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.68/src/firebird/cmd_tools/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2515 2023-07-07 07:05:58.000000 pyfirebird-0.0.68/src/firebird/cmd_tools/executor.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3582 2023-07-09 20:24:42.000000 pyfirebird-0.0.68/src/firebird/cmd_tools/executor_impl.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.68/src/firebird/cmd_tools/fbconsole.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3505 2023-06-28 09:30:24.000000 pyfirebird-0.0.68/src/firebird/cmd_tools/pipeline.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4918 2023-07-09 20:36:40.000000 pyfirebird-0.0.68/src/firebird/cmd_tools/pipeline_impl.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebird/libs/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       37 2023-07-07 05:29:05.000000 pyfirebird-0.0.68/src/firebird/libs/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1633 2023-07-09 07:20:57.000000 pyfirebird-0.0.68/src/firebird/libs/k8.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      448 2023-07-09 05:28:06.000000 pyfirebird-0.0.68/src/firebird/libs/template.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.68/src/firebird/rabbitmq.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.694822 pyfirebird-0.0.68/src/firebird/resources/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebird/resources/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2181 2023-07-09 06:36:53.000000 pyfirebird-0.0.68/src/firebird/resources/templates/pipeline.yaml
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebird/utils/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.68/src/firebird/utils/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.68/src/firebird/utils/checkpoint.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6729 2023-07-09 20:13:34.000000 pyfirebird-0.0.68/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/asgi.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/settings.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/wsgi.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/ui/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/admin.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/apps.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/ui/migrations/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/migrations/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-28 08:49:46.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/models.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.694822 pyfirebird-0.0.68/src/firebirdconsole/ui/static/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/ui/static/images/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/static/images/logo.jpeg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1557431 2023-07-09 21:00:46.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/home.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1675332 2023-07-09 21:00:46.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/pipeline.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/ui/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/templates/application.html
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/templates/index.html
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/ui/templatetags/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/templatetags/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/templatetags/app_filters.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/tests.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      365 2023-07-09 20:56:21.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/view_tools.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.698823 pyfirebird-0.0.68/src/firebirdconsole/ui/views/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/views/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.702823 pyfirebird-0.0.68/src/firebirdconsole/ui/views/apis/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       47 2023-06-28 00:42:11.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/views/apis/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3679 2023-07-09 20:57:05.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/views/apis/main.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/views/home.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.68/src/firebirdconsole/ui/views/pipeline.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:00:52.702823 pyfirebird-0.0.68/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 21:00:52.000000 pyfirebird-0.0.68/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1964 2023-07-09 21:00:52.000000 pyfirebird-0.0.68/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-09 21:00:52.000000 pyfirebird-0.0.68/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-07-09 21:00:52.000000 pyfirebird-0.0.68/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       72 2023-07-09 21:00:52.000000 pyfirebird-0.0.68/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-07-09 21:00:52.000000 pyfirebird-0.0.68/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.69/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1364 2023-07-09 21:08:20.000000 pyfirebird-0.0.69/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      178 2023-07-09 20:16:41.000000 pyfirebird-0.0.69/src/firebird/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.69/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.69/src/firebird/cmd_tools/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2515 2023-07-07 07:05:58.000000 pyfirebird-0.0.69/src/firebird/cmd_tools/executor.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3582 2023-07-09 20:24:42.000000 pyfirebird-0.0.69/src/firebird/cmd_tools/executor_impl.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.69/src/firebird/cmd_tools/fbconsole.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3505 2023-06-28 09:30:24.000000 pyfirebird-0.0.69/src/firebird/cmd_tools/pipeline.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4918 2023-07-09 20:36:40.000000 pyfirebird-0.0.69/src/firebird/cmd_tools/pipeline_impl.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebird/libs/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       37 2023-07-07 05:29:05.000000 pyfirebird-0.0.69/src/firebird/libs/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1633 2023-07-09 07:20:57.000000 pyfirebird-0.0.69/src/firebird/libs/k8.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      448 2023-07-09 05:28:06.000000 pyfirebird-0.0.69/src/firebird/libs/template.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.69/src/firebird/rabbitmq.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.824942 pyfirebird-0.0.69/src/firebird/resources/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebird/resources/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2181 2023-07-09 06:36:53.000000 pyfirebird-0.0.69/src/firebird/resources/templates/pipeline.yaml
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebird/utils/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.69/src/firebird/utils/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.69/src/firebird/utils/checkpoint.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6729 2023-07-09 21:08:13.000000 pyfirebird-0.0.69/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/asgi.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/settings.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/wsgi.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebirdconsole/ui/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/admin.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/apps.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebirdconsole/ui/migrations/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/migrations/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-28 08:49:46.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/models.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.824942 pyfirebird-0.0.69/src/firebirdconsole/ui/static/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.828942 pyfirebird-0.0.69/src/firebirdconsole/ui/static/images/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/static/images/logo.jpeg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1557431 2023-07-09 21:00:46.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/home.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1675332 2023-07-09 21:00:46.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/pipeline.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/src/firebirdconsole/ui/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/templates/application.html
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/templates/index.html
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/src/firebirdconsole/ui/templatetags/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/templatetags/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/templatetags/app_filters.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/tests.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      365 2023-07-09 20:56:21.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/view_tools.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/src/firebirdconsole/ui/views/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/views/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/src/firebirdconsole/ui/views/apis/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       47 2023-06-28 00:42:11.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/views/apis/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3679 2023-07-09 20:57:05.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/views/apis/main.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/views/home.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.69/src/firebirdconsole/ui/views/pipeline.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 21:08:36.832942 pyfirebird-0.0.69/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 21:08:36.000000 pyfirebird-0.0.69/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1964 2023-07-09 21:08:36.000000 pyfirebird-0.0.69/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-09 21:08:36.000000 pyfirebird-0.0.69/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-07-09 21:08:36.000000 pyfirebird-0.0.69/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       72 2023-07-09 21:08:36.000000 pyfirebird-0.0.69/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-07-09 21:08:36.000000 pyfirebird-0.0.69/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.68/setup.py` & `pyfirebird-0.0.69/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.68",
+    version="0.0.69",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.68/src/firebird/base.py` & `pyfirebird-0.0.69/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.69/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/cmd_tools/executor_impl.py` & `pyfirebird-0.0.69/src/firebird/cmd_tools/executor_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/cmd_tools/fbconsole.py` & `pyfirebird-0.0.69/src/firebird/cmd_tools/fbconsole.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.69/src/firebird/cmd_tools/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.69/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/libs/k8.py` & `pyfirebird-0.0.69/src/firebird/libs/k8.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/rabbitmq.py` & `pyfirebird-0.0.69/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/resources/templates/pipeline.yaml` & `pyfirebird-0.0.69/src/firebird/resources/templates/pipeline.yaml`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/utils/checkpoint.py` & `pyfirebird-0.0.69/src/firebird/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebird/zkdb.py` & `pyfirebird-0.0.69/src/firebird/zkdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,27 +88,27 @@
         for pipeline_id in self.zk.get_children("/pipelines"):
             status, pipeline = self.get_pipeline(pipeline_id)
             assert status == ZKError.OK
             assert pipeline is not None
             pipelines.append(pipeline)
         return pipelines
 
-    def get_executor(self, pipeline_id:str, executor_id:str) -> Tuple(ZKError, Any):
+    def get_executor(self, pipeline_id:str, executor_id:str) -> Tuple[ZKError, Any]:
         """
         Get information for an executor
         """
         executor_path = f"/pipelines/{pipeline_id}/executors/{executor_id}"
         if not self.zk.exists(executor_path):
             return ZKError.EXECUTOR_NOT_FOUND, None
         v, _ = self.zk.get(f"{executor_path}/info")
         executor_info = json.loads(v.decode("utf-8"))
         executor_info['id'] = executor_id
         return ZKError.OK, {"info": executor_info}
 
-    def get_pipeline(self, pipeline_id:str) -> Tuple(ZKError, Any):
+    def get_pipeline(self, pipeline_id:str) -> Tuple[ZKError, Any]:
         """
         Get information for a pipeline
         """
         pipeline_path = f"/pipelines/{pipeline_id}"
         if not self.zk.exists(pipeline_path):
             return ZKError.PIPELINE_NOT_REGISTERED, None
```

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/settings.py` & `pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/settings.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/firebirdconsole/urls.py` & `pyfirebird-0.0.69/src/firebirdconsole/firebirdconsole/urls.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/static/images/logo.jpeg` & `pyfirebird-0.0.69/src/firebirdconsole/ui/static/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/home.js` & `pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/home.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/pipeline.js` & `pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/pipeline.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt` & `pyfirebird-0.0.69/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/templates/application.html` & `pyfirebird-0.0.69/src/firebirdconsole/ui/templates/application.html`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/templatetags/app_filters.py` & `pyfirebird-0.0.69/src/firebirdconsole/ui/templatetags/app_filters.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/view_tools.py` & `pyfirebird-0.0.69/src/firebirdconsole/ui/view_tools.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/firebirdconsole/ui/views/apis/main.py` & `pyfirebird-0.0.69/src/firebirdconsole/ui/views/apis/main.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.68/src/pyfirebird.egg-info/SOURCES.txt` & `pyfirebird-0.0.69/src/pyfirebird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

