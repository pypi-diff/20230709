# Comparing `tmp/dotbot-1.19.1.tar.gz` & `tmp/dotbot-1.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotbot-1.19.1.tar", last modified: Sat Dec 17 20:15:31 2022, max compression
+gzip compressed data, was "dotbot-1.19.2.tar", last modified: Sun Jul  9 20:28:22 2023, max compression
```

## Comparing `dotbot-1.19.1.tar` & `dotbot-1.19.2.tar`

### file list

```diff
@@ -1,40 +1,50 @@
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2022-12-17 20:15:31.506864 dotbot-1.19.1/
--rw-r--r--   0 anish      (501) staff       (20)     1133 2022-01-30 18:34:49.000000 dotbot-1.19.1/LICENSE.md
--rw-r--r--   0 anish      (501) staff       (20)    17896 2022-12-17 20:15:31.507321 dotbot-1.19.1/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)    16946 2022-12-17 20:12:34.000000 dotbot-1.19.1/README.md
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2022-12-17 20:15:31.498008 dotbot-1.19.1/dotbot/
--rw-r--r--   0 anish      (501) staff       (20)       73 2022-12-17 20:13:46.000000 dotbot-1.19.1/dotbot/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)       61 2021-02-18 16:50:20.000000 dotbot-1.19.1/dotbot/__main__.py
--rw-r--r--   0 anish      (501) staff       (20)     5742 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/cli.py
--rw-r--r--   0 anish      (501) staff       (20)      763 2022-12-17 19:08:18.000000 dotbot-1.19.1/dotbot/config.py
--rw-r--r--   0 anish      (501) staff       (20)      849 2022-01-30 23:46:10.000000 dotbot-1.19.1/dotbot/context.py
--rw-r--r--   0 anish      (501) staff       (20)     2900 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/dispatcher.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2022-12-17 20:15:31.501353 dotbot-1.19.1/dotbot/messenger/
--rw-r--r--   0 anish      (501) staff       (20)       58 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/messenger/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)      172 2022-01-30 23:46:10.000000 dotbot-1.19.1/dotbot/messenger/color.py
--rw-r--r--   0 anish      (501) staff       (20)      114 2015-06-12 04:35:07.000000 dotbot-1.19.1/dotbot/messenger/level.py
--rw-r--r--   0 anish      (501) staff       (20)     1739 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/messenger/messenger.py
--rw-r--r--   0 anish      (501) staff       (20)      621 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/plugin.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2022-12-17 20:15:31.503293 dotbot-1.19.1/dotbot/plugins/
--rw-r--r--   0 anish      (501) staff       (20)      100 2021-02-18 16:50:20.000000 dotbot-1.19.1/dotbot/plugins/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)     2994 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/plugins/clean.py
--rw-r--r--   0 anish      (501) staff       (20)     1995 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/plugins/create.py
--rw-r--r--   0 anish      (501) staff       (20)    13733 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/plugins/link.py
--rw-r--r--   0 anish      (501) staff       (20)     2729 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/plugins/shell.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2022-12-17 20:15:31.506378 dotbot-1.19.1/dotbot/util/
--rw-r--r--   0 anish      (501) staff       (20)       34 2021-02-18 16:50:20.000000 dotbot-1.19.1/dotbot/util/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)     1412 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/util/common.py
--rw-r--r--   0 anish      (501) staff       (20)      211 2022-01-30 23:46:10.000000 dotbot-1.19.1/dotbot/util/compat.py
--rw-r--r--   0 anish      (501) staff       (20)     1269 2022-12-17 19:01:22.000000 dotbot-1.19.1/dotbot/util/module.py
--rw-r--r--   0 anish      (501) staff       (20)      239 2022-01-30 23:46:10.000000 dotbot-1.19.1/dotbot/util/singleton.py
--rw-r--r--   0 anish      (501) staff       (20)      193 2022-01-30 23:46:10.000000 dotbot-1.19.1/dotbot/util/string.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2022-12-17 20:15:31.500234 dotbot-1.19.1/dotbot.egg-info/
--rw-r--r--   0 anish      (501) staff       (20)    17896 2022-12-17 20:15:31.000000 dotbot-1.19.1/dotbot.egg-info/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)      732 2022-12-17 20:15:31.000000 dotbot-1.19.1/dotbot.egg-info/SOURCES.txt
--rw-r--r--   0 anish      (501) staff       (20)        1 2022-12-17 20:15:31.000000 dotbot-1.19.1/dotbot.egg-info/dependency_links.txt
--rw-r--r--   0 anish      (501) staff       (20)       39 2022-12-17 20:15:31.000000 dotbot-1.19.1/dotbot.egg-info/entry_points.txt
--rw-r--r--   0 anish      (501) staff       (20)       33 2022-12-17 20:15:31.000000 dotbot-1.19.1/dotbot.egg-info/requires.txt
--rw-r--r--   0 anish      (501) staff       (20)        7 2022-12-17 20:15:31.000000 dotbot-1.19.1/dotbot.egg-info/top_level.txt
--rw-r--r--   0 anish      (501) staff       (20)      117 2022-01-30 23:45:30.000000 dotbot-1.19.1/pyproject.toml
--rw-r--r--   0 anish      (501) staff       (20)       67 2022-12-17 20:15:31.508416 dotbot-1.19.1/setup.cfg
--rw-r--r--   0 anish      (501) staff       (20)     2304 2022-12-17 19:09:25.000000 dotbot-1.19.1/setup.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-07-09 20:28:22.973650 dotbot-1.19.2/
+-rw-r--r--   0 anish      (501) staff       (20)     1123 2023-03-05 12:37:08.000000 dotbot-1.19.2/LICENSE.md
+-rw-r--r--   0 anish      (501) staff       (20)    18272 2023-07-09 20:28:22.973917 dotbot-1.19.2/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)    17322 2023-07-09 20:20:27.000000 dotbot-1.19.2/README.md
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-07-09 20:28:22.948996 dotbot-1.19.2/dotbot/
+-rw-r--r--   0 anish      (501) staff       (20)       73 2023-07-09 20:28:05.000000 dotbot-1.19.2/dotbot/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)       61 2021-02-18 16:50:20.000000 dotbot-1.19.2/dotbot/__main__.py
+-rw-r--r--   0 anish      (501) staff       (20)     5758 2023-07-09 19:26:53.000000 dotbot-1.19.2/dotbot/cli.py
+-rw-r--r--   0 anish      (501) staff       (20)      763 2022-12-17 19:08:18.000000 dotbot-1.19.2/dotbot/config.py
+-rw-r--r--   0 anish      (501) staff       (20)      849 2022-01-30 23:46:10.000000 dotbot-1.19.2/dotbot/context.py
+-rw-r--r--   0 anish      (501) staff       (20)     2900 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/dispatcher.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-07-09 20:28:22.955819 dotbot-1.19.2/dotbot/messenger/
+-rw-r--r--   0 anish      (501) staff       (20)       58 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/messenger/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)      172 2022-01-30 23:46:10.000000 dotbot-1.19.2/dotbot/messenger/color.py
+-rw-r--r--   0 anish      (501) staff       (20)      114 2015-06-12 04:35:07.000000 dotbot-1.19.2/dotbot/messenger/level.py
+-rw-r--r--   0 anish      (501) staff       (20)     1739 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/messenger/messenger.py
+-rw-r--r--   0 anish      (501) staff       (20)      621 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/plugin.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-07-09 20:28:22.960425 dotbot-1.19.2/dotbot/plugins/
+-rw-r--r--   0 anish      (501) staff       (20)      100 2021-02-18 16:50:20.000000 dotbot-1.19.2/dotbot/plugins/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)     2994 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/plugins/clean.py
+-rw-r--r--   0 anish      (501) staff       (20)     1995 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/plugins/create.py
+-rw-r--r--   0 anish      (501) staff       (20)    12454 2023-07-09 20:23:49.000000 dotbot-1.19.2/dotbot/plugins/link.py
+-rw-r--r--   0 anish      (501) staff       (20)     2729 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/plugins/shell.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-07-09 20:28:22.965541 dotbot-1.19.2/dotbot/util/
+-rw-r--r--   0 anish      (501) staff       (20)       34 2021-02-18 16:50:20.000000 dotbot-1.19.2/dotbot/util/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)     1412 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/util/common.py
+-rw-r--r--   0 anish      (501) staff       (20)      211 2022-01-30 23:46:10.000000 dotbot-1.19.2/dotbot/util/compat.py
+-rw-r--r--   0 anish      (501) staff       (20)     1269 2022-12-17 19:01:22.000000 dotbot-1.19.2/dotbot/util/module.py
+-rw-r--r--   0 anish      (501) staff       (20)      239 2022-01-30 23:46:10.000000 dotbot-1.19.2/dotbot/util/singleton.py
+-rw-r--r--   0 anish      (501) staff       (20)      193 2022-01-30 23:46:10.000000 dotbot-1.19.2/dotbot/util/string.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-07-09 20:28:22.952524 dotbot-1.19.2/dotbot.egg-info/
+-rw-r--r--   0 anish      (501) staff       (20)    18272 2023-07-09 20:28:22.000000 dotbot-1.19.2/dotbot.egg-info/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)      914 2023-07-09 20:28:22.000000 dotbot-1.19.2/dotbot.egg-info/SOURCES.txt
+-rw-r--r--   0 anish      (501) staff       (20)        1 2023-07-09 20:28:22.000000 dotbot-1.19.2/dotbot.egg-info/dependency_links.txt
+-rw-r--r--   0 anish      (501) staff       (20)       39 2023-07-09 20:28:22.000000 dotbot-1.19.2/dotbot.egg-info/entry_points.txt
+-rw-r--r--   0 anish      (501) staff       (20)       33 2023-07-09 20:28:22.000000 dotbot-1.19.2/dotbot.egg-info/requires.txt
+-rw-r--r--   0 anish      (501) staff       (20)        7 2023-07-09 20:28:22.000000 dotbot-1.19.2/dotbot.egg-info/top_level.txt
+-rw-r--r--   0 anish      (501) staff       (20)      117 2022-01-30 23:45:30.000000 dotbot-1.19.2/pyproject.toml
+-rw-r--r--   0 anish      (501) staff       (20)       67 2023-07-09 20:28:22.974679 dotbot-1.19.2/setup.cfg
+-rw-r--r--   0 anish      (501) staff       (20)     2304 2022-12-17 19:09:25.000000 dotbot-1.19.2/setup.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-07-09 20:28:22.972906 dotbot-1.19.2/tests/
+-rw-r--r--   0 anish      (501) staff       (20)     1638 2022-12-17 19:01:22.000000 dotbot-1.19.2/tests/test_bin_dotbot.py
+-rw-r--r--   0 anish      (501) staff       (20)     4687 2022-12-17 19:12:07.000000 dotbot-1.19.2/tests/test_clean.py
+-rw-r--r--   0 anish      (501) staff       (20)     5282 2022-12-17 19:01:22.000000 dotbot-1.19.2/tests/test_cli.py
+-rw-r--r--   0 anish      (501) staff       (20)     1003 2022-12-17 19:01:22.000000 dotbot-1.19.2/tests/test_config.py
+-rw-r--r--   0 anish      (501) staff       (20)     1985 2022-12-17 19:01:22.000000 dotbot-1.19.2/tests/test_create.py
+-rw-r--r--   0 anish      (501) staff       (20)    31953 2023-07-09 20:20:27.000000 dotbot-1.19.2/tests/test_link.py
+-rw-r--r--   0 anish      (501) staff       (20)      518 2022-12-17 19:01:22.000000 dotbot-1.19.2/tests/test_noop.py
+-rw-r--r--   0 anish      (501) staff       (20)     7673 2022-12-17 19:01:22.000000 dotbot-1.19.2/tests/test_shell.py
+-rw-r--r--   0 anish      (501) staff       (20)     1991 2022-12-17 19:01:22.000000 dotbot-1.19.2/tests/test_shim.py
```

### Comparing `dotbot-1.19.1/LICENSE.md` & `dotbot-1.19.2/LICENSE.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 The MIT License (MIT)
 =====================
 
