# Comparing `tmp/yanga-0.6.0.tar.gz` & `tmp/yanga-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanga-0.6.0.tar", max compression
+gzip compressed data, was "yanga-0.7.0.tar", max compression
```

## Comparing `yanga-0.6.0.tar` & `yanga-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1066 2023-07-09 11:19:43.317508 yanga-0.6.0/LICENSE
--rw-r--r--   0        0        0     4695 2023-07-09 11:19:43.317508 yanga-0.6.0/README.md
--rw-r--r--   0        0        0     2384 2023-07-09 11:19:44.093508 yanga-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-09 11:19:44.065508 yanga-0.6.0/src/yanga/__init__.py
--rw-r--r--   0        0        0      347 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/_yrun.py
--rw-r--r--   0        0        0        0 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/__init__.py
--rw-r--r--   0        0        0     1810 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/build.py
--rw-r--r--   0        0        0     2500 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/init.py
--rw-r--r--   0        0        0     1364 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/install.py
--rw-r--r--   0        0        0      412 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/cookiecutter.json
--rw-r--r--   0        0        0       13 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
--rw-r--r--   0        0        0     5389 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1
--rw-r--r--   0        0        0    11054 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
--rw-r--r--   0        0        0      785 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
--rw-r--r--   0        0        0       34 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
--rw-r--r--   0        0        0      247 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
--rw-r--r--   0        0        0      219 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/scoopfile.json
--rw-r--r--   0        0        0      469 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/stages/my_stage.py
--rw-r--r--   0        0        0      176 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
--rw-r--r--   0        0        0        0 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/core/__init__.py
--rw-r--r--   0        0        0     4335 2023-07-09 11:19:43.317508 yanga-0.6.0/src/yanga/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/docs_utils.py
--rw-r--r--   0        0        0      278 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/exceptions.py
--rw-r--r--   0        0        0     1583 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/logging.py
--rw-r--r--   0        0        0     3430 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/runnable.py
--rw-r--r--   0        0        0     8971 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/scoop_wrapper.py
--rw-r--r--   0        0        0     1351 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/core/subprocess.py
--rw-r--r--   0        0        0        0 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/py.typed
--rw-r--r--   0        0        0        0 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/__init__.py
--rw-r--r--   0        0        0      917 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/build_main.py
--rw-r--r--   0        0        0      965 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/config.py
--rw-r--r--   0        0        0      477 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/environment.py
--rw-r--r--   0        0        0     4116 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/pipeline.py
--rw-r--r--   0        0        0      864 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/project.py
--rw-r--r--   0        0        0     1003 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/stages.py
--rw-r--r--   0        0        0      886 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ybuild/variant.py
--rw-r--r--   0        0        0     1070 2023-07-09 11:19:43.321508 yanga-0.6.0/src/yanga/ymain.py
--rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-09 16:48:22.264451 yanga-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4695 2023-07-09 16:48:22.264451 yanga-0.7.0/README.md
+-rw-r--r--   0        0        0     2384 2023-07-09 16:48:23.320458 yanga-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-09 16:48:23.280458 yanga-0.7.0/src/yanga/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/_yrun.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/__init__.py
+-rw-r--r--   0        0        0     1821 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/build.py
+-rw-r--r--   0        0        0     2548 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/init.py
+-rw-r--r--   0        0        0     1364 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/install.py
+-rw-r--r--   0        0        0      412 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/cookiecutter.json
+-rw-r--r--   0        0        0       13 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
+-rw-r--r--   0        0        0     5389 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1
+-rw-r--r--   0        0        0    11783 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
+-rw-r--r--   0        0        0      785 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
+-rw-r--r--   0        0        0       34 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
+-rw-r--r--   0        0        0      247 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/scoopfile.json
+-rw-r--r--   0        0        0      469 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/stages/my_stage.py
+-rw-r--r--   0        0        0      176 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
+-rw-r--r--   0        0        0        0 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/__init__.py
+-rw-r--r--   0        0        0     4335 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/docs_utils.py
+-rw-r--r--   0        0        0      278 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/exceptions.py
+-rw-r--r--   0        0        0     1583 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/logging.py
+-rw-r--r--   0        0        0     3764 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/runnable.py
+-rw-r--r--   0        0        0     8971 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     1517 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/core/subprocess.py
+-rw-r--r--   0        0        0        0 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/py.typed
+-rw-r--r--   0        0        0        0 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/ybuild/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/ybuild/build_main.py
+-rw-r--r--   0        0        0      965 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/ybuild/config.py
+-rw-r--r--   0        0        0      477 2023-07-09 16:48:22.268451 yanga-0.7.0/src/yanga/ybuild/environment.py
+-rw-r--r--   0        0        0     4116 2023-07-09 16:48:22.272451 yanga-0.7.0/src/yanga/ybuild/pipeline.py
+-rw-r--r--   0        0        0      864 2023-07-09 16:48:22.272451 yanga-0.7.0/src/yanga/ybuild/project.py
+-rw-r--r--   0        0        0     1003 2023-07-09 16:48:22.272451 yanga-0.7.0/src/yanga/ybuild/stages.py
+-rw-r--r--   0        0        0      886 2023-07-09 16:48:22.272451 yanga-0.7.0/src/yanga/ybuild/variant.py
+-rw-r--r--   0        0        0     1070 2023-07-09 16:48:22.272451 yanga-0.7.0/src/yanga/ymain.py
+-rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.7.0/PKG-INFO
```

### Comparing `yanga-0.6.0/LICENSE` & `yanga-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/README.md` & `yanga-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/pyproject.toml` & `yanga-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yanga"
-version = "0.6.0"
+version = "0.7.0"
 description = "Yet another ninja generator to build C/CPP projects."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/yanga"
 documentation = "https://yanga.readthedocs.io"
 classifiers = [
```

### Comparing `yanga-0.6.0/src/yanga/commands/build.py` & `yanga-0.7.0/src/yanga/commands/build.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 @dataclass
 class BuildCommandConfig(DataClassDictMixin):
     variant_name: str = field(metadata={"help": "SPL variant name."})
     build_config: str = field(metadata={"help": "Build configuration name."})
     build_target: str = field(metadata={"help": "Build target name."})
     project_dir: Path = field(
-        default=Path("."),
+        default=Path(".").absolute(),
         metadata={
             "help": "Project root directory. "
             "Defaults to the current directory if not specified."
         },
     )
 
     @classmethod
```

### Comparing `yanga-0.6.0/src/yanga/commands/init.py` & `yanga-0.7.0/src/yanga/commands/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,9 +64,12 @@
     def run(self, args: Namespace) -> int:
         self.logger.info(f"Running {self.name} with args {args}")
         YangaInit(InitCommandConfig.from_namespace(args)).run()
         return 0
 
     def _register_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
-            "--project-dir", help="Project directory", default=Path("."), type=Path
+            "--project-dir",
+            help="Project directory",
+            default=Path(".").absolute(),
+            type=Path,
         )
