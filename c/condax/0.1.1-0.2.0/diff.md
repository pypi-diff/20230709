# Comparing `tmp/condax-0.1.1.tar.gz` & `tmp/condax-0.2.0.tar.gz`

## Comparing `condax-0.1.1.tar` & `condax-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 condax-0.1.1/.coveragerc
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 condax-0.1.1/.flake8
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 condax-0.1.1/.gitattributes
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 condax-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 condax-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 condax-0.1.1/mkdocs.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 condax-0.1.1/pytest.ini
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 condax-0.1.1/tox.ini
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 condax-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 condax-0.1.1/.github/renovate.json
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 condax-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 condax-0.1.1/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 condax-0.1.1/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 condax-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 condax-0.1.1/.github/workflows/requirements-docs.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 condax-0.1.1/ci/requirements.txt
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 condax-0.1.1/condax/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 condax-0.1.1/condax/activation.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 condax-0.1.1/condax/cli.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 condax-0.1.1/condax/conda.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 condax-0.1.1/condax/config.py
--rw-r--r--   0        0        0    10410 2020-02-02 00:00:00.000000 condax-0.1.1/condax/core.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 condax-0.1.1/condax/metadata.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 condax-0.1.1/condax/paths.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 condax-0.1.1/docs/changelog.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 condax-0.1.1/docs/cli.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 condax-0.1.1/docs/config.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 condax-0.1.1/docs/contributing.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 condax-0.1.1/docs/how-this-works.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 condax-0.1.1/docs/index.md
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 condax-0.1.1/docs/installation.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 condax-0.1.1/news/TEMPLATE.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 condax-0.1.1/news/link-conflict.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 condax-0.1.1/news/specific-version.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 condax-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 condax-0.1.1/tests/test_condax.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 condax-0.1.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 condax-0.1.1/LICENSE-MIT
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 condax-0.1.1/README.md
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 condax-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 condax-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 condax-0.2.0/.coveragerc
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 condax-0.2.0/.flake8
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 condax-0.2.0/.gitattributes
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 condax-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 condax-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 condax-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 condax-0.2.0/pytest.ini
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 condax-0.2.0/tox.ini
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 condax-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 condax-0.2.0/.github/renovate.json
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/pythonpackage.yml
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 condax-0.2.0/.github/workflows/requirements-docs.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 condax-0.2.0/ci/requirements.txt
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 condax-0.2.0/condax/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 condax-0.2.0/condax/activation.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 condax-0.2.0/condax/cli.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 condax-0.2.0/condax/conda.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 condax-0.2.0/condax/config.py
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 condax-0.2.0/condax/core.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 condax-0.2.0/condax/metadata.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 condax-0.2.0/condax/paths.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 condax-0.2.0/docs/changelog.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 condax-0.2.0/docs/cli.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 condax-0.2.0/docs/config.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 condax-0.2.0/docs/contributing.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 condax-0.2.0/docs/how-this-works.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 condax-0.2.0/docs/index.md
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 condax-0.2.0/docs/installation.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 condax-0.2.0/news/TEMPLATE.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 condax-0.2.0/news/link-conflict.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 condax-0.2.0/news/specific-version.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 condax-0.2.0/news/upgrade-pydantic.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 condax-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 condax-0.2.0/tests/test_condax.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 condax-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 condax-0.2.0/LICENSE-MIT
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 condax-0.2.0/README.md
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 condax-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 condax-0.2.0/PKG-INFO
```

### Comparing `condax-0.1.1/CONTRIBUTING.md` & `condax-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/mkdocs.yml` & `condax-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/.github/workflows/docs.yml` & `condax-0.2.0/.github/workflows/docs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   build:
     name: Deploy docs
     runs-on: ubuntu-latest
     steps:
       - name: Checkout master
         uses: actions/checkout@v3
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - run: pip install mkdocs mkdocs-material mkdocs-typer
       - run: pip install .
       - run: mkdocs gh-deploy --force
       # - name: Deploy docs
       #   uses: mhausenblas/mkdocs-deploy-gh-pages@master
