# Comparing `tmp/load_environ_typed-0.1.1.tar.gz` & `tmp/load_environ_typed-0.2.0.tar.gz`

## Comparing `load_environ_typed-0.1.1.tar` & `load_environ_typed-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/Makefile
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/password.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/test.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/.github/workflows/workflow.yml
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/load_environ_typed/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/load_environ_typed/py.typed
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/README.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 load_environ_typed-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/Makefile
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/WISHLIST.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/password.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/test.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/load_environ_typed/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/load_environ_typed/py.typed
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/README.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 load_environ_typed-0.2.0/PKG-INFO
```

### Comparing `load_environ_typed-0.1.1/.github/workflows/workflow.yml` & `load_environ_typed-0.2.0/.github/workflows/workflow.yml`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,10 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements-dev.txt
-      - name: Typecheck
+      - name: Check
         run: |
-          mypy --strict .
-      - name: Unittest
-        run: |
-          python3 test.py
-      - name: SAST
-        run: |
-          pyflakes test.py
-      - name: Lint
-        run: |
-          pycodestyle test.py
+          make test PYTHON=$(which python3)
```

### Comparing `load_environ_typed-0.1.1/LICENSE.txt` & `load_environ_typed-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `load_environ_typed-0.1.1/pyproject.toml` & `load_environ_typed-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "load-environ-typed"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Johan B.W. de Vries" },
 ]
 description = "You define a class, we load it up from environment in a type safe way"
 readme = "README.md"
 license = {file = "LICENSE.txt" }
 requires-python = ">=3.7"
```

