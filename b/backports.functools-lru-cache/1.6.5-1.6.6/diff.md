# Comparing `tmp/backports.functools_lru_cache-1.6.5.tar.gz` & `tmp/backports.functools_lru_cache-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backports.functools_lru_cache-1.6.5.tar", last modified: Sat Jun 24 00:50:52 2023, max compression
+gzip compressed data, was "backports.functools_lru_cache-1.6.6.tar", last modified: Sun Jul  9 20:41:41 2023, max compression
```

## Comparing `backports.functools_lru_cache-1.6.5.tar` & `backports.functools_lru_cache-1.6.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.427822 backports.functools_lru_cache-1.6.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.427822 backports.functools_lru_cache-1.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.427822 backports.functools_lru_cache-1.6.5/backports/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/backports/functools_lru_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 00:50:52.000000 backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:50:52.431822 backports.functools_lru_cache-1.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-24 00:50:29.000000 backports.functools_lru_cache-1.6.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/backports/functools_lru_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-09 20:41:41.000000 backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-09 20:41:41.000000 backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:41:41.000000 backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-09 20:41:41.000000 backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 20:41:41.000000 backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:41.920867 backports.functools_lru_cache-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-09 20:41:20.000000 backports.functools_lru_cache-1.6.6/tox.ini
```

### Comparing `backports.functools_lru_cache-1.6.5/.github/workflows/main.yml` & `backports.functools_lru_cache-1.6.6/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -64,29 +64,29 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
@@ -109,16 +109,16 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `backports.functools_lru_cache-1.6.5/.gitignore` & `backports.functools_lru_cache-1.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `backports.functools_lru_cache-1.6.5/LICENSE` & `backports.functools_lru_cache-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `backports.functools_lru_cache-1.6.5/PKG-INFO` & `backports.functools_lru_cache-1.6.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backports.functools_lru_cache
-Version: 1.6.5
+Version: 1.6.6
 Summary: Backport of functools.lru_cache
 Home-page: https://github.com/jaraco/backports.functools_lru_cache
 Author: Raymond Hettinger
 Author-email: raymond.hettinger@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -62,14 +62,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `backports.functools_lru_cache-1.6.5/README.rst` & `backports.functools_lru_cache-1.6.6/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `backports.functools_lru_cache-1.6.5/backports/functools_lru_cache.py` & `backports.functools_lru_cache-1.6.6/backports/functools_lru_cache.py`

 * *Files identical despite different names*

### Comparing `backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/PKG-INFO` & `backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backports.functools-lru-cache
-Version: 1.6.5
+Version: 1.6.6
 Summary: Backport of functools.lru_cache
 Home-page: https://github.com/jaraco/backports.functools_lru_cache
 Author: Raymond Hettinger
 Author-email: raymond.hettinger@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -62,14 +62,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-backports.functools_lru_cache?utm_source=pypi-backports.functools_lru_cache&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `backports.functools_lru_cache-1.6.5/backports.functools_lru_cache.egg-info/SOURCES.txt` & `backports.functools_lru_cache-1.6.6/backports.functools_lru_cache.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 NEWS.rst
 README.rst
+SECURITY.md
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
 towncrier.toml
 tox.ini
 .github/FUNDING.yml
```

### Comparing `backports.functools_lru_cache-1.6.5/docs/conf.py` & `backports.functools_lru_cache-1.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `backports.functools_lru_cache-1.6.5/pytest.ini` & `backports.functools_lru_cache-1.6.6/pytest.ini`

 * *Files identical despite different names*

### Comparing `backports.functools_lru_cache-1.6.5/setup.cfg` & `backports.functools_lru_cache-1.6.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
```

### Comparing `backports.functools_lru_cache-1.6.5/tox.ini` & `backports.functools_lru_cache-1.6.6/tox.ini`

 * *Files identical despite different names*

