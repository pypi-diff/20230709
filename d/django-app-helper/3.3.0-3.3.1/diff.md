# Comparing `tmp/django-app-helper-3.3.0.tar.gz` & `tmp/django-app-helper-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-app-helper-3.3.0.tar", last modified: Sun May  7 16:48:47 2023, max compression
+gzip compressed data, was "django-app-helper-3.3.1.tar", last modified: Sun Jul  9 17:06:36 2023, max compression
```

## Comparing `django-app-helper-3.3.0.tar` & `django-app-helper-3.3.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14350 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23598 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/default_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.025045 django-app-helper-3.3.0/app_helper/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.025045 django-app-helper-3.3.0/app_helper/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/pytest_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.029045 django-app-helper-3.3.0/app_helper/test_data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/templates/fullwidth.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/test_data/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/app_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/django_app_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14350 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:48:28.000000 django-app-helper-3.3.0/django_app_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 16:48:47.000000 django-app-helper-3.3.0/django_app_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/djangocms_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/djangocms_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    38637 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_others.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/cms_helper_extra_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.033045 django-app-helper-3.3.0/tests/test_utils/custom_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/custom_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/custom_user/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/tests/test_utils/example1/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/cms_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/cms_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/tests/test_utils/example1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:48:47.037045 django-app-helper-3.3.0/tests/test_utils/example2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/example2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/helper_no_cms.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-07 16:47:58.000000 django-app-helper-3.3.0/tests/test_utils/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.191499 django-app-helper-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-07-09 17:06:36.191499 django-app-helper-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.167499 django-app-helper-3.3.1/app_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23598 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/default_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.155499 django-app-helper-3.3.1/app_helper/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.155499 django-app-helper-3.3.1/app_helper/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.171499 django-app-helper-3.3.1/app_helper/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/pytest_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.171499 django-app-helper-3.3.1/app_helper/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/test_data/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.171499 django-app-helper-3.3.1/app_helper/test_data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/test_data/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/test_data/templates/fullwidth.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/test_data/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/app_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.175499 django-app-helper-3.3.1/django_app_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-07-09 17:06:36.000000 django-app-helper-3.3.1/django_app_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-09 17:06:36.000000 django-app-helper-3.3.1/django_app_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:06:36.000000 django-app-helper-3.3.1/django_app_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 17:06:36.000000 django-app-helper-3.3.1/django_app_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:06:22.000000 django-app-helper-3.3.1/django_app_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 17:06:36.000000 django-app-helper-3.3.1/django_app_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 17:06:36.000000 django-app-helper-3.3.1/django_app_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.175499 django-app-helper-3.3.1/djangocms_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/djangocms_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-09 17:06:36.191499 django-app-helper-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.179499 django-app-helper-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38635 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_others.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.183499 django-app-helper-3.3.1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/cms_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/cms_helper_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/cms_helper_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/cms_helper_extra_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.183499 django-app-helper-3.3.1/tests/test_utils/custom_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/custom_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/custom_user/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.187499 django-app-helper-3.3.1/tests/test_utils/example1/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/cms_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/cms_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.191499 django-app-helper-3.3.1/tests/test_utils/example1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:06:36.191499 django-app-helper-3.3.1/tests/test_utils/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/example2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/helper_no_cms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-09 17:05:59.000000 django-app-helper-3.3.1/tests/test_utils/runners.py
```

### Comparing `django-app-helper-3.3.0/CONTRIBUTING.rst` & `django-app-helper-3.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/HISTORY.rst` & `django-app-helper-3.3.1/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+3.3.1 (2023-07-09)
+==================
+
+Bugfixes
+--------
+
+- Fix runner-options argument on Django test runner (#220)
+- Do not add mptt with django-filer 3+ (#225)
+
+
 3.3.0 (2023-05-07)
 ==================
 
 Features
 --------
 
 - Add support for Django 4.x (#208)
```

### Comparing `django-app-helper-3.3.0/LICENSE` & `django-app-helper-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/PKG-INFO` & `django-app-helper-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-app-helper
-Version: 3.3.0
+Version: 3.3.1
 Summary: Helper for django applications development
 Home-page: https://github.com/nephila/django-app-helper
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: GPLv2+
 Project-URL: Documentation, https://django-app-helper.readthedocs.io/
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
@@ -205,14 +205,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+3.3.1 (2023-07-09)
+==================
+
+Bugfixes
+--------
+
+- Fix runner-options argument on Django test runner (#220)
+- Do not add mptt with django-filer 3+ (#225)
+
+
 3.3.0 (2023-05-07)
 ==================
 
 Features
 --------
 
 - Add support for Django 4.x (#208)
```

### Comparing `django-app-helper-3.3.0/README.rst` & `django-app-helper-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/base_test.py` & `django-app-helper-3.3.1/app_helper/base_test.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/default_settings.py` & `django-app-helper-3.3.1/app_helper/default_settings.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/locale/en/LC_MESSAGES/django.po` & `django-app-helper-3.3.1/app_helper/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/main.py` & `django-app-helper-3.3.1/app_helper/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
     TestRunner = get_runner(settings)  # NOQA
 
     kwargs = {"verbosity": verbose, "interactive": False, "failfast": failfast}
     if runner_options:
         if "PytestTestRunner" in test_runner:
             kwargs["pytest_args"] = runner_options
         else:
+            if not isinstance(runner_options, list):
+                runner_options = runner_options.split(" ")
             extra = _parse_runner_options(TestRunner, runner_options)
             extra.update(kwargs)
             kwargs = extra
     test_runner = TestRunner(**kwargs)
     failures = test_runner.run_tests(test_labels)
     return failures
```

### Comparing `django-app-helper-3.3.0/app_helper/pytest_runner.py` & `django-app-helper-3.3.1/app_helper/pytest_runner.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/runner.py` & `django-app-helper-3.3.1/app_helper/runner.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/server.py` & `django-app-helper-3.3.1/app_helper/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         rs.inner_run,
         **{
             "addrport": "{}:{}".format(bind, port),
             "insecure_serving": True,
             "use_static_handler": True,
             "use_threading": True,
             "verbosity": verbose,
+            "skip_checks": True,
             "use_reloader": True,
         },
     )
 
 
 def _setup_db(migrate_cmd):
     """Initialize the database running migrations and creating the default user."""
```

### Comparing `django-app-helper-3.3.0/app_helper/test_data/templates/base.html` & `django-app-helper-3.3.1/app_helper/test_data/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/urls.py` & `django-app-helper-3.3.1/app_helper/urls.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/app_helper/utils.py` & `django-app-helper-3.3.1/app_helper/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,19 @@
         for middleware in middleware_top:
             default_settings["MIDDLEWARE_CLASSES"].insert(0, middleware)
 
     if "cms" in default_settings["INSTALLED_APPS"]:
         if "treebeard" not in default_settings["INSTALLED_APPS"]:
             default_settings["INSTALLED_APPS"].append("treebeard")
     if "filer" in default_settings["INSTALLED_APPS"] and "mptt" not in default_settings["INSTALLED_APPS"]:
-        default_settings["INSTALLED_APPS"].append("mptt")
+        from filer import __version__
+
+        if __version__ < "3":
+            # As of django-filer 3.0 mptt is not needed as a dependency
+            default_settings["INSTALLED_APPS"].append("mptt")
     if "filer" in default_settings["INSTALLED_APPS"] and "easy_thumbnails" not in default_settings["INSTALLED_APPS"]:
         default_settings["INSTALLED_APPS"].append("easy_thumbnails")
 
     default_settings["TEMPLATES"] = [
         {
             "NAME": "django",
             "BACKEND": "django.template.backends.django.DjangoTemplates",
```

### Comparing `django-app-helper-3.3.0/django_app_helper.egg-info/PKG-INFO` & `django-app-helper-3.3.1/django_app_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-app-helper
-Version: 3.3.0
+Version: 3.3.1
 Summary: Helper for django applications development
 Home-page: https://github.com/nephila/django-app-helper
 Author: Iacopo Spalletti
 Author-email: i.spalletti@nephila.digital
 License: GPLv2+
 Project-URL: Documentation, https://django-app-helper.readthedocs.io/
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
@@ -205,14 +205,24 @@
 
 *******
 History
 *******
 
 .. towncrier release notes start
 
+3.3.1 (2023-07-09)
+==================
+
+Bugfixes
+--------
+
+- Fix runner-options argument on Django test runner (#220)
+- Do not add mptt with django-filer 3+ (#225)
+
+
 3.3.0 (2023-05-07)
 ==================
 
 Features
 --------
 
 - Add support for Django 4.x (#208)
```

### Comparing `django-app-helper-3.3.0/django_app_helper.egg-info/SOURCES.txt` & `django-app-helper-3.3.1/django_app_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/pyproject.toml` & `django-app-helper-3.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/setup.cfg` & `django-app-helper-3.3.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.3.0
+current_version = 3.3.1
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.?)(?P<release>[a-z]*)(?P<relver>\d*)
 serialize = 
 	{major}.{minor}.{patch}.{release}{relver}
 	{major}.{minor}.{patch}
 commit = True
 tag = False
 sign_tags = True
```

### Comparing `django-app-helper-3.3.0/tests/test_base_classes.py` & `django-app-helper-3.3.1/tests/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_commands.py` & `django-app-helper-3.3.1/tests/test_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,15 +600,15 @@
                 with self.assertRaises(SystemExit) as exit_state:
                     args = copy(DEFAULT_ARGS)
                     args["test"] = True
                     args["<application>"] = "example1"
                     args["--persistent"] = True
                     args["--runner"] = "runners.CapturedOutputRunner"
                     args["<test-label>"] = self.application
-                    args["--runner-options"] = ["--tag=a-tag"]
+                    args["--runner-options"] = "--tag=a-tag"
                     core(args, self.application)
             self.assertTrue("Ran 1 test in" in err.getvalue())
             self.assertEqual(exit_state.exception.code, 0)
 
     def test_testrun_persistent_path(self):
         """Run test via API using custom runner which only picks tests in sample applications with persistent data."""
         try:
```

### Comparing `django-app-helper-3.3.0/tests/test_others.py` & `django-app-helper-3.3.1/tests/test_others.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_utils/cms_helper.py` & `django-app-helper-3.3.1/tests/test_utils/cms_helper.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_utils/cms_helper_custom.py` & `django-app-helper-3.3.1/tests/test_utils/cms_helper_custom.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_utils/cms_helper_extra.py` & `django-app-helper-3.3.1/tests/test_utils/cms_helper_extra.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_utils/example1/tests/test_fake.py` & `django-app-helper-3.3.1/tests/test_utils/example1/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_utils/helper.py` & `django-app-helper-3.3.1/tests/test_utils/helper.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_utils/helper_no_cms.py` & `django-app-helper-3.3.1/tests/test_utils/helper_no_cms.py`

 * *Files identical despite different names*

### Comparing `django-app-helper-3.3.0/tests/test_utils/runners.py` & `django-app-helper-3.3.1/tests/test_utils/runners.py`

 * *Files identical despite different names*