```

### Comparing `yanga-0.6.0/src/yanga/commands/install.py` & `yanga-0.7.0/src/yanga/commands/install.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1` & `yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/bootstrap.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py` & `yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import List, Optional
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("build")
 
 
 this_dir = Path(__file__).parent
+this_file = Path(__file__).name
 package_manager = "{{ cookiecutter.python_package_manager }}"
 
 
 class Runnable(ABC):
     @abstractmethod
     def run(self) -> int:
         """Run stage"""
@@ -76,15 +77,15 @@
             },
             "outputs": {
                 str(path): self.get_file_hash(path) for path in runnable.get_outputs()
             },
         }
 
         run_info_path = self.get_runnable_run_info_file(runnable)
-
+        run_info_path.parent.mkdir(parents=True, exist_ok=True)
         with run_info_path.open("w") as f:
             # pretty print the json file
             json.dump(file_info, f, indent=4)
 
     def get_runnable_run_info_file(self, runnable: Runnable) -> Path:
         return self.cache_dir / f"{runnable.get_name()}{self.RUN_INFO_FILE_EXTENSION}"
 
@@ -122,29 +123,35 @@
 
 
 class UserNotificationException(Exception):
     pass
 
 
 class SubprocessExecutor:
-    def __init__(self, command: List[str | Path], cwd: Optional[Path] = None):
+    def __init__(
+        self,
+        command: List[str | Path],
+        cwd: Optional[Path] = None,
+        capture_output: bool = True,
+    ):
         self.command = " ".join([str(cmd) for cmd in command])
         self.current_working_directory = cwd