```

### Comparing `condax-0.1.1/.github/workflows/pythonpackage.yml` & `condax-0.2.0/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/.github/workflows/release.yml` & `condax-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/condax/cli.py` & `condax-0.2.0/condax/cli.py`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/condax/conda.py` & `condax-0.2.0/condax/conda.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,43 +116,38 @@
 def package_name(package_spec: str):
     """Get the package name from a package spec"""
     m = _RE_PKG_NAME.match(package_spec)
     assert m is not None
     return m.group(0)
 
 
-def detemine_executables_from_env(
+def determine_executables_from_env(
     package: str, env_prefix: Optional[Path] = None
 ) -> Set[Path]:
     if env_prefix is None:
         env_prefix = conda_env_prefix(package)
     name = package_name(package)
     metas = (env_prefix / "conda-meta").glob(f"{name}*.json")
     for path in metas:
         package_info = json.loads(path.read_text())
         if package_info["name"] == name:
             logging.debug("Candidate files: %s", package_info["files"])
-            potential_executables: List[str] = [
-                fn
-                for fn in package_info["files"]
-                if (
-                    fn.startswith("bin/")
-                    or fn.startswith("sbin/")
-                    # They are Windows style path
-                    or (
-                        is_windows()
-                        and (
-                            fn.lower().startswith("scripts\\")
-                            or fn.lower().startswith("library\\mingw-w64\\bin\\")
-                            or re.match(r"library\\.*\\bin\\", fn.lower())
-                        )
-                    )
-                )
-            ]
-            # TODO: Handle windows style paths
+            potential_executables: List[str] = []
+            for fn in package_info["files"]:
+                if is_windows():
+                    processed_fn = fn.lower().replace("\\", "/")
+                    if (
+                        processed_fn.startswith("scripts/")
+                        or processed_fn.startswith("library/mingw-w64/bin/")
+                        or re.match(r"library/.*/bin/", processed_fn)
+                    ):
+                        potential_executables.append(fn)
+                else:
+                    if fn.startswith("bin/") or fn.startswith("sbin/"):
+                        potential_executables.append(fn)
             break
     else:
         raise ValueError("Could not determine package files")
 
     pathext = os.environ.get("PATHEXT", "").split(";")
     executables: Set[Path] = set()
     for fn in potential_executables:
```

### Comparing `condax-0.1.1/condax/config.py` & `condax-0.2.0/condax/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import os
 import platform
 import warnings
 from pathlib import Path
-from typing import TYPE_CHECKING, Generator, Optional
+from typing import TYPE_CHECKING, Generator, List, Optional
 
 import yaml
-from pydantic import BaseSettings, Field
+from pydantic import ConfigDict, Field
 
 with warnings.catch_warnings():
     # requests which is a transitive dependency has some chatty warnings during import
     warnings.simplefilter("ignore", Warning)
     import requests  # noqa: F401
 
 from ensureconda.api import ensureconda
+from pydantic_settings import BaseSettings
 
 if TYPE_CHECKING:
     from _typeshed import StrPath
 
 
 def is_windows() -> bool:
     return platform.system() == "Windows"
 
 
 class Config(BaseSettings):
     prefix_path: Path = Path("~").expanduser() / ".condax"
     link_destination: Path = Path("~").expanduser() / ".local" / "bin"
-    channels = ["conda-forge", "defaults"]
+    channels: List[str] = ["conda-forge", "defaults"]
     conda_executable: Optional[Path] = Field(
         default=ensureconda(
             mamba=True, micromamba=True, conda=True, conda_exe=True, no_install=True
         )
     )
-
-    class Config:
-        env_prefix = "CONDAX_"
+    model_config = ConfigDict(env_prefix="CONDAX_")
 
     def ensure_conda_executable(self, require_mamba: bool = True):
         def candidates() -> "Generator[Optional[StrPath], None, None]":
             yield ensureconda(
                 mamba=True,
                 micromamba=True,
                 conda=False,
```

### Comparing `condax-0.1.1/condax/core.py` & `condax-0.2.0/condax/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 import os
 import pathlib
 import subprocess
 import sys
 from enum import Enum
 from pathlib import Path
-from typing import Any, Collection, Dict, Generator, List, Optional
+from typing import Collection, Dict, Generator, List, Optional
 
 import typer
 
 from . import conda
 from .config import CONFIG, is_windows
 from .metadata import PrefixMetadata
 
@@ -126,25 +126,20 @@
         )
 
 
 @contextlib.contextmanager
 def prefix_metadata(env_prefix: Path) -> Generator[PrefixMetadata, None, None]:
     metadata_path = env_prefix / ".condax-metadata.json"
     if metadata_path.exists():
-        ret = PrefixMetadata.parse_file(metadata_path)
+        ret = PrefixMetadata.model_validate_json(metadata_path.read_text())
     else:
         ret = PrefixMetadata(prefix=env_prefix)
     yield ret
 
-    def encoder(obj: Any) -> "str | Any":
-        if isinstance(obj, Path):
-            return str(obj)
-        return obj
-
-    metadata_path.write_text(ret.json(indent=2, exclude_unset=True, encoder=encoder))
+    metadata_path.write_text(ret.model_dump_json(indent=2, exclude_unset=True))
 
 
 def remove_links(executables_to_unlink: Collection[Path], env_prefix: Path) -> None:
     removed_links: Dict[Path, Path] = {}
 
     for exe in executables_to_unlink:
         link = link_path(exe)
@@ -174,15 +169,15 @@
     package: str,
     channels: Optional[List[str]] = None,
     link_conflict_action=LinkConflictAction.ERROR,
 ) -> None:
     if channels is None:
         channels = CONFIG.channels
     conda.create_conda_environment(package, channels=channels)
