# Comparing `tmp/gouge-1.5.0.post2.tar.gz` & `tmp/gouge-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gouge-1.5.0.post2.tar", last modified: Sun Jul  9 11:23:24 2023, max compression
+gzip compressed data, was "gouge-2.0.tar", last modified: Sun Jul  9 10:19:22 2023, max compression
```

## Comparing `gouge-1.5.0.post2.tar` & `gouge-2.0.tar`

### file list

```diff
@@ -1,24 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:24.045945 gouge-1.5.0.post2/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-09 11:23:24.045945 gouge-1.5.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:24.041945 gouge-1.5.0.post2/gouge/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/gouge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/gouge/colourcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/gouge/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/gouge/parseable.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/gouge/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/gouge/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:24.045945 gouge-1.5.0.post2/gouge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-09 11:23:23.000000 gouge-1.5.0.post2/gouge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-09 11:23:23.000000 gouge-1.5.0.post2/gouge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:23:23.000000 gouge-1.5.0.post2/gouge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 11:23:23.000000 gouge-1.5.0.post2/gouge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 11:23:23.000000 gouge-1.5.0.post2/gouge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-09 11:23:24.045945 gouge-1.5.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:23:24.045945 gouge-1.5.0.post2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/test/test_caplog.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/test/test_coloring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/test/test_colourcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-09 11:23:22.000000 gouge-1.5.0.post2/test/test_shifting_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.671860 gouge-2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.663860 gouge-2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.667860 gouge-2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-09 10:19:13.000000 gouge-2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-09 10:19:13.000000 gouge-2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-09 10:19:13.000000 gouge-2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-09 10:19:13.000000 gouge-2.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.667860 gouge-2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-09 10:19:13.000000 gouge-2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-09 10:19:22.671860 gouge-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-09 10:19:13.000000 gouge-2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.667860 gouge-2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:13.000000 gouge-2.0/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-09 10:19:13.000000 gouge-2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.667860 gouge-2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:13.000000 gouge-2.0/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    31000 2023-07-09 10:19:13.000000 gouge-2.0/docs/_static/snapshot1.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.667860 gouge-2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:13.000000 gouge-2.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-09 10:19:13.000000 gouge-2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-09 10:19:13.000000 gouge-2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-07-09 10:19:13.000000 gouge-2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-09 10:19:13.000000 gouge-2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-09 10:19:13.000000 gouge-2.0/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-09 10:19:13.000000 gouge-2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 10:19:22.671860 gouge-2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.663860 gouge-2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.671860 gouge-2.0/src/gouge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:13.000000 gouge-2.0/src/gouge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-09 10:19:13.000000 gouge-2.0/src/gouge/colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-09 10:19:13.000000 gouge-2.0/src/gouge/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-09 10:19:13.000000 gouge-2.0/src/gouge/parseable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:13.000000 gouge-2.0/src/gouge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.671860 gouge-2.0/src/gouge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-09 10:19:22.000000 gouge-2.0/src/gouge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-09 10:19:22.000000 gouge-2.0/src/gouge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 10:19:22.000000 gouge-2.0/src/gouge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-09 10:19:22.000000 gouge-2.0/src/gouge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 10:19:22.000000 gouge-2.0/src/gouge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:19:22.671860 gouge-2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-09 10:19:13.000000 gouge-2.0/test/test_caplog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-09 10:19:13.000000 gouge-2.0/test/test_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-09 10:19:13.000000 gouge-2.0/test/test_colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-09 10:19:13.000000 gouge-2.0/test/test_shifting_filter.py
```

### Comparing `gouge-1.5.0.post2/README.rst` & `gouge-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `gouge-1.5.0.post2/gouge/colourcli.py` & `gouge-2.0/src/gouge/colourcli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module contains everything needed to emit colourful messages on the CLI
 """
 import logging
+import sys
 from logging import Handler, LogRecord
-from typing import Any, List, Optional
+from typing import Any, List, Mapping, Optional
 
 import colorama as clr
 
 
 class Simple(logging.Formatter):
     """
     Fancy, colorised log output adding ANSI escape codes to the log output.
@@ -19,17 +20,20 @@
         is is meant to give a concise, readable output. If you need to see
         tracebacks on the console, you can override this setting using
         *show_exc*.
     """
 
     @staticmethod
     def basicConfig(
-        show_exc=True, show_threads=False, force_styling=False, show_pid=False, **kwargs
-    ):
-        # type: (bool, bool, bool, bool, Any) -> List[Handler]
+        show_exc: bool = True,
+        show_threads: bool = False,
+        force_styling: bool = False,
+        show_pid: bool = False,
+        **kwargs: Any,
+    ) -> List[Handler]:
         """
         Convenience method to have a one-liner set-up.
 
         *show_exc*, *show_threads*, *show_pid* and *force_styling* are directly
         passed to :py:class:`~.Simple`. The remaining *kwargs* are passed on to
         :py:func:`logging.basicConfig`.
 
@@ -49,47 +53,59 @@
             if not stream:
                 continue
 
             stream_name = getattr(stream, "name", None)
             if stream_name not in ("<stderr>", "<stdout>"):
                 continue
 
-            handler.setFormatter(Simple(show_exc, show_threads, show_pid=show_pid))
+            handler.setFormatter(
+                Simple(
+                    show_exc=show_exc,
+                    show_threads=show_threads,
+                    show_pid=show_pid,
+                )
+            )
             output.append(handler)
         return output
 
     def __init__(
         self,
-        show_exc=False,
-        show_threads=False,
-        fmt=None,
-        datefmt=None,
-        force_styling=False,
-        show_pid=False,
+        fmt: Optional[str] = None,
+        datefmt: Optional[str] = None,
+        style: str = "%",
+        validate: bool = True,
+        *,
+        defaults: Optional[Mapping[str, Any]] = None,
+        show_exc: bool = False,
+        show_threads: bool = False,
+        force_styling: bool = False,
+        show_pid: bool = False,
     ):
-        # type: (bool, bool, Optional[str], Optional[str], bool, bool) -> None
-        logging.Formatter.__init__(self, fmt, datefmt)
+        python_310_args = {"defaults": defaults, "validate": validate}
+        if sys.version_info < (3, 10):
+            python_310_args.pop("defaults")
+        if sys.version_info < (3, 8):
+            python_310_args.pop("validate")
+        super().__init__(fmt, datefmt, style, **python_310_args)
         self.show_threads = show_threads
         self.show_exc = show_exc
         self.force_styling = force_styling
         self.show_pid = show_pid
 
-    def colorised_exception(self, level, exc_text):
-        # type: (int, str) -> str
+    def colorised_exception(self, level: int, exc_text: str) -> str:
         """
         Colorises the exception text based on log level
         """
         if level >= logging.ERROR:
             output = "\n{f.RED}{exc_text}{s.RESET_ALL}"
         else:
             output = "\n{f.WHITE}{s.DIM}{exc_text}{s.RESET_ALL}"
         return output
 
-    def format(self, record):
-        # type: (LogRecord) -> str
+    def format(self, record: LogRecord) -> str:
         if record.levelno <= logging.DEBUG:
             colorize = clr.Style.BRIGHT + clr.Fore.BLACK
         elif record.levelno <= logging.INFO:
             colorize = clr.Fore.CYAN
         elif record.levelno <= logging.WARNING:
             colorize = clr.Fore.YELLOW
         elif record.levelno <= logging.ERROR:
@@ -106,28 +122,30 @@
             "{s.BRIGHT}[{name}]{s.RESET_ALL}",
             "{message}",
         ]
         if self.show_threads:
             message_items.insert(0, "{threadName:<10}")
 
         if self.show_pid:
-            message_items.insert(0, "{s.BRIGHT}[PID: {process:<5}]{s.RESET_ALL}")
+            message_items.insert(
+                0, "{s.BRIGHT}[PID: {process:<5}]{s.RESET_ALL}"
+            )
 
         message_template = " ".join(message_items)
 
         if self.show_exc:
             if record.exc_info:
                 # Cache the traceback text to avoid converting it multiple times
                 # (it's constant anyway)
                 exc_text = getattr(record, "exc_text", "")
                 if not exc_text:
-                    record.exc_text = self.formatException(  # type: ignore
-                        record.exc_info
-                    )
+                    record.exc_text = self.formatException(record.exc_info)
 
             exc_text = getattr(record, "exc_text", "")
             if exc_text:
-                message_template += self.colorised_exception(record.levelno, exc_text)
+                message_template += self.colorised_exception(
+                    record.levelno, exc_text
+                )
 
         return message_template.format(
             levelcolor=colorize, f=clr.Fore, s=clr.Style, **vars(record)
         )
```

