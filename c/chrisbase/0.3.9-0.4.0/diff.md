# Comparing `tmp/chrisbase-0.3.9.tar.gz` & `tmp/chrisbase-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisbase-0.3.9.tar", last modified: Thu Jun 29 13:53:46 2023, max compression
+gzip compressed data, was "chrisbase-0.4.0.tar", last modified: Sun Jul  9 15:13:02 2023, max compression
```

## Comparing `chrisbase-0.3.9.tar` & `chrisbase-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.140365 chrisbase-0.3.9/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-06-29 13:39:47.000000 chrisbase-0.3.9/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-06-29 13:53:46.140365 chrisbase-0.3.9/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-06-29 13:39:47.000000 chrisbase-0.3.9/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-06-29 13:39:47.000000 chrisbase-0.3.9/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      956 2023-06-29 13:53:46.140365 chrisbase-0.3.9/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.136366 chrisbase-0.3.9/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.136366 chrisbase-0.3.9/src/chrisbase/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    23190 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/io.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/morp.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/time.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5122 2023-06-29 13:39:47.000000 chrisbase-0.3.9/src/chrisbase/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-29 13:53:46.140365 chrisbase-0.3.9/src/chrisbase.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      431 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      138 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-06-29 13:53:46.000000 chrisbase-0.3.9/src/chrisbase.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-29 13:53:45.000000 chrisbase-0.3.9/src/chrisbase.egg-info/zip-safe
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1066 2023-07-08 17:51:01.000000 chrisbase-0.4.0/LICENSE
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      816 2023-07-09 15:13:02.541626 chrisbase-0.4.0/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      286 2023-07-08 17:51:01.000000 chrisbase-0.4.0/README.md
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       81 2023-07-08 17:51:01.000000 chrisbase-0.4.0/pyproject.toml
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      961 2023-07-09 15:13:02.541626 chrisbase-0.4.0/setup.cfg
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/src/
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/src/chrisbase/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        0 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/__init__.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      151 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/cli.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)    24356 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/io.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     2170 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/morp.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     1059 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/time.py
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)     5122 2023-07-08 17:51:01.000000 chrisbase-0.4.0/src/chrisbase/util.py
+drwxr-xr-x   0 chrisjihee (1000016) users    (1000001)        0 2023-07-09 15:13:02.541626 chrisbase-0.4.0/src/chrisbase.egg-info/
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      816 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/PKG-INFO
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      431 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       48 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/entry_points.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)      143 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/requires.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)       10 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/top_level.txt
+-rw-r--r--   0 chrisjihee (1000016) users    (1000001)        1 2023-07-09 15:13:02.000000 chrisbase-0.4.0/src/chrisbase.egg-info/zip-safe
```

### Comparing `chrisbase-0.3.9/LICENSE` & `chrisbase-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.9/PKG-INFO` & `chrisbase-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.3.9
+Version: 0.4.0
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrisbase-0.3.9/setup.cfg` & `chrisbase-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrisbase
-version = 0.3.9
+version = 0.4.0
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrisbase
 description = A base tool for python programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -18,15 +18,15 @@
 [options]
 zip_safe = True
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
-	typer
+	typer[all]
 	tqdm
 	numpy
 	scipy
 	pandas
 	pymongo
 	tabulate
 	chrisdict
```

### Comparing `chrisbase-0.3.9/src/chrisbase/io.py` & `chrisbase-0.4.0/src/chrisbase/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import json
+import logging
 import os
 import shutil
 import socket
 import subprocess
 import sys
 import traceback
 import warnings
-from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from itertools import chain
 from logging import getLogger
 from pathlib import Path
-from sys import stdout
 from time import sleep
 from typing import Optional, Iterable
 
 import pandas as pd
 from chrisdict import AttrDict
-from dataclasses_json import DataClassJsonMixin
 from tabulate import tabulate
 
-from chrisbase.time import from_timestamp, now, str_delta
+from chrisbase.time import from_timestamp, str_delta
 from chrisbase.util import tupled, SP, NO, OX
 
+logger = logging.getLogger(__name__)
 sys_stdout = sys.stdout
 sys_stderr = sys.stderr
 
 
+class LoggingFormat:
+    CHECK: str = ' ┇ '.join(['%(asctime)s', '%(levelname)-8s', '%(name)48s', '%(message)s'])
+    DEBUG: str = ' ┇ '.join(['%(pathname)120s:%(lineno)-5d', '%(asctime)s', '%(levelname)-8s', '%(name)48s', '%(message)s'])
+
+
 def cwd(path=None) -> Path:
     if not path:
         return Path.cwd()
     else:
         os.chdir(path)
         return Path(path)
 
