# Comparing `tmp/inline_snapshot-0.2.0.tar.gz` & `tmp/inline_snapshot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.2.0.tar", max compression
+gzip compressed data, was "inline_snapshot-0.2.1.tar", max compression
```

## Comparing `inline_snapshot-0.2.0.tar` & `inline_snapshot-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.2.0/LICENSE
--rw-r--r--   0        0        0     2053 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/README.md
--rw-r--r--   0        0        0       62 2023-06-20 18:24:16.714717 inline_snapshot-0.2.0/inline_snapshot/__init__.py
--rw-r--r--   0        0        0      121 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/_format.py
--rw-r--r--   0        0        0    14391 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0     5497 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0     5445 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     1603 2023-06-20 18:24:32.250870 inline_snapshot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 inline_snapshot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2053 2023-06-20 18:24:23.890787 inline_snapshot-0.2.1/README.md
+-rw-r--r--   0        0        0       62 2023-06-20 18:24:16.714717 inline_snapshot-0.2.1/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-09 13:33:21.148429 inline_snapshot-0.2.1/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    14708 2023-07-09 13:33:21.148429 inline_snapshot-0.2.1/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0     5448 2023-07-09 13:33:21.148429 inline_snapshot-0.2.1/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0     5445 2023-06-20 18:24:23.890787 inline_snapshot-0.2.1/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     1620 2023-07-09 13:34:15.181578 inline_snapshot-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3433 1970-01-01 00:00:00.000000 inline_snapshot-0.2.1/PKG-INFO
```

### Comparing `inline_snapshot-0.2.0/LICENSE` & `inline_snapshot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.2.0/README.md` & `inline_snapshot-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.2.0/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.2.1/inline_snapshot/_inline_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import ast
 import contextlib
 import inspect
 import io
 import token
 import tokenize
+from pathlib import Path
 from typing import Any
 from typing import Dict  # noqa
 from typing import overload
 from typing import Tuple  # noqa
 from typing import TypeVar
 
 from executing import Source
 
-from ._format import format
+from ._format import format_code
 from ._rewrite_code import ChangeRecorder
 from ._rewrite_code import end_of
 from ._rewrite_code import start_of
 
 
 # sentinels
 class Undefined:
@@ -472,44 +473,50 @@
     """Write string literal value with a best effort attempt to avoid
     backslashes."""
     string, quote_types = _str_literal_helper(string, quote_types=['"""', "'''"])
     quote_type = quote_types[0]
     return f"{quote_type}{string}{quote_type}"
 
 
-def value_to_token(value):
-    input = io.StringIO(format(repr(value)))
-
-    def map_string(tok):
-        """Convert strings with newlines in triple quoted strings."""
-        if tok.type == token.STRING:
-            s = ast.literal_eval(tok.string)
-            if isinstance(s, str) and "\n" in s:
-                # unparse creates a triple quoted string here,
-                # because it thinks that the string should be a docstring
-                tripple_quoted_string = triple_quote(s)
-
-                assert ast.literal_eval(tripple_quoted_string) == s
-
-                return tok.type, tripple_quoted_string
-
-        return (tok.type, tok.string)
-
-    return [
-        map_string(t)
-        for t in tokenize.generate_tokens(input.readline)
-        if t.type not in ignore_tokens
-    ]
-
-
 class Snapshot:
     def __init__(self, value, expr):
         self._expr = expr
         self._value = Value(value)
 
