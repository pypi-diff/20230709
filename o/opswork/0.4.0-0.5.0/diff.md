# Comparing `tmp/opswork-0.4.0.tar.gz` & `tmp/opswork-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opswork-0.4.0.tar", last modified: Fri Jul  7 23:43:38 2023, max compression
+gzip compressed data, was "opswork-0.5.0.tar", last modified: Sun Jul  9 21:56:27 2023, max compression
```

## Comparing `opswork-0.4.0.tar` & `opswork-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.070668 opswork-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.050668 opswork-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.050668 opswork-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.050668 opswork-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-07 23:43:17.000000 opswork-0.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 23:43:17.000000 opswork-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 23:43:17.000000 opswork-0.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 23:43:17.000000 opswork-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-07 23:43:17.000000 opswork-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-07 23:43:17.000000 opswork-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 23:43:17.000000 opswork-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 23:43:17.000000 opswork-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-07 23:43:38.070668 opswork-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-07 23:43:17.000000 opswork-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 23:43:17.000000 opswork-0.4.0/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 23:43:17.000000 opswork-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.042668 opswork-0.4.0/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 23:43:17.000000 opswork-0.4.0/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 23:43:17.000000 opswork-0.4.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-07 23:43:38.070668 opswork-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-07 23:43:17.000000 opswork-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.042668 opswork-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.054668 opswork-0.4.0/src/opswork/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.062668 opswork-0.4.0/src/opswork/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/command/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.062668 opswork-0.4.0/src/opswork/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.062668 opswork-0.4.0/src/opswork/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.066668 opswork-0.4.0/src/opswork/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-07 23:43:17.000000 opswork-0.4.0/src/opswork/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.058668 opswork-0.4.0/src/opswork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:43:37.000000 opswork-0.4.0/src/opswork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 23:43:38.000000 opswork-0.4.0/src/opswork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.070668 opswork-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 23:43:17.000000 opswork-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:38.070668 opswork-0.4.0/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:43:17.000000 opswork-0.4.0/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-07 23:43:17.000000 opswork-0.4.0/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-07 23:43:17.000000 opswork-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 21:56:07.000000 opswork-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-09 21:56:07.000000 opswork-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-09 21:56:07.000000 opswork-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-09 21:56:07.000000 opswork-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-09 21:56:07.000000 opswork-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-09 21:56:07.000000 opswork-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-09 21:56:07.000000 opswork-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-09 21:56:07.000000 opswork-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-09 21:56:27.888142 opswork-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-09 21:56:07.000000 opswork-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 21:56:07.000000 opswork-0.5.0/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-09 21:56:07.000000 opswork-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.880142 opswork-0.5.0/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-09 21:56:07.000000 opswork-0.5.0/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 21:56:07.000000 opswork-0.5.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-09 21:56:27.892142 opswork-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-09 21:56:07.000000 opswork-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.884142 opswork-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/command/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-09 21:56:07.000000 opswork-0.5.0/src/opswork/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/src/opswork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 21:56:27.000000 opswork-0.5.0/src/opswork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 21:56:07.000000 opswork-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:27.888142 opswork-0.5.0/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 21:56:07.000000 opswork-0.5.0/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-09 21:56:07.000000 opswork-0.5.0/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-09 21:56:07.000000 opswork-0.5.0/tox.ini
```

### Comparing `opswork-0.4.0/.github/workflows/release.yml` & `opswork-0.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/.gitignore` & `opswork-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/CODE_OF_CONDUCT.md` & `opswork-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/CONTRIBUTING.rst` & `opswork-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/LICENSE.txt` & `opswork-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/Makefile` & `opswork-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/PKG-INFO` & `opswork-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.4.0
+Version: 0.5.0
 Summary: OpsWork Swiss Knife.
 Home-page: https://github.com/Clivern/OpsWork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/Clivern/OpsWork/
 Project-URL: Source, https://github.com/Clivern/OpsWork/
```

### Comparing `opswork-0.4.0/README.rst` & `opswork-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/recipe/motd/recipe.yml` & `opswork-0.5.0/recipe/motd/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/recipe/nginx/recipe.yml` & `opswork-0.5.0/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/recipe/ping/recipe.yml` & `opswork-0.5.0/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/setup.cfg` & `opswork-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/setup.py` & `opswork-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/__init__.py` & `opswork-0.5.0/src/opswork/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/cli.py` & `opswork-0.5.0/src/opswork/cli.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/command/__init__.py` & `opswork-0.5.0/src/opswork/command/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/command/configs.py` & `opswork-0.5.0/src/opswork/command/configs.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/command/hosts.py` & `opswork-0.5.0/src/opswork/command/hosts.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,43 +23,64 @@
 import click
 import subprocess
 
 from opswork.model.host import Host
 from opswork.module.logger import Logger
 from opswork.module.output import Output
 from opswork.module.config import Config