+        self.capture_output = capture_output
 
     def execute(self) -> None:
         result = None
         try:
             current_dir = (self.current_working_directory or Path.cwd()).as_posix()
             logger.info(f"Running command: {self.command} in {current_dir}")
             # print all virtual environment variables
             logger.debug(json.dumps(dict(os.environ), indent=4))
             result = subprocess.run(
                 self.command.split(),
                 cwd=current_dir,
-                capture_output=True,
+                capture_output=self.capture_output,
                 text=True,  # to get stdout and stderr as strings instead of bytes
             )  # nosec
             result.check_returncode()
         except subprocess.CalledProcessError as e:
             raise UserNotificationException(
                 f"Command '{self.command}' failed with:\n"
                 f"{result.stdout if result else ''}\n"
@@ -172,25 +179,25 @@
                 )
             raise UserNotificationException(
                 f"Failed to create virtual environment in {self.venv_dir}.\n"
                 f"Please make sure you have the necessary permissions.\n"
                 f"Error: {e}"
             )
 
-    def pip(self, *args: str) -> None:
+    def pip(self, args: List[str]) -> None:
         """
         Execute a pip command within the virtual environment. This method should behave as if the
         user had activated the virtual environment and run `pip` from the command line.
 
         Args:
             *args: Command-line arguments to pip. For example, `pip('install', 'requests')` should
                    behave similarly to `pip install requests` at the command line.
         """
 