-**Copyright (c) 2014-2021 Anish Athalye (me@anishathalye.com)**
+**Copyright (c) Anish Athalye (me@anishathalye.com)**
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `dotbot-1.19.1/PKG-INFO` & `dotbot-1.19.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotbot
-Version: 1.19.1
+Version: 1.19.2
 Summary: A tool that bootstraps your dotfiles
 Home-page: https://github.com/anishathalye/dotbot
 Author: Anish Athalye
 Author-email: me@anishathalye.com
 License: MIT
 Keywords: dotfiles
 Classifier: Development Status :: 5 - Production/Stable
@@ -223,14 +223,16 @@
 | `**`     | matches any **file**, recursively (Python >= 3.5 only) |
 | `?`      | matches any single character                           |
 | `[seq]`  | matches any character in `seq`                         |
 | `[!seq]` | matches any character not in `seq`                     |
 
 However, due to the design of `glob.glob`, using a glob pattern such as `config/*`, will **not** match items that begin with `.`. To specifically capture items that being with `.`, you will need to include the `.` in the pattern, like this: `config/.*`.
 
+When using glob with the `exclude:` option, the paths in the exclude paths should be relative to the base directory, same as the glob pattern itself. For example, if a glob pattern `vim/*` matches directories `vim/autoload`, `vim/ftdetect`, `vim/ftplugin`, and `vim/spell`, and you want to ignore the spell directory, then you should use `exclude: ["vim/spell"]` (not just `"spell"`).
+
 #### Example
 
 ```yaml
 - link:
     ~/.config/terminator:
       create: true
       path: config/terminator
@@ -483,15 +485,15 @@
 ## Contributing
 
 Do you have a feature request, bug report, or patch? Great! See
 [CONTRIBUTING.md][contributing] for information on what you can do about that.
 
 ## License
 
-Copyright (c) 2014-2021 Anish Athalye. Released under the MIT License. See
+Copyright (c) Anish Athalye. Released under the MIT License. See
 [LICENSE.md][license] for details.
 
 [PyPI]: https://pypi.org/project/dotbot/
 [init-dotfiles]: https://github.com/Vaelatern/init-dotfiles
 [dotfiles-template]: https://github.com/anishathalye/dotfiles_template
 [inspiration]: https://github.com/anishathalye/dotbot/wiki/Users
 [windows-symlinks]: https://learn.microsoft.com/en-us/windows/security/threat-protection/security-policy-settings/create-symbolic-links
```

### Comparing `dotbot-1.19.1/README.md` & `dotbot-1.19.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,16 @@
 | `**`     | matches any **file**, recursively (Python >= 3.5 only) |
 | `?`      | matches any single character                           |
 | `[seq]`  | matches any character in `seq`                         |
 | `[!seq]` | matches any character not in `seq`                     |
 
 However, due to the design of `glob.glob`, using a glob pattern such as `config/*`, will **not** match items that begin with `.`. To specifically capture items that being with `.`, you will need to include the `.` in the pattern, like this: `config/.*`.
 
+When using glob with the `exclude:` option, the paths in the exclude paths should be relative to the base directory, same as the glob pattern itself. For example, if a glob pattern `vim/*` matches directories `vim/autoload`, `vim/ftdetect`, `vim/ftplugin`, and `vim/spell`, and you want to ignore the spell directory, then you should use `exclude: ["vim/spell"]` (not just `"spell"`).
+
 #### Example
 
 ```yaml
 - link:
     ~/.config/terminator:
       create: true
       path: config/terminator
@@ -457,15 +459,15 @@
 ## Contributing
 
 Do you have a feature request, bug report, or patch? Great! See
 [CONTRIBUTING.md][contributing] for information on what you can do about that.
 
 ## License
 
-Copyright (c) 2014-2021 Anish Athalye. Released under the MIT License. See
+Copyright (c) Anish Athalye. Released under the MIT License. See
 [LICENSE.md][license] for details.
 
 [PyPI]: https://pypi.org/project/dotbot/
 [init-dotfiles]: https://github.com/Vaelatern/init-dotfiles
 [dotfiles-template]: https://github.com/anishathalye/dotfiles_template
 [inspiration]: https://github.com/anishathalye/dotbot/wiki/Users
 [windows-symlinks]: https://learn.microsoft.com/en-us/windows/security/threat-protection/security-policy-settings/create-symbolic-links
```

### Comparing `dotbot-1.19.1/dotbot/cli.py` & `dotbot-1.19.2/dotbot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         if options.version:
             try:
                 with open(os.devnull) as devnull:
                     git_hash = subprocess.check_output(
                         ["git", "rev-parse", "HEAD"],
                         cwd=os.path.dirname(os.path.abspath(__file__)),
                         stderr=devnull,
-                    )
+                    ).decode("ascii")
                 hash_msg = " (git %s)" % git_hash[:10]
             except (OSError, subprocess.CalledProcessError):
                 hash_msg = ""
             print("Dotbot version %s%s" % (dotbot.__version__, hash_msg))
             exit(0)
         if options.super_quiet:
             log.set_level(Level.WARNING)
```

### Comparing `dotbot-1.19.1/dotbot/config.py` & `dotbot-1.19.2/dotbot/config.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/context.py` & `dotbot-1.19.2/dotbot/context.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/dispatcher.py` & `dotbot-1.19.2/dotbot/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/messenger/messenger.py` & `dotbot-1.19.2/dotbot/messenger/messenger.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/plugin.py` & `dotbot-1.19.2/dotbot/plugin.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/plugins/clean.py` & `dotbot-1.19.2/dotbot/plugins/clean.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/plugins/create.py` & `dotbot-1.19.2/dotbot/plugins/create.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/plugins/link.py` & `dotbot-1.19.2/dotbot/plugins/link.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,72 +55,47 @@
                 path = self._default_source(destination, source.get("path"))
             else:
                 path = self._default_source(destination, source)
             if test is not None and not self._test_success(test):
                 self._log.lowinfo("Skipping %s" % destination)
                 continue
             path = os.path.normpath(os.path.expandvars(os.path.expanduser(path)))
-            if use_glob:
+            if use_glob and self._has_glob_chars(path):
                 glob_results = self._create_glob_results(path, exclude_paths)
-                if len(glob_results) == 0:
-                    self._log.warning("Globbing couldn't find anything matching " + str(path))
-                    success = False
-                    continue
-                if len(glob_results) == 1 and destination[-1] == "/":
-                    self._log.error("Ambiguous action requested.")
-                    self._log.error(
-                        "No wildcard in glob, directory use undefined: "
-                        + destination
-                        + " -> "
-                        + str(glob_results)
+                self._log.lowinfo("Globs from '" + path + "': " + str(glob_results))
+                for glob_full_item in glob_results:
+                    # Find common dirname between pattern and the item:
+                    glob_dirname = os.path.dirname(os.path.commonprefix([path, glob_full_item]))
+                    glob_item = (
+                        glob_full_item
+                        if len(glob_dirname) == 0
+                        else glob_full_item[len(glob_dirname) + 1 :]
                     )
-                    self._log.warning("Did you want to link the directory or into it?")
-                    success = False
-                    continue
-                elif len(glob_results) == 1 and destination[-1] != "/":
-                    # perform a normal link operation
+                    # Add prefix to basepath, if provided
+                    if base_prefix:
+                        glob_item = base_prefix + glob_item
+                    # where is it going
+                    glob_link_destination = os.path.join(destination, glob_item)
                     if create:
-                        success &= self._create(destination)
+                        success &= self._create(glob_link_destination)
                     if force or relink:
-                        success &= self._delete(path, destination, relative, canonical_path, force)
-                    success &= self._link(
-                        path, destination, relative, canonical_path, ignore_missing
-                    )
-                else:
-                    self._log.lowinfo("Globs from '" + path + "': " + str(glob_results))
-                    for glob_full_item in glob_results:
-                        # Find common dirname between pattern and the item:
-                        glob_dirname = os.path.dirname(os.path.commonprefix([path, glob_full_item]))
-                        glob_item = (
-                            glob_full_item
-                            if len(glob_dirname) == 0
-                            else glob_full_item[len(glob_dirname) + 1 :]
-                        )
-                        # Add prefix to basepath, if provided
-                        if base_prefix:
-                            glob_item = base_prefix + glob_item
-                        # where is it going
-                        glob_link_destination = os.path.join(destination, glob_item)
-                        if create:
-                            success &= self._create(glob_link_destination)
-                        if force or relink:
-                            success &= self._delete(
-                                glob_full_item,
-                                glob_link_destination,
-                                relative,
-                                canonical_path,
-                                force,
-                            )
-                        success &= self._link(
+                        success &= self._delete(
                             glob_full_item,
                             glob_link_destination,
                             relative,
                             canonical_path,
-                            ignore_missing,
+                            force,
                         )
+                    success &= self._link(
+                        glob_full_item,
+                        glob_link_destination,
+                        relative,
+                        canonical_path,
+                        ignore_missing,
+                    )
             else:
                 if create:
                     success &= self._create(destination)
                 if not ignore_missing and not self._exists(
                     os.path.join(self._context.base_directory(), path)
                 ):
                     # we seemingly check this twice (here and in _link) because
@@ -151,14 +126,17 @@
             if basename.startswith("."):
                 return basename[1:]
             else:
                 return basename
         else:
             return source
 
+    def _has_glob_chars(self, path):
+        return any(i in path for i in "?*[")
+
     def _glob(self, path):
         """
         Wrap `glob.glob` in a python agnostic way, catching errors in usage.
         """
         if sys.version_info < (3, 5) and "**" in path:
             self._log.error(
                 'Link cannot handle recursive glob ("**") for Python < version 3.5: "%s"' % path
```

### Comparing `dotbot-1.19.1/dotbot/plugins/shell.py` & `dotbot-1.19.2/dotbot/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/util/common.py` & `dotbot-1.19.2/dotbot/util/common.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot/util/module.py` & `dotbot-1.19.2/dotbot/util/module.py`

 * *Files identical despite different names*

### Comparing `dotbot-1.19.1/dotbot.egg-info/PKG-INFO` & `dotbot-1.19.2/dotbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotbot
-Version: 1.19.1
+Version: 1.19.2
 Summary: A tool that bootstraps your dotfiles
 Home-page: https://github.com/anishathalye/dotbot
 Author: Anish Athalye
 Author-email: me@anishathalye.com
 License: MIT
 Keywords: dotfiles
 Classifier: Development Status :: 5 - Production/Stable
@@ -223,14 +223,16 @@
 | `**`     | matches any **file**, recursively (Python >= 3.5 only) |
 | `?`      | matches any single character                           |
 | `[seq]`  | matches any character in `seq`                         |
 | `[!seq]` | matches any character not in `seq`                     |
 
 However, due to the design of `glob.glob`, using a glob pattern such as `config/*`, will **not** match items that begin with `.`. To specifically capture items that being with `.`, you will need to include the `.` in the pattern, like this: `config/.*`.
 
+When using glob with the `exclude:` option, the paths in the exclude paths should be relative to the base directory, same as the glob pattern itself. For example, if a glob pattern `vim/*` matches directories `vim/autoload`, `vim/ftdetect`, `vim/ftplugin`, and `vim/spell`, and you want to ignore the spell directory, then you should use `exclude: ["vim/spell"]` (not just `"spell"`).
+
 #### Example
 
 ```yaml
 - link:
     ~/.config/terminator:
       create: true
       path: config/terminator
@@ -483,15 +485,15 @@
 ## Contributing
 
 Do you have a feature request, bug report, or patch? Great! See
 [CONTRIBUTING.md][contributing] for information on what you can do about that.
 
 ## License
 
-Copyright (c) 2014-2021 Anish Athalye. Released under the MIT License. See
+Copyright (c) Anish Athalye. Released under the MIT License. See
 [LICENSE.md][license] for details.
 
 [PyPI]: https://pypi.org/project/dotbot/
 [init-dotfiles]: https://github.com/Vaelatern/init-dotfiles
 [dotfiles-template]: https://github.com/anishathalye/dotfiles_template
 [inspiration]: https://github.com/anishathalye/dotbot/wiki/Users
 [windows-symlinks]: https://learn.microsoft.com/en-us/windows/security/threat-protection/security-policy-settings/create-symbolic-links
```

### Comparing `dotbot-1.19.1/setup.py` & `dotbot-1.19.2/setup.py`

 * *Files identical despite different names*

