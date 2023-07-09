# Comparing `tmp/condax-0.2.0.tar.gz` & `tmp/condax-0.2.1.tar.gz`

## Comparing `condax-0.2.0.tar` & `condax-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 condax-0.2.0/.coveragerc
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 condax-0.2.0/.flake8
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 condax-0.2.0/.gitattributes
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 condax-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 condax-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 condax-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 condax-0.2.0/pytest.ini
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 condax-0.2.0/tox.ini
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 condax-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 condax-0.2.0/.github/renovate.json
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/requirements-docs.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 condax-0.2.0/ci/requirements.txt
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 condax-0.2.0/condax/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 condax-0.2.0/condax/activation.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 condax-0.2.0/condax/cli.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 condax-0.2.0/condax/conda.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 condax-0.2.0/condax/config.py
--rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 condax-0.2.0/condax/core.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 condax-0.2.0/condax/metadata.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 condax-0.2.0/condax/paths.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 condax-0.2.0/docs/changelog.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 condax-0.2.0/docs/cli.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 condax-0.2.0/docs/config.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 condax-0.2.0/docs/contributing.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 condax-0.2.0/docs/how-this-works.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 condax-0.2.0/docs/index.md
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 condax-0.2.0/docs/installation.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 condax-0.2.0/news/TEMPLATE.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 condax-0.2.0/news/link-conflict.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 condax-0.2.0/news/specific-version.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 condax-0.2.0/news/upgrade-pydantic.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 condax-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 condax-0.2.0/tests/test_condax.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 condax-0.2.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 condax-0.2.0/LICENSE-MIT
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 condax-0.2.0/README.md
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 condax-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 condax-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 condax-0.2.1/.coveragerc
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 condax-0.2.1/.flake8
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 condax-0.2.1/.gitattributes
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 condax-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 condax-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 condax-0.2.1/mkdocs.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 condax-0.2.1/pytest.ini
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 condax-0.2.1/tox.ini
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 condax-0.2.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 condax-0.2.1/.github/renovate.json
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 condax-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 condax-0.2.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 condax-0.2.1/.github/workflows/pythonpackage.yml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 condax-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 condax-0.2.1/.github/workflows/requirements-docs.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 condax-0.2.1/ci/requirements.txt
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 condax-0.2.1/condax/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 condax-0.2.1/condax/activation.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 condax-0.2.1/condax/cli.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 condax-0.2.1/condax/conda.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 condax-0.2.1/condax/config.py
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 condax-0.2.1/condax/core.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 condax-0.2.1/condax/metadata.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 condax-0.2.1/condax/paths.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 condax-0.2.1/docs/changelog.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 condax-0.2.1/docs/cli.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 condax-0.2.1/docs/config.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 condax-0.2.1/docs/contributing.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 condax-0.2.1/docs/how-this-works.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 condax-0.2.1/docs/index.md
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 condax-0.2.1/docs/installation.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 condax-0.2.1/news/TEMPLATE.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 condax-0.2.1/news/link-conflict.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 condax-0.2.1/news/specific-version.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 condax-0.2.1/news/upgrade-pydantic.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 condax-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 condax-0.2.1/tests/test_condax.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 condax-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 condax-0.2.1/LICENSE-MIT
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 condax-0.2.1/README.md
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 condax-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 condax-0.2.1/PKG-INFO
```

### Comparing `condax-0.2.0/CONTRIBUTING.md` & `condax-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/mkdocs.yml` & `condax-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/.github/workflows/docs.yml` & `condax-0.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/.github/workflows/pythonpackage.yml` & `condax-0.2.1/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/.github/workflows/release.yml` & `condax-0.2.1/.github/workflows/release.yml`

 * *Files 3% similar despite different names*

```diff
@@ -27,12 +27,12 @@
           python -m build
       - name: Check files
         run: |
           ls dist
         shell: bash
 
       - name: Publish a Python distribution to PyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_PASSWORD }}
-        if: ${{ github.event_name == 'release' }}
+        if: ${{ github.event_name == 'release' }}
```

### Comparing `condax-0.2.0/condax/cli.py` & `condax-0.2.1/condax/cli.py`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/condax/conda.py` & `condax-0.2.1/condax/conda.py`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/condax/config.py` & `condax-0.2.1/condax/config.py`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/condax/core.py` & `condax-0.2.1/condax/core.py`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/condax/metadata.py` & `condax-0.2.1/condax/metadata.py`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/condax/paths.py` & `condax-0.2.1/condax/paths.py`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/docs/contributing.md` & `condax-0.2.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/docs/index.md` & `condax-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/docs/installation.md` & `condax-0.2.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/tests/test_condax.py` & `condax-0.2.1/tests/test_condax.py`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/LICENSE-MIT` & `condax-0.2.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/README.md` & `condax-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/pyproject.toml` & `condax-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `condax-0.2.0/PKG-INFO` & `condax-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condax
-Version: 0.2.0
+Version: 0.2.1
 Summary: Install and run applications packaged with conda in isolated environments
 Project-URL: Homepage, https://github.com/mariusvniekerk/condax
 Project-URL: Documentation, https://mariusvniekerk.github.io/condax/
 Author-email: Marius van Niekerk <marius.v.niekerk@gmail.com>
 License-Expression: MIT
 License-File: LICENSE-MIT
 Classifier: Development Status :: 4 - Beta
```

