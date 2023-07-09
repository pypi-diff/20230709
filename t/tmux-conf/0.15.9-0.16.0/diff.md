# Comparing `tmp/tmux_conf-0.15.9.tar.gz` & `tmp/tmux_conf-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmux_conf-0.15.9.tar", last modified: Thu Dec 15 19:08:26 2022, max compression
+gzip compressed data, was "tmux_conf-0.16.0.tar", last modified: Sun Jul  9 10:44:02 2023, max compression
```

## Comparing `tmux_conf-0.15.9.tar` & `tmux_conf-0.16.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.644983 tmux_conf-0.15.9/
--rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-12 14:51:08.000000 tmux_conf-0.15.9/LICENSE
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2022-12-15 19:08:26.644538 tmux_conf-0.15.9/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-12 14:51:08.000000 tmux_conf-0.15.9/README.md
--rw-r--r--   0 jaclu      (501) staff       (20)     1593 2022-12-15 19:07:27.000000 tmux_conf-0.15.9/pyproject.toml
--rw-r--r--   0 jaclu      (501) staff       (20)       38 2022-12-15 19:08:26.645091 tmux_conf-0.15.9/setup.cfg
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.637104 tmux_conf-0.15.9/src/
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.642180 tmux_conf-0.15.9/src/tmux_conf/
--rw-r--r--   0 jaclu      (501) staff       (20)      202 2022-12-12 14:51:08.000000 tmux_conf-0.15.9/src/tmux_conf/__init__.py
--rw-r--r--   0 jaclu      (501) staff       (20)      269 2022-12-15 19:07:12.000000 tmux_conf-0.15.9/src/tmux_conf/constants.py
--rw-r--r--   0 jaclu      (501) staff       (20)     5698 2022-12-14 17:36:04.000000 tmux_conf-0.15.9/src/tmux_conf/embedded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)    16555 2022-12-15 18:53:00.000000 tmux_conf-0.15.9/src/tmux_conf/plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    23447 2022-12-15 18:49:51.000000 tmux_conf-0.15.9/src/tmux_conf/tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4780 2022-12-12 17:30:59.000000 tmux_conf-0.15.9/src/tmux_conf/utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     3364 2022-12-15 18:41:09.000000 tmux_conf-0.15.9/src/tmux_conf/vers_check.py
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2022-12-15 19:08:26.644045 tmux_conf-0.15.9/src/tmux_conf.egg-info/
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)      370 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/SOURCES.txt
--rw-r--r--   0 jaclu      (501) staff       (20)        1 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/dependency_links.txt
--rw-r--r--   0 jaclu      (501) staff       (20)       10 2022-12-15 19:08:26.000000 tmux_conf-0.15.9/src/tmux_conf.egg-info/top_level.txt
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.800334 tmux_conf-0.16.0/
+-rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-16 01:20:21.000000 tmux_conf-0.16.0/LICENSE
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-07-09 10:44:02.799896 tmux_conf-0.16.0/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-16 01:20:21.000000 tmux_conf-0.16.0/README.md
+-rw-r--r--   0 jaclu      (501) staff       (20)     1588 2023-07-09 10:43:20.000000 tmux_conf-0.16.0/pyproject.toml
+-rw-r--r--   0 jaclu      (501) staff       (20)       38 2023-07-09 10:44:02.800508 tmux_conf-0.16.0/setup.cfg
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.784356 tmux_conf-0.16.0/src/
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.793074 tmux_conf-0.16.0/src/tmux_conf/
+-rw-r--r--   0 jaclu      (501) staff       (20)      202 2022-12-16 01:20:21.000000 tmux_conf-0.16.0/src/tmux_conf/__init__.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      269 2023-07-08 10:30:28.000000 tmux_conf-0.16.0/src/tmux_conf/constants.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     5394 2023-05-12 13:52:19.000000 tmux_conf-0.16.0/src/tmux_conf/embedded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      436 2023-05-12 13:47:26.000000 tmux_conf-0.16.0/src/tmux_conf/exceptions.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    16598 2023-05-15 11:48:01.000000 tmux_conf-0.16.0/src/tmux_conf/plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    25531 2023-07-09 10:17:40.000000 tmux_conf-0.16.0/src/tmux_conf/tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4780 2023-04-25 08:10:55.000000 tmux_conf-0.16.0/src/tmux_conf/utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     3968 2023-05-12 20:08:07.000000 tmux_conf-0.16.0/src/tmux_conf/vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.795317 tmux_conf-0.16.0/src/tmux_conf.egg-info/
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)      519 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)        1 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)       10 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/top_level.txt
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.799137 tmux_conf-0.16.0/tests/
+-rw-r--r--   0 jaclu      (501) staff       (20)     3775 2023-07-09 10:30:18.000000 tmux_conf-0.16.0/tests/test_embeded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     8194 2023-07-09 10:30:15.000000 tmux_conf-0.16.0/tests/test_plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    15013 2023-07-09 10:30:02.000000 tmux_conf-0.16.0/tests/test_tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4061 2023-07-09 10:30:07.000000 tmux_conf-0.16.0/tests/test_utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     2915 2023-07-09 10:30:10.000000 tmux_conf-0.16.0/tests/test_vers_check.py
```

### Comparing `tmux_conf-0.15.9/LICENSE` & `tmux_conf-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.15.9/PKG-INFO` & `tmux_conf-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux_conf
-Version: 0.15.9
+Version: 0.16.0
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.15.9/README.md` & `tmux_conf-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.15.9/pyproject.toml` & `tmux_conf-0.16.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tmux_conf"
-version = "0.15.9"
+version = "0.16.0"
 authors = [
   { name="Jacob Lundqvist", email="Jacob.Lundqvist@gmail.com" },
 ]
 description = "Generates version checked tmux conf"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["tmux", "automation"]