@@ -70,14 +74,16 @@
         for call_stack in get_call_stack():
             if call_stack['name'] == '<module>':
                 return Path(call_stack['file'])
         raise RuntimeError("Cannot find current path")
 
 
 def hr(c="=", w=137, t=0, b=0):
+    # w=137-26 : %(asctime)s %(levelname)-8s %(message)s
+    # w=137-47 : %(asctime)s %(levelname)-8s %(filename)15s:%(lineno)-4d %(message)s
     # w=137 (for ipynb on Chrome using D2Coding 13pt) with scroll
     # w=139 (for ipynb on Chrome using D2Coding 13pt) without scroll
     # w=165 (for ipynb on GitHub using D2Coding 13pt)
     return "\n" * t + c * w + "\n" * b
 
 
 def file_hr(*args, file=sys_stdout, c=None, ct=None, cb=None, title=None, sleep_sec=0.0, **kwargs):
@@ -104,29 +110,33 @@
     file_hr(*args, file=sys_stdout, **kwargs)
 
 
 def err_hr(*args, **kwargs):
     file_hr(*args, file=sys_stderr, **kwargs)
 
 
-def file_table(tabular_data, headers=(), tablefmt="pipe", showindex="default", transposed_df=False, file=sys_stdout, **kwargs):
+def str_table(tabular_data, headers=(), tablefmt="pipe", showindex="default", transposed_df=False, **kwargs):
     if not headers and isinstance(tabular_data, pd.DataFrame):
         if showindex is True or showindex == "default" or showindex == "always" or \
                 not isinstance(showindex, str) and isinstance(showindex, Iterable) and len(showindex) != len(tabular_data):
             if transposed_df:
                 if isinstance(tabular_data.columns, pd.RangeIndex):
                     headers = ['key'] + list(map(str(range(1, len(tabular_data.columns) + 1))))
                 else:
                     headers = ['key'] + list(tabular_data.columns)
             else:
                 headers = ['#'] + list(tabular_data.columns)
                 showindex = range(1, len(tabular_data) + 1)
         else:
             headers = tabular_data.columns
-    print(tabulate(tabular_data, headers=headers, tablefmt=tablefmt, showindex=showindex, **kwargs), file=file)
+    return tabulate(tabular_data, headers=headers, tablefmt=tablefmt, showindex=showindex, **kwargs)
+
+
+def file_table(*args, file=sys_stdout, **kwargs):
+    print(str_table(*args, **kwargs), file=file)
 
 
 def out_table(*args, **kwargs):
     file_table(*args, file=sys_stdout, **kwargs)
 
 
 def err_table(*args, **kwargs):
@@ -167,15 +177,15 @@
             flush_or(self.preout, self.preerr, sec=self.flush_sec if self.flush_sec else None)
             sys.stdout = self.stdout
             sys.stderr = self.stderr
         except Exception as e:
             print(f"[MuteStd.__enter__()] [{type(e)}] {e}", file=sys_stderr)
             exit(11)
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
         try:
             flush_or(self.stdout, self.stderr, sec=self.flush_sec if self.flush_sec else None)
             if self.mute_logger:
                 for x in self.mute_logger:
                     x.disabled = False
                     x.propagate = True
             if self.mute_warning:
@@ -187,107 +197,98 @@
         except Exception as e:
             print(f"[MuteStd.__exit__()] [{type(e)}] {e}", file=sys_stderr)
             exit(22)
 
 
 class JobTimer:
     def __init__(self, name=None, prefix=None, postfix=None, verbose=False, mt=0, mb=0, pt=0, pb=0, rt=0, rb=0, rc='-',
-                 file=stdout, flush_sec=None, mute_logger=None, mute_warning=None):
-        self.mute = open(os.devnull, 'w')
+                 flush_sec=None, mute_loggers=None, mute_warning=None):
         self.name = name
         self.prefix = prefix if prefix and len(prefix) > 0 else None
         self.postfix = postfix if postfix and len(postfix) > 0 else None
         self.flush_sec = flush_sec
         self.mt: int = mt
         self.mb: int = mb
         self.pt: int = pt
         self.pb: int = pb
         self.rt: int = rt
         self.rb: int = rb
         self.rc: str = rc
