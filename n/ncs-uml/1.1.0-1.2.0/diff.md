# Comparing `tmp/ncs-uml-1.1.0.tar.gz` & `tmp/ncs-uml-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncs-uml-1.1.0.tar", last modified: Sat Jul  8 00:02:12 2023, max compression
+gzip compressed data, was "ncs-uml-1.2.0.tar", last modified: Sun Jul  9 04:35:20 2023, max compression
```

## Comparing `ncs-uml-1.1.0.tar` & `ncs-uml-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-08 00:02:12.887773 ncs-uml-1.1.0/
--rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.1.0/LICENSE
--rw-r--r--   0 kkotari    (501) staff       (20)       75 2023-06-23 13:29:14.000000 ncs-uml-1.1.0/MANIFEST.in
--rw-r--r--   0 kkotari    (501) staff       (20)    15420 2023-07-08 00:02:12.887555 ncs-uml-1.1.0/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)    14419 2023-07-07 22:58:31.000000 ncs-uml-1.1.0/README.md
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-08 00:02:12.886108 ncs-uml-1.1.0/ncs_uml/
--rw-r--r--   0 kkotari    (501) staff       (20)      253 2023-07-07 21:24:49.000000 ncs-uml-1.1.0/ncs_uml/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     4926 2023-07-07 22:52:17.000000 ncs-uml-1.1.0/ncs_uml/main.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-08 00:02:12.887310 ncs-uml-1.1.0/ncs_uml/scripts/
--rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-07 21:00:13.000000 ncs-uml-1.1.0/ncs_uml/scripts/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     2298 2023-07-07 23:28:30.000000 ncs-uml-1.1.0/ncs_uml/scripts/run.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5953 2023-07-07 22:23:07.000000 ncs-uml-1.1.0/ncs_uml/utils.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-08 00:02:12.887016 ncs-uml-1.1.0/ncs_uml.egg-info/
--rw-r--r--   0 kkotari    (501) staff       (20)    15420 2023-07-08 00:02:12.000000 ncs-uml-1.1.0/ncs_uml.egg-info/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)      347 2023-07-08 00:02:12.000000 ncs-uml-1.1.0/ncs_uml.egg-info/SOURCES.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-07-08 00:02:12.000000 ncs-uml-1.1.0/ncs_uml.egg-info/dependency_links.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       87 2023-07-08 00:02:12.000000 ncs-uml-1.1.0/ncs_uml.egg-info/entry_points.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-07-08 00:02:12.000000 ncs-uml-1.1.0/ncs_uml.egg-info/requires.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-07-08 00:02:12.000000 ncs-uml-1.1.0/ncs_uml.egg-info/top_level.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.1.0/requirements.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-07-08 00:02:12.887831 ncs-uml-1.1.0/setup.cfg
--rw-r--r--   0 kkotari    (501) staff       (20)     1699 2023-07-07 21:55:17.000000 ncs-uml-1.1.0/setup.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.574653 ncs-uml-1.2.0/
+-rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.2.0/LICENSE
+-rw-r--r--   0 kkotari    (501) staff       (20)       58 2023-07-09 04:23:25.000000 ncs-uml-1.2.0/MANIFEST.in
+-rw-r--r--   0 kkotari    (501) staff       (20)    15420 2023-07-09 04:35:20.574446 ncs-uml-1.2.0/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)    14419 2023-07-07 22:58:31.000000 ncs-uml-1.2.0/README.md
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.572449 ncs-uml-1.2.0/ncs_uml/
+-rw-r--r--   0 kkotari    (501) staff       (20)      253 2023-07-09 01:46:50.000000 ncs-uml-1.2.0/ncs_uml/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5171 2023-07-09 04:21:55.000000 ncs-uml-1.2.0/ncs_uml/main.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.573983 ncs-uml-1.2.0/ncs_uml/scripts/
+-rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-07 21:00:13.000000 ncs-uml-1.2.0/ncs_uml/scripts/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     3179 2023-07-09 04:22:51.000000 ncs-uml-1.2.0/ncs_uml/scripts/run.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     6206 2023-07-09 04:21:24.000000 ncs-uml-1.2.0/ncs_uml/utils.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.573629 ncs-uml-1.2.0/ncs_uml.egg-info/
+-rw-r--r--   0 kkotari    (501) staff       (20)    15420 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)      347 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/SOURCES.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/dependency_links.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       87 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/entry_points.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/requires.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/top_level.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.2.0/requirements.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-07-09 04:35:20.574708 ncs-uml-1.2.0/setup.cfg
+-rw-r--r--   0 kkotari    (501) staff       (20)     1699 2023-07-07 21:55:17.000000 ncs-uml-1.2.0/setup.py
```

### Comparing `ncs-uml-1.1.0/LICENSE` & `ncs-uml-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.1.0/PKG-INFO` & `ncs-uml-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.1.0
+Version: 1.2.0
 Summary: The ncs-uml creates plantUML files for the given YANG file and its dependencies
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
```

### Comparing `ncs-uml-1.1.0/README.md` & `ncs-uml-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.1.0/ncs_uml/main.py` & `ncs-uml-1.2.0/ncs_uml/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,17 @@
             self.util.cmd.call(f'cp -r {each}/* {self.ncs_uml}')
 
     def get_dependencies(self, file):
         dep_files = set()
         # read makefile to identify the dependency yang files
         makefile = f"{file.parent.parent}/Makefile"
         if not self.util.file.is_file(makefile):
-            msg = f"could not find Makefile in the following path: {makefile}"
-            raise FileNotFoundError(msg)
+            # msg = f"could not find Makefile in the following path: {makefile}"
+            # raise FileNotFoundError(msg)
+            return '.'
 
         mkf = self.util.make.read(makefile)
         yang_paths = mkf.get('YANGPATH', '').split()
         for each in yang_paths:
             if each == '--yangpath':
                 continue
             dep_files.add(f'{file.parent.parent}/{each}')