+from opswork.module.encrypt import Encrypt
 from opswork.module.database import Database
 from opswork.module.file_system import FileSystem
 
 
 class Hosts:
     """Hosts Class"""
 
     def __init__(self):
         self.output = Output()
         self.database = Database()
         self.config = Config()
+        self.encrypt = Encrypt()
         self.file_system = FileSystem()
         self.logger = Logger().get_logger(__name__)
 
     def init(self):
         """Init database and configs"""
-        self._configs = self.config.load()
-        self.database.connect(self._configs["database"]["path"])
+        self.configs = self.config.load()
+        self.database.connect(self.configs["database"]["path"])
         self.database.migrate()
+
         return self
 
     def add(self, host, force):
         """Add a new host"""
         if force:
             self.database.delete_host(host.name)
 
         if self.database.get_host(host.name) is not None:
             raise click.ClickException(f"Host with name {host.name} exists")
 
+        # Encrypt the user
+        if host.user != "":
+            host.user = self.encrypt.encrypt(
+                self.configs["database"]["token"], host.user
+            )
+
+        # Encrypt the password
+        if host.password != "":
+            host.password = self.encrypt.encrypt(
+                self.configs["database"]["token"], host.password
+            )
+
+        # Encrypt the private key
+        if host.ssh_private_key != "":
+            host.ssh_private_key = self.encrypt.encrypt(
+                self.configs["database"]["token"], host.ssh_private_key
+            )
+
         self.database.insert_host(host)
 
         click.echo(f"Host with name {host.name} got created")
 
     def list(self, tag, output):
         """List hosts"""
         data = []
@@ -123,19 +144,37 @@
             raise click.ClickException(f"Host with name {name} not found")
 
         if host.ssh_private_key == "":
             raise click.ClickException(
                 f"SSH feature is only for hosts with private keys"
             )
 
-        tmp_path = self._configs["cache"]["path"]
+        tmp_path = self.configs["cache"]["path"]
 
         if self.file_system.file_exists(f"{tmp_path}/{host.id}.pem"):
             self.file_system.delete_file(f"{tmp_path}/{host.id}.pem")
 
+        # Decrypt the ssh key
+        if host.ssh_private_key != "":
+            host.ssh_private_key = self.encrypt.decrypt(
+                self.configs["database"]["token"], host.ssh_private_key
+            )
+
+        # Decrypt the password
+        if host.password != "":
+            host.password = self.encrypt.decrypt(
+                self.configs["database"]["token"], host.password
+            )
+
+        # Decrypt the username
+        if host.user != "":
+            host.user = self.encrypt.decrypt(
+                self.configs["database"]["token"], host.user
+            )
+
         self.file_system.write_file(
             f"{tmp_path}/{host.id}.pem",
             host.ssh_private_key,
         )
 
         self.file_system.change_permission(f"{tmp_path}/{host.id}.pem", 0o400)
```

### Comparing `opswork-0.4.0/src/opswork/command/random.py` & `opswork-0.5.0/src/opswork/command/random.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/command/recipes.py` & `opswork-0.5.0/src/opswork/command/recipes.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,33 +24,35 @@
 import yaml
 import click
 
 from opswork.model.recipe import Recipe
 from opswork.module.logger import Logger
 from opswork.module.output import Output
 from opswork.module.config import Config
+from opswork.module.encrypt import Encrypt
 from opswork.module.database import Database
 from opswork.module.playbook import Playbook
 from opswork.module.file_system import FileSystem
 
 
 class Recipes:
     """Recipes Class"""
 
     def __init__(self):
         self.output = Output()
-        self.database = Database()
         self.config = Config()
+        self.encrypt = Encrypt()
+        self.database = Database()
         self.file_system = FileSystem()
         self.logger = Logger().get_logger(__name__)
 
     def init(self):
         """Init database and configs"""
-        self._configs = self.config.load()
-        self.database.connect(self._configs["database"]["path"])
+        self.configs = self.config.load()
+        self.database.connect(self.configs["database"]["path"])
         self.database.migrate()
         return self
 
     def add(self, name, configs, force):
         """Add a Recipe"""
         recipe = ""
         templates = []
@@ -159,21 +161,59 @@
         if host_name != "":
             host = self.database.get_host(host_name)
 
             if host is None:
                 raise click.ClickException(f"Host with name {name} not found")
 
             found = host.id