@@ -53,20 +53,20 @@
 addopts = "--cov=src/tmux_conf --cov-report=term-missing"
 testpaths = [
     "tests",
 ]
 
 [tool.mypy]
 mypy_path = "src"
-#check_untyped_defs = true
+check_untyped_defs = true
 disallow_any_generics = true
 ignore_missing_imports = true
 no_implicit_optional = true
 show_error_codes = true
 strict_equality = true
 
 warn_redundant_casts = true
-#warn_return_any = true
+warn_return_any = true
 
-#warn_unreachable = true
-#warn_unused_configs = true
-#no_implicit_reexport = true
+warn_unreachable = true
+warn_unused_configs = true
+no_implicit_reexport = true
```

### Comparing `tmux_conf-0.15.9/src/tmux_conf/embedded_scripts.py` & `tmux_conf-0.16.0/src/tmux_conf/embedded_scripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 #
 #  See the README.md in the repository for more info
 #
 
 import os
 import pathlib
 import stat
-import subprocess
 import sys
 
 from .constants import XDG_CONFIG_HOME
-from .utils import tilde_home_dir
+from .utils import run_shell, tilde_home_dir
 
 
 class EmbeddedScripts:
     """Handles scripts, either embedded or stored in scripts/ as external"""
 
     def __init__(self, conf_file: str, use_embedded_scripts: bool):
-
         #  Ensure conf file is using ~ or full path if ~ not applicable
         conf_file = tilde_home_dir(conf_file)
         if conf_file[0] not in ("~", "/"):
             conf_file = tilde_home_dir(os.path.join(os.getcwd(), conf_file))
         self._conf_file = conf_file
 
         self._use_embedded_scripts = use_embedded_scripts
@@ -72,39 +70,30 @@
             fname = f"{script_dir}/{scr_name}.sh"
             with open(fname, "w", encoding="utf-8") as f:
                 for line in script:
                     f.write(f"{line}\n")
 
             #  Make it run able
             f = pathlib.Path(fname)
-            f.chmod(f.stat().st_mode | stat.S_IEXEC |
-                    stat.S_IXGRP | stat.S_IXOTH)
+            f.chmod(f.stat().st_mode | stat.S_IEXEC | stat.S_IXGRP | stat.S_IXOTH)
 
     def run_it(self, scr_name: str, in_bg: bool = False) -> str:
         """Generate the code to run an embedded/external script"""
         cmd = "run "
         if in_bg:
             cmd += "-b "
         cmd += '"'
         if self._use_embedded_scripts:
             cmd += f"cut -c3- {self._conf_file} | "
             if scr_name in self._bash_scripts:
                 if not self._bash_shell:
-                    self._bash_shell = (
-                        subprocess.run(
-                            ["which", "bash"],
-                            stdout=subprocess.PIPE,
-                            check=True,
-                        )
-                        .stdout.decode("utf-8")
-                        .strip()
-                    )
-                    if not self._bash_shell:
+                    bash_shell = run_shell("command -v bash")
+                    if not (bash_shell):
                         sys.exit("Failed to find bash!")