-        self.file = self.mute if not verbose else file or self.mute
-        self.preout = sys.stdout
-        self.preerr = sys.stderr
-        assert isinstance(mute_logger, (type(None), str, list, tuple, set))
+        self.verbose: bool = verbose
+        assert isinstance(mute_loggers, (type(None), str, list, tuple, set))
         assert isinstance(mute_warning, (type(None), str, list, tuple, set))
-        self.mute_logger = tupled(mute_logger)
+        self.mute_loggers = tupled(mute_loggers)
         self.mute_warning = tupled(mute_warning)
-        self.verbose: bool = verbose
         self.t1: Optional[datetime] = datetime.now()
         self.t2: Optional[datetime] = datetime.now()
         self.td: Optional[timedelta] = self.t2 - self.t1
 
     def __enter__(self):
         try:
-            self.mute_logger = [getLogger(x) for x in self.mute_logger] if self.mute_logger else None
-            if self.mute_logger:
-                for x in self.mute_logger:
+            self.mute_loggers = [getLogger(x) for x in self.mute_loggers] if self.mute_loggers else None
+            if self.mute_loggers:
+                for x in self.mute_loggers:
                     x.disabled = True
                     x.propagate = False
             if self.mute_warning:
                 for x in self.mute_warning:
                     warnings.filterwarnings('ignore', category=UserWarning, module=x)
-            flush_or(self.preout, self.preerr, sec=self.flush_sec if self.flush_sec else None)
-            sys.stdout = self.file
-            sys.stderr = self.file
+            flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
             if self.verbose:
                 if self.mt > 0:
                     for _ in range(self.mt):
-                        print(file=self.file)
+                        logger.info('')
                 if self.rt > 0:
                     for _ in range(self.rt):
-                        file_hr(c=self.rc, file=self.file)
+                        logger.info(hr(c=self.rc))
                 if self.name:
-                    print(f'{now()} {self.prefix + SP if self.prefix else NO}[INIT] {self.name}{SP + self.postfix if self.postfix else NO}', file=self.file)
+                    logger.info(f'{self.prefix + SP if self.prefix else NO}[INIT] {self.name}{SP + self.postfix if self.postfix else NO}')
                     if self.rt > 0:
                         for _ in range(self.rt):
-                            file_hr(c=self.rc, file=self.file)
+                            logger.info(hr(c=self.rc))
                 if self.pt > 0:
                     for _ in range(self.pt):
-                        print(file=self.file)
+                        logger.info('')
                 flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
             self.t1 = datetime.now()
             return self
         except Exception as e:
-            print(f"[MyTimer.__enter__()] [{type(e)}] {e}", file=sys_stderr)
+            logger.error(f"[JobTimer.__enter__()] [{type(e)}] {e}")
             exit(11)
 
     def __exit__(self, exc_type=None, exc_val=None, exc_tb=None):
         try:
             self.t2 = datetime.now()
             self.td = self.t2 - self.t1
             flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
             if self.verbose:
                 if self.pb > 0:
                     for _ in range(self.pb):
-                        print(file=self.file)
+                        logger.info('')
                 if self.rb > 0:
                     for _ in range(self.rb):
-                        file_hr(c=self.rc, file=self.file)
+                        logger.info(hr(c=self.rc))
                 if self.name:
-                    print(f'{now()} {self.prefix + SP if self.prefix else NO}[EXIT] {self.name}{SP + self.postfix if self.postfix else NO} ($={str_delta(self.td)})', file=self.file)
+                    logger.info(f'{self.prefix + SP if self.prefix else NO}[EXIT] {self.name}{SP + self.postfix if self.postfix else NO} ($={str_delta(self.td)})')
                     if self.rb > 0:
                         for _ in range(self.rb):
-                            file_hr(c=self.rc, file=self.file)
+                            logger.info(hr(c=self.rc))
                 if self.mb > 0:
                     for _ in range(self.mb):
-                        print(file=self.file)
+                        logger.info('')
                 flush_or(sys.stdout, sys.stderr, sec=self.flush_sec if self.flush_sec else None)
-            if self.mute_logger:
-                for x in self.mute_logger:
+            if self.mute_loggers:
+                for x in self.mute_loggers:
                     x.disabled = False
                     x.propagate = True
             if self.mute_warning:
                 for x in self.mute_warning:
                     warnings.filterwarnings('default', category=UserWarning, module=x)
-            sys.stdout = self.preout
-            sys.stderr = self.preerr
-            self.mute.close()
         except Exception as e:
-            print(f"[MyTimer.__exit__()] [{type(e)}] {e}", file=sys_stderr)
+            logger.error(f"[JobTimer.__exit__()] [{type(e)}] {e}")
             exit(22)
 
 
 def exists_or(path):
     path = Path(path)
     return path if path.exists() else None
 
