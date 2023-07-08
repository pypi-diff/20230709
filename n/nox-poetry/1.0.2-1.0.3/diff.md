# Comparing `tmp/nox-poetry-1.0.2.tar.gz` & `tmp/nox_poetry-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nox-poetry-1.0.2.tar", max compression
+gzip compressed data, was "nox_poetry-1.0.3.tar", max compression
```

## Comparing `nox-poetry-1.0.2.tar` & `nox_poetry-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1072 2022-11-08 08:38:15.703550 nox-poetry-1.0.2/LICENSE
--rw-r--r--   0        0        0     7648 2022-11-08 08:38:15.703550 nox-poetry-1.0.2/README.md
--rw-r--r--   0        0        0     1792 2022-11-08 08:38:28.355526 nox-poetry-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1309 2022-11-08 08:38:15.707550 nox-poetry-1.0.2/src/nox_poetry/__init__.py
--rw-r--r--   0        0        0     4475 2022-11-08 08:38:15.707550 nox-poetry-1.0.2/src/nox_poetry/poetry.py
--rw-r--r--   0        0        0        0 2022-11-08 08:38:15.707550 nox-poetry-1.0.2/src/nox_poetry/py.typed
--rw-r--r--   0        0        0    10744 2022-11-08 08:38:15.707550 nox-poetry-1.0.2/src/nox_poetry/sessions.py
--rw-r--r--   0        0        0     1342 2022-11-08 08:38:15.707550 nox-poetry-1.0.2/src/nox_poetry/sessions.pyi
--rw-r--r--   0        0        0     8574 2022-11-08 08:38:30.636229 nox-poetry-1.0.2/setup.py
--rw-r--r--   0        0        0     8574 2022-11-08 08:38:30.636863 nox-poetry-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-08 23:14:46.147585 nox_poetry-1.0.3/LICENSE
+-rw-r--r--   0        0        0     7648 2023-07-08 23:14:46.147585 nox_poetry-1.0.3/README.md
+-rw-r--r--   0        0        0     2073 2023-07-08 23:15:11.471531 nox_poetry-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1309 2023-07-08 23:14:46.151585 nox_poetry-1.0.3/src/nox_poetry/__init__.py
+-rw-r--r--   0        0        0     6162 2023-07-08 23:14:46.151585 nox_poetry-1.0.3/src/nox_poetry/poetry.py
+-rw-r--r--   0        0        0        0 2023-07-08 23:14:46.151585 nox_poetry-1.0.3/src/nox_poetry/py.typed
+-rw-r--r--   0        0        0    10744 2023-07-08 23:14:46.151585 nox_poetry-1.0.3/src/nox_poetry/sessions.py
+-rw-r--r--   0        0        0     1341 2023-07-08 23:14:46.151585 nox_poetry-1.0.3/src/nox_poetry/sessions.pyi
+-rw-r--r--   0        0        0     8625 1970-01-01 00:00:00.000000 nox_poetry-1.0.3/PKG-INFO
```

### Comparing `nox-poetry-1.0.2/LICENSE` & `nox_poetry-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nox-poetry-1.0.2/README.md` & `nox_poetry-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nox-poetry-1.0.2/pyproject.toml` & `nox_poetry-1.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nox-poetry"
-version = "1.0.2"
+version = "1.0.3"
 description = "nox-poetry"
 authors = ["Claudio Jolowicz <mail@claudiojolowicz.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cjolowicz/nox-poetry"
 repository = "https://github.com/cjolowicz/nox-poetry"
 documentation = "https://nox-poetry.readthedocs.io"
@@ -27,32 +27,35 @@
 safety = ">=1.10.3"
 mypy = ">=0.931"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = ">=2.17.0"
-flake8 = ">=4.0.1"
+flake8 = {version = ">=4.0.1", python = ">= 3.8"}
 black = ">=22.3"
-flake8-bandit = ">=2.1.2"
-flake8-bugbear = ">=22.1.11"
-flake8-docstrings = ">=1.6.0"
-flake8-rst-docstrings = ">=0.2.5"
-pep8-naming = ">=0.12.1"
+flake8-bandit = {version = ">=2.1.2", python = ">= 3.8"}
+flake8-bugbear = {version = ">=22.1.11", python = ">= 3.8"}
+flake8-docstrings = {version = ">=1.6.0", python = ">= 3.8"}
+flake8-rst-docstrings = {version = ">=0.2.5", python = ">= 3.8"}
+pep8-naming = {version = ">=0.12.1", python = ">= 3.8"}
 darglint = ">=1.8.1"
 pre-commit-hooks = ">=4.1.0"
 furo = ">=2022.1.2"
 Pygments = ">=2.11.2"
 poetry = ">=1.1.12"
 pytest-datadir = ">=1.3.1"
 typing-extensions = ">=4.0.1"
 pyupgrade = ">=2.31.0"
 isort = ">=5.10.1"
 myst-parser = ">=0.16.1"
 
+[tool.poetry.group.dev.dependencies]
+importlib-metadata = {version = "<6.8", python = "<3.8"}
+
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["nox_poetry"]
```

### Comparing `nox-poetry-1.0.2/src/nox_poetry/__init__.py` & `nox_poetry-1.0.3/src/nox_poetry/__init__.py`

 * *Files identical despite different names*

### Comparing `nox-poetry-1.0.2/src/nox_poetry/poetry.py` & `nox_poetry-1.0.3/src/nox_poetry/poetry.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Poetry interface."""
+import re
 import sys
 from enum import Enum
 from pathlib import Path
 from typing import Any
 from typing import Iterable
 from typing import Iterator
 from typing import List
@@ -45,26 +46,73 @@
         """Return the package extras."""
         extras = self._config.get("extras", {})
         assert isinstance(extras, dict) and all(  # noqa: S101
             isinstance(extra, str) for extra in extras
         )
         return list(extras)
 
+    @property
+    def dependency_groups(self) -> List[str]:
+        """Return the dependency groups."""
+        groups = self._config.get("group", {})
+        if not groups and "dev-dependencies" in self._config:
+            return ["dev"]
+        return list(groups)
+
+
+VERSION_PATTERN = re.compile(r"[0-9]+(\.[0-9+])+[-+.0-9a-zA-Z]+")
+
 
 class Poetry:
     """Helper class for invoking Poetry inside a Nox session.
 
     Attributes:
         session: The Session object.
     """
 
     def __init__(self, session: Session) -> None:
         """Initialize."""
         self.session = session
         self._config: Optional[Config] = None
+        self._version: Optional[str] = None
+
+    @property
+    def version(self) -> str:
+        """Return the Poetry version."""
+        if self._version is not None:
+            return self._version
+
+        output = self.session.run_always(
+            "poetry",
+            "--version",
+            "--no-ansi",
+            external=True,
+            silent=True,
+            stderr=None,
+        )
+        if output is None:
+            raise CommandSkippedError(
+                "The command `poetry --version` was not executed"
+                " (a possible cause is specifying `--no-install`)"
+            )
+
+        assert isinstance(output, str)  # noqa: S101
+
+        match = VERSION_PATTERN.search(output)
+        if match:
+            self._version = match.group()
+            return self._version
+
+        raise RuntimeError("Cannot parse output of `poetry --version`")
+
+    @property
+    def has_dependency_groups(self) -> bool:
+        """Return True if Poetry version supports dependency groups."""
+        version = tuple(int(part) for part in self.version.split(".")[:2])
+        return version >= (1, 2)
 
     @property
     def config(self) -> Config:
         """Return the package configuration."""
         if self._config is None:
             self._config = Config(Path.cwd())
         return self._config
@@ -74,28 +122,34 @@
 
         Returns:
             The generated requirements as text.
 
         Raises:
             CommandSkippedError: The command `poetry export` was not executed.
         """
+        dependency_groups = (
+            [f"--with={group}" for group in self.config.dependency_groups]
+            if self.has_dependency_groups
+            else ["--dev"]
+        )
+
         output = self.session.run_always(
             "poetry",
             "export",
             "--format=requirements.txt",
-            "--dev",
+            *dependency_groups,
             *[f"--extras={extra}" for extra in self.config.extras],
             "--without-hashes",
             external=True,
             silent=True,
             stderr=None,
         )
 
         if output is None:
-            raise CommandSkippedError(
+            raise CommandSkippedError(  # pragma: no cover
                 "The command `poetry export` was not executed"
                 " (a possible cause is specifying `--no-install`)"
             )
 
         assert isinstance(output, str)  # noqa: S101
 
         def _stripwarnings(lines: Iterable[str]) -> Iterator[str]:
```

### Comparing `nox-poetry-1.0.2/src/nox_poetry/sessions.py` & `nox_poetry-1.0.3/src/nox_poetry/sessions.py`

 * *Files identical despite different names*

### Comparing `nox-poetry-1.0.2/src/nox_poetry/sessions.pyi` & `nox_poetry-1.0.3/src/nox_poetry/sessions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from typing import TypeVar
 from typing import Union
 from typing import overload
 
 import nox.sessions
 import nox.virtualenv
 
-
 Python = Optional[Union[str, Sequence[str], bool]]
 
 class _PoetrySession:
     def install(self, *args: str, **kwargs: Any) -> None: ...
     def installroot(
         self, *, distribution_format: str = ..., extras: Iterable[str] = ...
     ) -> None: ...
```

### Comparing `nox-poetry-1.0.2/setup.py` & `nox_poetry-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,215 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nox-poetry
+Version: 1.0.3
+Summary: nox-poetry
+Home-page: https://github.com/cjolowicz/nox-poetry
+License: MIT
+Author: Claudio Jolowicz
+Author-email: mail@claudiojolowicz.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nox (>=2020.8.22)
+Requires-Dist: packaging (>=20.9)
+Requires-Dist: tomlkit (>=0.7)
+Project-URL: Changelog, https://github.com/cjolowicz/nox-poetry/releases
+Project-URL: Documentation, https://nox-poetry.readthedocs.io
+Project-URL: Repository, https://github.com/cjolowicz/nox-poetry
+Description-Content-Type: text/markdown
+
+# nox-poetry
+
+[![PyPI](https://img.shields.io/pypi/v/nox-poetry.svg)][pypi_]
+[![Python Version](https://img.shields.io/pypi/pyversions/nox-poetry)][python version]
+[![License](https://img.shields.io/pypi/l/nox-poetry)][license]
+
+[![Read the documentation at https://nox-poetry.readthedocs.io/](https://img.shields.io/readthedocs/nox-poetry/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/cjolowicz/nox-poetry/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/cjolowicz/nox-poetry/branch/main/graph/badge.svg)][codecov]
+
+[pypi_]: https://pypi.org/project/nox-poetry/
+[python version]: https://pypi.org/project/nox-poetry
+[read the docs]: https://nox-poetry.readthedocs.io/
+[tests]: https://github.com/cjolowicz/nox-poetry/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/cjolowicz/nox-poetry
+
+Use [Poetry] inside [Nox] sessions
+
+This package provides a drop-in replacement for the `nox.session` decorator,
+and for the `nox.Session` object passed to user-defined session functions.
+This enables `session.install` to install packages at the versions specified in the Poetry lock file.
+
+```python
+from nox_poetry import session
+
+@session(python=["3.10", "3.9"])
+def tests(session):
+    session.install("pytest", ".")
+    session.run("pytest")
+```
+
+**Disclaimer:** _This project is not affiliated with Nox, and not an official Nox plugin._
+
+## Installation
+
+Install `nox-poetry` from the Python Package Index:
+
+```console
+$ pip install nox-poetry
+```
+
+**Important:**
+This package must be installed into the same environment that Nox is run from.
+If you installed Nox using [pipx],
+use the following command to install this package into the same environment:
+
+```console
+$ pipx inject nox nox-poetry
+```
+
+## Requirements
+
+- Python 3.7+
+- Poetry >= 1.0.0
+
+You need to have a Poetry installation on your system.
+`nox-poetry` uses Poetry via its command-line interface.
+
+## Usage
+
+Import the `@session` decorator from `nox_poetry` instead of `nox`.
+There is nothing else you need to do.
+The `session.install` method automatically honors the Poetry lock file when installing dependencies.
+This allows you to manage packages used in Nox sessions as development dependencies in Poetry.
+
+This works because session functions are passed instances of `nox_poetry.Session`,
+a proxy for `nox.Session` adding Poetry-related functionality.
+Behind the scenes, nox-poetry uses Poetry to export a [constraints file] and build the package.
+
+For more fine-grained control, additional utilities are available under the `session.poetry` attribute:
+
+- `session.poetry.installroot(distribution_format=["wheel"|"sdist"])`
+- `session.poetry.build_package(distribution_format=["wheel"|"sdist"])`
+- `session.poetry.export_requirements()`
+
+Note that `distribution_format` is a [keyword-only parameter].
+
+Here is a comparison of the different installation methods:
+
+- Use `session.install(...)` to install specific development dependencies, e.g. `session.install("pytest")`.
+- Use `session.install(".")` (or `session.poetry.installroot()`) to install your own package.
+- Use `session.run_always("poetry", "install", external=True)` to install your package with _all_ development dependencies.
+
+Please read the next section for the tradeoffs of each method.
+
+## Why?
+
+Let's look at an example:
+
+```python
+from nox_poetry import session
+
+@session(python=["3.10", "3.9"])
+def tests(session):
+    session.install("pytest", ".")
+    session.run("pytest")
+```
+
+This session performs the following steps:
+
+- Build a wheel from the local package.
+- Install the wheel as well as the `pytest` package.
+- Invoke `pytest` to run the test suite against the installation.
+
+Consider what would happen in this session
+if we had imported `@session` from `nox` instead of `nox_poetry`:
+
+- Package dependencies would only be constrained by the wheel metadata, not by the lock file.
+  In other words, their versions would not be _pinned_.
+- The `pytest` dependency would not be constrained at all.
+- Poetry would be installed as a build backend every time.
+
+Unpinned dependencies mean that your checks are not reproducible and deterministic,
+which can lead to surprises in Continuous Integration and when collaborating with others.
+You can solve these issues by declaring `pytest` as a development dependency,
+and installing your package and its dependencies using `poetry install`:
+
+```python
+@nox.session
+def tests(session: Session) -> None:
+    """Run the test suite."""
+    session.run_always("poetry", "install", external=True)
+    session.run("pytest")
+```
+
+Unfortunately, this approach comes with its own set of problems:
+
+- Checks run against an editable installation of your package,
+  i.e. your local copy of the code, instead of the installed wheel your users see.
+  In the best case, any mistakes will still be caught during Continuous Integration.
+  In the worst case, you publish a buggy release because you forgot to commit some changes.
+- The package is installed, as well as all of its core and development dependencies,
+  no matter which tools a session actually runs.
+  Code formatters or linters, for example, don't need your package installed at all.
+  Besides being wasteful, it goes against the idea of running checks in isolated environments.
+
+`nox-poetry` uses a third approach:
+
+- Installations are performed by pip, via the `session.install` method.
+- When installing your own package, Poetry is used to build a wheel, which is passed to pip.
+- When installing third-party packages, Poetry is used to export a [constraints file],
+  which is passed to pip along with the packages.
+  The constraints file ensures that package versions are pinned by the lock file,
+  without forcing an installation of every listed dependency and sub-dependency.
+
+In summary, this approach brings the following advantages:
+
+- You can manage tools like `pytest` as development dependencies in Poetry.
+- Dependencies are pinned by Poetry's lock file, making checks predictable and deterministic.
+- You can run checks against an installed wheel, instead of your local copy of the code.
+- Every tool can run in an isolated environment with minimal dependencies.
+- No need to install your package with all its dependencies if all you need is some linter.
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_nox-poetry_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[nox]: https://nox.thea.codes/
+[poetry]: https://python-poetry.org/
+[constraints file]: https://pip.pypa.io/en/stable/user_guide/#constraints-files
+[file an issue]: https://github.com/cjolowicz/nox-poetry/issues
+[keyword-only parameter]: https://docs.python.org/3/glossary.html#keyword-only-parameter
+[nox.sessions.session.install]: https://nox.thea.codes/en/stable/config.html#nox.sessions.Session.install
+[nox.sessions.session.run]: https://nox.thea.codes/en/stable/config.html#nox.sessions.Session.run
+[pip install]: https://pip.pypa.io/en/stable/reference/pip_install/
+[pip]: https://pip.pypa.io/
+[pipx]: https://pipxproject.github.io/pipx/
 
-package_dir = \
-{'': 'src'}
+<!-- github-only -->
 
-packages = \
-['nox_poetry']
+[license]: https://github.com/cjolowicz/nox-poetry/blob/main/LICENSE
+[contributor guide]: https://github.com/cjolowicz/nox-poetry/blob/main/CONTRIBUTING.md
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['nox>=2020.8.22', 'packaging>=20.9', 'tomlkit>=0.7']
-
-setup_kwargs = {
-    'name': 'nox-poetry',
-    'version': '1.0.2',
-    'description': 'nox-poetry',
-    'long_description': '# nox-poetry\n\n[![PyPI](https://img.shields.io/pypi/v/nox-poetry.svg)][pypi_]\n[![Python Version](https://img.shields.io/pypi/pyversions/nox-poetry)][python version]\n[![License](https://img.shields.io/pypi/l/nox-poetry)][license]\n\n[![Read the documentation at https://nox-poetry.readthedocs.io/](https://img.shields.io/readthedocs/nox-poetry/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/cjolowicz/nox-poetry/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/cjolowicz/nox-poetry/branch/main/graph/badge.svg)][codecov]\n\n[pypi_]: https://pypi.org/project/nox-poetry/\n[python version]: https://pypi.org/project/nox-poetry\n[read the docs]: https://nox-poetry.readthedocs.io/\n[tests]: https://github.com/cjolowicz/nox-poetry/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/cjolowicz/nox-poetry\n\nUse [Poetry] inside [Nox] sessions\n\nThis package provides a drop-in replacement for the `nox.session` decorator,\nand for the `nox.Session` object passed to user-defined session functions.\nThis enables `session.install` to install packages at the versions specified in the Poetry lock file.\n\n```python\nfrom nox_poetry import session\n\n@session(python=["3.10", "3.9"])\ndef tests(session):\n    session.install("pytest", ".")\n    session.run("pytest")\n```\n\n**Disclaimer:** _This project is not affiliated with Nox, and not an official Nox plugin._\n\n## Installation\n\nInstall `nox-poetry` from the Python Package Index:\n\n```console\n$ pip install nox-poetry\n```\n\n**Important:**\nThis package must be installed into the same environment that Nox is run from.\nIf you installed Nox using [pipx],\nuse the following command to install this package into the same environment:\n\n```console\n$ pipx inject nox nox-poetry\n```\n\n## Requirements\n\n- Python 3.7+\n- Poetry >= 1.0.0\n\nYou need to have a Poetry installation on your system.\n`nox-poetry` uses Poetry via its command-line interface.\n\n## Usage\n\nImport the `@session` decorator from `nox_poetry` instead of `nox`.\nThere is nothing else you need to do.\nThe `session.install` method automatically honors the Poetry lock file when installing dependencies.\nThis allows you to manage packages used in Nox sessions as development dependencies in Poetry.\n\nThis works because session functions are passed instances of `nox_poetry.Session`,\na proxy for `nox.Session` adding Poetry-related functionality.\nBehind the scenes, nox-poetry uses Poetry to export a [constraints file] and build the package.\n\nFor more fine-grained control, additional utilities are available under the `session.poetry` attribute:\n\n- `session.poetry.installroot(distribution_format=["wheel"|"sdist"])`\n- `session.poetry.build_package(distribution_format=["wheel"|"sdist"])`\n- `session.poetry.export_requirements()`\n\nNote that `distribution_format` is a [keyword-only parameter].\n\nHere is a comparison of the different installation methods:\n\n- Use `session.install(...)` to install specific development dependencies, e.g. `session.install("pytest")`.\n- Use `session.install(".")` (or `session.poetry.installroot()`) to install your own package.\n- Use `session.run_always("poetry", "install", external=True)` to install your package with _all_ development dependencies.\n\nPlease read the next section for the tradeoffs of each method.\n\n## Why?\n\nLet\'s look at an example:\n\n```python\nfrom nox_poetry import session\n\n@session(python=["3.10", "3.9"])\ndef tests(session):\n    session.install("pytest", ".")\n    session.run("pytest")\n```\n\nThis session performs the following steps:\n\n- Build a wheel from the local package.\n- Install the wheel as well as the `pytest` package.\n- Invoke `pytest` to run the test suite against the installation.\n\nConsider what would happen in this session\nif we had imported `@session` from `nox` instead of `nox_poetry`:\n\n- Package dependencies would only be constrained by the wheel metadata, not by the lock file.\n  In other words, their versions would not be _pinned_.\n- The `pytest` dependency would not be constrained at all.\n- Poetry would be installed as a build backend every time.\n\nUnpinned dependencies mean that your checks are not reproducible and deterministic,\nwhich can lead to surprises in Continuous Integration and when collaborating with others.\nYou can solve these issues by declaring `pytest` as a development dependency,\nand installing your package and its dependencies using `poetry install`:\n\n```python\n@nox.session\ndef tests(session: Session) -> None:\n    """Run the test suite."""\n    session.run_always("poetry", "install", external=True)\n    session.run("pytest")\n```\n\nUnfortunately, this approach comes with its own set of problems:\n\n- Checks run against an editable installation of your package,\n  i.e. your local copy of the code, instead of the installed wheel your users see.\n  In the best case, any mistakes will still be caught during Continuous Integration.\n  In the worst case, you publish a buggy release because you forgot to commit some changes.\n- The package is installed, as well as all of its core and development dependencies,\n  no matter which tools a session actually runs.\n  Code formatters or linters, for example, don\'t need your package installed at all.\n  Besides being wasteful, it goes against the idea of running checks in isolated environments.\n\n`nox-poetry` uses a third approach:\n\n- Installations are performed by pip, via the `session.install` method.\n- When installing your own package, Poetry is used to build a wheel, which is passed to pip.\n- When installing third-party packages, Poetry is used to export a [constraints file],\n  which is passed to pip along with the packages.\n  The constraints file ensures that package versions are pinned by the lock file,\n  without forcing an installation of every listed dependency and sub-dependency.\n\nIn summary, this approach brings the following advantages:\n\n- You can manage tools like `pytest` as development dependencies in Poetry.\n- Dependencies are pinned by Poetry\'s lock file, making checks predictable and deterministic.\n- You can run checks against an installed wheel, instead of your local copy of the code.\n- Every tool can run in an isolated environment with minimal dependencies.\n- No need to install your package with all its dependencies if all you need is some linter.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_nox-poetry_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[nox]: https://nox.thea.codes/\n[poetry]: https://python-poetry.org/\n[constraints file]: https://pip.pypa.io/en/stable/user_guide/#constraints-files\n[file an issue]: https://github.com/cjolowicz/nox-poetry/issues\n[keyword-only parameter]: https://docs.python.org/3/glossary.html#keyword-only-parameter\n[nox.sessions.session.install]: https://nox.thea.codes/en/stable/config.html#nox.sessions.Session.install\n[nox.sessions.session.run]: https://nox.thea.codes/en/stable/config.html#nox.sessions.Session.run\n[pip install]: https://pip.pypa.io/en/stable/reference/pip_install/\n[pip]: https://pip.pypa.io/\n[pipx]: https://pipxproject.github.io/pipx/\n\n<!-- github-only -->\n\n[license]: https://github.com/cjolowicz/nox-poetry/blob/main/LICENSE\n[contributor guide]: https://github.com/cjolowicz/nox-poetry/blob/main/CONTRIBUTING.md\n',
-    'author': 'Claudio Jolowicz',
-    'author_email': 'mail@claudiojolowicz.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/cjolowicz/nox-poetry',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