-
+                    self._bash_shell = bash_shell
                 cmd += self._bash_shell
             else:
                 cmd += "sh"
             cmd += f" -s {scr_name}"
         else:
             cmd += f"{self.get_dir()}/{scr_name}.sh"
         cmd += '"'
@@ -144,25 +133,23 @@
                 output.append(f"# {script_line}")
         output.append('# "$@" #  This triggers the embedded script')
         return output
 
     def get_dir(self):
         """Retrieves the location where scripts should be saved"""
         if self._use_embedded_scripts:
-            raise SyntaxError(
-                "get_dir() called when use_embedded_scripts is True")
+            raise SyntaxError("get_dir() called when use_embedded_scripts is True")
 
         if tilde_home_dir(self._conf_file) == "~/.tmux.conf":
             scripts_dir = os.path.expanduser("~/.tmux/scripts")
         else:
             conf_file = os.path.expanduser(self._conf_file)
 
             xdg_home = os.environ.get(XDG_CONFIG_HOME)
             # pylint: disable=consider-using-assignment-expr
             if xdg_home:
                 conf_base = xdg_home
             else:
                 conf_base = os.path.dirname(os.path.dirname(conf_file))
 
-            scripts_dir = os.path.expanduser(
-                os.path.join(conf_base, "tmux", "scripts"))
+            scripts_dir = os.path.expanduser(os.path.join(conf_base, "tmux", "scripts"))
         return scripts_dir
```

### Comparing `tmux_conf-0.15.9/src/tmux_conf/plugins.py` & `tmux_conf-0.16.0/src/tmux_conf/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,39 +165,41 @@
         #  not to config file. Since program will exit after displaying
         #  plugin details, no need to reset this variable.
         #
         verbose = self._plugins_display == 3
 
         for name, info in self._used_plugins.items():
             if verbose:
-                name = self._name_sans_prefix(name)
+                inner_name = self._name_sans_prefix(name)
                 suffix = self._remove_if_found(
-                    plugin_items, name, " *** Not installed ***"
+                    plugin_items, inner_name, " *** Not installed ***"
+                )
+                print("".ljust(len(inner_name) + 2, "-"))
+                print(
+                    f"> {inner_name:<{max_l_name - 2}} - {info[PLUGIN_VERS_MIN]} {suffix}"
                 )
-                print("".ljust(len(name) + 2, "-"))
-                print(f"> {name:<{max_l_name - 2}} - {info[PLUGIN_VERS_MIN]} {suffix}")
                 info[PLUGIN_MTHD]()
                 #
                 #  Skip indention, for easier read
                 #
                 for line in info[PLUGIN_STATIC_CODE].split("\n"):
                     # if line == line.strip():
                     print(f"{line.strip()}")
                 # print()
             else:
-                name = self._name_sans_prefix(name)
+                inner_name = self._name_sans_prefix(name)
                 suffix = self._remove_if_found(
-                    plugin_items, name, " *** Not installed ***"
+                    plugin_items, inner_name, " *** Not installed ***"
                 )
-                print(f"{name:<{max_l_name}} - {info[PLUGIN_VERS_MIN]} {suffix}")
+                print(f"{inner_name:<{max_l_name}} - {info[PLUGIN_VERS_MIN]} {suffix}")
 
         #  Remove skipped plugins from plugin_items
         for _, name in self._skipped_plugins:
-            name = self._name_sans_prefix(name)
-            _ = self._remove_if_found(plugin_items, name)
+            inner_name = self._name_sans_prefix(name)
+            _ = self._remove_if_found(plugin_items, inner_name)
 
         if plugin_items:
             print("\n-----   Unused plugins found   -----")
             for s in plugin_items:
                 print("\t", s)
 
         if not self._skipped_plugins or self._plugins_display != 2:
@@ -210,14 +212,15 @@
         #  List all plugins installed, but not used
         #
         max_l_v = 0
         self._skipped_plugins.sort()
         for vers, name in self._skipped_plugins:
             max_l_v = max(max_l_v, len(vers))
         print("-----   Plugins ignored   -----")
+        #  TODO: space after Min
         print(f'{"Min":<{max_l_v}}|{" Plugin name":<{max_l_name}}')
         print(f'{"vers":<{max_l_v}}|\n')
         for vers, name in self._skipped_plugins:
             print(f"{vers:>{max_l_v}}  {name:<{max_l_name}}")
 
         sys.exit(0)
 
