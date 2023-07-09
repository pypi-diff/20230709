# Comparing `tmp/geneweaver_testing-0.0.1a9.tar.gz` & `tmp/geneweaver_testing-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_testing-0.0.1a9.tar", max compression
+gzip compressed data, was "geneweaver_testing-0.0.1b0.tar", max compression
```

## Comparing `geneweaver_testing-0.0.1a9.tar` & `geneweaver_testing-0.0.1b0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1716 2023-03-19 21:28:30.693746 geneweaver_testing-0.0.1a9/README.md
--rw-r--r--   0        0        0      786 2023-03-31 19:31:33.866559 geneweaver_testing-0.0.1a9/pyproject.toml
--rw-r--r--   0        0        0      272 2023-03-26 00:31:18.190850 geneweaver_testing-0.0.1a9/src/geneweaver/testing/__init__.py
--rw-r--r--   0        0        0      129 2023-03-26 00:24:24.566114 geneweaver_testing-0.0.1a9/src/geneweaver/testing/fixtures/__init__.py
--rw-r--r--   0        0        0     2232 2023-03-26 00:33:27.819693 geneweaver_testing-0.0.1a9/src/geneweaver/testing/fixtures/package.py
--rw-r--r--   0        0        0      154 2023-03-26 00:23:47.188317 geneweaver_testing-0.0.1a9/src/geneweaver/testing/package/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-26 00:30:12.634892 geneweaver_testing-0.0.1a9/src/geneweaver/testing/package/can_import.py
--rw-r--r--   0        0        0    10526 2023-03-31 19:30:53.705168 geneweaver_testing-0.0.1a9/src/geneweaver/testing/package/pyproject.py
--rw-r--r--   0        0        0     2012 2023-03-26 00:17:00.859495 geneweaver_testing-0.0.1a9/src/geneweaver/testing/package/structure.py
--rw-r--r--   0        0        0      108 2023-03-30 22:01:30.340056 geneweaver_testing-0.0.1a9/src/geneweaver/testing/style/__init__.py
--rw-r--r--   0        0        0      988 2023-03-26 14:53:08.095511 geneweaver_testing-0.0.1a9/src/geneweaver/testing/style/black.py
--rw-r--r--   0        0        0      754 2023-03-26 00:36:44.526293 geneweaver_testing-0.0.1a9/src/geneweaver/testing/style/ruff.py
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 geneweaver_testing-0.0.1a9/setup.py
--rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 geneweaver_testing-0.0.1a9/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-09 15:15:26.945858 geneweaver_testing-0.0.1b0/LICENSE
+-rw-r--r--   0        0        0     1716 2023-03-19 21:28:30.693746 geneweaver_testing-0.0.1b0/README.md
+-rw-r--r--   0        0        0      786 2023-07-09 15:54:05.709112 geneweaver_testing-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0      272 2023-03-26 00:31:18.190850 geneweaver_testing-0.0.1b0/src/geneweaver/testing/__init__.py
+-rw-r--r--   0        0        0      129 2023-03-26 00:24:24.566114 geneweaver_testing-0.0.1b0/src/geneweaver/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0     2232 2023-03-26 00:33:27.819693 geneweaver_testing-0.0.1b0/src/geneweaver/testing/fixtures/package.py
+-rw-r--r--   0        0        0      177 2023-03-31 22:19:10.723784 geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-26 00:30:12.634892 geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/can_import.py
+-rw-r--r--   0        0        0      152 2023-03-31 22:15:03.300526 geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/generic/__init__.py
+-rw-r--r--   0        0        0    11867 2023-07-09 15:44:22.238863 geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/generic/pyproject.py
+-rw-r--r--   0        0        0     1553 2023-03-31 22:19:10.722082 geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/generic/structure.py
+-rw-r--r--   0        0        0      859 2023-03-31 22:19:13.924373 geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/pyproject.py
+-rw-r--r--   0        0        0     1159 2023-07-09 15:14:47.911876 geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/structure.py
+-rw-r--r--   0        0        0      108 2023-03-30 22:01:30.340056 geneweaver_testing-0.0.1b0/src/geneweaver/testing/style/__init__.py
+-rw-r--r--   0        0        0      988 2023-03-26 14:53:08.095511 geneweaver_testing-0.0.1b0/src/geneweaver/testing/style/black.py
+-rw-r--r--   0        0        0      754 2023-03-26 00:36:44.526293 geneweaver_testing-0.0.1b0/src/geneweaver/testing/style/ruff.py
+-rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 geneweaver_testing-0.0.1b0/PKG-INFO
```

### Comparing `geneweaver_testing-0.0.1a9/README.md` & `geneweaver_testing-0.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_testing-0.0.1a9/pyproject.toml` & `geneweaver_testing-0.0.1b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "geneweaver-testing"
-version = "0.0.1a9"
+version = "0.0.1b0"
 description = "A library to standardize testing of GeneWeaver pacakges."
 authors = ["Alexander Berger <alexander.berger@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://bergsalex.github.io/geneweaver-docs/"
 repository = "https://github.com/bergsalex/geneweaver-testing"
 packages = [
     { include = "geneweaver/testing", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-ruff = "^0.0.254"
-black = "^23.1.0"
+ruff = "^0.0.277"
+black = "^23.3.0"
 isort = "^5.12.0"
-pytest = "^7.2.2"
-mypy = "^1.0.1"
+pytest = "^7.4.0"
+mypy = "^1.4.1"
 tomli = "^2.0.1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 
 [tool.ruff]
 select = ['F', 'E', 'W', 'A', 'C90', 'N', 'B', 'ANN', 'D', 'I', 'ERA', 'PD', 'NPY', 'PT']
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `geneweaver_testing-0.0.1a9/src/geneweaver/testing/fixtures/package.py` & `geneweaver_testing-0.0.1b0/src/geneweaver/testing/fixtures/package.py`

 * *Files identical despite different names*

### Comparing `geneweaver_testing-0.0.1a9/src/geneweaver/testing/package/can_import.py` & `geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/can_import.py`

 * *Files identical despite different names*

### Comparing `geneweaver_testing-0.0.1a9/src/geneweaver/testing/package/pyproject.py` & `geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/generic/pyproject.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""Test that pyproject.toml file is present and has required sections and contents."""
+"""Generic tests that pyproject.toml has required sections and contents."""
 import pathlib
+import warnings
 from typing import Optional
 
 import pytest
 
 __all__ = [
     "test_has_pyproject_toml",
     "test_has_tool_poetry_section",
@@ -13,18 +14,18 @@
     "test_pyproject_has_authors",
     "test_pyproject_has_license",
     "test_pyproject_has_readme",
     "test_poetry_has_packages_definition",
     "test_poetry_has_homepage",
     "test_poetry_has_repository",
     "test_poetry_packages_defined_in_src_dir",
-    "test_poetry_packages_in_geneweaver_namespace",
     "test_pyproject_has_ruff",
     "test_pyproject_ruff_has_required_rules",
     "test_pyproject_ruff_does_not_have_other_specifications",
+    "test_ruff_per_files_ignores",
 ]
 
 POETRY_ERROR_MESSAGE = (
     "see https://python-poetry.org/docs/ for information on getting started with "
     "Python Poetry"
 )
 
@@ -147,40 +148,25 @@
 
 
 def test_poetry_packages_defined_in_src_dir(
     pyproject_toml_contents: Optional[dict],
 ) -> None:
     """Test that the pyproject.toml file has its package defined from src directory."""
     error_msg = (
-        "all Geneweaver packages must be defined in the `src` directory, see "
+        "all packages must be defined in the `src` directory, see "
         "https://python-poetry.org/docs/pyproject/#packages for more information."
     )
     for package in pyproject_toml_contents["tool"]["poetry"]["packages"]:
         assert "from" in package, (
             "pyproject.toml file does not have a `from` definition for a package. "
             f"{error_msg}"
         )
         assert package["from"] == "src", error_msg
 
 
-def test_poetry_packages_in_geneweaver_namespace(
-    pyproject_toml_contents: Optional[dict],
-) -> None:
-    """Test that the pyproject.toml has package defined in the geneweaver namespace."""
-    for package in pyproject_toml_contents["tool"]["poetry"]["packages"]:
-        assert (
-            "include" in package
-        ), "pyproject.toml file does not have an `include` definition for a package."
-        include = package["include"].split("/")
-        assert include[0] == "geneweaver", (
-            "all Geneweaver packages must be located in the `geneweaver` namespace "
-            "package. See https://peps.python.org/pep-0420/ for more information."
-        )
-
-
 def test_poetry_build_system_definition(
     pyproject_toml_contents: Optional[dict],
 ) -> None:
     """Test that the pyproject.toml file has a complete [build-system] section."""
     error_msg = (
         "pyproject.toml file does not have a complete [build-system] section, see"
         "https://python-poetry.org/docs/pyproject/#poetry-and-pep-517 "
@@ -219,15 +205,15 @@
     "ERA": "Eradicate (dead code)",
     "PD": "Pandas Specific Linting",
     "NPY": "NumPy Speficic Linting",
     "PT": "PyTest Style",
 }
 
 RUFF_ERROR_MSG = (
-    "\n\nGeneweaver pyproject.toml `ruff` section should look like: \n"
+    "\n\npyproject.toml `ruff` section should look like: \n"
     "[tool.ruff]\n"
     f"select = {list(REQUIRED_RUFF_RULES.keys())}"
 )
 
 
 @pytest.mark.parametrize("rule", REQUIRED_RUFF_RULES.keys())
 def test_pyproject_ruff_has_required_rules(
@@ -244,14 +230,37 @@
     ) + RUFF_ERROR_MSG
 
     assert rule in pyproject_toml_contents["tool"]["ruff"]["select"], (
         f"pyproject.toml [tool.ruff] select = section missing rule `{rule}`."
     ) + RUFF_ERROR_MSG
 
 
+PER_FILES_IGNORES_MSG = (
+    "pyproject.toml [tool.ruff.per-file-ignores] is only allowed to specify "
+    "tests/*.\nIt should look like: \n\n"
+    '[tool.ruff.per-file-ignores]\n"tests/*" = ["ANN201"]\n\n'
+    "You can optionally ignore argument type annotations (`ANN001`), but it is "
+    "not recommended.\n"
+)
+
+IGNORING_ALLOWED_WARN = (
+    "\n\nGeneweaver allows ignoring argument and return type annotations in "
+    "tests.\nMost tests return nothing, and so it is not necessary to specify "
+    "`-> None` for every test.\n"
+    "It is recommended not to ignore argument type annotations, but is allowed "
+    "at the discretion of the developer.\n\n"
+    "To ignore return type annotations in test, add the following to you "
+    "pyproject.toml file:\n\n"
+    '[tool.ruff.per-file-ignores]\n"tests/*" = ["ANN201"]\n'
+    "To ignore return and argument type annotations in test, add the following "
+    "to you pyproject.toml file:\n\n"
+    '[tool.ruff.per-file-ignores]\n"tests/*" = ["ANN001", "ANN201"]\n'
+)
+
+
 def test_pyproject_ruff_does_not_have_other_specifications(
     pyproject_toml_contents: Optional[dict],
 ) -> None:
     """Test that the pyproject.toml file does not have other specifications."""
     assert "ruff" in pyproject_toml_contents["tool"], (
         "pyproject.toml file does not have a [tool.ruff] section\n"
         "see https://beta.ruff.rs/docs/configuration/ for more information."
@@ -263,10 +272,33 @@
 
     assert len(pyproject_toml_contents["tool"]["ruff"]["select"]) == len(
         REQUIRED_RUFF_RULES.keys()
     ), (
         "pyproject.toml [tool.ruff] select = section has other specifications."
     ) + RUFF_ERROR_MSG
 
-    assert len(pyproject_toml_contents["tool"]["ruff"]) == 1, (
+    ruff_section_length = 1
+
+    # You can optionally ignore argument and return type annotations in tests.
+    per_files_ignores = pyproject_toml_contents["tool"]["ruff"].get("per-file-ignores")
+    if per_files_ignores:
+        ruff_section_length = 2
+
+    assert len(pyproject_toml_contents["tool"]["ruff"]) == ruff_section_length, (
         "pyproject.toml [tool.ruff] section has non-standard specifications."
     ) + RUFF_ERROR_MSG
+
+
+def test_ruff_per_files_ignores(
+    pyproject_toml_contents: Optional[dict],
+) -> None:
+    """Ensure that the ruff configuration only ignores allowed errors."""
+    # You can optionally ignore argument and return type annotations in tests.
+    per_files_ignores = pyproject_toml_contents["tool"]["ruff"].get("per-file-ignores")
+    if per_files_ignores:
+        assert len(per_files_ignores) == 1, PER_FILES_IGNORES_MSG
+        assert "tests/*" in per_files_ignores, PER_FILES_IGNORES_MSG
+        assert len(per_files_ignores["tests/*"]) in (1, 2), PER_FILES_IGNORES_MSG
+        for ignore in per_files_ignores["tests/*"]:
+            assert ignore in ("ANN201", "ANN001"), PER_FILES_IGNORES_MSG
+    else:
+        warnings.warn(IGNORING_ALLOWED_WARN)
```

### Comparing `geneweaver_testing-0.0.1a9/src/geneweaver/testing/package/structure.py` & `geneweaver_testing-0.0.1b0/src/geneweaver/testing/package/generic/structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-"""Test that the package structure is correct."""
+"""Generic tests that the package structure is correct."""
 
 __all__ = [
     "test_has_src_directory",
-    "test_has_geneweaver_directory",
-    "test_geneweaver_dir_is_namespace_package",
-    "test_has_package_directory",
     "test_has_tests_directory",
     "test_has_contributing_file",
+    "test_has_readme_file",
+    "test_has_license_file",
 ]
 
 import pathlib
 
 
 def test_has_src_directory(project_root: pathlib.Path) -> None:
     """Test that the src directory exists."""
     assert (
         project_root / "src"
     ).is_dir(), '"src" directory expected at root of git repository'
 
 
-def test_has_geneweaver_directory(project_root: pathlib.Path) -> None:
-    """Test that the geneweaver namespace exists."""
-    assert (
-        project_root / "src" / "geneweaver"
-    ).is_dir(), '"geneweaver" namespace expected in "src" directory'
-
-
-def test_geneweaver_dir_is_namespace_package(project_root: pathlib.Path) -> None:
-    """Test that the geneweaver namespace is a namespace package."""
-    assert (project_root / "src" / "geneweaver" / "__init__.py").is_file() is False, (
-        '"geneweaver" namespace is not a namespace package, '
-        "it should not have an __init__.py file"
-    )
-
-
-def test_has_package_directory(
-    project_root: pathlib.Path, package_submodule_name: str
-) -> None:
-    """Test that the package directory exists."""
-    assert (project_root / "src" / "geneweaver" / package_submodule_name).is_dir(), (
-        f'"{package_submodule_name}" package directory '
-        f'expected in "geneweaver" namespace'
-    )
-
-
 def test_has_tests_directory(project_root: pathlib.Path) -> None:
     """Test that the tests directory exists."""
     assert (
         project_root / "tests"
     ).is_dir(), '"tests" directory expected at root of git repository'
 
 
 def test_has_contributing_file(project_root: pathlib.Path) -> None:
     """Test that the CONTRIBUTING.md file exists."""
     assert (project_root / "CONTRIBUTING.md").is_file(), (
         "CONTRIBUTING.md file not found, "
         "you may need to create one at the root of your git repository"
     )
+
+
+def test_has_readme_file(project_root: pathlib.Path) -> None:
+    """Test that the README.md file exists."""
+    assert (project_root / "README.md").is_file(), (
+        "README.md file not found, "
+        "you may need to create one at the root of your git repository"
+    )
+
+
+def test_has_license_file(project_root: pathlib.Path) -> None:
+    """Test that the LICENSE file exists."""
+    assert (project_root / "LICENSE").is_file(), (
+        "LICENSE file not found, "
+        "you may need to create one at the root of your git repository"
+    )
```

### Comparing `geneweaver_testing-0.0.1a9/src/geneweaver/testing/style/black.py` & `geneweaver_testing-0.0.1b0/src/geneweaver/testing/style/black.py`

 * *Files identical despite different names*

### Comparing `geneweaver_testing-0.0.1a9/src/geneweaver/testing/style/ruff.py` & `geneweaver_testing-0.0.1b0/src/geneweaver/testing/style/ruff.py`

 * *Files identical despite different names*

### Comparing `geneweaver_testing-0.0.1a9/PKG-INFO` & `geneweaver_testing-0.0.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: geneweaver-testing
-Version: 0.0.1a9
+Version: 0.0.1b0
 Summary: A library to standardize testing of GeneWeaver pacakges.
 Home-page: https://bergsalex.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Alexander Berger
 Author-email: alexander.berger@jax.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=23.1.0,<24.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
-Requires-Dist: mypy (>=1.0.1,<2.0.0)
-Requires-Dist: pytest (>=7.2.2,<8.0.0)
-Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
-Requires-Dist: ruff (>=0.0.254,<0.0.255)
+Requires-Dist: mypy (>=1.4.1,<2.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
+Requires-Dist: ruff (>=0.0.277,<0.0.278)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/bergsalex/geneweaver-testing
 Description-Content-Type: text/markdown
 
 # Geneweaver Testing
 This package is used to test the Geneweaver project. It contains tools for running tests against Geneweaver project
 packages and components to aid in the development of Geneweaver.
```

