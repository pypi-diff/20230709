# Comparing `tmp/hatch_conda-0.3.2.tar.gz` & `tmp/hatch_conda-0.4.0.tar.gz`

## Comparing `hatch_conda-0.3.2.tar` & `hatch_conda-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.flake8
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.gitattributes
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/HISTORY.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/hooks.py
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch_conda/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/test_config.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/tests/utils.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/hatch.toml
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 hatch_conda-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.flake8
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/HISTORY.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/hooks.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/test_config.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/utils.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch.toml
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/PKG-INFO
```

### Comparing `hatch_conda-0.3.2/HISTORY.md` & `hatch_conda-0.4.0/HISTORY.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 -----
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] - 02/07/2023
+
+### Added
+- A conda `environment.yml` file can specified, which will be used to set up the environment. This allows installing packages from, e.g., the `conda-forge` index.
+
 ## [0.3.2] - 09/06/2023
 
 ### Fixed
 - Enter shell should now work correctly.
 
 ## [0.3.1] - 30/09/2022
```

### Comparing `hatch_conda-0.3.2/.github/workflows/build.yml` & `hatch_conda-0.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/.github/workflows/test.yml` & `hatch_conda-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/hatch_conda/plugin.py` & `hatch_conda-0.4.0/hatch_conda/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
+import os
+import re
 import shutil
 import signal
 import sys
 from contextlib import contextmanager
+from pathlib import Path
 from types import FrameType
 from typing import Callable
 
 import pexpect
 from hatch.env.plugin.interface import EnvironmentInterface
 
 
@@ -48,24 +51,25 @@
     PLUGIN_NAME = 'conda'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._config_command = None
         self._config_conda_forge = None
+        self._config_environment_file = None
         self.__python_version = None
 
         self.conda_env_name = f'{self.metadata.core.name}_{self.name}_{self.python_version}'
         self.project_path = '.'
 
         self.shells = ShellManager(self)
 
     @staticmethod
     def get_option_types():
