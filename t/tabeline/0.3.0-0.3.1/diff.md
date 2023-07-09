# Comparing `tmp/tabeline-0.3.0.tar.gz` & `tmp/tabeline-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabeline-0.3.0.tar", max compression
+gzip compressed data, was "tabeline-0.3.1.tar", max compression
```

## Comparing `tabeline-0.3.0.tar` & `tabeline-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1062 2023-06-28 10:08:20.880692 tabeline-0.3.0/LICENSE
--rw-r--r--   0        0        0     1708 2023-04-26 09:54:10.670471 tabeline-0.3.0/README.md
--rw-r--r--   0        0        0     1914 2023-06-28 10:16:38.864033 tabeline-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      136 2023-06-27 13:07:54.545095 tabeline-0.3.0/src/tabeline/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-03 23:40:51.395289 tabeline-0.3.0/src/tabeline/_concatenate.py
--rw-r--r--   0        0        0    22663 2023-06-27 12:23:24.487028 tabeline-0.3.0/src/tabeline/_data_frame.py
--rw-r--r--   0        0        0      365 2023-04-21 01:31:22.563413 tabeline-0.3.0/src/tabeline/_dummy.py
--rw-r--r--   0        0        0      195 2023-06-27 13:06:17.969366 tabeline-0.3.0/src/tabeline/_expression/__init__.py
--rw-r--r--   0        0        0     2832 2023-05-04 11:38:10.169202 tabeline-0.3.0/src/tabeline/_expression/_functions.py
--rw-r--r--   0        0        0     4071 2023-06-27 13:13:14.028287 tabeline-0.3.0/src/tabeline/_expression/_parser.py
--rw-r--r--   0        0        0     5363 2022-04-10 13:57:42.631712 tabeline-0.3.0/src/tabeline/_expression/_substitute.py
--rw-r--r--   0        0        0     3744 2022-04-10 13:57:42.631712 tabeline-0.3.0/src/tabeline/_expression/_to_polars.py
--rw-r--r--   0        0        0     2788 2023-06-27 13:13:17.724278 tabeline-0.3.0/src/tabeline/_expression/ast.py
--rw-r--r--   0        0        0      733 2023-05-03 12:09:48.914426 tabeline-0.3.0/src/tabeline/_validation.py
--rw-r--r--   0        0        0     3570 2023-05-03 23:40:51.395289 tabeline-0.3.0/src/tabeline/exceptions.py
--rw-r--r--   0        0        0      381 2023-04-21 01:31:22.559414 tabeline-0.3.0/src/tabeline/testing.py
--rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 tabeline-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-28 10:08:20.880692 tabeline-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1708 2023-04-26 09:54:10.670471 tabeline-0.3.1/README.md
+-rw-r--r--   0        0        0     2304 2023-07-09 12:51:46.917779 tabeline-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-09 12:51:14.429760 tabeline-0.3.1/src/tabeline/__init__.py
+-rw-r--r--   0        0        0     1419 2023-06-28 15:53:44.753714 tabeline-0.3.1/src/tabeline/_concatenate.py
+-rw-r--r--   0        0        0    22789 2023-07-09 12:51:15.537760 tabeline-0.3.1/src/tabeline/_data_frame.py
+-rw-r--r--   0        0        0      365 2023-04-21 01:31:22.563413 tabeline-0.3.1/src/tabeline/_dummy.py
+-rw-r--r--   0        0        0      139 2023-06-28 15:38:00.904206 tabeline-0.3.1/src/tabeline/_expression/__init__.py
+-rw-r--r--   0        0        0     3671 2023-07-09 12:51:15.537760 tabeline-0.3.1/src/tabeline/_expression/_functions.py
+-rw-r--r--   0        0        0     4071 2023-06-27 13:13:14.028287 tabeline-0.3.1/src/tabeline/_expression/_parser.py
+-rw-r--r--   0        0        0     5363 2022-04-10 13:57:42.631712 tabeline-0.3.1/src/tabeline/_expression/_substitute.py
+-rw-r--r--   0        0        0     3744 2023-06-29 12:57:02.032034 tabeline-0.3.1/src/tabeline/_expression/_to_polars.py
+-rw-r--r--   0        0        0     2788 2023-06-27 13:13:17.724278 tabeline-0.3.1/src/tabeline/_expression/ast.py
+-rw-r--r--   0        0        0      796 2023-07-04 16:11:44.006619 tabeline-0.3.1/src/tabeline/_validation.py
+-rw-r--r--   0        0        0     3965 2023-07-04 15:02:57.136441 tabeline-0.3.1/src/tabeline/exceptions.py
+-rw-r--r--   0        0        0      381 2023-04-21 01:31:22.559414 tabeline-0.3.1/src/tabeline/testing.py
+-rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 tabeline-0.3.1/PKG-INFO
```

### Comparing `tabeline-0.3.0/LICENSE` & `tabeline-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.0/README.md` & `tabeline-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.0/pyproject.toml` & `tabeline-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tabeline"
-version = "0.3.0"
+version = "0.3.1"
 description = "A data frame and data grammar library"
 authors = ["David Hagen <david@drhagen.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://tabeline.drhagen.com"
 repository = "https://github.com/drhagen/tabeline"
 keywords = ["dataframe", "datatable", "datagrammar", "dplyr"]
@@ -32,35 +32,35 @@
 pyarrow = "^11.0.0"
 pandas = "^1.4"
 
 # Test
 pytest = "^7.2"
 pytest-cov = "*"
 
-# Black
-black = ">=22.3.0"
-
-# Isort
-isort = "^5.9.3"
-
-# Flake8
-flake8 = "^4.0.1"
-pyproject-flake8 = "^0.0.1a3"
-pep8-naming = "^0.12.1"
-flake8-noqa = "^1.2.1"
+# Lint
+black = ">=23.3"
+ruff = ">=0.0.275"
 
 # Docs
 mkdocs-material = "^9"
 
 [tool.poetry.extras]
 pandas = ["pandas", "pyarrow"]
 
 
 [tool.pytest.ini_options]
+addopts = [
+    "--strict-config",
+    "--strict-markers",
+]
 xfail_strict = true
+filterwarnings = [
+    # When running tests, treat warnings as errors (e.g. -Werror).
+    "error",
+]
 
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [
@@ -75,26 +75,38 @@
     ".nox/test*/lib/python*/site-packages/",
     ".nox/test*/Lib/site-packages/",
 ]
 
 
 [tool.black]
 line-length = 99
-preview = true
-
 
-[tool.isort]
-profile = "black"
-line_length = 99
-extra_standard_library = ["typing_extensions"]
 
-
-[tool.flake8]
-max-line-length = 99
-noqa-require-code = true
+[tool.ruff]
+src = ["src"]
+line-length = 99
+extend-select = [
+    "I", # isort
+    "N", # pep8-naming
+    "RUF", # ruff
+    "B", # flake8-bugbear
+    "N", # flake8-broken-line
+    "C4", # flake8-comprehensions
+    "PIE", # flake8-pie
+    "PT", # flake8-pytest-style
+    "PTH", # flake8-use-pathlib
+    "ERA", # flake8-eradicate
+]
 # F821: undefined-name; Parsita triggers this, but code coverage will catch it
 extend-ignore = ["F821"]
 
+[tool.ruff.per-file-ignores]
+# F401: unused-import; Allow unused imports in __init__.py files
+"__init__.py" = ["F401"]
+
+[tool.ruff.isort]
+extra-standard-library = ["typing_extensions"]
+
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tabeline-0.3.0/src/tabeline/_data_frame.py` & `tabeline-0.3.1/src/tabeline/_data_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import polars as pl
 
 from ._dummy import dummy_frame, dummy_name
 from ._expression import substitute, to_polars
 from ._expression.ast import Expression
 from ._validation import assert_legal_columns, missing
 from .exceptions import (
-    GroupColumn,
-    HasGroups,
-    IndexOutOfRange,
-    NoGroups,
-    NonexistentColumn,
-    RenameExisting,
+    GroupColumnError,
+    HasGroupsError,
+    IndexOutOfRangeError,
+    NoGroupsError,
+    NonexistentColumnError,
+    RenameExistingError,
 )
 
 # Singleton indicating that the default value is to error
 error = object()
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -86,50 +86,50 @@
         return DataFrame(pl.from_pandas(df))
 
     def to_pandas(self) -> pd.DataFrame:
         import numpy as np
         import pandas as pd
 
         if len(self.group_levels) != 0:
-            raise HasGroups()
+            raise HasGroupsError()
 
         if self.width == 0:
             # Polars does not understand columnless data frames
             return pd.DataFrame(np.empty((self.height, 0)))
 
         return self._df.to_pandas()
 
     @staticmethod
     def from_polars(df: pl.DataFrame) -> DataFrame:
         return DataFrame(df)
 
     def to_polars(self) -> pl.DataFrame:
         if len(self.group_levels) != 0:
-            raise HasGroups()
+            raise HasGroupsError()
 
         return self._df
 
     @staticmethod
     def read_csv(path: Path) -> DataFrame:
         df = pl.read_csv(str(path))
         return DataFrame(df)
 
     def write_csv(self, path: Path) -> None:
         if len(self.group_levels) != 0:
-            raise HasGroups()
+            raise HasGroupsError()
 
         self._df.write_csv(str(path))
 
     def slice0(self, indexes: list[int], /) -> DataFrame:
         # Negative indexes are not supported by Polars, so they are not
         # supported in Tabeline.
         if self.width == 0:
             for index in indexes:
                 if index >= self.height or index < 0:
-                    raise IndexOutOfRange(index, self.height)
+                    raise IndexOutOfRangeError(index, self.height)
             return DataFrame(self._df, self.group_levels, len(indexes))
         else:
             group_names = self.group_names
             if len(group_names) == 0:
                 # Polars chokes on empty groups
                 return DataFrame(self._df.select(pl.all().take(indexes)), self.group_levels)
             else:
@@ -308,21 +308,21 @@
         # Sometime in the 0.13.x series, Polars switched from sequential to
         # parallel. dplyr has always been sequential.
 
         columns_set = set(self.column_names)
 
         for old_column in names.values():
             if old_column not in columns_set:
-                raise NonexistentColumn(old_column)
+                raise NonexistentColumnError(old_column)
             else:
                 columns_set.remove(old_column)
 
         for new_column in names.keys():
             if new_column in columns_set:
-                raise RenameExisting(names[new_column], new_column)
+                raise RenameExistingError(names[new_column], new_column)
             else:
                 columns_set.add(new_column)
 
         rename_map = {old: new for new, old in names.items()}
 
         groups = tuple(
             tuple(rename_map.get(column, column) for column in level)
@@ -331,15 +331,15 @@
 
         return DataFrame(self._df.rename(rename_map), groups, self.height)
 
     def mutate(self, **mutators: str) -> DataFrame:
         group_set = set(self.group_names)
         for column in mutators.keys():
             if column in group_set:
-                raise GroupColumn(column)
+                raise GroupColumnError(column)
 
         if self.width == 0:
             df = dummy_frame(self.height)
         else:
             df = self._df
 
         # Both mutate and transmute must compute each column individually
@@ -384,30 +384,30 @@
         elif order == "sort":
             ordered_df = self.sort(*columns)
         else:
             raise TypeError(
                 f"For order, expected 'original', 'cluster', or 'sort', but got {order!r}"
             )
 
-        return DataFrame(ordered_df._df, self.group_levels + (columns,), self.height)
+        return DataFrame(ordered_df._df, (*self.group_levels, columns), self.height)
 
     def group(
         self, *columns: str, order: Literal["original", "cluster", "sort"] = "original"
     ) -> DataFrame:
         return self.group_by(*columns, order=order)
 
     def ungroup(self) -> DataFrame:
         if len(self.group_levels) == 0:
-            raise NoGroups()
+            raise NoGroupsError()
         else:
             return DataFrame(self._df, self.group_levels[:-1], self.height)
 
     def summarize(self, **reducers: str) -> DataFrame:
         if len(self.group_levels) == 0:
-            raise NoGroups()
+            raise NoGroupsError()
 
         # There is no way to sequentially evaluate expressions in a groupby
         # context, so each reducer must be substituted into subsequent reducers:
         # https://stackoverflow.com/q/71120396/
         substituted_reducers = {}
         for name, reducer in reducers.items():
             substituted_reducers[name] = substitute(
@@ -432,19 +432,21 @@
                 polars_expressions
             )
 
             return DataFrame(summarized, self.group_levels[:-1])
 
     def spread(self, key: str, value: str, *, fill: Any = error) -> DataFrame:
         if len(self.group_levels) == 0:
-            raise NoGroups()
+            raise NoGroupsError()
 
         assert_legal_columns([key, value], self.column_names, self.group_names)
 
-        df = self._df.pivot(index=list(self.group_names), columns=key, values=value)
+        df = self._df.pivot(
+            index=list(self.group_names), columns=key, values=value, aggregate_function=None
+        )
 
         return DataFrame(df, self.group_levels[:-1])
 
     def gather(self, key: str, value: str, *columns: str) -> DataFrame:
         column_set = set(columns)
         all_columns = [column for column in self.column_names if column not in column_set]
```

### Comparing `tabeline-0.3.0/src/tabeline/_expression/_parser.py` & `tabeline-0.3.1/src/tabeline/_expression/_parser.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.0/src/tabeline/_expression/_substitute.py` & `tabeline-0.3.1/src/tabeline/_expression/_substitute.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.0/src/tabeline/_expression/_to_polars.py` & `tabeline-0.3.1/src/tabeline/_expression/_to_polars.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.0/src/tabeline/_expression/ast.py` & `tabeline-0.3.1/src/tabeline/_expression/ast.py`

 * *Files identical despite different names*

### Comparing `tabeline-0.3.0/src/tabeline/_validation.py` & `tabeline-0.3.1/src/tabeline/_validation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 __all__ = ["missing", "assert_legal_columns"]
 
 from typing import Sequence
 
-from tabeline.exceptions import DuplicateColumn, GroupColumn, NonexistentColumn
+from tabeline.exceptions import DuplicateColumnError, GroupColumnError, NonexistentColumnError
 
 missing = object()
 
 
 def assert_legal_columns(
     columns: Sequence[str],
     existing_columns: Sequence[str],
     illegal_group_columns: Sequence[str] = (),
 ) -> None:
     columns_set: set[str] = set()
     existing_columns_set = set(existing_columns)
     group_column_set = set(illegal_group_columns)
     for column in columns:
         if column in columns_set:
-            raise DuplicateColumn(column)
+            raise DuplicateColumnError(column)
 
         if column not in existing_columns_set:
-            raise NonexistentColumn(column)
+            raise NonexistentColumnError(column)
 
         if column in group_column_set:
-            raise GroupColumn(column)
+            raise GroupColumnError(column)
+
+        columns_set.add(column)
```

### Comparing `tabeline-0.3.0/src/tabeline/exceptions.py` & `tabeline-0.3.1/src/tabeline/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-class TabelineException(Exception):
+class TabelineError(Exception):
     pass
 
 
-class NonexistentColumn(TabelineException):
+class NonexistentColumnError(TabelineError):
     def __init__(self, column: str):
         super().__init__(column)
         self.column = column
 
     def __str__(self) -> str:
         return f"Cannot perform this operation using nonexistent column {self.column}"
 
 
-class DuplicateColumn(TabelineException):
+class DuplicateColumnError(TabelineError):
     def __init__(self, column: str):
         super().__init__(column)
         self.column = column
 
     def __str__(self) -> str:
         return f"Column {self.column} is duplicated."
 
 
-class RenameExisting(TabelineException):
+class RenameExistingError(TabelineError):
     def __init__(self, old_column: str, new_column: str):
         super().__init__(old_column, new_column)
         self.old_column = old_column
         self.new_column = new_column
 
     def __str__(self) -> str:
         return (
             f"Cannot rename {self.old_column} to {self.new_column} because"
             f" {self.new_column} already exists"
         )
 
 
-class HasGroups(TabelineException):
+class HasGroupsError(TabelineError):
     def __str__(self) -> str:
         return "Cannot perform this operation on a data frame with any group levels"
 
 
-class NoGroups(TabelineException):
+class NoGroupsError(TabelineError):
     def __str__(self) -> str:
         return "Cannot perform this operation on a data frame with no group levels"
 
 
-class GroupColumn(TabelineException):
+class GroupColumnError(TabelineError):
     def __init__(self, column: str):
         super().__init__(column)
         self.column = column
 
     def __str__(self) -> str:
         return f"Cannot perform this operation on group column {self.column}"
 
 
-class RowlessDataFrame(TabelineException):
+class RowlessDataFrameError(TabelineError):
     def __str__(self) -> str:
         return "Cannot perform this operation on a data frame with no rows"
 
 
-class IndexOutOfRange(TabelineException):
+class IndexOutOfRangeError(TabelineError):
     def __init__(self, index: int, length: int):
         self.index = index
         self.length = length
 
     def __str__(self) -> str:
         return f"Cannot index element {self.index} from data frame with {self.length} rows"
 
 
-class UnmatchedColumns(TabelineException):
+class UnmatchedColumnsError(TabelineError):
     def __init__(self, expected_columns: tuple[str, ...], actual_columns: tuple[str, ...]):
         super().__init__(expected_columns, actual_columns)
         self.expected_columns = expected_columns
         self.actual_columns = actual_columns
 
     def __str__(self) -> str:
         return (
             "Columns do not match\n"
             f"Expected columns: {list(self.expected_columns)}\n"
             f"Actual columns: {list(self.actual_columns)}"
         )
 
 
-class UnmatchedGroupLevels(TabelineException):
+class UnmatchedGroupLevelsError(TabelineError):
     def __init__(
         self,
         expected_group_levels: tuple[tuple[str, ...], ...],
         actual_group_levels: tuple[tuple[str, ...], ...],
     ):
         super().__init__(expected_group_levels, actual_group_levels)
         self.expected_group_levels = expected_group_levels
@@ -94,17 +94,28 @@
         expected_str = ",".join(
             "[" + ",".join(level) + "]" for level in self.expected_group_levels
         )
         actual_str = ",".join("[" + ",".join(level) + "]" for level in self.actual_group_levels)
         return f"Group levels do not match; expected {expected_str} but got {actual_str}"
 
 
-class UnmatchedHeight(TabelineException):
+class UnmatchedHeightError(TabelineError):
     def __init__(self, expected_height: int, actual_height: int):
         super().__init__(expected_height, actual_height)
         self.expected_height = expected_height
         self.actual_height = actual_height
 
     def __str__(self) -> str:
         return (
             f"Heights do not match; expected {self.expected_height} but got {self.actual_height}"
         )
+
+
+class NotSameError(TabelineError):
+    def __init__(self, column: tuple[object, ...]):
+        super().__init__(column)
+        self.column = column
+
+    def __str__(self) -> str:
+        used = set()
+        unique_elements = [x for x in self.column if x not in used and (used.add(x) or True)]
+        return f"Assertion that all elements are the same failed, found {unique_elements}"
```

### Comparing `tabeline-0.3.0/PKG-INFO` & `tabeline-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabeline
-Version: 0.3.0
+Version: 0.3.1
 Summary: A data frame and data grammar library
 Home-page: https://github.com/drhagen/tabeline
 License: MIT
 Keywords: dataframe,datatable,datagrammar,dplyr
 Author: David Hagen
 Author-email: david@drhagen.com
 Requires-Python: >=3.9,<4.0
```