-    executables_to_link = conda.detemine_executables_from_env(package)
+    executables_to_link = conda.determine_executables_from_env(package)
     CONFIG.link_destination.mkdir(parents=True, exist_ok=True)
     create_links(
         executables_to_link,
         link_conflict_action,
         env_prefix=conda.conda_env_prefix(package),
     )
     typer.secho(
@@ -200,15 +195,15 @@
     if channels is None:
         channels = CONFIG.channels
 
     prefix = conda.conda_env_prefix(package)
     conda.install_conda_packages(extra_packages, channels=channels, prefix=prefix)
     if include_apps:
         for extra_package in extra_packages:
-            executables_to_link = conda.detemine_executables_from_env(
+            executables_to_link = conda.determine_executables_from_env(
                 extra_package, env_prefix=prefix
             )
             CONFIG.link_destination.mkdir(parents=True, exist_ok=True)
             create_links(executables_to_link, link_conflict_action, env_prefix=prefix)
     with prefix_metadata(prefix) as metadata:
         metadata.injected_packages = list(
             sorted(set(metadata.injected_packages) | set(extra_packages))
@@ -232,15 +227,15 @@
             f"`{package}` is not installed with condax", err=True, fg=typer.colors.RED
         )
         sys.exit(0)
 
 
 def remove_package(package) -> None:
     exit_if_not_installed(package)
-    executables_to_unlink = conda.detemine_executables_from_env(package)
+    executables_to_unlink = conda.determine_executables_from_env(package)
     prefix = conda.conda_env_prefix(package)
     remove_links(executables_to_unlink, env_prefix=prefix)
     with prefix_metadata(prefix) as metadata:
         additional_removals = metadata.links.keys()
     remove_links(additional_removals, env_prefix=prefix)
 
     conda.remove_conda_env(package)
@@ -264,24 +259,24 @@
     exit_if_not_installed(package)
     env_prefix = conda.conda_env_prefix(package)
     with prefix_metadata(env_prefix) as metadata:
         executables_already_linked = set(metadata.links.keys())
         injected = metadata.injected_packages
         injected_with_apps = metadata.injected_packages_with_apps
     try:
-        executables_already_linked |= set(conda.detemine_executables_from_env(package))
+        executables_already_linked |= set(conda.determine_executables_from_env(package))
 
         conda.update_conda_env(package)
         env_prefix = conda.conda_env_prefix(package)
         executables_linked_in_updated = set(
-            conda.detemine_executables_from_env(package)
+            conda.determine_executables_from_env(package)
         )
         for p in injected_with_apps:
             executables_linked_in_updated |= set(
-                conda.detemine_executables_from_env(p, env_prefix=env_prefix)
+                conda.determine_executables_from_env(p, env_prefix=env_prefix)
             )
 
         to_create = executables_linked_in_updated - executables_already_linked
         to_delete = executables_already_linked - executables_linked_in_updated
 
         remove_links(to_delete, env_prefix=env_prefix)
         create_links(to_create, link_conflict_action, env_prefix=env_prefix)
```

### Comparing `condax-0.1.1/condax/metadata.py` & `condax-0.2.0/condax/metadata.py`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/condax/paths.py` & `condax-0.2.0/condax/paths.py`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/docs/contributing.md` & `condax-0.2.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/docs/index.md` & `condax-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/docs/installation.md` & `condax-0.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/tests/test_condax.py` & `condax-0.2.0/tests/test_condax.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,13 +39,13 @@
     print("Files:", files)
 
     post_install = which("jq", path=os.environ["PATH"])
     assert post_install is not None
     assert post_install.startswith(conf["link"])
 
     # ensure that the executable installed is on PATH
-    subprocess.check_call(["jq", "--help"])
+    subprocess.check_call(["jq", "--help"], shell=True)
 
     # remove the env
     remove_package("jq")
     post_remove = which("jq", path=os.environ["PATH"])
     assert (post_remove is None) or (not post_remove.startswith(conf["link"]))
```

### Comparing `condax-0.1.1/LICENSE-MIT` & `condax-0.2.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/README.md` & `condax-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `condax-0.1.1/pyproject.toml` & `condax-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 dependencies = [
 	"click",
 	"requests",
 	"userpath",
 	"PyYAML",
 	"ensureconda",
 	"typer",
-	"pydantic",
+	"pydantic >=2",
+	"pydantic-settings",
 	'importlib_metadata; python_version < "3.8.0"',
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = 'https://github.com/mariusvniekerk/condax'
 Documentation = 'https://mariusvniekerk.github.io/condax/'
```

### Comparing `condax-0.1.1/PKG-INFO` & `condax-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: condax
-Version: 0.1.1
+Version: 0.2.0
 Summary: Install and run applications packaged with conda in isolated environments
 Project-URL: Homepage, https://github.com/mariusvniekerk/condax
 Project-URL: Documentation, https://mariusvniekerk.github.io/condax/
 Author-email: Marius van Niekerk <marius.v.niekerk@gmail.com>
+License-Expression: MIT
 License-File: LICENSE-MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Installation/Setup
 Requires-Python: >=3.7
 Requires-Dist: click
 Requires-Dist: ensureconda
 Requires-Dist: importlib-metadata; python_version < '3.8.0'
-Requires-Dist: pydantic
+Requires-Dist: pydantic-settings
+Requires-Dist: pydantic>=2
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: typer
 Requires-Dist: userpath
 Description-Content-Type: text/markdown
 
 # condax
```