-    def run(self, *args: str) -> None:
+    def run(self, args: List[str], capture_output: bool = True) -> None:
         """
         Run an arbitrary command within the virtual environment. This method should behave as if the
         user had activated the virtual environment and run the given command from the command line.
 
         Args:
             *args: Command-line arguments. For example, `run('python', 'setup.py', 'install')`
                    should behave similarly to `python setup.py install` at the command line.
@@ -198,97 +205,98 @@
 
 
 class WindowsVirtualEnvironment(VirtualEnvironment):
     def __init__(self, venv_dir: Path) -> None:
         super().__init__(venv_dir)
         self.activate_script = self.venv_dir.joinpath("Scripts/activate")
 
-    def pip(self, *args: str) -> None:
+    def pip(self, args: List[str]) -> None:
         pip_path = self.venv_dir.joinpath("Scripts/pip").as_posix()
         SubprocessExecutor([pip_path, *args], this_dir).execute()
 
-    def run(self, *args: str) -> None:
+    def run(self, args: List[str], capture_output: bool = True) -> None:
         SubprocessExecutor(
-            [f"cmd /c {self.activate_script.as_posix()} && ", *args], this_dir
+            [f"cmd /c {self.activate_script.as_posix()} && ", *args],
+            this_dir,
+            capture_output,
         ).execute()
 
 
 class UnixVirtualEnvironment(VirtualEnvironment):
     def __init__(self, venv_dir: Path) -> None:
         super().__init__(venv_dir)
         self.activate_script = self.venv_dir.joinpath("bin/activate")
 
-    def pip(self, *args: str) -> None:
+    def pip(self, args: List[str]) -> None:
         pip_path = self.venv_dir.joinpath("bin/pip").as_posix()
         SubprocessExecutor([pip_path, *args]).execute()
 
-    def run(self, *args: str) -> None:
+    def run(self, args: List[str], capture_output: bool = True) -> None:
         # Create a temporary shell script
         with tempfile.NamedTemporaryFile("w", delete=False, suffix=".sh") as f:
             f.write("#!/bin/bash\n")  # Add a shebang line
             f.write(
                 f"source {self.activate_script.as_posix()}\n"
             )  # Write the activate command
             f.write(" ".join(args))  # Write the provided command
             temp_script_path = f.name  # Get the path of the temporary script
 
         # Make the temporary script executable
         SubprocessExecutor(["chmod", "+x", temp_script_path]).execute()
         # Run the temporary script
-        SubprocessExecutor([f"{Path(temp_script_path).as_posix()}"], this_dir).execute()
+        SubprocessExecutor(
+            [f"{Path(temp_script_path).as_posix()}"], this_dir, capture_output
+        ).execute()
         # Delete the temporary script
         os.remove(temp_script_path)
 
 
-class BuildVirtualEnvironment(Runnable):
+class CreateVirtualEnvironment(Runnable):
     def __init__(
         self,
     ) -> None:
         self.root_dir = this_dir
-
-    @property
-    def venv_dir(self) -> Path:
-        return self.root_dir / ".venv"
+        self.venv_dir = self.root_dir / ".venv"
+        self.virtual_env = self.instantiate_os_specific_venv()
 
     @property
     def package_manager_name(self) -> str:
         match = re.match(r"^([a-zA-Z0-9_-]+)", package_manager)
 
         if match:
             return match.group(1)
         else:
             raise UserNotificationException(
                 f"Could not extract the package manager name from {package_manager}"
             )
 
     def run(self) -> int:
         logger.info("Running project build script")
-        virtual_env = self.instantiate_os_specific_venv()
-        virtual_env.create(clear=self.venv_dir.exists())
-        virtual_env.pip("install", package_manager)
-        virtual_env.run(self.package_manager_name, "install")
+        self.virtual_env.create(clear=self.venv_dir.exists())
+        self.virtual_env.pip(["install", package_manager])
+        self.virtual_env.run([self.package_manager_name, "install"])
         return 0
 
     def instantiate_os_specific_venv(self) -> VirtualEnvironment:
         if sys.platform.startswith("win32"):
             return WindowsVirtualEnvironment(self.venv_dir)
         elif sys.platform.startswith("linux") or sys.platform.startswith("darwin"):
             return UnixVirtualEnvironment(self.venv_dir)
         else:
             raise UserNotificationException(
                 f"Unsupported operating system: {sys.platform}"
             )
 
     def get_name(self) -> str:
-        return "bootstrap"
+        return "create-virtual-environment"
 
     def get_inputs(self) -> List[Path]:
         return [
             self.root_dir / file
-            for file in ["poetry.lock", "poetry.toml", "pyproject.toml", "build.py"]
+            for file in ["poetry.lock", "poetry.toml", "pyproject.toml", this_file]
         ]
 
     def get_outputs(self) -> List[Path]:
         return []
 
 
 def print_environment_info() -> None:
@@ -299,16 +307,21 @@
     logger.info(f"Arguments: {sys.argv[1:]}")
     logger.info(str_bar)
 
 
 def main() -> int:
     try:
         # print_environment_info()
-        build = BuildVirtualEnvironment()
+        build = CreateVirtualEnvironment()
         Executor(build.venv_dir).execute(build)
+        # In case there is a yanga.yml file and the script was called with arguments,
+        # run 'yanga build' with all input arguments
+        args = sys.argv[1:]
+        if this_dir.joinpath("yanga.yaml").exists() and len(args) > 0:
+            build.virtual_env.run(["yanga", "build"] + args, False)
     except UserNotificationException as e:
         logger.error(e)
         return 1
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `yanga-0.6.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1` & `yanga-0.7.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/core/cmd_line.py` & `yanga-0.7.0/src/yanga/core/cmd_line.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/core/docs_utils.py` & `yanga-0.7.0/src/yanga/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/core/logging.py` & `yanga-0.7.0/src/yanga/core/logging.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/core/runnable.py` & `yanga-0.7.0/src/yanga/core/runnable.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import hashlib
 import json
 from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import List
 
+from .logging import logger
+
 
 class Runnable(ABC):
     @abstractmethod
     def run(self) -> int:
         """Run stage"""
 
     @abstractmethod
@@ -22,18 +24,18 @@
 
     @abstractmethod
     def get_outputs(self) -> List[Path]:
         """Get stage outputs"""
 
 
 class RunInfoStatus(Enum):
-    MATCH = (False, "Previous execution info matches")
-    NO_INFO = (True, "No previous execution info found")
-    FILE_NOT_FOUND = (True, "File not found")
-    FILE_CHANGED = (True, "File has changed")
+    MATCH = (False, "Nothing changed. Previous execution info matches.")
+    NO_INFO = (True, "No previous execution info found.")
+    FILE_NOT_FOUND = (True, "File not found.")
+    FILE_CHANGED = (True, "File has changed.")
 
     def __init__(self, should_run: bool, message: str) -> None:
         self.should_run = should_run
         self.message = message
 
 
 class Executor:
@@ -62,15 +64,15 @@
             },
             "outputs": {
                 str(path): self.get_file_hash(path) for path in runnable.get_outputs()
             },
         }
 
         run_info_path = self.get_runnable_run_info_file(runnable)
-
+        run_info_path.parent.mkdir(parents=True, exist_ok=True)
         with run_info_path.open("w") as f:
             # pretty print the json file
             json.dump(file_info, f, indent=4)
 
     def get_runnable_run_info_file(self, runnable: Runnable) -> Path:
         return self.cache_dir / f"{runnable.get_name()}{self.RUN_INFO_FILE_EXTENSION}"
 
@@ -89,13 +91,19 @@
                     return RunInfoStatus.FILE_NOT_FOUND
                 elif self.get_file_hash(path) != previous_hash:
                     return RunInfoStatus.FILE_CHANGED
         return RunInfoStatus.MATCH
 
     def execute(self, runnable: Runnable) -> int:
         run_info_status = self.previous_run_info_matches(runnable)
-        print(run_info_status.message)
         if run_info_status.should_run:
+            logger.info(
+                f"Runnable '{runnable.get_name()}' must run. {run_info_status.message}"
+            )
             exit_code = runnable.run()
             self.store_run_info(runnable)
             return exit_code
+        logger.info(
+            f"Runnable '{runnable.get_name()}' execution skipped. {run_info_status.message}"
+        )
+
         return 0
```

### Comparing `yanga-0.6.0/src/yanga/core/scoop_wrapper.py` & `yanga-0.7.0/src/yanga/core/scoop_wrapper.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/core/subprocess.py` & `yanga-0.7.0/src/yanga/core/subprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,27 +10,34 @@
 def which(app_name: str) -> Optional[Path]:
     """Return the path to the app if it is in the PATH, otherwise return None."""
     app_path = shutil.which(app_name)
     return Path(app_path) if app_path else None
 
 
 class SubprocessExecutor:
-    def __init__(self, command: List[str | Path], cwd: Optional[Path] = None):
+    def __init__(
+        self,
+        command: List[str | Path],
+        cwd: Optional[Path] = None,
+        capture_output: bool = True,
+    ):
         self.command = " ".join([str(cmd) for cmd in command])
         self.current_working_directory = cwd
+        self.capture_output = capture_output
 
     def execute(self) -> None:
         result = None
         try:
             logger.info(f"Running command: {self.command}")
             result = subprocess.run(
                 self.command.split(),
                 cwd=(self.current_working_directory or Path.cwd()).as_posix(),
-                capture_output=True,
+                capture_output=self.capture_output,
                 text=True,  # to get stdout and stderr as strings instead of bytes
             )  # nosec
             result.check_returncode()
         except subprocess.CalledProcessError as e:
-            err_message = result.stderr if result else e
             raise UserNotificationException(
-                f"Command '{self.command}' failed with error:\n{err_message}"
+                f"Command '{self.command}' failed with:\n"
+                f"{result.stdout if result else ''}\n"
+                f"{result.stderr if result else e}"
             )
```

### Comparing `yanga-0.6.0/src/yanga/ybuild/build_main.py` & `yanga-0.7.0/src/yanga/ybuild/build_main.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/ybuild/config.py` & `yanga-0.7.0/src/yanga/ybuild/config.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/ybuild/pipeline.py` & `yanga-0.7.0/src/yanga/ybuild/pipeline.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/ybuild/project.py` & `yanga-0.7.0/src/yanga/ybuild/project.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/ybuild/stages.py` & `yanga-0.7.0/src/yanga/ybuild/stages.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/ybuild/variant.py` & `yanga-0.7.0/src/yanga/ybuild/variant.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/src/yanga/ymain.py` & `yanga-0.7.0/src/yanga/ymain.py`

 * *Files identical despite different names*

### Comparing `yanga-0.6.0/PKG-INFO` & `yanga-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanga
-Version: 0.6.0
+Version: 0.7.0
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
-Metadata-Version: 2.1 Name: yanga Version: 0.6.0 Summary: Yet another ninja
+Metadata-Version: 2.1 Name: yanga Version: 0.7.0 Summary: Yet another ninja
 generator to build C/CPP projects. Home-page: https://github.com/cuinixam/yanga
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