### Comparing `gouge-1.5.0.post2/gouge/filters.py` & `gouge-2.0/src/gouge/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains generally useful filters.
 """
 import logging
 from typing import Set
 from warnings import warn
 
 
-class ShiftingFilter:
+class ShiftingFilter(logging.Filter):
     """
     This filter will shift the logging level of log records a certain number of
     log levels.
 
     For example:
 
     ``ShiftingFilter(1)`` will convert a message with level ``INFO`` to
@@ -39,35 +39,38 @@
     :param min: Don't shift below this level.
     :param max: Don't shift above this level.
     :param offset: An explicit, fine-grained offset value. This overrides
         *shift_by*!
     """
 
     def __init__(
-        self, shift_by=0, logger="", min=logging.NOTSET, max=logging.CRITICAL, offset=0
-    ):
-        # type: (int, str, int, int, int) -> None
+        self,
+        shift_by: int = 0,
+        logger: str = "",
+        min: int = logging.NOTSET,
+        max: int = logging.CRITICAL,
+        offset: int = 0,
+    ) -> None:
         if offset and shift_by:
             warn(
                 'You specified both "offset" and "shift_by"! "shift_by" '
                 "will be ignored!",
                 SyntaxWarning,
             )
 
         if offset:
             self.offset = offset
         else:
             self.offset = 10 * shift_by
         self.logger = logger
         self.max = max
         self.min = min
-        self.injected_loggers = set()  # type: Set[logging.Logger]
+        self.injected_loggers: Set[logging.Logger] = set()
 
-    def inject(self, parent):
-        # type: (str) -> None
+    def inject(self, parent: str) -> None:
         """
         Loop over each known logger and attach this filter.
 
         You can remove the attached filters again using
         :py:meth:`~.ShiftingFilter.cleanup`.
 
         .. note::
