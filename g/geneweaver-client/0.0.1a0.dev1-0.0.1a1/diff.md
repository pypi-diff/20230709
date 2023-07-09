# Comparing `tmp/geneweaver_client-0.0.1a0.dev1.tar.gz` & `tmp/geneweaver_client-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_client-0.0.1a0.dev1.tar", max compression
+gzip compressed data, was "geneweaver_client-0.0.1a1.tar", max compression
```

## Comparing `geneweaver_client-0.0.1a0.dev1.tar` & `geneweaver_client-0.0.1a1.tar`

### file list

```diff
@@ -1,24 +1,18 @@
--rw-r--r--   0        0        0    11356 2023-06-29 12:40:34.692952 geneweaver_client-0.0.1a0.dev1/LICENSE
--rw-r--r--   0        0        0      568 2023-06-29 21:51:24.356766 geneweaver_client-0.0.1a0.dev1/README.md
--rw-r--r--   0        0        0     1127 2023-06-29 21:51:27.895618 geneweaver_client-0.0.1a0.dev1/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-28 18:15:46.077427 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/__init__.py
--rw-r--r--   0        0        0       37 2023-06-29 12:46:46.688012 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/__init__.py
--rw-r--r--   0        0        0       70 2023-06-26 23:35:00.775445 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/auth.py
--rw-r--r--   0        0        0      238 2023-06-28 18:06:18.299347 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/exc.py
--rw-r--r--   0        0        0     1454 2023-06-29 12:45:06.212514 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/genesets.py
--rw-r--r--   0        0        0     2033 2023-06-29 16:22:14.199284 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/legacy.py
--rw-r--r--   0        0        0     1356 2023-06-29 16:16:12.508098 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/utils.py
--rw-r--r--   0        0        0       66 2023-06-29 16:15:01.097656 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/batch/__init__.py
--rw-r--r--   0        0        0       48 2023-06-29 16:24:20.097633 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/__init__.py
--rw-r--r--   0        0        0      704 2023-06-29 19:25:08.024792 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/main.py
--rw-r--r--   0        0        0     1552 2023-06-29 16:31:43.842718 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/parser.py
--rw-r--r--   0        0        0     3112 2023-06-29 16:11:53.517604 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/config.py
--rw-r--r--   0        0        0      699 2023-06-29 13:51:51.654691 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/exceptions.py
--rw-r--r--   0        0        0       55 2023-06-29 16:07:27.581298 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/__init__.py
--rw-r--r--   0        0        0     6080 2023-06-29 12:45:06.228269 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/csv.py
--rw-r--r--   0        0        0     3332 2023-06-29 20:09:30.754509 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/general.py
--rw-r--r--   0        0        0     1374 2023-06-29 20:39:58.278826 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/utils.py
--rw-r--r--   0        0        0     7619 2023-06-29 13:46:46.600190 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/xlsx.py
--rw-r--r--   0        0        0      194 2023-06-28 19:49:38.153124 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/types.py
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 geneweaver_client-0.0.1a0.dev1/setup.py
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 geneweaver_client-0.0.1a0.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-05 21:07:23.284859 geneweaver_client-0.0.1a1/LICENSE
+-rw-r--r--   0        0        0      568 2023-06-29 21:51:24.356766 geneweaver_client-0.0.1a1/README.md
+-rw-r--r--   0        0        0     1184 2023-07-09 17:04:55.256180 geneweaver_client-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-05 21:07:23.286523 geneweaver_client-0.0.1a1/src/geneweaver/client/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-05 21:07:23.287009 geneweaver_client-0.0.1a1/src/geneweaver/client/api/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-05 21:07:23.287299 geneweaver_client-0.0.1a1/src/geneweaver/client/api/auth.py
+-rw-r--r--   0        0        0      226 2023-07-09 16:35:05.329005 geneweaver_client-0.0.1a1/src/geneweaver/client/api/exc.py
+-rw-r--r--   0        0        0     1454 2023-07-05 21:07:23.288345 geneweaver_client-0.0.1a1/src/geneweaver/client/api/genesets.py
+-rw-r--r--   0        0        0     2033 2023-07-05 21:07:23.289106 geneweaver_client-0.0.1a1/src/geneweaver/client/api/legacy.py
+-rw-r--r--   0        0        0     1348 2023-07-09 16:35:05.309693 geneweaver_client-0.0.1a1/src/geneweaver/client/api/utils.py
+-rw-r--r--   0        0        0       66 2023-07-05 21:07:23.290199 geneweaver_client-0.0.1a1/src/geneweaver/client/batch/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-05 21:07:23.290573 geneweaver_client-0.0.1a1/src/geneweaver/client/cli/__init__.py
+-rw-r--r--   0        0        0      704 2023-07-05 21:07:23.291282 geneweaver_client-0.0.1a1/src/geneweaver/client/cli/main.py
+-rw-r--r--   0        0        0     1755 2023-07-09 16:59:53.325737 geneweaver_client-0.0.1a1/src/geneweaver/client/cli/parser.py
+-rw-r--r--   0        0        0     3112 2023-07-05 21:07:23.292485 geneweaver_client-0.0.1a1/src/geneweaver/client/config.py
+-rw-r--r--   0        0        0       55 2023-06-29 16:07:27.581298 geneweaver_client-0.0.1a1/src/geneweaver/client/parser/__init__.py
+-rw-r--r--   0        0        0     3410 2023-07-09 17:05:40.859176 geneweaver_client-0.0.1a1/src/geneweaver/client/parser/general.py
+-rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 geneweaver_client-0.0.1a1/PKG-INFO
```

### Comparing `geneweaver_client-0.0.1a0.dev1/LICENSE` & `geneweaver_client-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev1/README.md` & `geneweaver_client-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev1/pyproject.toml` & `geneweaver_client-0.0.1a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-client"
-version = "0.0.1a0-dev1"
+version = "0.0.1a1"
 description = "A Python Client for the Geneweaver API"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://bergsalex.github.io/geneweaver-docs/"
 repository = "https://bitbucket.org/jacksonlaboratory/geneweaver-client/"
 packages = [
@@ -17,26 +17,29 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 pydantic = {extras = ["dotenv"], version = "^1.10.7"}
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
-geneweaver-core = "^0.1.0a1"
+geneweaver-core = "0.2.0a0"
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.4.2"
 openpyxl = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 geneweaver-testing = "^0.0.1a10"
 
 [tool.ruff]
 select = ['F', 'E', 'W', 'A', 'C90', 'N', 'B', 'ANN', 'D', 'I', 'ERA', 'PD', 'NPY', 'PT']
 
+[tool.ruff.per-file-ignores]
+"tests/*" = ["ANN001", "ANN201"]
+
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/genesets.py` & `geneweaver_client-0.0.1a1/src/geneweaver/client/api/genesets.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/legacy.py` & `geneweaver_client-0.0.1a1/src/geneweaver/client/api/legacy.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/utils.py` & `geneweaver_client-0.0.1a1/src/geneweaver/client/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """API related utilities, helpers, and other internal functions."""
 from contextlib import contextmanager
 from typing import Any
 
 import requests
-from geneweaver.client.api.exc import GeneweaverAPIException
+from geneweaver.client.api.exc import GeneweaverAPIError
 
 
 def _raise_for_status_hook(
     response: requests.Response, *args: Any, **kwargs: Any  # noqa: ANN401
 ) -> None:
     """Have request responses raise an exception for non-200 status codes."""
     response.raise_for_status()
@@ -28,8 +28,8 @@
             yield session
         except requests.exceptions.RequestException as err:
             # TODO: We SHOULD try extracting the error message from the response,
             #  could even check the JSON.
             err_str = (
                 f"There was a problem calling the Geneweaver API: {err.response.text}"
             )
-            raise GeneweaverAPIException(err_str) from err
+            raise GeneweaverAPIError(err_str) from err
```

### Comparing `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/main.py` & `geneweaver_client-0.0.1a1/src/geneweaver/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/parser.py` & `geneweaver_client-0.0.1a1/src/geneweaver/client/cli/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """CLI for parsing data files."""
 from pathlib import Path
 
 import typer
-from geneweaver.client.exceptions import EmptyFileError
-from geneweaver.client.parser import general, xlsx
+from geneweaver.client.parser import general
+from geneweaver.core.parse import xlsx
+from geneweaver.core.parse.exceptions import EmptyFileError, UnsupportedFileTypeError
 from rich import print
 from rich.console import Console
 from rich.table import Table
 
 cli = typer.Typer()
 console = Console()
 
 
 @cli.command()
 def get_headers(file_path: Path, sheet: str = None) -> None:
     """Get the headers from a data file."""
     headers = []
     try:
         headers = general.get_headers(file_path, sheet_name=sheet)
-    except (EmptyFileError, ValueError) as e:
+    except (EmptyFileError, ValueError, UnsupportedFileTypeError) as e:
         print(e)
         raise typer.Exit(code=1) from e
 
     for header in headers:
         print(header)
 
 
@@ -31,15 +32,18 @@
     """Preview the data in a data file."""
     rows = []
     try:
         headers, headers_idx = general.get_headers(file_path, sheet_name=sheet)
         rows = general.data_file_to_dict_n_rows(
             file_path, rows_to_read, headers_idx, sheet_name=sheet
         )
-    except (EmptyFileError, ValueError) as e:
+    except ValueError as e:
+        print("File is empty.")
+        raise typer.Exit(code=1) from e
+    except (EmptyFileError, UnsupportedFileTypeError) as e:
         print(e)
         raise typer.Exit(code=1) from e
 
     table = Table(*headers)
     for row in rows:
         table.add_row(*(str(r) for r in row.values()))
     console.print(table)
```

### Comparing `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/config.py` & `geneweaver_client-0.0.1a1/src/geneweaver/client/config.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/general.py` & `geneweaver_client-0.0.1a1/src/geneweaver/client/parser/general.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 """A module that marshals access to specific file type parsing."""
 from typing import List, Optional
 
-from geneweaver.client.parser import csv, utils, xlsx
-from geneweaver.client.types import DictRow, StringOrPath
+from geneweaver.core.parse import csv, utils, xlsx
+from geneweaver.core.parse.exceptions import UnsupportedFileTypeError
+from geneweaver.core.types import DictRow, StringOrPath
 
 
 def get_headers(file_path: StringOrPath, sheet_name: Optional[str] = None) -> List[str]:
     """Retrieve the header row from a CSV or Excel file.
 
     This function first determines the file type (CSV or Excel) and then uses
     the appropriate helper function to get the headers.
 
     :param file_path: The path to the file.
     :param sheet_name: Name of the sheet to read from (for Excel files).
                        If not provided, the function will read from the active sheet.
                        This argument is ignored for CSV files.
 
-    Returns
-    -------
-    List[str]: A list of strings representing the header row of the file.
-
-    Raises
-    ------
-    ValueError: If the file type is neither CSV nor Excel (.xlsx).
+    :returns: A list of strings representing the header row of the file.
+
+    :raises ValueError: If the file type is neither CSV nor Excel (.xlsx).
     """
     file_type = utils.get_file_type(file_path)
 
     if file_type == "csv":
         data, _ = csv.get_headers(file_path)
 
     elif file_type == "xlsx":
         data, _ = xlsx.get_headers(file_path, sheet_name)
 
     else:
-        raise ValueError(f"Unsupported file type: {file_type}")
+        raise UnsupportedFileTypeError(f"Unsupported file type: {file_type}")
 
     return data
 
 
 def data_file_to_dict(
     file_path: StringOrPath, sheet_name: Optional[str] = None
 ) -> List[DictRow]:
@@ -46,29 +43,27 @@
     Parse a CSV or Excel file into a list of dictionaries, with keys as column names and
      values as column values.
 
     :param file_path: The file path to the CSV or Excel file.
     :param sheet_name: Name of the sheet to read from (for Excel files). If not
     provided, the function will read from the active sheet. Ignored for CSV files.
 
-    Returns
-    -------
-    List[DictRow]: A list of dictionaries, where each dictionary represents a row from
-    the CSV or Excel file.
+    :returns: A list of dictionaries, where each dictionary represents a row from the
+    CSV or Excel file.
     """
     file_type = utils.get_file_type(file_path)
 
     if file_type == "csv":
         data = csv.read_to_dict(file_path)
 
     elif file_type == "xlsx":
         data = xlsx.read_to_dict(file_path, sheet_name)
 
     else:
-        raise ValueError(f"Unsupported file type: {file_type}")
+        raise UnsupportedFileTypeError(f"Unsupported file type: {file_type}")
 
     return data
 
 
 def data_file_to_dict_n_rows(
     file_path: StringOrPath,
     n: int,
@@ -78,27 +73,26 @@
     """Parse n lines of a CSV or Excel file into a list of dictionaries.
 
     Parse a CSV or Excel file into a list of dictionaries, with keys as column names and
     values as column values.
 
     :param file_path: The file path to the CSV or Excel file.
     :param n: The number of rows of data to return.
+    :param start_row: The row to start reading from. Defaults to 0.
     :param sheet_name: Name of the sheet to read from (for Excel files). If not
     provided, the function will read from the active sheet. Ignored for CSV files.
 
-    Returns
-    -------
-    List[DictRow]: A list of dictionaries, where each dictionary
-    represents a row from the CSV or Excel file.
+    :returns: A list of dictionaries, where each dictionary represents a row from the
+    CSV or Excel file.
     """
     file_type = utils.get_file_type(file_path)
 
     if file_type == "csv":
         data = csv.read_to_dict_n_rows(file_path, n, start_row)
 
     elif file_type == "xlsx":
         data = xlsx.read_to_dict_n_rows(file_path, n, start_row, sheet_name)
 
     else:
-        raise ValueError(f"Unsupported file type: {file_type}")
+        raise UnsupportedFileTypeError(f"Unsupported file type: {file_type}")
 
     return data
```

### Comparing `geneweaver_client-0.0.1a0.dev1/PKG-INFO` & `geneweaver_client-0.0.1a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: geneweaver-client
-Version: 0.0.1a0.dev1
+Version: 0.0.1a1
 Summary: A Python Client for the Geneweaver API
 Home-page: https://bergsalex.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: geneweaver-core (>=0.1.0a1,<0.2.0)
+Requires-Dist: geneweaver-core (==0.2.0a0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
```