@@ -657,30 +658,52 @@
 def environ_to_dataframe(max_value_len=200, columns=None):
     from chrisbase.util import to_dataframe
     return to_dataframe(copy_dict(dict(os.environ),
                                   keys=[x for x in sorted(os.environ.keys()) if len(str(os.environ[x])) <= max_value_len]),
                         columns=columns)
 
 
-@dataclass
-class ProjectEnv(DataClassJsonMixin):
-    project: str = field()
-    hostname: str = field(init=False)
-    hostaddr: str = field(init=False)
-    python_path: Path = field(init=False)
-    working_path: Path = field(init=False)
-    running_file: Path = field(init=False)
-    logging_file: Path = field(default="logger.out")
-    argument_file: Path = field(default="arguments.json")
-
-    def __post_init__(self):
-        assert self.project, "Project name must be provided"
-        self.hostname = get_hostname()
-        self.hostaddr = get_hostaddr()
-        self.python_path = Path(sys.executable)
-        self.running_file = running_file()
-        self.project_path = first_or([x for x in self.running_file.parents if x.name.startswith(self.project)])
-        assert self.project_path, f"Could not find project path for {self.project} in {', '.join([str(x) for x in self.running_file.parents])}"
-        self.working_path = cwd(self.project_path)
-        self.running_file = self.running_file.relative_to(self.working_path)
-        self.logging_file = Path(self.logging_file)
-        self.argument_file = Path(self.argument_file)
+def configure_unit_logger(level=logging.INFO, force=True,
+                          stream=sys_stdout, filename=None, filemode="a", existing_content=None,
+                          fmt=logging.BASIC_FORMAT, datefmt="[%m.%d %H:%M:%S]"):
+    formatter = logging.Formatter(fmt=fmt, datefmt=datefmt)
+    handlers = make_logging_handlers(formatter=formatter, stream=stream, filename=filename, filemode=filemode, existing_content=existing_content)[-1:]
+    logging.basicConfig(level=level, force=force, handlers=handlers)
+    update_existing_handlers(handlers=handlers)
+
+
+def configure_dual_logger(level=logging.INFO, force=True,
+                          stream=sys_stdout, filename="running.log", filemode="a", existing_content=None,
+                          fmt=logging.BASIC_FORMAT, datefmt="[%m.%d %H:%M:%S]"):
+    formatter = logging.Formatter(fmt=fmt, datefmt=datefmt)
+    handlers = make_logging_handlers(formatter=formatter, stream=stream, filename=filename, filemode=filemode, existing_content=existing_content)
+    logging.basicConfig(level=level, force=force, handlers=handlers)
+    update_existing_handlers(handlers=handlers)
+
+
+def make_logging_handlers(formatter, stream, filename, filemode, existing_content=None):
+    handlers = []
+    if stream:
+        h = logging.StreamHandler(stream=stream)
+        h.setFormatter(formatter)
+        handlers.append(h)
+    if filename and filemode:
+        h = logging.FileHandler(filename=make_parent_dir(filename), mode=filemode, encoding="utf-8")
+        h.setFormatter(formatter)
+        handlers.append(h)
+        if existing_content:
+            h.stream.write(existing_content)
+    assert len(handlers) > 0, f"Empty handlers: filename={filename}, filemode={filemode}, stream={stream}"
+    return handlers
+
+
+def update_existing_handlers(handlers):
+    for x in logging.Logger.manager.loggerDict.values():
+        if isinstance(x, logging.Logger):
+            if len(x.handlers) > 0:
+                for h in x.handlers:
+                    if isinstance(h, logging.FileHandler):
+                        h.stream.close()
+                    x.removeHandler(h)
+                for h in handlers:
+                    x.addHandler(h)
+                logger.debug(f"logging.getLogger({x.name:<20s}) = Logger(level={x.level}, handlers={x.handlers}, disabled={x.disabled}, propagate={x.propagate}, parent={x.parent})")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chrisbase-0.3.9/src/chrisbase/morp.py` & `chrisbase-0.4.0/src/chrisbase/morp.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.9/src/chrisbase/time.py` & `chrisbase-0.4.0/src/chrisbase/time.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.9/src/chrisbase/util.py` & `chrisbase-0.4.0/src/chrisbase/util.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.9/src/chrisbase.egg-info/PKG-INFO` & `chrisbase-0.4.0/src/chrisbase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.3.9
+Version: 0.4.0
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