@@ -76,30 +79,30 @@
             logger exists before calling this! You can look at all the existing
             loggers using ``logging.Logger.manager.loggerDict``.
 
         :param parent: Attach the filter to this and all descendant loggers.
         """
         if not isinstance(parent, str):
             parent = parent.name
-        items = logging.Logger.manager.loggerDict.items()  # type: ignore
+        items = logging.Logger.manager.loggerDict.items()
         for name, logger in items:
-            if name.startswith(parent) and not isinstance(logger, logging.PlaceHolder):
+            if name.startswith(parent) and not isinstance(
+                logger, logging.PlaceHolder
+            ):
                 logger.addFilter(self)
                 self.injected_loggers.add(logger)
 
-    def cleanup(self):
-        # type: () -> None
+    def cleanup(self) -> None:
         """
         Remove all filters applied via :py:meth:`~.ShiftingFilter.inject`.
         """
         for logger in self.injected_loggers:
-            logger.removeFilter(self)  # type: ignore
+            logger.removeFilter(self)
 
-    def filter(self, record):
-        # type: (logging.LogRecord) -> bool
+    def filter(self, record: logging.LogRecord) -> bool:
         """
         Always returns *True* but will modify the logging level of *record* by
         the rules defined in this filter.
 
         See :py:meth:`logging.Filter.filter`
         """
         if record.name.startswith(self.logger):
```

### Comparing `gouge-1.5.0.post2/gouge/parseable.py` & `gouge-2.0/src/gouge/parseable.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,38 +26,36 @@
     * thread
     * threadName
     * message
     * exc_text
     """
 
     @staticmethod
-    def basicConfig(**kwargs):
-        # type: (Any) -> None
+    def basicConfig(**kwargs: Any) -> None:
         logging.basicConfig(**kwargs)
         root = logging.getLogger()
         for handler in root.handlers:
             handler.setFormatter(CSVLog())
 
-    def __init__(self, fmt=None, datefmt=None):
-        # type: (Optional[str], Optional[str]) -> None
+    def __init__(
+        self, fmt: Optional[str] = None, datefmt: Optional[str] = None
+    ) -> None:
         logging.Formatter.__init__(self, fmt, datefmt)
         self.buffer = io.StringIO()
         self.writer = csv.writer(self.buffer)
 
-    def format(self, record):
-        # type: (logging.LogRecord) -> str
-
+    def format(self, record: logging.LogRecord) -> str:
         record.message = record.getMessage()
 
         if record.exc_info:
             # Cache the traceback text to avoid converting it multiple times
             # (it's constant anyway)
             exc_text = getattr(record, "exc_text", "")
             if not exc_text:
-                record.exc_text = self.formatException(record.exc_info)  # type: ignore
+                record.exc_text = self.formatException(record.exc_info)
 
         exc_text = getattr(record, "exc_text", "")
         message_items = [
             record.created,
             record.filename,
             record.funcName,
             record.levelname,
@@ -107,39 +105,37 @@
             <threadName />
             <message />
             <exc_text />
         </record>
     """
 
     @staticmethod
-    def basicConfig(**kwargs):
-        # type: (Any) -> None
+    def basicConfig(**kwargs: Any) -> None:
         logging.basicConfig(**kwargs)
         root = logging.getLogger()
         for handler in root.handlers:
             handler.setFormatter(XMLLog())
 
-    def __init__(self, fmt=None, datefmt=None):
-        # type: (Optional[str], Optional[str]) -> None
+    def __init__(
+        self, fmt: Optional[str] = None, datefmt: Optional[str] = None
+    ) -> None:
         logging.Formatter.__init__(self, fmt, datefmt)
-        from xml.dom.minidom import Document  # type: ignore
+        from xml.dom.minidom import Document
 
         self.doc = Document()
 
-    def format(self, record):
-        # type: (logging.LogRecord) -> str
-
+    def format(self, record: logging.LogRecord) -> str:
         record.message = record.getMessage()
 
         if record.exc_info:
             # Cache the traceback text to avoid converting it multiple times
             # (it's constant anyway)
             exc_text = getattr(record, "exc_text", "")
             if not exc_text:
-                record.exc_text = self.formatException(record.exc_info)  # type: ignore
+                record.exc_text = self.formatException(record.exc_info)
 
         exc_text = getattr(record, "exc_text", "")
         message_items = [
             ("created", record.created),
             ("filename", record.filename),
             ("funcName", record.funcName),
             ("levelname", record.levelname),
@@ -159,9 +155,9 @@
         ]
 
         element = self.doc.createElement("record")
         for tagname, value in message_items:
             subelement = self.doc.createElement(tagname)
             subelement.appendChild(self.doc.createTextNode(str(value)))
             element.appendChild(subelement)
-        output = element.toxml()  # type: str
+        output: str = element.toxml()
         return output
```

### Comparing `gouge-1.5.0.post2/setup.py` & `gouge-2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,50 @@
-import sys
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
 
-from setuptools import find_packages, setup
-
-dependencies = [
-    "colorama",
+[project]
+name = "gouge"
+version = "2.0"
+authors = [
+    {name = "Michel Albert", email = "michel@albert.lu"},
 ]
-
-if sys.version_info < (3, 5):
-    dependencies.append("typing")
-
-setup(
-    name="gouge",
-    version=open("gouge/version.txt").read().strip(),
-    packages=find_packages(),
-    install_requires=dependencies,
-    requires=dependencies,
-    provides=["gouge"],
-    include_package_data=True,
-    package_data={"gouge": ["py.typed"]},
-    author="Michel Albert",
-    author_email="michel@albert.lu",
-    description="Collection of logging formatters.",
-    license="BSD",
-    url="https://github.com/exhuma/gouge",
-    classifiers=[
+description = "Collection of logging formatters."
+readme = "README.rst"
+requires-python = ">=3.7"
+license = {text = "BSD-3-Clause"}
+classifiers = [
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Topic :: Other/Nonlisted Topic",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Logging",
-    ],
-)
+]
+dependencies = [
+    "colorama",
+]
+
+[project.urls]
+Repository = "https://github.com/exhuma/gouge"
+
+[project.optional-dependencies]
+dev = [
+    "furo",
+    "types-colorama",
+]
+test = [
+    "pytest"
+]
+
+[tool.black]
+line_length = 80
+
+[tool.isort]
+profile = "black"
+line_length = 80
+virtual_env = "env"
```

### Comparing `gouge-1.5.0.post2/test/test_coloring.py` & `gouge-2.0/test/test_coloring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from logging import LogRecord
 
 import pytest
+
 from gouge.colourcli import Simple
 
 
 @pytest.mark.parametrize(
     "level,color_code",
     [
         (logging.DEBUG, "\x1b[30mDEBUG"),
```

### Comparing `gouge-1.5.0.post2/test/test_colourcli.py` & `gouge-2.0/test/test_colourcli.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,7 +55,36 @@
     """
     record = LogRecord(
         "name", logging.DEBUG, "path", 42, "message", args={}, exc_info=None
     )
     formatter = Simple(show_pid=True)
     output = formatter.format(record)
     assert re.search(r"\[PID: \d+\s*\]", output)
+
+
+def test_dictconfig():
+    """
+    Ensure that we can configure loggers with dictConfig while using gouge
+    """
+    config = {
+        "version": 1,
+        "formatters": {
+            "simple": {
+                "class": "gouge.colourcli.Simple",
+            },
+        },
+        "handlers": {
+            "console": {
+                "class": "logging.StreamHandler",
+                "formatter": "simple",
+            },
+        },
+        "loggers": {
+            "": {
+                "handlers": ["console"],
+                "level": "DEBUG",
+            },
+        },
+    }
+    import logging.config
+
+    logging.config.dictConfig(config)
```

### Comparing `gouge-1.5.0.post2/test/test_shifting_filter.py` & `gouge-2.0/test/test_shifting_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,212 @@
 import io
 import logging
-import unittest
 from functools import partial
 
+import pytest
+
 from gouge.filters import ShiftingFilter
 
 SimpleRecord = partial(
     logging.LogRecord, pathname="", lineno=0, msg="", args={}, exc_info=None
 )
 
 
-class TestShiftingFilter(unittest.TestCase):
-    def test_noshift(self):
-        """
-        A default instance should not shift anything
-        """
-        record = SimpleRecord(name="a.b.c", level=logging.DEBUG)
-        filter_ = ShiftingFilter()
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.DEBUG)
-
-    def test_noshift_unmatching(self):
-        """
-        If the name does not match, no shifting should occur.
-        """
-        filter_ = ShiftingFilter(1, "foo.bar")
-        record = SimpleRecord(name="a.b.c", level=logging.DEBUG)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.DEBUG)
-
-    def test_noshift_parent(self):
-        """
-        Parent nodes should not be shifted.
-        """
-        filter_ = ShiftingFilter(1, "a.b.c")
-        record = SimpleRecord(name="a.b", level=logging.DEBUG)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.DEBUG)
-
-    def test_shift_fullmatch(self):
-        """
-        If the name matches exactly, we should shift
-        """
-        filter_ = ShiftingFilter(1, "a.b.c")
-        record = SimpleRecord(name="a.b.c", level=logging.DEBUG)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.INFO)
-
-    def test_shift_child(self):
-        """
-        Child nodes should be shifted
-        """
-        filter_ = ShiftingFilter(1, "a.b.c")
-        record = SimpleRecord(name="a.b.c.d.e", level=logging.DEBUG)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.INFO)
-
-    def test_shift_reversed(self):
-        """
-        We should also allow shifting in reverse.
-        """
-        filter_ = ShiftingFilter(-1)
-        record = SimpleRecord(name="a.b.c", level=logging.INFO)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.DEBUG)
-
-    def test_shift_fine_grained(self):
-        """
-        Instead of shifting by levels, the user should be allowed to shift by an
-        exact offset.
-        """
-        filter_ = ShiftingFilter(offset=2)
-        record = SimpleRecord(name="a.b.c", level=logging.NOTSET)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, 2)
-
-    def test_shift_min(self):
-        """
-        We should never go below level.NOTSET
-        """
-        filter_ = ShiftingFilter(-1)
-        record = SimpleRecord(name="a.b.c", level=logging.NOTSET)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.NOTSET)
-
-    def test_shift_max(self):
-        """
-        We also stop above logging.CRITICAL
-        """
-        filter_ = ShiftingFilter(1)
-        record = SimpleRecord(name="a.b.c", level=logging.CRITICAL)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.CRITICAL)
-
-    def test_shift_custom_min(self):
-        """
-        The user should have the option to refuse shifting below a certain
-        level.
-        """
-        filter_ = ShiftingFilter(-1, min=logging.INFO)
-        record = SimpleRecord(name="a.b.c", level=logging.INFO)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.INFO)
-
-    def test_shift_custom_max(self):
-        """
-        The user should have the option to refuse shifting above a certain
-        level.
-        """
-        filter_ = ShiftingFilter(1, max=logging.ERROR)
-        record = SimpleRecord(name="a.b.c", level=logging.ERROR)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, logging.ERROR)
-
-    def test_shift_custom_min_outside_bounds(self):
-        """
-        We allow specifying a custom min value outside of the "standard" bounds.
-        """
-        filter_ = ShiftingFilter(-1, min=-10)
-        record = SimpleRecord(name="a.b.c", level=logging.NOTSET)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, -10)
-
-    def test_shift_custom_max_outside_bounds(self):
-        """
-        We allow specifying a custom max value outside of the "standard" bounds.
-        """
-        filter_ = ShiftingFilter(1, max=60)
-        record = SimpleRecord(name="a.b.c", level=logging.CRITICAL)
-        filter_.filter(record)
-        self.assertEqual(record.levelno, 60)
-
-
-class TestLoggingWithFilter(unittest.TestCase):
-    def tearDown(self):
+@pytest.fixture
+def reset_logging():
+    try:
+        yield
+    finally:
         logging.shutdown()
         for logger in logging.Logger.manager.loggerDict.values():
             if isinstance(logger, logging.PlaceHolder):
                 continue
             del logger.handlers[:]
             del logger.filters[:]
 