@@ -252,15 +255,14 @@
         for name, info in self._used_plugins.items():
             info[1]()
 
         #
         #  Add plugin references and hard coded plugin settings.
         #
         for name, info in self._used_plugins.items():
-
             output.append("#------------------------------")
             output.append(f'set -g @plugin "{name}"')
             for line in info[2].split("\n"):
                 output.append(line.strip())
 
         if self._plugin_handler == "manual":
             #
@@ -455,18 +457,15 @@
 
         if not os.path.exists(plugins_dir):
             return  # nothing to clear
 
         for file_name in os.listdir(plugins_dir):
             path = os.path.join(plugins_dir, file_name)
             print(f"removing plugin {file_name}")
-            try:
-                shutil.rmtree(path)
-            except OSError:
-                os.remove(path)
+            shutil.rmtree(path)
 
     def _name_sans_prefix(self, name: str) -> str:
         if name.find("/") > -1:
             name = name.split("/")[1]
         return name
 
     def _remove_if_found(self, lst: list, item: str, warning: str = "") -> str:
```

### Comparing `tmux_conf-0.15.9/src/tmux_conf/tmux_conf.py` & `tmux_conf-0.16.0/src/tmux_conf/tmux_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,36 @@
 #
 #  All paths stored internally are done so with ~ expanded
 #
 
 
 import os
 import shutil
-import subprocess  # nosec
 import sys
 from collections.abc import Callable
 from datetime import datetime
 
 import __main__
 
 from .constants import __version__
 from .embedded_scripts import EmbeddedScripts
+from .exceptions import TmuxConfNotTmuxCommand
 from .plugins import Plugins
 from .utils import (
     btick_unescaped,
     expanduser_plus,
     is_executable,
     parse_cmdline,
     run_shell,
     verify_conf_file_usable,
 )
 from .vers_check import VersionCheck
 
 
 class TmuxConfig:
-
     #
     #  I have forked a tpm that uses TPM_BIN to use the right tmux
     #  context. If you just use one version of tmux, this does not
     #  matter, but if you experiment with various versions,
     #  this is essential. It ensures tpm and other processes started
     #  inside tmux use the running tmux bin.
     #
@@ -138,19 +137,19 @@
         self.conf_file = verify_conf_file_usable(conf_file)
 
         #
         #  add the class to have the functionality needed during
         #  self.find_tmux_bin(), it will later be called again with
         #  the version details for the actually used version
         #
-        self.define_tmux_vers()
+        # self.define_tmux_vers()
 
-        self.find_tmux_bin(tmux_bin)
+        self.find_tmux_bin(tmux_bin, requested_vers=tmux_version)
         if tmux_version and (tmux_version != self.vers.get()):