+    @property
+    def _filename(self):
+        return self._expr.source.filename
+
+    def _format(self, text):
+        return format_code(text, Path(self._filename))
+
+    def _value_to_token(self, value):
+        input = io.StringIO(self._format(repr(value)))
+
+        def map_string(tok):
+            """Convert strings with newlines in triple quoted strings."""
+            if tok.type == token.STRING:
+                s = ast.literal_eval(tok.string)
+                if isinstance(s, str) and "\n" in s:
+                    # unparse creates a triple quoted string here,
+                    # because it thinks that the string should be a docstring
+                    tripple_quoted_string = triple_quote(s)
+
+                    assert ast.literal_eval(tripple_quoted_string) == s
+
+                    return tok.type, tripple_quoted_string
+
+            return (tok.type, tok.string)
+
+        return [
+            map_string(t)
+            for t in tokenize.generate_tokens(input.readline)
+            if t.type not in ignore_tokens
+        ]
+
     def _change(self):
         assert self._expr is not None
 
         change = ChangeRecorder.current.new_change()
 
         tokens = list(self._expr.source.asttokens().get_tokens(self._expr.node))
         assert tokens[0].string == "snapshot"
@@ -525,20 +532,22 @@
             or _update_flags.create
             and self._value._needs_create
             or _update_flags.trim
             and self._value._needs_trim
         ):
             new_value = self._value.get_result(_update_flags)
 
-            text = format(tokenize.untokenize(value_to_token(new_value))).strip()
+            text = self._format(
+                tokenize.untokenize(self._value_to_token(new_value))
+            ).strip()
 
             change.replace(
                 (end_of(tokens[1]), start_of(tokens[-1])),
                 text,
-                filename=self._expr.source.filename,
+                filename=self._filename,
             )
 
     def _current_tokens(self):
         return [
             (t.type, t.string)
             for t in self._expr.source.asttokens().get_tokens(self._expr.node.args[0])
             if t.type not in ignore_tokens
@@ -553,12 +562,12 @@
             s.add("trim")
         if self._value._needs_create():
             s.add("create")
 
         if (
             "create" not in s
             and self._expr is not None
-            and self._current_tokens() != value_to_token(self._value._old_value)
+            and self._current_tokens() != self._value_to_token(self._value._old_value)
         ):
             s.add("update")
 
         return s
```

### Comparing `inline_snapshot-0.2.0/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.2.1/inline_snapshot/_rewrite_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 from collections import defaultdict
 from dataclasses import dataclass
 
 import asttokens.util
 from asttokens import LineNumbers
 
-from ._format import format
+from ._format import format_code
 
 try:
     from itertools import pairwise
 except ImportError:
     from itertools import tee
 
     def pairwise(iterable):  # type: ignore
@@ -136,22 +136,20 @@
         apply."""
         replacements = list(self.replacements)
         replacements.sort()
 
         for r in replacements:
             assert r.range.start <= r.range.end
 
-        # TODO check for overlapping replacements
         for lhs, rhs in pairwise(replacements):
             assert lhs.range.end <= rhs.range.start
 
-        with open(self.filename, newline="") as code:
-            code = code.read()
+        code = self.filename.read_text()
 
-        is_formatted = code == format(code)
+        is_formatted = code == format_code(code, self.filename)
 
         line_numbers = LineNumbers(code)
 
         new_code = asttokens.util.replace(
             code,
             [
                 (
@@ -160,15 +158,15 @@
                     r.text,
                 )
                 for r in replacements
             ],
         )
 
         if is_formatted:
-            new_code = format(new_code)
+            new_code = format_code(new_code, self.filename)
 
         return new_code
 
 
 class ChangeRecorder:
     current: ChangeRecorder
```

### Comparing `inline_snapshot-0.2.0/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.2.1/inline_snapshot/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.2.0/pyproject.toml` & `inline_snapshot-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,20 @@
   "Framework :: Pytest"
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 asttokens = "^2.0.5"
 black = "^23.3.0"
+click = "^8.1.4"
 executing = "^1.2.0"
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.3"
 coverage-enable-subprocess = "^1.0"
 hypothesis = "^6.75.5"
```

### Comparing `inline_snapshot-0.2.0/PKG-INFO` & `inline_snapshot-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.2.0
+Version: 0.2.1
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: asttokens (>=2.0.5,<3.0.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: executing (>=1.2.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/15r10nk/inline-snapshots/issues
 Project-URL: Repository, https://github.com/15r10nk/inline-snapshots
 Description-Content-Type: text/markdown
 
 # inline-snapshot
```

