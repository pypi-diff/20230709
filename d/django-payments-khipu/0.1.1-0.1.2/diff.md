# Comparing `tmp/django_payments_khipu-0.1.1.tar.gz` & `tmp/django_payments_khipu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_payments_khipu-0.1.1.tar", max compression
+gzip compressed data, was "django_payments_khipu-0.1.2.tar", max compression
```

## Comparing `django_payments_khipu-0.1.1.tar` & `django_payments_khipu-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-07-08 21:14:31.283371 django_payments_khipu-0.1.1/LICENSE
--rw-r--r--   0        0        0     1789 2023-07-08 23:05:22.139338 django_payments_khipu-0.1.1/README.md
--rw-r--r--   0        0        0      675 2023-07-08 22:59:38.481168 django_payments_khipu-0.1.1/django_payments_khipu/KhipuProvider.py
--rw-r--r--   0        0        0       49 2023-07-08 22:59:52.356657 django_payments_khipu-0.1.1/django_payments_khipu/__init__.py
--rw-r--r--   0        0        0     1786 2023-07-08 23:00:00.080378 django_payments_khipu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 django_payments_khipu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-09 20:31:18.029811 django_payments_khipu-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2513 2023-07-09 20:31:18.029811 django_payments_khipu-0.1.2/README.md
+-rw-r--r--   0        0        0     5935 2023-07-09 20:31:18.029811 django_payments_khipu-0.1.2/django_payments_khipu/KhipuProvider.py
+-rw-r--r--   0        0        0       49 2023-07-09 20:31:18.029811 django_payments_khipu-0.1.2/django_payments_khipu/__init__.py
+-rw-r--r--   0        0        0     1997 2023-07-09 20:31:18.029811 django_payments_khipu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3720 1970-01-01 00:00:00.000000 django_payments_khipu-0.1.2/PKG-INFO
```

### Comparing `django_payments_khipu-0.1.1/LICENSE` & `django_payments_khipu-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_payments_khipu-0.1.1/pyproject.toml` & `django_payments_khipu-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-payments-khipu"
-version = "0.1.1"
+version = "0.1.2"
 description = "Soporte Khipu para Django Payments"
 authors = ["Mario Hernandez <mariofix@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_payments_khipu"}]
 repository = "https://github.com/mariofix/django-payments-khipu"
 documentation = "https://mariofix.github.io/django-payments-khipu/"
@@ -13,48 +13,55 @@
     "khipu",
     "pagos",
     "django",
     "payment",
     "django-payments"
 ]
 classifiers=[
-    "Development Status :: 4 - Beta",
+    "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Framework :: Django",
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 pykhipu = "^0.1.9"
 django-payments = "^2.0.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "*"
-black = "*"
-pytest = "*"
-coverage = "*"
-flake8 = "*"
-isort = "*"
-mkdocs = {extras = ["i18n"], version = "*"}
-mkdocs-material = "*"
-mkdocstrings = {extras = ["python"], version = "*"}
-mkdocs-git-authors-plugin = "*"
+pre-commit = "^3.3.3"
+black = "^23.3.0"
+isort = "^5.12.0"
+coverage = "^7.2.7"
+pytest = "^7.4.0"
+flake8 = "^6.0.0"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.18"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-git-revision-date-localized-plugin = "^1.2.0"
+mkdocs-git-committers-plugin-2 = "^1.1.2"
+pillow = "^10.0.0"
+cairosvg = "^2.7.0"
+faker = "^18.13.0"
+lxml = "^4.9.3"
+
 
 [tool.pytest.ini_options]
+DJANGO_SETTINGS_MODULE = "tests.django_settings"
 minversion = "6.0"
 addopts = "-ra"
 testpaths = [
     "tests",
 ]
 python_files =[
     "test*.py"
```

### Comparing `django_payments_khipu-0.1.1/PKG-INFO` & `django_payments_khipu-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-payments-khipu
-Version: 0.1.1
+Version: 0.1.2
 Summary: Soporte Khipu para Django Payments
 Home-page: https://www.khipu.com/page/guia-de-implementacion/
 License: MIT
 Keywords: khipu,pagos,django,payment,django-payments
 Author: Mario Hernandez
 Author-email: mariofix@proton.me
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django-payments (>=2.0.0,<3.0.0)
 Requires-Dist: pykhipu (>=0.1.9,<0.2.0)
 Project-URL: Documentation, https://mariofix.github.io/django-payments-khipu/
 Project-URL: Repository, https://github.com/mariofix/django-payments-khipu
 Description-Content-Type: text/markdown
 
@@ -31,15 +31,24 @@
 `Proyecto en desarrollo activo, no listo para produccion`
 
 `django-payments-khipu` es una variante de Django Payments que implementa la
 creación, confirmación y expiración de pagos realizados a través de Khipu. Este
 módulo proporciona integración con la API de Khipu para facilitar el
 procesamiento y gestión de pagos en tu aplicación web Django.
 
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-khipu/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-khipu/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-khipu/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7dc3c8d6fe844fdaa1de0cb86c242934)](https://app.codacy.com/gh/mariofix/django-payments-khipu/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/mariofix/django-payments-khipu/main.svg)](https://results.pre-commit.ci/latest/github/mariofix/django-payments-khipu/main)
+![PyPI](https://img.shields.io/pypi/v/django-payments-khipu)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-payments-khipu)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/django-payments-khipu)
+![PyPI - License](https://img.shields.io/pypi/l/django-payments-khipu)
+![PyPI - Status](https://img.shields.io/pypi/status/django-payments-khipu)
+
+
 
 ## Introducción
 
 `django-payments-khipu` está diseñado para simplificar la integración de
 pagos de Khipu en tu proyecto Django Payments. Con este módulo, puedes crear y
 gestionar pagos utilizando la pasarela de pago de Khipu de manera sencilla.
 
@@ -72,11 +81,13 @@
     "khipu": ("django_payments_khipu.KhipuProvider", {
         "key": 1,
         "secret": "qwertyasdf0123456789",
     })
 }
 ```
 
+Puedes ver mas opciones de configuracion [en la documentacion](https://mariofix.github.io/django-payments-khipu/uso/#variables-de-configuracion)
+
 ## Licencia
 
 El código está bajo licencia MIT
```