-    def test_attached_to_handler(self):
-        blob = io.StringIO()
-        handler = logging.StreamHandler(blob)
-        handler.setFormatter(logging.Formatter("%(levelno)s %(levelname)s %(msg)s"))
-        handler.addFilter(ShiftingFilter(-1))
-        logger_c = logging.getLogger("a.b.c")
-        logger_d = logging.getLogger("a.b.d")
-        logger_parent = logging.getLogger("a")
-        logger_parent.setLevel(logging.DEBUG)
-        logger_parent.addHandler(handler)
-
-        logger_c.error("error - c")
-        logger_d.info("info - d")
-        logger_d.debug("debug - d")
-
-        lines = blob.getvalue().splitlines()
-
-        expected = [
-            "30 WARNING error - c",
-            "10 DEBUG info - d",
-            "0 NOTSET debug - d",
-        ]
-        self.assertEqual(lines, expected)
-
-    def test_attached_to_logger(self):
-        blob = io.StringIO()
-        handler = logging.StreamHandler(blob)
-        handler.setFormatter(logging.Formatter("%(levelno)s %(levelname)s %(msg)s"))
-
-        logger_c = logging.getLogger("a.b.c")
-        logger_d = logging.getLogger("a.b.d")
-        logger_parent = logging.getLogger("a")
-        logger_parent.setLevel(logging.DEBUG)
-        logger_parent.addHandler(handler)
-
-        filter = ShiftingFilter(-1)
-        filter.inject("a")
-
-        logger_c.error("error - c")
-        logger_d.info("info - d")
-        logger_d.debug("debug - d")
-
-        filter.cleanup()
-
-        lines = blob.getvalue().splitlines()
-
-        expected = [
-            "30 WARNING error - c",
-            "10 DEBUG info - d",
-            "0 NOTSET debug - d",
-        ]
-        self.assertEqual(lines, expected)
+
+def test_noshift():
+    """
+    A default instance should not shift anything
+    """
+    record = SimpleRecord(name="a.b.c", level=logging.DEBUG)
+    filter_ = ShiftingFilter()
+    filter_.filter(record)
+    assert record.levelno == logging.DEBUG
+
+
+def test_noshift_unmatching():
+    """
+    If the name does not match, no shifting should occur.
+    """
+    filter_ = ShiftingFilter(1, "foo.bar")
+    record = SimpleRecord(name="a.b.c", level=logging.DEBUG)
+    filter_.filter(record)
+    assert record.levelno == logging.DEBUG
+
+
+def test_noshift_parent():
+    """
+    Parent nodes should not be shifted.
+    """
+    filter_ = ShiftingFilter(1, "a.b.c")
+    record = SimpleRecord(name="a.b", level=logging.DEBUG)
+    filter_.filter(record)
+    assert record.levelno == logging.DEBUG
+
+
+def test_shift_fullmatch():
+    """
+    If the name matches exactly, we should shift
+    """
+    filter_ = ShiftingFilter(1, "a.b.c")
+    record = SimpleRecord(name="a.b.c", level=logging.DEBUG)
+    filter_.filter(record)
+    assert record.levelno == logging.INFO
+
+
+def test_shift_child():
+    """
+    Child nodes should be shifted
+    """
+    filter_ = ShiftingFilter(1, "a.b.c")
+    record = SimpleRecord(name="a.b.c.d.e", level=logging.DEBUG)
+    filter_.filter(record)
+    assert record.levelno == logging.INFO
+
+
+def test_shift_reversed():
+    """
+    We should also allow shifting in reverse.
+    """
+    filter_ = ShiftingFilter(-1)
+    record = SimpleRecord(name="a.b.c", level=logging.INFO)
+    filter_.filter(record)
+    assert record.levelno == logging.DEBUG
+
+
+def test_shift_fine_grained():
+    """
+    Instead of shifting by levels, the user should be allowed to shift by an
+    exact offset.
+    """
+    filter_ = ShiftingFilter(offset=2)
+    record = SimpleRecord(name="a.b.c", level=logging.NOTSET)
+    filter_.filter(record)
+    assert record.levelno == 2
+
+
+def test_shift_min():
+    """
+    We should never go below level.NOTSET
+    """
+    filter_ = ShiftingFilter(-1)
+    record = SimpleRecord(name="a.b.c", level=logging.NOTSET)
+    filter_.filter(record)
+    assert record.levelno == logging.NOTSET
+
+
+def test_shift_max():
+    """
+    We also stop above logging.CRITICAL
+    """
+    filter_ = ShiftingFilter(1)
+    record = SimpleRecord(name="a.b.c", level=logging.CRITICAL)
+    filter_.filter(record)
+    assert record.levelno == logging.CRITICAL
+
+
+def test_shift_custom_min():
+    """
+    The user should have the option to refuse shifting below a certain
+    level.
+    """
+    filter_ = ShiftingFilter(-1, min=logging.INFO)
+    record = SimpleRecord(name="a.b.c", level=logging.INFO)
+    filter_.filter(record)
+    assert record.levelno == logging.INFO
+
+
+def test_shift_custom_max():
+    """
+    The user should have the option to refuse shifting above a certain
+    level.
+    """
+    filter_ = ShiftingFilter(1, max=logging.ERROR)
+    record = SimpleRecord(name="a.b.c", level=logging.ERROR)
+    filter_.filter(record)
+    assert record.levelno == logging.ERROR
+
+
+def test_shift_custom_min_outside_bounds():
+    """
+    We allow specifying a custom min value outside of the "standard" bounds.
+    """
+    filter_ = ShiftingFilter(-1, min=-10)
+    record = SimpleRecord(name="a.b.c", level=logging.NOTSET)
+    filter_.filter(record)
+    assert record.levelno == -10
+
+
+def test_shift_custom_max_outside_bounds():
+    """
+    We allow specifying a custom max value outside of the "standard" bounds.
+    """
+    filter_ = ShiftingFilter(1, max=60)
+    record = SimpleRecord(name="a.b.c", level=logging.CRITICAL)
+    filter_.filter(record)
+    assert record.levelno == 60
+
+
+def test_attached_to_handler(reset_logging):
+    blob = io.StringIO()
+    handler = logging.StreamHandler(blob)
+    handler.setFormatter(logging.Formatter("%(levelno)s %(levelname)s %(msg)s"))
+    handler.addFilter(ShiftingFilter(-1))
+    logger_c = logging.getLogger("a.b.c")
+    logger_d = logging.getLogger("a.b.d")
+    logger_parent = logging.getLogger("a")
+    logger_parent.setLevel(logging.DEBUG)
+    logger_parent.addHandler(handler)
+
+    logger_c.error("error - c")
+    logger_d.info("info - d")
+    logger_d.debug("debug - d")
+
+    lines = blob.getvalue().splitlines()
+
+    expected = [
+        "30 WARNING error - c",
+        "10 DEBUG info - d",
+        "0 NOTSET debug - d",
+    ]
+    assert lines == expected
+
+
+def test_attached_to_logger(reset_logging):
+    blob = io.StringIO()
+    handler = logging.StreamHandler(blob)
+    handler.setFormatter(logging.Formatter("%(levelno)s %(levelname)s %(msg)s"))
+
+    logger_c = logging.getLogger("a.b.c")
+    logger_d = logging.getLogger("a.b.d")
+    logger_parent = logging.getLogger("a")
+    logger_parent.setLevel(logging.DEBUG)
+    logger_parent.addHandler(handler)
+
+    filter = ShiftingFilter(-1)
+    filter.inject("a")
+
+    logger_c.error("error - c")
+    logger_d.info("info - d")
+    logger_d.debug("debug - d")
+
+    filter.cleanup()
+
+    lines = blob.getvalue().splitlines()
+
+    expected = [
+        "30 WARNING error - c",
+        "10 DEBUG info - d",
+        "0 NOTSET debug - d",
+    ]
+    assert lines == expected
```