-            self.define_tmux_vers(tmux_version)
+            # self.define_tmux_vers(tmux_version)
             if not self.is_tmate():
                 #
                 #  Only display off version info when bin is tmux
                 #
                 print()
                 print(
                     "Config has been requested for another version of tmux,"
@@ -169,21 +168,19 @@
 
         self.es = EmbeddedScripts(self.conf_file, self.use_embedded_scripts)
 
         #
         #  If current tmux is too old to handle tpm plugins,
         #  disable plugins entirely
         #
-        if not self.vers_ok("1.9"):
-            self.plugin_handler = ""
-            if plugins_display > 0:
-                sys.exit(
-                    "Versions < 1.9 does not support tpm, "
-                    + "so plugin info can not be displayed"
-                )
+        if not self.vers_ok("1.9") and self.plugin_handler:
+            # tpm not available before 1.9, since it was defined, ensure
+            # this is set to manual
+            self.plugin_handler = "manual"
+
         self.plugins = Plugins(
             conf_file=self.conf_file,
             vers_class=self.vers,
             es_class=self.es,
             plugin_handler=self.plugin_handler,
             clear_plugins=clear_plugins,
             plugins_display=plugins_display,
@@ -302,20 +299,14 @@
 
         #
         #  Inform plugin handler if this is to be treated as a
         #  limited host, displaying progress as tpm is processed etc
         #
         self.plugins.set_limited_host(self.is_limited_host)
 
-        # if not (verbose := self.plugins_display == 3):
-        #     #
-        #     # App terminates at end of display_info(),
-        #     # so can be left disabled
-        #     #
-        #     self._calling_class.write_enable(False)
         self._write_stdout = True  # Needs to be true during plugin init
         self.write_enable(False)
         if self.plugin_handler:
             self.plugins.scan(self.list_plugin_methods())
             if self.plugins_display == 3:
                 self.write_enable(True)
             if self.plugins_display:
@@ -328,15 +319,14 @@
 
         self.content()
         #
         #  check the edit_config() header in this class for hints on
         #  how to override the edit key
         #
         self.edit_config()
-
         if self.plugin_handler and self.plugins.found():
             w(
                 """#======================================================
             #
             #   Plugins
             #
             # ======================================================\n"""
@@ -438,45 +428,37 @@
             return
 
         #
         #  Convert to lines actually to be written
         #
         lines: list[str] = []
         for raw_line in cmd.split("\n"):
-            ## print(f">> raw_line [{raw_line}]")
             #
             #  Returns a list of lines. If input contained a -N and notes
             #  are not supported by this tmux, the note is extracted and
             #  the following is returned.
             #  self.use_notes_as_comments = True
             #   - empty string, vertical spacer
             #   - note as a comment
             #   - the remainder of the initial line
             #  self.use_notes_as_comments = False
             #   - the remainder of the initial line
             #
             for line in self.filter_note(raw_line.strip()):
                 lines.append(line)
 
-        if self._write_stdout:
-            #
-            #  Used for displaying plugin settings
-            #
+        with open(self.conf_file, "a", encoding="utf-8") as f:
             for line in lines:
-                print(line)
-        else:
-            with open(self.conf_file, "a", encoding="utf-8") as f:
-                for line in lines:
-                    if self.use_embedded_scripts and (btick_unescaped(line)):
-                        raise SyntaxError(
-                            "Un-escaped back-ticks can not be present in "
-                            + "the generated config when\n"
-                            + "embedded_scripts are used!"
-                        )
-                    f.write(f"{line}{eol}")
+                if self.use_embedded_scripts and (btick_unescaped(line)):
+                    raise SyntaxError(
+                        "Un-escaped back-ticks can not be present in "
+                        + "the generated config when\n"
+                        + "embedded_scripts are used!"
+                    )
+                f.write(f"{line}{eol}")
 
     def filter_note(self, line: str):
         """Returns list of lines, if notes are not supported
         first an empty spacer line, then the note as a comment,
         and finally the actual command without the note
         if self.use_notes_as_comments is False
         only the third line from above is returned
@@ -488,15 +470,14 @@
             or line.find("-N") < 0
             or (self.vers_ok("3.1") and self.use_notes_as_comments)
         ):
             return [line]
         parts = line.split("-N")
         pre = parts[0].strip()
         post = parts[1].strip()
-        print(f">> pre [{pre}] [{post}]")
         if not post:
             # Propably an -N at end of line, so not related to a note
             return [pre]
         p0 = post[0]
         if p0 in {'"', "'"}:
             end_note = post[1:].find(p0)
             x = end_note + 1
@@ -546,94 +527,34 @@
         if confirmation not in ("y", "Y"):
             print("Terminating...")
             sys.exit(1)
 
     #
     #  Selecting tmux bin
     #
-    def use_tmux_bin(self, cmd: str):
-        """Verify this is a valid tmux, and store its path & version
-
-        self.tmux_bin   The tmux used
-        self.tmux_vers  The version used
-
+    def find_tmux_bin(self, cmd: str = "", requested_vers: str = "") -> bool:
+        """if tmux should use a specific version, when generating config
+        set requested_vers parameter, if empy the actual version is used
         """
-        # Do a basic sanity check
-        if self.is_tmux_bin(cmd):
-            self.tmux_bin = cmd
-            self.define_tmux_vers()
-        else:
-            sys.exit(f"ERROR: tmux bin seems invalid: {cmd}")
-
-    def find_tmux_bin(self, cmd: str = "") -> bool:
         if not cmd:
             #  Use the first that gives something
             cmd = self.find_cmd_1() or self.find_cmd_2() or self.find_cmd_3()
 
-        if cmd:
-            # the asdf check needs to know what version this is
-            self.use_tmux_bin(cmd)
-        #
-        #  asdf refers to bins via its shim dir, where versions cant be
-        #  identified, since it depends on other ENV variables,
-        #  in this case try to extract a full path to the tmux bin itself,
-        #  but make sure not to expand an asdf path that has already
-        #  been processed!
-        #
-        if cmd.find(".asdf") > -1 and cmd.find("/installs/") < 0:
-            if not self.is_tmux_bin(cmd):
-                print(f"ERROR: asdf tmux does not seem to be valid: {cmd}")
-                sys.exit(1)
-            cmd_asdf = (
-                f'{cmd.split("shims/")[0]}installs/tmux/'
-                f'{self.vers.get().split("-")[0]}/bin/tmux'
-            )
-            self.use_tmux_bin(cmd_asdf)
-
         if not cmd:
+            raise TmuxConfNotTmuxCommand("No tmux command found")
+        self.expand_cmd_path(cmd, requested_vers)
+
+        # ==== 1 =
+
+        if not self.tmux_bin:
             #  tmux not found abort
             print("ERROR could not find tmux binary, aborting")
             sys.exit(1)
         return True
 
-    def is_tmate(self):
-        return self.tmux_bin.find("tmate") > -1
-
-    def is_tmux_bin(self, cmd: str = "") -> bool:
-        """Only checks if the requested bin seems to be a tmux or tmate,
-        checking name and doing simplified version check, ie if
-        the second part of version is int"""
-        if not cmd:
-            raise SyntaxError("cmd empty")
-        c = shutil.which(cmd)
-        if not c:
-            raise SyntaxError(f"tmux cmd not found: {cmd}")
-        cmd = c
-        output = run_shell(f"{cmd} -V")
-        name, v = output.split()
-        if name not in ("tmux", "tmate"):
-            return False
-        i, _ = self.vers.get_sub_vers(v.split(".")[1])
-        try:
-            int(i)
-        except ValueError:
-            return False
-        return True
-
-    #  TODO: use a better name
-    def define_tmux_vers(self, vers="", tmux_bin: str = "tmux"):
-        if not tmux_bin:
-            tmux_bin = self.tmux_bin
-        vers_found = run_shell(f"{tmux_bin} -V | cut -d' ' -f2")
-
-        self.vers = VersionCheck(vers_found, vers)
-
-    #
-    #  Various attempt at finding the tmux bin
-    #
     def find_cmd_1(self):
         """First check is to see if the tmux used to generate the
         previous config can be extracted.
         """
         cmd = ""
         if os.path.isfile(self.conf_file):
             s = f'grep "TMUX_BIN=" {self.conf_file} | cut -d= -f 2 | sed s/\\"//g'
@@ -645,23 +566,16 @@
                 return ""
             cmd = c2
             print(f"found {cmd} in conf file")
         return cmd
 
     def find_cmd_2(self):
         """Next check PATH"""
-        cmd = ""
-        try:
-            c = run_shell("command -v tmux")
-        except subprocess.CalledProcessError:
-            c = ""
-        if c and c.lower().find("not found") < 0:
-            cmd = c
-            print(f"found {cmd} in PATH")
-        return cmd
+        print("find_cmd_2()")
+        return self.full_path_cmd()
 
     def find_cmd_3(self):
         """Finally try some likely locations"""
         cmd = ""
         for c in (
             "/usr/local/bin/tmux",
             "/home/linuxbrew/.linuxbrew/bin/tmux",
@@ -669,11 +583,140 @@
         ):
             c2 = expanduser_plus(c)
             if is_executable(c2):
                 cmd = c2
                 break
         return cmd
 
+    def use_tmux_bin(self, tmux_bin="tmux", requested_vers=""):
+        """Returns True if this was a valid tmux bin
+        If this was the case self.tmux_bin & self.vers will have been set
+        """
+        parts = run_shell(f"{tmux_bin} -V").split(" ")
+        if len(parts) != 2 or parts[0] not in ("tmux", "tmate"):
+            raise TmuxConfNotTmuxCommand("{tmux} Doesnt seem to be a tmux binary")
+        #
+        #  Ensure version generated for a previous tmux bin is not still
+        #  arround
+        #
+        self.vers = None
+
+        vers = VersionCheck(actual_vers=parts[1], requested_vers=requested_vers)
+        # except TmuxConfInvalidTmuxVersion:
+        #     print("{parts[[1]} Doesnt seem to be a valid tmux version")
+        #     return False
+        self.tmux_bin = tmux_bin
+        self.vers = vers
+        return True
+
+    #
+    #  Various attempt at finding the tmux bin
+    #
+    def expand_cmd_path(self, cmd, requested_vers=""):
+        """If this is an asdf tmux, we need to translate path from shim
+        to actual bin, in order to ptoperly detect version, but make sure
+        not to expand an asdf path that has already been processed!
+
+        Any process starting in the same dir as tmux was started will
+        inherrit potential local asdf tmux selection, but processes
+        starting in other dirs will use asdf default version.
+        By expanding the initial shim into a full path,
+        the correct tmux will be used in all cases.
+        """
+        if cmd:
+            #  First use what in the asdf case might be a shim, in order
+            #  to get full path
+            #
+            if not self.use_tmux_bin(cmd, requested_vers):
+                self.tmux_bin = ""
+                return
+        # get full path notation for tmux
+        cmd = self.full_path_cmd(self.tmux_bin)
+        if cmd.find(".asdf") > -1 and cmd.find("/installs/") < 0:
+            if not self.use_tmux_bin(cmd):
+                print(f"ERROR: asdf tmux does not seem to be valid: {cmd}")
+                sys.exit(1)
+            #
+            #  Convert asdf shim into absolute path
+            #
+            cmd_asdf = (
+                f'{cmd.split("shims/")[0]}installs/tmux/'
+                f'{self.vers.get().split("-",maxsplit=1)[0]}/bin/tmux'
+            )
+            self.use_tmux_bin(cmd_asdf)
+
+    def full_path_cmd(self, cmd="tmux"):
+        c = run_shell(f"command -v {cmd}")
+        if c and c.lower().find("not found") < 0:
+            cmd = c
+            print(f"found {cmd} in PATH")
+        return cmd
+
     def remove_conf_file(self):
         if os.path.exists(self.conf_file):
             #  Ensure we start with an empty file
             os.remove(self.conf_file)
+
+    # def extract_tmux_vers(self, vers_str_in):
+    #     parts = vers_str_in.split(".")
+    #     if len(parts) != 2:
+    #         raise TmuxConfInvalidTmuxVersion("Version string is not two parts separated by '.'")
+    #     try:
+    #         maj = int(parts[0])
+    #     except ValueError as exc:
+    #         raise TmuxConfInvalidTmuxVersion(
+    #             f"First part of version string is not int: {parts[0]}"
+    #         ) from exc
+
+    #     #  loop over parts[1] as long as each char is an int, then
+    #     #  ensure next char is a-z
+    #     return maj, min
+
+    # def use_tmux_bin(self, cmd: str):
+    #     """Verify this is a valid tmux, and store its path & version
+
+    #     self.tmux_bin   The tmux used
+    #     self.tmux_vers  The version used
+
+    #     """
+    #     # Do a basic sanity check
+    #     if self.is_tmux_bin(cmd):
+    #         self.tmux_bin = cmd
+    #         self.define_tmux_vers(tmux_bin=cmd)
+    #     else:
+    #         sys.exit(f"ERROR: tmux bin seems invalid: {cmd}")
+
+    def is_tmate(self):
+        return self.tmux_bin.find("tmate") > -1
+
+    # def is_tmux_bin(self, cmd: str) -> bool:
+    #     """Only checks if the requested bin seems to be a tmux or tmate,
+    #     checking name and doing simplified version check, ie if
+    #     the second part of version is int"""
+    #     if not cmd:
+    #         raise SyntaxError("cmd empty")
+    #     c = shutil.which(cmd)
+    #     if not c:
+    #         raise SyntaxError(f"tmux cmd not found: {cmd}")
+    #     cmd = c
+    #     output = run_shell(f"{cmd} -V")
+    #     name, v = output.split()
+    #     if name not in ("tmux", "tmate"):
+    #         return False
+    #     # i, _ = self.vers.get_sub_vers(v.split(".")[1])
+    #     i = v.split(".")[0]
+    #     try:
+    #         int(i)
+    #     except ValueError:
+    #         return False
+    #     return True
+
+    # #  TODO: use a better name
+    # def define_tmux_vers(self, vers="", tmux_bin: str = "tmux"):
+    #     if not tmux_bin:
+    #         tmux_bin = self.tmux_bin
+    #     vers_found = run_shell(f"{tmux_bin} -V | cut -d' ' -f2")
+    #     if not vers_found:
+    #         raise FileNotFoundError(
+    #             f"tmux: [{tmux_bin}] does not seem to be a tmux bin"
+    #         )
+    #     self.vers = VersionCheck(vers_found, vers)
```

### Comparing `tmux_conf-0.15.9/src/tmux_conf/utils.py` & `tmux_conf-0.16.0/src/tmux_conf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     conf_location = os.path.dirname(conf_file)
     try:
         os.makedirs(conf_location, exist_ok=True)
     except PermissionError as error:
         print("ERROR: Could not create directory for config file!")
         raise PermissionError from error
     except OSError as error:
-        print(f"ERRPR: read only file system reported for {conf_file}")
+        print(f"ERROR: read only file system reported for {conf_file}")
         raise OSError from error
 
     #  Ensure it can be written to
     # pylint: disable=too-many-try-statements
     try:
         with open(conf_file, "a", encoding="utf-8") as _:
             pass
```

### Comparing `tmux_conf-0.15.9/src/tmux_conf/vers_check.py` & `tmux_conf-0.16.0/src/tmux_conf/vers_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,18 +27,15 @@
         #
         #  tmux derivative tmate uses versions like 2.4.0
         #  for compatibility checks only the first two are needed
         #  This syntax handles both normal tmux and tmate
         #
         parts = self._vers.split(".")
         v_maj = parts[0]
-        try:
-            v_min = parts[1]
-        except IndexError:
-            raise IndexError(f"ERROR: Failed to extract v_min: {self._vers}")
+        v_min = parts[1]
         try:
             self.v_maj = int(v_maj)
         except ValueError as exc:
             print(f"Error: v_maj was not int: {self._vers}")
             raise ValueError from exc
         self.v_min, self.v_suffix = self.get_sub_vers(v_min)
 
@@ -55,38 +52,33 @@
         Param is forgiving, can be int, float or string.
         When given as int .0 is appended
         In many cases a float is sufficient, like 2.8, 3.0 etc
         Some versions have character suffixes like 3.3a, then a string
         param is needed. Internally version refs are allways treated as
         strings.
         """
-        v = self.normalize_vers(vers)
-        try:
-            a, b = v.split(".")
-        except ValueError as exc:
-            print(f"ERROR: vers_ok({v}) - bad syntax, expected maj.min notation!")
-            raise ValueError from exc
+        a, b = self.normalize_vers(vers).split(".")
 
         try:
             vers_maj = int(a)
         except ValueError as exc:
-            print(f"ERROR: vers_ok({v}) - maj part not int!")
+            print(f"ERROR: vers_ok({vers}) - maj part not int!")
             raise ValueError from exc
 
         vers_min, suffix = self.get_sub_vers(b)
 
         if vers_maj > self.v_maj:
             return False
         if vers_maj < self.v_maj:
             return True
 
         r = True
         if vers_min > self.v_min:
             r = False
-        elif suffix > self.v_suffix:
+        elif vers_min == self.v_min and suffix > self.v_suffix:
             r = False
         return r
 
     def get_sub_vers(self, v2: str):
         int_part = ""
         for c in v2:
             try:
@@ -99,14 +91,37 @@
         i = int(int_part)
         s = v2.split(int_part)[1]
         return i, s
 
     def normalize_vers(self, vers) -> str:
         """Normalizes vers into a string"""
         # param fixes
+
+        if vers == "next-3.4":
+            #
+            #  Alpine tmux-3.3a_git20230428 reports version as next-3.4
+            #  Change this into 3.3a-git20230428, so that notation follows
+            #  the normal logic, and can be used in vers checks
+            #
+            vers = "3.3a-git20230428"
+
+        if isinstance(vers, str) and vers.find(".") < 0:
+            try:
+                vers = int(vers)
+            except ValueError as err:
+                print(f"ERROR: vers_check normalize_vers({vers}) bad param")
+                raise ValueError from err
         if isinstance(vers, int):
             vers = f"{vers}.0"
         elif isinstance(vers, float):
             vers = f"{vers}"
         #  correct , -> .
         vers = vers.replace(",", ".")
-        return vers
+        #
+        #  Only keep first two items
+        #
+        parts = vers.split(".")
+        # if len(parts) > 2:
+        #     raise ValueError(f"ERROR: normalize_vers({vers}) > 2 parts")
+        if len(parts) < 2:
+            raise ValueError(f"ERROR: normalize_vers({vers}) < 2 parts")
+        return ".".join(parts[:2])
```

### Comparing `tmux_conf-0.15.9/src/tmux_conf.egg-info/PKG-INFO` & `tmux_conf-0.16.0/src/tmux_conf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux-conf
-Version: 0.15.9
+Version: 0.16.0
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

