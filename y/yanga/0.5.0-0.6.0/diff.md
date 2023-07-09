# Comparing `tmp/yanga-0.5.0.tar.gz` & `tmp/yanga-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanga-0.5.0.tar", max compression
+gzip compressed data, was "yanga-0.6.0.tar", max compression
```

## Comparing `yanga-0.5.0.tar` & `yanga-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1066 2023-07-05 20:19:43.532355 yanga-0.5.0/LICENSE
--rw-r--r--   0        0        0     4695 2023-07-05 20:19:43.532355 yanga-0.5.0/README.md
--rw-r--r--   0        0        0     2384 2023-07-05 20:19:44.296362 yanga-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-05 20:19:44.264362 yanga-0.5.0/src/yanga/__init__.py
--rw-r--r--   0        0        0      347 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/_yrun.py
--rw-r--r--   0        0        0        0 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/__init__.py
--rw-r--r--   0        0        0     1810 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/build.py
--rw-r--r--   0        0        0     2500 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/init.py
--rw-r--r--   0        0        0     1364 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/install.py
--rw-r--r--   0        0        0      412 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/project-template/cookiecutter.json
--rw-r--r--   0        0        0       13 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
--rw-r--r--   0        0        0     5389 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1
--rw-r--r--   0        0        0     3853 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
--rw-r--r--   0        0        0      785 2023-07-05 20:19:43.532355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
--rw-r--r--   0        0        0       34 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
--rw-r--r--   0        0        0      247 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
--rw-r--r--   0        0        0      219 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/scoopfile.json
--rw-r--r--   0        0        0      397 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/stages/my_stage.py
--rw-r--r--   0        0        0      176 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
--rw-r--r--   0        0        0        0 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/core/__init__.py
--rw-r--r--   0        0        0     4335 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/core/docs_utils.py
--rw-r--r--   0        0        0      278 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/core/exceptions.py
--rw-r--r--   0        0        0     1583 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/core/logging.py
--rw-r--r--   0        0        0     6618 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/core/scoop_wrapper.py
--rw-r--r--   0        0        0     1343 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/core/subprocess.py
--rw-r--r--   0        0        0        0 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/py.typed
--rw-r--r--   0        0        0        0 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/__init__.py
--rw-r--r--   0        0        0      917 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/build_main.py
--rw-r--r--   0        0        0      965 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/config.py
--rw-r--r--   0        0        0      477 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/environment.py
--rw-r--r--   0        0        0     4666 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/pipeline.py
--rw-r--r--   0        0        0      864 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/project.py
--rw-r--r--   0        0        0      920 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/stages.py
--rw-r--r--   0        0        0      886 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ybuild/variant.py
--rw-r--r--   0        0        0     1070 2023-07-05 20:19:43.536355 yanga-0.5.0/src/yanga/ymain.py
--rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-09 11:19:43.317508 yanga-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4695 2023-07-09 11:19:43.317508 yanga-0.6.0/README.md
+-rw-r--r--   0        0        0     2384 2023-07-09 11:19:44.093508 yanga-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-09 11:19:44.065508 yanga-0.6.0/src/yanga/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/_yrun.py
+-rw-r--r--   0        0        0        0 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/__init__.py
+-rw-r--r--   0        0        0     1810 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/build.py
+-rw-r--r--   0        0        0     2500 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/init.py
+-rw-r--r--   0        0        0     1364 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/install.py
+-rw-r--r--   0        0        0      412 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/cookiecutter.json
+-rw-r--r--   0        0        0       13 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
+-rw-r--r--   0        0        0     5389 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1
+-rw-r--r--   0        0        0    11054 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
+-rw-r--r--   0        0        0      785 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
+-rw-r--r--   0        0        0       34 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
+-rw-r--r--   0        0        0      247 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/scoopfile.json
+-rw-r--r--   0        0        0      469 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/stages/my_stage.py
+-rw-r--r--   0        0        0      176 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
+-rw-r--r--   0        0        0        0 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/core/__init__.py
+-rw-r--r--   0        0        0     4335 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/docs_utils.py
+-rw-r--r--   0        0        0      278 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/exceptions.py
+-rw-r--r--   0        0        0     1583 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/logging.py
+-rw-r--r--   0        0        0     3430 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/runnable.py
+-rw-r--r--   0        0        0     8971 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     1351 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/subprocess.py
+-rw-r--r--   0        0        0        0 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/py.typed
+-rw-r--r--   0        0        0        0 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/build_main.py
+-rw-r--r--   0        0        0      965 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/config.py
+-rw-r--r--   0        0        0      477 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/environment.py
+-rw-r--r--   0        0        0     4116 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/pipeline.py
+-rw-r--r--   0        0        0      864 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/project.py
+-rw-r--r--   0        0        0     1003 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/stages.py
+-rw-r--r--   0        0        0      886 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/variant.py
+-rw-r--r--   0        0        0     1070 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ymain.py
+-rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.6.0/PKG-INFO
```

### Comparing `yanga-0.5.0/LICENSE` & `yanga-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/README.md` & `yanga-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/pyproject.toml` & `yanga-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yanga"
-version = "0.5.0"
+version = "0.6.0"
 description = "Yet another ninja generator to build C/CPP projects."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/yanga"
 documentation = "https://yanga.readthedocs.io"
 classifiers = [
```

### Comparing `yanga-0.5.0/src/yanga/commands/build.py` & `yanga-0.6.0/src/yanga/commands/build.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/commands/init.py` & `yanga-0.6.0/src/yanga/commands/init.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/commands/install.py` & `yanga-0.6.0/src/yanga/commands/install.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1` & `yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1` & `yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/core/cmd_line.py` & `yanga-0.6.0/src/yanga/core/cmd_line.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/core/docs_utils.py` & `yanga-0.6.0/src/yanga/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/core/logging.py` & `yanga-0.6.0/src/yanga/core/logging.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/core/scoop_wrapper.py` & `yanga-0.6.0/src/yanga/core/scoop_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import re
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from dataclasses import dataclass, field
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, List, Optional, Union
 
 from mashumaro import DataClassDictMixin
 from mashumaro.mixins.json import DataClassJSONMixin
@@ -45,33 +46,44 @@
 
     def to_file(self, scoop_file: Path) -> None:
         with open(scoop_file, "w") as f:
             json.dump(self.to_dict(), f, indent=4)
 
 
 @dataclass
-class InstalledScoopApp:
+class InstalledApp:
+    #: App name
     name: str
+    #: App version
     version: str
+    #: App root directory
     path: Path
-    manifest_file: Path
+    #: List of bin directories relative to the app path
     bin_dirs: List[Path]
 
 
+@dataclass
+class InstalledScoopApp(InstalledApp):
+    #: App scoop manifest file
+    manifest_file: Path
+
+
 class ScoopWrapper:
     def __init__(self) -> None:
         self.scoop_executable = self._find_scoop_executable()
         self.scoop_root_dir = self._find_scoop_root_dir(self.scoop_executable)
         self.logger = logger.bind()
 
     @property
     def apps_directory(self) -> Path:
         return self.scoop_root_dir.joinpath("apps")
 
-    def install(self, scoop_file: Path) -> List[ScoopFileElement]:
+    def install(self, scoop_file: Path) -> List[InstalledScoopApp]:
+        """Install scoop apps from a scoop file.
+        It returns a list with all apps required to be installed as installed apps."""
         return self.do_install(
             ScoopInstallConfigFile.from_file(scoop_file), self.get_installed_apps()
         )
 
     def _find_scoop_executable(self) -> Path:
         scoop_path = which("scoop")
         if not scoop_path:
@@ -98,78 +110,127 @@
 
         def get_parent_dir(bin_entry: Union[str, List[str]]) -> Optional[Path]:
             bin_path = (
                 Path(bin_entry[0]) if isinstance(bin_entry, list) else Path(bin_entry)
             )
             return bin_path.parent if len(bin_path.parts) > 1 else None
 
+        result = []
         if isinstance(bin_data, str):
-            return [parent for parent in [get_parent_dir(bin_data)] if parent]
+            result = [parent for parent in [get_parent_dir(bin_data)] if parent]
         elif isinstance(bin_data, list):
-            return [
+            result = [
                 parent
                 for parent in [get_parent_dir(bin_entry) for bin_entry in bin_data]
                 if parent
             ]
-        return []
+        return list(set(result))
+
+    def parse_manifest_file(self, manifest_file: Path) -> InstalledScoopApp:
+        app_directory: Path = manifest_file.parent
+        tool_name: str = app_directory.parent.name
+        with open(manifest_file) as f:
+            manifest_data: Dict[str, Any] = json.load(f)
+            tool_version: str = manifest_data.get("version", None)
+            bin_dirs: List[Path] = self.parse_bin_dirs(manifest_data.get("bin", []))
+            return InstalledScoopApp(
+                name=tool_name,
+                version=tool_version,
+                path=app_directory,
+                manifest_file=manifest_file,
+                bin_dirs=bin_dirs,
+            )
 
     def get_installed_apps(self) -> List[InstalledScoopApp]:
         installed_tools: List[InstalledScoopApp] = []
         self.logger.info(f"Looking for installed apps in {self.apps_directory}")
-        for manifest_file in self.apps_directory.glob("**/manifest.json"):
-            app_directory: Path = manifest_file.parent
-            # There is a directory level for the version of the tool
-            tool_name: str = app_directory.parent.name
-            with open(manifest_file) as f:
-                manifest_data: Dict[str, Any] = json.load(f)
-                tool_version: str = manifest_data.get("version", None)
-                bin_dirs: List[Path] = self.parse_bin_dirs(manifest_data.get("bin", []))
-                installed_tools.append(
-                    InstalledScoopApp(
-                        name=tool_name,
-                        version=tool_version,
-                        path=app_directory,
-                        manifest_file=manifest_file,
-                        bin_dirs=bin_dirs,
-                    )
-                )
+        manifest_files = list(self.apps_directory.glob("*/*/manifest.json"))
+
+        with ThreadPoolExecutor() as executor:
+            future_to_file = {
+                executor.submit(self.parse_manifest_file, manifest_file): manifest_file
+                for manifest_file in manifest_files
+            }
+            for future in as_completed(future_to_file):
+                installed_tools.append(future.result())
+
         return installed_tools
 
     def do_install(
         self,
         scoop_install_config: ScoopInstallConfigFile,
         installed_apps: List[InstalledScoopApp],
+    ) -> List[InstalledScoopApp]:
+        """Install scoop apps from a scoop file."""
+
+        newly_installed_apps = self.do_install_missing(
+            scoop_install_config, installed_apps
+        )
+        # If some apps where just installed we need to update the list of installed apps
+        if newly_installed_apps:
+            self.logger.info(
+                "New apps were installed, update the list of installed apps."
+            )
+            updated_installed_apps = self.get_installed_apps()
+        else:
+            updated_installed_apps = installed_apps
+        apps = self.map_required_apps_to_installed_apps(
+            scoop_install_config.app_names, updated_installed_apps
+        )
+        return apps
+
+    def do_install_missing(
+        self,
+        scoop_install_config: ScoopInstallConfigFile,
+        installed_apps: List[InstalledScoopApp],
     ) -> List[ScoopFileElement]:
         """Check which apps are installed and install the missing ones."""
         apps_to_install = self.get_tools_to_be_installed(
             scoop_install_config, installed_apps
         )
         if not apps_to_install:
             self.logger.info("All Scoop apps already installed. Skip installation.")
             return []
         already_installed_apps = set(scoop_install_config.apps) - set(apps_to_install)
+        if already_installed_apps:
+            self.logger.info(
+                f"Scoop apps already installed: {','.join(str(app) for app in already_installed_apps)}"
+            )
         self.logger.info(
-            f"Scoop apps already installed: {','.join(str(app) for app in already_installed_apps)}"
-        )
-        self.logger.info(
-            f"Scoop apps to install: {','.join(str(app) for app in apps_to_install)}"
+            f"Start installing missing apps: {','.join(str(app) for app in apps_to_install)}"
         )
 
         # Create a temporary scoopfile with the remaining apps to install and install them
         with TemporaryDirectory() as tmp_dir:
             tmp_scoop_file = Path(tmp_dir).joinpath("scoopfile.json")
             ScoopInstallConfigFile(
                 scoop_install_config.buckets, apps_to_install
             ).to_file(tmp_scoop_file)
             SubprocessExecutor(
                 [self.scoop_executable, "import", tmp_scoop_file]
             ).execute()
         return apps_to_install
 
     @staticmethod
+    def map_required_apps_to_installed_apps(
+        app_names: List[str],
+        installed_apps: List[InstalledScoopApp],
+    ) -> List[InstalledScoopApp]:
+        """Map the required apps to the installed apps."""
+        # convert the list of installed apps into a dictionary for faster lookup
+        installed_apps_dict = {app.name: app for app in installed_apps}
+        try:
+            apps = [installed_apps_dict[app_name] for app_name in app_names]
+        except KeyError as e:
+            raise UserNotificationException(
+                f"Could not find {e} in the installed apps. Something went wrong during the scoop installation."
+            )
+        return apps
+
+    @staticmethod
     def get_tools_to_be_installed(
         scoop_install_config: ScoopInstallConfigFile,
         installed_tools: List[InstalledScoopApp],
     ) -> List[ScoopFileElement]:
         """Check which apps are installed and install the missing ones."""
         installed_tools_names = {tool.name for tool in installed_tools}
         return [
```

### Comparing `yanga-0.5.0/src/yanga/core/subprocess.py` & `yanga-0.6.0/src/yanga/core/subprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.current_working_directory = cwd
 
     def execute(self) -> None:
         result = None
         try:
             logger.info(f"Running command: {self.command}")
             result = subprocess.run(
-                self.command,
+                self.command.split(),
                 cwd=(self.current_working_directory or Path.cwd()).as_posix(),
                 capture_output=True,
                 text=True,  # to get stdout and stderr as strings instead of bytes
             )  # nosec
             result.check_returncode()
         except subprocess.CalledProcessError as e:
             err_message = result.stderr if result else e
```

### Comparing `yanga-0.5.0/src/yanga/ybuild/build_main.py` & `yanga-0.6.0/src/yanga/ybuild/build_main.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/ybuild/config.py` & `yanga-0.6.0/src/yanga/ybuild/config.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/ybuild/pipeline.py` & `yanga-0.6.0/src/yanga/ybuild/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-from abc import ABC, abstractmethod
+from abc import ABC
 from dataclasses import dataclass
 from importlib import import_module
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 from typing import List, Type
 
 from yanga.core.exceptions import UserNotificationException
+from yanga.core.runnable import Executor, Runnable
 from yanga.ybuild.config import PipelineConfig, StageConfig
 from yanga.ybuild.environment import BuildEnvironment
 
 
-class Stage(ABC):
+class Stage(Runnable, ABC):
     def __init__(self, environment: BuildEnvironment, group_name: str) -> None:
         self.environment = environment
         self.output_dir = self.environment.artifacts_locator.build_dir / group_name
 
-    @abstractmethod
-    def run(self) -> None:
-        """Run stage"""
-
-    @abstractmethod
-    def get_dependencies(self) -> List[Path]:
-        """Get stage dependencies"""
-
-    @abstractmethod
-    def get_outputs(self) -> List[Path]:
-        """Get stage outputs"""
-
 
 @dataclass
 class BuildStage:
     group_name: str
     _class: Type[Stage]
 
 
@@ -107,15 +96,8 @@
 
     def __init__(self, environment: BuildEnvironment, stage: BuildStage) -> None:
         self.environment = environment
         self.stage = stage
 
     def run(self) -> None:
         stage = self.stage._class(self.environment, self.stage.group_name)
-        if self._must_run(stage):
-            stage.run()
-
-    def _must_run(self, stage: Stage) -> bool:
-        """A stage shall run if any of the dependencies changed or one of the outputs is missing.
-        All dependencies and outputs relevant information is stored in the stage output directory
-        in a <stage>.deps file."""
-        return True
+        Executor(stage.output_dir).execute(stage)
```

### Comparing `yanga-0.5.0/src/yanga/ybuild/project.py` & `yanga-0.6.0/src/yanga/ybuild/project.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/ybuild/stages.py` & `yanga-0.6.0/src/yanga/ybuild/stages.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 
 
 class YangaScoopInstall(Stage):
     def __init__(self, environment: BuildEnvironment, group_name: str) -> None:
         super().__init__(environment, group_name)
         self.logger = logger.bind()
 
+    def get_name(self) -> str:
+        return "yanga_scoop_install"
+
     @property
     def scoop_file(self) -> Path:
         return self.environment.project_root_dir.joinpath("scoopfile.json")
 
-    def run(self) -> None:
+    def run(self) -> int:
         self.logger.info(
             f"Run {self.__class__.__name__} stage. Output dir: {self.output_dir}"
         )
         ScoopWrapper().install(self.scoop_file)
+        return 0
 
-    def get_dependencies(self) -> List[Path]:
+    def get_inputs(self) -> List[Path]:
         return [self.scoop_file]
 
     def get_outputs(self) -> List[Path]:
         return []
```

### Comparing `yanga-0.5.0/src/yanga/ybuild/variant.py` & `yanga-0.6.0/src/yanga/ybuild/variant.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/src/yanga/ymain.py` & `yanga-0.6.0/src/yanga/ymain.py`

 * *Files identical despite different names*

### Comparing `yanga-0.5.0/PKG-INFO` & `yanga-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanga
-Version: 0.5.0
+Version: 0.6.0
 Summary: Yet another ninja generator to build C/CPP projects.
 Home-page: https://github.com/cuinixam/yanga
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yanga Version: 0.5.0 Summary: Yet another ninja
+Metadata-Version: 2.1 Name: yanga Version: 0.6.0 Summary: Yet another ninja
 generator to build C/CPP projects. Home-page: https://github.com/cuinixam/yanga
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