-        return {'command': str, 'conda-forge': bool}
+        return {'command': str, 'conda-forge': bool, 'environment-file': str}
 
     def _config_value(self, field_name, default, valid=None):
         class_name = f'_config_{field_name.replace("-", "_")}'
         if self.__dict__[class_name] is None:
             value = self.config.get(field_name, default)
             if not isinstance(value, self.get_option_types()[field_name]):
                 raise TypeError(
@@ -75,74 +79,90 @@
             if valid is not None and value not in valid:
                 raise ValueError(f'Field `tool.hatch.envs.{self.name}.{field_name}` must be any of [{valid}] values.')
             self.__dict__[class_name] = value
         return self.__dict__[class_name]
 
     @property
     def config_command(self):
-        return self._config_value('command', 'conda', ['conda', 'mamba'])
+        return self._config_value('command', 'conda', ['conda', 'mamba', 'micromamba'])
 
     @property
     def config_conda_forge(self):
         return self._config_value('conda-forge', True)
 
     @property
+    def environment_file(self):
+        return self._config_value('environment-file', False)
+
+    @property
     def python_version(self):
         if self.__python_version is None:
             python_version = self.config.get('python', '')
             if not python_version:
                 python_version = '.'.join(map(str, sys.version_info[:2]))
             elif python_version.isdigit() and len(python_version) > 1:
                 python_version = f'{python_version[0]}.{python_version[1:]}'
 
             self.__python_version = python_version
 
         return self.__python_version
 
-    def _get_conda_env_path(self, name):
-        output = self.platform.check_command_output([self.config_command, 'env', 'list'])
-        env_names, env_paths = zip(
-            *[(line.split(' ')[0], line.split(' ')[-1]) for line in output.splitlines() if len(line.split(' ')[0]) > 1]
-        )
-        if name not in env_names:
-            return None
-        return env_paths[env_names.index(name)]
+    def _get_conda_env_path(self, name: str):
+        if self.config_command == 'micromamba':
+            output = self.platform.check_command_output([self.config_command, 'info', '--name', name])
+
+            match_env_location = r'env location : ([\S]*)\n'
+            return re.findall(match_env_location, output)[0]
+
+        else:
+            output = self.platform.check_command_output([self.config_command, 'env', 'list'])
+            env_names, env_paths = zip(
+                *[
+                    (line.split(' ')[0], line.split(' ')[-1])
+                    for line in output.splitlines()
+                    if len(line.split(' ')[0]) > 1
+                ]
+            )
+            if name not in env_names:
+                return None
+            return env_paths[env_names.index(name)]
 
     def find(self):
         return self._get_conda_env_path(self.conda_env_name)
 
     def create(self):
-        command = [
-            self.config_command,
-            'create',
-            '-y',
-            '-n',
-            self.conda_env_name,
-        ]
-        if self.config_conda_forge:
+        if not self.environment_file:
+            command = [self.config_command, 'create', '-y']
+            if self.config_conda_forge:
+                command += ['-c', 'conda-forge', '--no-channel-priority']
             command += [
-                '-c',
-                'conda-forge',
-                '--no-channel-priority',
+                f'python={self.python_version}',
+                'pip',
             ]
-        command += [
-            f'python={self.python_version}',
-            'pip',
-        ]
+        elif self.config_command == 'micromamba':
+            command = ['micromamba', 'create', '-y', '--file', self.environment_file]
+        else:
+            command = [self.config_command, 'env', 'create', '--file', self.environment_file]
+
+        command += ['-n', self.conda_env_name]
+
         if self.verbosity > 0:  # no cov
             self.platform.check_command(command)
         else:
             self.platform.check_command_output(command)
         self.apply_env_vars()
 
     def remove(self):
         self.platform.check_command_output([self.config_command, 'env', 'remove', '-y', '--name', self.conda_env_name])
 
     def exists(self):
-        return bool(self._get_conda_env_path(self.conda_env_name))
+        env_path = self._get_conda_env_path(self.conda_env_name)
+        if env_path is not None:
+            return Path(self._get_conda_env_path(self.conda_env_name)).exists()
+        return False
 
     def construct_conda_run_command(self, command):
         return [self.config_command, 'run', '-n', self.conda_env_name] + command
 
     def construct_pip_install_command(self, *args, **kwargs):
         return self.construct_conda_run_command(super().construct_pip_install_command(*args, **kwargs))
 
@@ -197,16 +217,20 @@
         if shell_executor is None:
             raise NotImplementedError(f'entering {name} shell in not supported yet')
         else:
             self.apply_env_vars()
             shell_executor(path, args, cmdl)
 
     def apply_env_vars(self):
-        env_vars = []
-        for env_var, value in dict(self.env_vars).items():
-            value_fixed = value
-            if sys.platform == 'win32':
-                value_fixed = value_fixed.replace('%', '%%%%%%%%')
-            env_vars.append(f'{env_var}={value_fixed}')
-        self.platform.check_command(
-            ['conda', 'env', 'config', 'vars', 'set', '-n', self.conda_env_name, '--'] + env_vars
-        )
+        if self.config_command == 'micromamba':
+            for env_var, value in dict(self.env_vars).items():
+                os.environ[env_var] = value
+        else:
+            env_vars = []
+            for env_var, value in dict(self.env_vars).items():
+                value_fixed = value
+                if sys.platform == 'win32':
+                    value_fixed = value_fixed.replace('%', '%%%%%%%%')
+                env_vars.append(f'{env_var}={value_fixed}')
+            self.platform.check_command(
+                ['conda', 'env', 'config', 'vars', 'set', '-n', self.conda_env_name, '--'] + env_vars
+            )
```

### Comparing `hatch_conda-0.3.2/tests/conftest.py` & `hatch_conda-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/tests/test_config.py` & `hatch_conda-0.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/tests/utils.py` & `hatch_conda-0.4.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/LICENSE.txt` & `hatch_conda-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/README.md` & `hatch_conda-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 **Table of Contents**
 
 - [Installation](#installation)
 - [Configuration](#configuration)
   - [Python](#python)
   - [Command](#command)
   - [Conda-forge](#conda-forge)
+  - [Environment file](#environment-file)
 - [Notes](#notes)
-- [Future](#future)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install hatch-conda
 ```
@@ -51,15 +51,15 @@
 
 If the [Python version](https://hatch.pypa.io/latest/config/environment/#python-version) is set to a multi-character integer like `310` then it will be interpreted as its `<MAJOR>.<MINOR>` form e.g. `3.10`.
 
 If not set, then the `<MAJOR>.<MINOR>` version of the first `python` found along your `PATH` will be used, defaulting to the Python executable Hatch is running on.
 
 ### Command
 
-The `command` option specifies the command that will be used to setup the environment. The possible options are `conda` and `mamba`.
+The `command` option specifies the command that will be used to setup the environment. The possible options are `conda`, `mamba` and `micromamba`.
 
 Default:
 
 ```toml
 [envs.<ENV_NAME>]
 command = "conda"
 ```
@@ -71,19 +71,25 @@
 Default:
 
 ```toml
 [envs.<ENV_NAME>]
 conda-forge = true
 ```
 
-## Notes
+### Environment file
+By default packages will be installed using pip. However, to install packages using conda, conda-forge, or any other channel, you can specify a conda environment file:
 
-- There must be a `conda` or `mamba` executable along your `PATH`.
-- The `env-exclude` [environment variable filter](https://hatch.pypa.io/latest/config/environment/#filters) has no effect.
+```toml
+[envs.<ENV_NAME>]
+environment-file = "environment.yml"
+```
+
+When using an environment file, the channel and python version specified in the environment file will be used. After installing the environment, any extra packages specified in the dependencies will be installed, as well as the local package. 
 
-## Future
+## Notes
 
-1. Install available packages from conda + conda-forge before using pip.
+- There must be a `conda`, `mamba`, or `micromamba` executable along your `PATH`.
+- The `env-exclude` [environment variable filter](https://hatch.pypa.io/latest/config/environment/#filters) has no effect.
 
 ## License
 
 `hatch-conda` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `hatch_conda-0.3.2/hatch.toml` & `hatch_conda-0.4.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/pyproject.toml` & `hatch_conda-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.3.2/PKG-INFO` & `hatch_conda-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-conda
-Version: 0.3.2
+Version: 0.4.0
 Summary: Hatch plugin for conda environments
 Project-URL: History, https://github.com/OldGrumpyViking/hatch-conda/blob/master/HISTORY.md
 Project-URL: Issues, https://github.com/OldGrumpyViking/hatch-conda/issues
 Project-URL: Source, https://github.com/OldGrumpyViking/hatch-conda
 Author-email: OldGrumpyViking <old.grumpy.viking@hotmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -42,16 +42,16 @@
 **Table of Contents**
 
 - [Installation](#installation)
 - [Configuration](#configuration)
   - [Python](#python)
   - [Command](#command)
   - [Conda-forge](#conda-forge)
+  - [Environment file](#environment-file)
 - [Notes](#notes)
-- [Future](#future)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install hatch-conda
 ```
@@ -78,15 +78,15 @@
 
 If the [Python version](https://hatch.pypa.io/latest/config/environment/#python-version) is set to a multi-character integer like `310` then it will be interpreted as its `<MAJOR>.<MINOR>` form e.g. `3.10`.
 
 If not set, then the `<MAJOR>.<MINOR>` version of the first `python` found along your `PATH` will be used, defaulting to the Python executable Hatch is running on.
 
 ### Command
 
-The `command` option specifies the command that will be used to setup the environment. The possible options are `conda` and `mamba`.
+The `command` option specifies the command that will be used to setup the environment. The possible options are `conda`, `mamba` and `micromamba`.
 
 Default:
 
 ```toml
 [envs.<ENV_NAME>]
 command = "conda"
 ```
@@ -98,19 +98,25 @@
 Default:
 
 ```toml
 [envs.<ENV_NAME>]
 conda-forge = true
 ```
 
-## Notes
+### Environment file
+By default packages will be installed using pip. However, to install packages using conda, conda-forge, or any other channel, you can specify a conda environment file:
 
-- There must be a `conda` or `mamba` executable along your `PATH`.
-- The `env-exclude` [environment variable filter](https://hatch.pypa.io/latest/config/environment/#filters) has no effect.
+```toml
+[envs.<ENV_NAME>]
+environment-file = "environment.yml"
+```
+
+When using an environment file, the channel and python version specified in the environment file will be used. After installing the environment, any extra packages specified in the dependencies will be installed, as well as the local package. 
 
-## Future
+## Notes
 
-1. Install available packages from conda + conda-forge before using pip.
+- There must be a `conda`, `mamba`, or `micromamba` executable along your `PATH`.
+- The `env-exclude` [environment variable filter](https://hatch.pypa.io/latest/config/environment/#filters) has no effect.
 
 ## License
 
 `hatch-conda` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