@@ -107,15 +108,19 @@
         self.generate_umlfile(cmd, file)
 
     def generate_umlfile(self, cmd, file):
         uml_file = f"{file.stem}.uml"
         cmd += f" -f uml {file} --path={self.ncs_uml}"
         cmd += f" --uml-no=module,import,annotation"
         if not self.opt.skip_grouping:
-            cmd += f" --uml-inline-groupings"
+            cmd += f" --uml-inline-groupings "
+        if getattr(self.opt, 'skip_module', False):
+            cmd += f"--uml-skip-module={','.join(self.opt.skip_module)} "
+        if getattr(self.opt, 'add_legend', False):
+            cmd += f"--uml-add-legend "
         cmd += f" --uml-output-directory=. 1> {uml_file} 2> /dev/null"
         self.log.debug(f"command: {cmd}")
         self.util.cmd.call(cmd)
         self.log.info(f"uml file: {uml_file}")
 
         self.clean_uml(uml_file)
         self.log.info(f"uml clean up done.")
```

### Comparing `ncs-uml-1.1.0/ncs_uml/scripts/run.py` & `ncs-uml-1.2.0/ncs_uml/scripts/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,39 @@
 #!/usr/bin/env python
 from __future__ import absolute_import
 from logging import INFO, DEBUG
 import optparse
 
 import ncs_uml
 from ncs_uml.main import NcsUml
+from ncs_uml.utils import Command
 
 
+def get_pyang_addons():
+    addl_opt = [
+        optparse.make_option("--skip-module",
+                             dest="skip_module",
+                             action="append",
+                             default=[],
+                             metavar="SKIP MODULE",
+                             help="skips given modules, i.e., --skip-module=tailf-ncs"),
+        optparse.make_option("--add-legend",
+                             dest="add_legend",
+                             action="store_true",
+                             help="Adds legend about grouping yang file in the UML"),
+    ]
+    try:
+        cmd = Command(allow_log=False)
+        help = cmd.run(['pyang', '--help'])
+        if '--uml-skip-module' in help:
+            return addl_opt
+    except Exception as e:
+        pass
+    return []
+
 def get_options():
     usage = f"""{ncs_uml.__name__} [options] [<filename>...]
 
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins."""
 
     optlist = [
@@ -35,16 +58,16 @@
                              dest="dpath",
                              default=[],
                              action="append",
                              help="dependent yang module paths"),
     ]
     optparser = optparse.OptionParser(usage, add_help_option = False)
     optparser.version = f'{ncs_uml.__name__} {ncs_uml.__version__}'
+    optlist += get_pyang_addons()
     optparser.add_options(optlist)
-
     return optparser
 
 
 def run():
     optparser = get_options()
     (o, args) = optparser.parse_args()
     uml = None
```

### Comparing `ncs-uml-1.1.0/ncs_uml/utils.py` & `ncs-uml-1.2.0/ncs_uml/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,52 +61,54 @@
 
 
 class Command(metaclass=Singleton):
     name = __name__
     stdout = subprocess.PIPE
     stderr = subprocess.PIPE
 
-    def __init__(self):
-        self.log = Logger().setup()
+    def __init__(self, allow_log=True):
+        self.allow_log = allow_log
+        if self.allow_log:
+            self.log = Logger().setup()
 
     def decode(self, args):
         return (i.decode('utf-8') for i in args)
 
     def call(self, cmd): # _run_bash_commands
-        self.log.debug("executing $ {}".format(cmd))
+        if self.allow_log: self.log.debug("executing $ {}".format(cmd))
         try:
             subprocess.call(cmd, shell=True)
-            self.log.debug("done")
+            if self.allow_log: self.log.debug("done")
         except EnvironmentError as e:
-            self.log.error("failed to run: {}".format(cmd))
-            self.log.error(e)
+            if self.allow_log: self.log.error("failed to run: {}".format(cmd))
+            if self.allow_log: self.log.error(e)
 
     def run(self, cmd, raiseError=True): # _run_command
-        self.log.debug("executing $ {}".format(cmd))
+        if self.allow_log: self.log.debug("executing $ {}".format(cmd))
         try:
             p = subprocess.Popen(
                     cmd, 
                     stdout=self.stdout,
                     stderr=self.stderr
                 )
             out, err = self.decode(p.communicate())
             if err == '' or 'env.sh' in err:
-                self.log.debug('done')
+                if self.allow_log: self.log.debug('done')
                 return out
             if raiseError:
                 if '% Total' in err:
                     return err
-                self.log.debug('validating the error')
+                if self.allow_log: self.log.debug('validating the error')
                 if 'command not found' in err or 'Unknown command' in err:
                     msg = "command `{}` not found".format(cmd)
                     raise SyntaxError(msg)
                 raise SyntaxError(err)
         except SyntaxError as e:
-            self.log.error("failed to run: {}".format(cmd))
-            self.log.error(e)
+            if self.allow_log: self.log.error("failed to run: {}".format(cmd))
+            if self.allow_log: self.log.error(e)
 
 
 class MakeFile(metaclass=Singleton):
     name = __name__
 
     def __init__(self) -> None:
         self.log = Logger().setup()
```

### Comparing `ncs-uml-1.1.0/ncs_uml.egg-info/PKG-INFO` & `ncs-uml-1.2.0/ncs_uml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.1.0
+Version: 1.2.0
 Summary: The ncs-uml creates plantUML files for the given YANG file and its dependencies
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
```

### Comparing `ncs-uml-1.1.0/setup.py` & `ncs-uml-1.2.0/setup.py`

 * *Files identical despite different names*