+
+            # Decrypt the ssh key
+            if host.ssh_private_key != "":
+                host.ssh_private_key = self.encrypt.decrypt(
+                    self.configs["database"]["token"], host.ssh_private_key
+                )
+
+            # Decrypt the password
+            if host.password != "":
+                host.password = self.encrypt.decrypt(
+                    self.configs["database"]["token"], host.password
+                )
+
+            # Decrypt the username
+            if host.user != "":
+                host.user = self.encrypt.decrypt(
+                    self.configs["database"]["token"], host.user
+                )
+
             hosts.append(host)
 
         if tag != "":
             items = self.database.list_hosts()
             for item in items:
                 if tag not in item.tags or found == item.id:
                     continue
+
+                # Decrypt the ssh key
+                if item.ssh_private_key != "":
+                    item.ssh_private_key = self.encrypt.decrypt(
+                        self.configs["database"]["token"], item.ssh_private_key
+                    )
+
+                # Decrypt the password
+                if item.password != "":
+                    item.password = self.encrypt.decrypt(
+                        self.configs["database"]["token"], item.password
+                    )
+
+                # Decrypt the username
+                if item.user != "":
+                    item.user = self.encrypt.decrypt(
+                        self.configs["database"]["token"], item.user
+                    )
+
                 hosts.append(item)
 
         if len(hosts) == 0:
             raise click.ClickException(f"No hosts matching!")
 
         var_override = {}
 
@@ -181,15 +221,15 @@
             if "=" not in item:
                 continue
             data = item.split("=")
             var_override[data[0]] = data[1]
 
         playbook = Playbook(
             str(uuid.uuid4()),
-            self._configs["cache"]["path"].rstrip("/"),
+            self.configs["cache"]["path"].rstrip("/"),
             hosts,
             recipe,
             var_override,
         )
 
         playbook.build()
         playbook.run()
```

### Comparing `opswork-0.4.0/src/opswork/command/secret.py` & `opswork-0.5.0/src/opswork/command/secret.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/exception/__init__.py` & `opswork-0.5.0/src/opswork/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/model/__init__.py` & `opswork-0.5.0/src/opswork/model/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/model/host.py` & `opswork-0.5.0/src/opswork/model/host.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,14 +92,29 @@
         return self._ssh_private_key
 
     @property
     def tags(self):
         """Host Tags"""
         return self._tags
 
+    @user.setter
+    def user(self, user):
+        """Set User"""
+        self._user = user
+
+    @password.setter
+    def password(self, password):
+        """Set Password"""
+        self._password = password
+
+    @ssh_private_key.setter
+    def ssh_private_key(self, ssh_private_key):
+        """Set SSH Private Key"""
+        self._ssh_private_key = ssh_private_key
+
     @property
     def created_at(self):
         """Host Created At"""
         return self._created_at
 
     @property
     def updated_at(self):
```

### Comparing `opswork-0.4.0/src/opswork/model/recipe.py` & `opswork-0.5.0/src/opswork/model/recipe.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/model/secret.py` & `opswork-0.5.0/src/opswork/model/secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,20 +57,21 @@
         return self._value
 
     @property
     def tags(self):
         """Secret Tags"""
         return self._tags
 
+    @value.setter
+    def value(self, value):
+        """Set Value"""
+        self._value = value
+
     @property
     def created_at(self):
         """Secret Created At"""
         return self._created_at
 
     @property
     def updated_at(self):
         """Secret Updated At"""
         return self._updated_at
-
-    @value.setter
-    def value(self, value):
-        self._value = value
```

### Comparing `opswork-0.4.0/src/opswork/model/task.py` & `opswork-0.5.0/src/opswork/model/task.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/__init__.py` & `opswork-0.5.0/src/opswork/module/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/config.py` & `opswork-0.5.0/src/opswork/module/config.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/database.py` & `opswork-0.5.0/src/opswork/module/database.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/encrypt.py` & `opswork-0.5.0/src/opswork/module/encrypt.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/file_system.py` & `opswork-0.5.0/src/opswork/module/file_system.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/logger.py` & `opswork-0.5.0/src/opswork/module/logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/output.py` & `opswork-0.5.0/src/opswork/module/output.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork/module/playbook.py` & `opswork-0.5.0/src/opswork/module/playbook.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/src/opswork.egg-info/PKG-INFO` & `opswork-0.5.0/src/opswork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opswork
-Version: 0.4.0
+Version: 0.5.0
 Summary: OpsWork Swiss Knife.
 Home-page: https://github.com/Clivern/OpsWork/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/Clivern/OpsWork/
 Project-URL: Source, https://github.com/Clivern/OpsWork/
```

### Comparing `opswork-0.4.0/src/opswork.egg-info/SOURCES.txt` & `opswork-0.5.0/src/opswork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/tests/__init__.py` & `opswork-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/tests/module/test_logger.py` & `opswork-0.5.0/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `opswork-0.4.0/tox.ini` & `opswork-0.5.0/tox.ini`

 * *Files identical despite different names*

