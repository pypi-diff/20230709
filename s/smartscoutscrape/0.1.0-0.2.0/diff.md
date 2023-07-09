# Comparing `tmp/smartscoutscrape-0.1.0.tar.gz` & `tmp/smartscoutscrape-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartscoutscrape-0.1.0.tar", max compression
+gzip compressed data, was "smartscoutscrape-0.2.0.tar", max compression
```

## Comparing `smartscoutscrape-0.1.0.tar` & `smartscoutscrape-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    10912 2023-06-21 00:43:17.419814 smartscoutscrape-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0    15459 2023-07-03 17:05:32.016003 smartscoutscrape-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4173 2023-07-01 17:10:53.999740 smartscoutscrape-0.1.0/README.md
--rw-r--r--   0        0        0     2338 2023-07-03 17:07:07.693217 smartscoutscrape-0.1.0/smartscoutscrape/__init__.py
--rw-r--r--   0        0        0     7525 2023-07-03 17:05:04.932695 smartscoutscrape-0.1.0/smartscoutscrape/amazon.py
--rw-r--r--   0        0        0    31342 2023-07-03 16:55:27.331114 smartscoutscrape-0.1.0/smartscoutscrape/cli.py
--rw-r--r--   0        0        0    14612 2023-07-03 17:05:04.933694 smartscoutscrape-0.1.0/smartscoutscrape/session.py
--rw-r--r--   0        0        0     1892 2023-07-01 16:44:40.327989 smartscoutscrape-0.1.0/smartscoutscrape/utils.py
--rw-r--r--   0        0        0     5814 1970-01-01 00:00:00.000000 smartscoutscrape-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10912 2023-06-21 00:43:17.419814 smartscoutscrape-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0    15504 2023-07-09 03:55:21.817334 smartscoutscrape-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4173 2023-07-01 17:10:53.999740 smartscoutscrape-0.2.0/README.md
+-rw-r--r--   0        0        0     2331 2023-07-09 03:29:25.504056 smartscoutscrape-0.2.0/smartscoutscrape/__init__.py
+-rw-r--r--   0        0        0     7509 2023-07-08 23:43:27.927487 smartscoutscrape-0.2.0/smartscoutscrape/amazon.py
+-rw-r--r--   0        0        0     6318 2023-07-09 02:15:49.073930 smartscoutscrape-0.2.0/smartscoutscrape/cli.py
+-rw-r--r--   0        0        0     6638 2023-07-09 03:51:24.420503 smartscoutscrape-0.2.0/smartscoutscrape/pandas.py
+-rw-r--r--   0        0        0    14978 2023-07-09 02:49:29.826968 smartscoutscrape-0.2.0/smartscoutscrape/smartscout.py
+-rw-r--r--   0        0        0    28096 2023-07-09 03:26:04.334379 smartscoutscrape-0.2.0/smartscoutscrape/sqlite.py
+-rw-r--r--   0        0        0     1892 2023-07-01 16:44:40.327989 smartscoutscrape-0.2.0/smartscoutscrape/utils.py
+-rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 smartscoutscrape-0.2.0/PKG-INFO
```

### Comparing `smartscoutscrape-0.1.0/LICENSE.txt` & `smartscoutscrape-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.1.0/pyproject.toml` & `smartscoutscrape-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # This is the version of your project. Keep it up-to-date and follow semantic versioning.
 # It's used in the PyPi, wheels, Docker, and GitHub packages.
 # Also make sure to use exactly this version when creating a GitHub release,
 # but prefix a "v" to the GitHub release.
 # E.g. This might be "1.2.13", and the GitHub release will be "v1.2.13".
 # Although semantic versioning allows for build tags (metadata),
 # not all tools are compatible with it, so avoid it if you can.
-version = "0.1.0"
+version = "0.2.0"
 
 # TODO: Set the description and keywords here
 description = "Lightweight data-extraction & general use library for smartscout.com"
 keywords = ["scraper", "data science", "requests", "python", "data"]
 authors = ["Parker Wahle <regulad@regulad.xyz>"]
 maintainers = ["Parker Wahle <regulad@regulad.xyz>"]
 # This must be an identifier listed in https://spdx.org/licenses/
@@ -100,14 +100,17 @@
 typer = { version = "^0.9.0", extras = ["all"] }
 requests = "^2.31.0"
 undetected-chromedriver = "^3.5.0"
 selenium = "^4.10.0"
 rich = "^13.4.2"
 beautifulsoup4 = "^4.12.2"
 minify-html = "^0.11.1"
+pandas = "^2"
+jupyter = "^1.0.0"
+tqdm = "^4"
 
 [tool.poetry.dev-dependencies]
 # TODO Remove build dependencies you don't want (like xdoctest, perhaps)
 # These are dependencies that Poetry uses only when testing
 # They all are included as dependencies in tox.ini
 # Where `dev` is from `[tool.poetry.extras]` below
```

### Comparing `smartscoutscrape-0.1.0/README.md` & `smartscoutscrape-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.1.0/smartscoutscrape/__init__.py` & `smartscoutscrape-0.2.0/smartscoutscrape/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,79 @@
-"""
-Metadata for this smartscout-scrape.
-
-Copyright 2023 Parker Wahle <regulad@regulad.xyz>
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
-or implied. See the License for the specific language governing
-permissions and limitations under the License.
-
-"""
-import logging
-from importlib.metadata import PackageNotFoundError
-from importlib.metadata import metadata as __load
-from pathlib import Path
-from typing import Sequence
-
-from .amazon import *
-from .session import *
-
-pkg = Path(__file__).absolute().parent.name
-logger = logging.getLogger(pkg)
-metadata = None
-try:
-    metadata = __load(pkg)
-    __status__ = "Development"
-    __copyright__ = "Copyright 2023"
-    __date__ = "2023-06-20"
-    __uri__ = metadata["home-page"]
-    __title__ = metadata["name"]
-    __summary__ = metadata["summary"]
-    __license__ = metadata["license"]
-    __version__ = metadata["version"]
-    __author__ = metadata["author"]
-    __maintainer__ = metadata["maintainer"]
-    __contact__ = metadata["maintainer"]
-except PackageNotFoundError:  # pragma: no cover
-    logger.error(f"Could not load package metadata for {pkg}. Is it installed?")
-
-
-class SmartscoutscrapeAssets:
-    """
-    Utilities and resources for ${Project}.
-    """
-
-    @classmethod
-    def path(cls, *nodes: Sequence[str]) -> Path:
-        """
-        Gets the ``Path`` of an asset under ``resources``.
-
-        Args:
-            nodes: Path nodes underneath ``resources``
-
-        Returns:
-            The final ``Path``
-
-        Raises:
-            FileNotFoundError: If the path does not exist
-        """
-        path = Path(__file__.parent, "resources", *nodes)
-        if not path.exists():
-            raise FileNotFoundError(f"Asset {path} not found")
-
-
-if __name__ == "__main__":  # pragma: no cover
-    if metadata is not None:
-        print(f"{pkg} (v{metadata['version']})")
-    else:
+"""
+Metadata for this smartscout-scrape.
+
+Copyright 2023 Parker Wahle <regulad@regulad.xyz>
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
+or implied. See the License for the specific language governing
+permissions and limitations under the License.
+
+"""
+import logging
+from importlib.metadata import PackageNotFoundError
+from importlib.metadata import metadata as __load
+from pathlib import Path
+from typing import Sequence
+
+from .amazon import *
+from .pandas import *
+from .smartscout import *
+from .sqlite import *
+from .utils import *
+
+pkg = Path(__file__).absolute().parent.name
+logger = logging.getLogger(pkg)
+metadata = None
+try:
+    metadata = __load(pkg)
+    __status__ = "Development"
+    __copyright__ = "Copyright 2023"
+    __date__ = "2023-06-20"
+    __uri__ = metadata["home-page"]
+    __title__ = metadata["name"]
+    __summary__ = metadata["summary"]
+    __license__ = metadata["license"]
+    __version__ = metadata["version"]
+    __author__ = metadata["author"]
+    __maintainer__ = metadata["maintainer"]
+    __contact__ = metadata["maintainer"]
+except PackageNotFoundError:  # pragma: no cover
+    logger.error(f"Could not load package metadata for {pkg}. Is it installed?")
+
+
+class SmartscoutscrapeAssets:
+    """
+    Utilities and resources for ${Project}.
+    """
+
+    @classmethod
+    def path(cls, *nodes: Sequence[str]) -> Path:
+        """
+        Gets the ``Path`` of an asset under ``resources``.
+
+        Args:
+            nodes: Path nodes underneath ``resources``
+
+        Returns:
+            The final ``Path``
+
+        Raises:
+            FileNotFoundError: If the path does not exist
+        """
+        path = Path(__file__.parent, "resources", *nodes)
+        if not path.exists():
+            raise FileNotFoundError(f"Asset {path} not found")
+
+
+if __name__ == "__main__":  # pragma: no cover
+    if metadata is not None:
+        print(f"{pkg} (v{metadata['version']})")
+    else:
         print(f"Unknown project info for {pkg}")
```

### Comparing `smartscoutscrape-0.1.0/smartscoutscrape/amazon.py` & `smartscoutscrape-0.2.0/smartscoutscrape/amazon.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from requests.exceptions import HTTPError
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.chrome.webdriver import WebDriver as ChromeDriver
 from selenium.webdriver.support.wait import WebDriverWait
 from undetected_chromedriver import Chrome as UndetectedChromeDriver
 from undetected_chromedriver import ChromeOptions as UndetectedChromeOptions
 
-from smartscoutscrape.utils import THREADING_SAFE_MAX_WORKERS
+from .utils import THREADING_SAFE_MAX_WORKERS
 
 
 class AmazonBaseSession(metaclass=ABCMeta):
     def get_asin_html(self, asin: str) -> BeautifulSoup:
         """
         Get the HTML for an ASIN.
         """
```

### Comparing `smartscoutscrape-0.1.0/smartscoutscrape/cli.py` & `smartscoutscrape-0.2.0/smartscoutscrape/sqlite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,188 +1,114 @@
-"""
-Command-line interface for smartscout-scrape.
-
-Copyright 2023 Parker Wahle <regulad@regulad.xyz>
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
-or implied. See the License for the specific language governing
-permissions and limitations under the License.
-
-"""
-
-# fmt: off
-
-from __future__ import annotations
-
 import logging
-import sqlite3
-import time
+import warnings
 import zlib
-from concurrent.futures.thread import ThreadPoolExecutor
-from functools import partial
-from pathlib import Path
-from threading import Lock
-from typing import Optional, cast
+from concurrent.futures import CancelledError, ThreadPoolExecutor, as_completed
+from queue import Empty, Queue
+from sqlite3 import Connection
+from threading import Event, Lock, Thread
+from typing import Generator, Literal, Self, overload
 
 import minify_html
-import typer
 from requests import HTTPError
-from rich.logging import RichHandler
-from rich.progress import Progress, TextColumn
 
-from smartscoutscrape import AmazonScrapeSession, SmartScoutSession, __copyright__, __title__, __version__, metadata
-from smartscoutscrape.utils import THREADING_SAFE_MAX_WORKERS, top_level_dict
+from .amazon import AmazonBaseSession
+from .smartscout import SmartScoutSession
+from .utils import top_level_dict
 
-using_python_profiler = False
-try:
-    import cProfile as profile
-except ImportError:
-    using_python_profiler = True
-    import profile
-
-import pstats
+logger = logging.getLogger(__package__)
 
-# fmt: on
 
-logger = logging.getLogger(__package__)
-cli = typer.Typer()
+class SmartScoutSQLiteHelper:
+    """Helps dump data from SmartScout & Amazon into a SQLite database."""
 
+    # initialization arguments
+    database_connection: Connection
+    _owns_database_connection: bool
+
+    smartscout_session: SmartScoutSession
+    _owns_smartscout_session: bool
+
+    amazon_session: AmazonBaseSession
+    _owns_amazon_session: bool
+
+    # variables
+    connection_lock: Lock
+    closed: bool
+
+    # class vars (cache)
+    _total_products_cache: int | None = None
+
+    def __init__(
+        self,
+        *,
+        database_connection: Connection,
+        owns_connection: bool = False,
+        smartscout_session: SmartScoutSession,
+        owns_smartscout_session: bool = False,
+        amazon_session: AmazonBaseSession,
+        owns_amazon_session: bool = False,
+    ) -> None:
+        """Initialize the helper. The setup function must be called prior to using the helper."""
+        self.database_connection = database_connection
+        self._owns_database_connection = owns_connection
+        self.smartscout_session = smartscout_session
+        self._owns_smartscout_session = owns_smartscout_session
+        self.amazon_session = amazon_session
+        self._owns_amazon_session = owns_amazon_session
+
+        self.connection_lock = Lock()
+        self.closed = False
+
+    def close(self) -> None:
+        """Close the helper."""
+        if self._owns_database_connection:
+            self.database_connection.close()
+        if self._owns_smartscout_session:
+            self.smartscout_session.close()
+        if self._owns_amazon_session:
+            self.amazon_session.close()
+        self.closed = True
+
+    def __del__(self) -> None:
+        """Close the helper."""
+        if not self.closed:
+            warnings.warn(
+                "Unclosed SmartScoutSQLiteHelper. Call close() on the helper to close it.",
+                ResourceWarning,
+                stacklevel=2,
+            )
+            self.close()
 
-def info(n_seconds: float = 0.01, verbose: bool = False) -> None:
-    """
-    Get info about smartscout-scrape.
-
-    Args:
-        n_seconds: Number of seconds to wait between processing.
-        verbose: Output more info
-
-    Example:
-        To call this, run: ::
-
-            from testme import info
-            info(0.02)
-    """
-    typer.echo(f"{__title__} version {__version__}, {__copyright__}")
-    if verbose:
-        typer.echo(str(metadata.__dict__))
-    total = 0
-    with typer.progressbar(range(100)) as progress:
-        for value in progress:
-            time.sleep(n_seconds)
-            total += 1
-    typer.echo(f"Processed {total} things.")
-
-
-@cli.command()
-def generate(
-    username: str,
-    password: Optional[str] = None,
-    database_path: Path = Path("smartscout.db"),
-    threads: int = THREADING_SAFE_MAX_WORKERS,
-    proxy: Optional[str] = None,
-    dump: bool = True,
-    extend: bool = False,  # impossibly slow
-    images: bool = True,
-    dump_html: bool = False,  # impossibly space-consuming
-    timeout: float = 5.0,
-    log_level: str = "WARNING",
-) -> None:
-    """
-    Generate a CSV file of all products and their data on SmartScout.
-
-    Args:
-        username: Your SmartScout username.
-        password: Your SmartScout password. If not provided, you will be prompted.
-        database_path: Path to the database file.
-        threads: Number of threads to use.
-        dump: If products should be dumped. ⚠️ only disable this on your second run or you will experience integrity errors
-        proxy: Proxy to use, i.e. socks5://localhost:1055
-        extend: Extend the database with extra columns like amazon description & images. WARNING: This is impossibly slow, and is likely to get your IP banned by Amazon.
-        images: Fetch images.
-        log_level: Log level.
-        dump_html: If HTML data should be dumped along with the extension data. Enabling this also enables extend.
-        timeout: Amount of time to wait if data does not return instantly
-    """
-    if dump_html:
-        extend = True
-
-    if password is None:
-        password = typer.prompt("Please enter your password", hide_input=True)
-
-    log_level_int = cast(int, logging.getLevelName(log_level.upper()))
-    log_level_info_or_higher = log_level_int <= logging.INFO  # check to see if safe to print
-    log_level_debug_or_higher = log_level_int <= logging.DEBUG  # check to see if safe to print
-    logging.basicConfig(level=log_level_int, handlers=[RichHandler()])
-
-    if sqlite3.threadsafety < 2:
-        raise RuntimeError("sqlite3 is not threadsafe. Please use a different Python version.")
-
-    startup_lock = Lock()
-    con_lock = Lock()
-
-    # fmt: off
-    with profile.Profile() as pr, \
-            SmartScoutSession(proxy=proxy, threads=threads) as smartscout_session, \
-            AmazonScrapeSession(proxy=proxy, threads=threads) as amazon_session, \
-            sqlite3.Connection(database_path, timeout=timeout, check_same_thread=False) as conn, \
-            Progress(
-                TextColumn("[bold cyan]{task.completed}/{task.total}[/bold cyan]"),
-                *Progress.get_default_columns(),
-            ) as progress, \
-            ThreadPoolExecutor(thread_name_prefix="CategoryDownloader", max_workers=threads) as category_downloader:
-        # fmt: on
-
-        # calibrate profiler
-        if using_python_profiler:
-            calibration_task = progress.add_task("Calibrating...", total=5)
-            for _ in progress.track(range(5), 5, task_id=calibration_task):
-                pr.calibrate(10000)
-            progress.remove_task(calibration_task)
-
-        # We do our own SQLite synchronization, so we don't need it to exclusively be on the same thread
-
-        # login
-        login_task = progress.add_task("Logging in...", total=None)
-        smartscout_session.login(username, password)
-        progress.update(login_task, total=1, completed=1)
-        progress.remove_task(login_task)
+    def __enter__(self) -> Self:
+        """Enter the context manager."""
+        self.setup()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
+        """Exit the context manager."""
+        self.close()
 
+    def setup(self) -> None:
         # categories
-        category_task = progress.add_task("Getting categories...", total=None)
-        categories = smartscout_session.categories()
-        progress.update(category_task, total=len(categories))
-        conn.execute("CREATE TABLE IF NOT EXISTS categories (id INTEGER PRIMARY KEY, name TEXT)")
+        categories = self.smartscout_session.categories()
+        self.database_connection.execute("CREATE TABLE IF NOT EXISTS categories (id INTEGER PRIMARY KEY, name TEXT)")
         for category in categories:
             try:
-                conn.execute(
+                self.database_connection.execute(
                     "INSERT INTO categories VALUES (:id, :name) ON CONFLICT (id) DO UPDATE SET (name) = (:name);",
-                    category
+                    category,
                 )
             except Exception as e:
-                conn.rollback()
+                self.database_connection.rollback()
                 raise e
-            finally:
-                progress.advance(category_task)
-        conn.commit()
-
-        progress.remove_task(category_task)
+        self.database_connection.commit()
 
         # subcategories
-        subcategory_task = progress.add_task("Getting subcategories...", total=None)
-        subcategories = smartscout_session.subcategories()
-        progress.update(subcategory_task, total=len(subcategories))
-        conn.execute(
+        subcategories = self.smartscout_session.subcategories()
+        self.database_connection.execute(
             "CREATE TABLE IF NOT EXISTS subcategories ("
             "   'analyticsSearchable' BOOLEAN NULL,"
             "   'pathById' TEXT NULL,"
             "   'parentId' UNSIGNED BIG INT NULL,"
             "   'level' INTEGER NULL,"
             "   'momGrowth' REAL NULL,"
             "   'momGrowth12' REAL NULL,"
@@ -205,18 +131,20 @@
             "   'sellerRevenuePct' REAL NULL,"
             "   'azRevenuePct' REAL NULL,"
             "   'avgListedSinceDays' REAL NULL,"  # INTEGER
             "   'ttm' REAL NULL,"
             "   'isParent' BOOLEAN NULL"
             ");"
         )
-        conn.execute("CREATE INDEX IF NOT EXISTS subcategories_parentId ON subcategories(parentId);")
+        self.database_connection.execute(
+            "CREATE INDEX IF NOT EXISTS subcategories_parentId ON subcategories(parentId);"
+        )
         for subcategory in subcategories:
             try:
-                conn.execute(
+                self.database_connection.execute(
                     "INSERT INTO subcategories VALUES ("
                     "   :analyticsSearchable,"
                     "   :pathById,"
                     "   :parentId,"
                     "   :level,"
                     "   :momGrowth,"
                     "   :momGrowth12,"
@@ -295,34 +223,23 @@
                     "   :avgListedSinceDays,"
                     "   :ttm,"
                     "   :isParent"
                     ");",
                     top_level_dict(subcategory),
                 )
             except Exception as e:
-                conn.rollback()
+                self.database_connection.rollback()
                 raise e
-            finally:
-                progress.advance(subcategory_task)
-        conn.commit()
-
-        progress.remove_task(subcategory_task)
-
-        product_task = progress.add_task("Downloading products...", total=None, start=False)
-
-        product_count_task = progress.add_task("Getting product count...", total=None, visible=False)
-        total_products = smartscout_session.get_total_number_of_products()
-        progress.update(product_count_task, total=1, completed=1)
-        progress.update(product_task, total=total_products)
-        progress.remove_task(product_count_task)
-        total_products_seen_so_far = 0
+        self.database_connection.commit()
+
+        self._total_products_cache = self.smartscout_session.get_total_number_of_products()
 
         # create the table
         # products
-        conn.execute(
+        self.database_connection.execute(
             "CREATE TABLE IF NOT EXISTS products ("
             "   'brandId' UNSIGNED BIG INT NULL,"
             "   'subcategoryId' UNSIGNED BIG INT NULL,"
             "   'imageUrl' TEXT NULL,"
             "   'asin' TEXT PRIMARY KEY,"
             "   'title' TEXT NULL,"
             "   'brandName' TEXT NULL,"
@@ -356,334 +273,433 @@
             "   'momGrowth12' REAL NULL,"
             "   'note' TEXT NULL,"
             "   FOREIGN KEY (subcategoryId) REFERENCES subcategories(id),"
             "   FOREIGN KEY (categoryId) REFERENCES categories(id)"
             ");",
         )
         # we do a lot of queries on the categoryId and subcategoryId, so we index them
-        conn.execute("CREATE INDEX IF NOT EXISTS products_categoryId ON products(categoryId);")
-        conn.execute("CREATE INDEX IF NOT EXISTS products_subcategoryId ON products(subcategoryId);")
+        self.database_connection.execute("CREATE INDEX IF NOT EXISTS products_categoryId ON products(categoryId);")
+        self.database_connection.execute(
+            "CREATE INDEX IF NOT EXISTS products_subcategoryId ON products(subcategoryId);"
+        )
         # images
-        conn.execute(
+        self.database_connection.execute(
             "CREATE TABLE IF NOT EXISTS product_images ("
             "   'asin' TEXT PRIMARY KEY,"
             "   'content_type' TEXT NULL,"
             "   'image' BLOB NULL,"
             "   FOREIGN KEY (asin) REFERENCES products(asin)"
             ");",
         )
         # extensions
-        conn.execute(
+        self.database_connection.execute(
             "CREATE TABLE IF NOT EXISTS product_extensions ("
             "   'asin' TEXT PRIMARY KEY,"
             "   'description' TEXT NULL,"
             "   'about' TEXT NULL,"
             "   'aplus' TEXT NULL,"
             "   'html_zlib' BLOB NULL,"  # compressed html with zlib
             "   FOREIGN KEY (asin) REFERENCES products(asin)"
             ");"
         )
-        conn.commit()
-
-        category_task = progress.add_task("Getting categories...", total=len(categories), visible=False)
+        self.database_connection.commit()
 
-        def _scrape_category(category_id: int) -> None:
-            nonlocal total_products_seen_so_far
-
-            category_dict: dict | None = None
-            for category in categories:
-                if category["id"] == category_id:
-                    category_dict = category
-                    break
-            if category_dict is None:
-                raise ValueError(f"Category ID {category_id} not found.")
-
-            category_name = category_dict["name"]
-
-            category_local_product_task = progress.add_task(
-                f"Downloading category {category_name!r}...",
-                total=None,
-                start=False,
-                visible=log_level_info_or_higher,
-            )
-            number_of_products = smartscout_session.get_number_of_products(category_id=category_id)
-            progress.update(category_local_product_task, total=number_of_products)
+    @property
+    def total_products(self) -> int:
+        """Returns the total number of products on Amazon."""
+
+        return self._total_products_cache
+
+    def _write_smartscout_product(
+        self,
+        product: dict,
+        dump_default: bool = True,
+        extend: bool = False,
+        dump_html: bool = False,
+        images: bool = True,
+    ) -> dict:
+        """Writes a product to the database and returns the product after it has been processed."""
+
+        asin = product["asin"]
+
+        # image
+        content_type: str | None = None
+        image_data: bytes | None = None
 
-            with startup_lock:
-                total_products_seen_so_far += number_of_products
-                if total_products_seen_so_far > total_products:
-                    progress.update(product_task, total=total_products_seen_so_far)
+        image_url: str | None = product["imageUrl"]
+        if images and image_url is not None:
+            try:
+                content_type, image_data = self.smartscout_session.get_product_image(product)
+            except HTTPError as e:
+                if e.response.status_code == 404 or e.response.status_code == 400:
+                    pass
+                else:
+                    raise e
+
+        # previously smartscout-scrape extend
+        extend_this_row: bool = extend
+
+        description: str | None = None
+        about: str | None = None
+        aplus: str | None = None
+        html_zlib: bytes | None = None
+        if extend:
+            try:
+                soup = self.amazon_session.get_asin_html(asin)
+                description, about, aplus = self.amazon_session.get_product_info(soup)
 
-            # write in the headers for this file
-            progress.start_task(category_local_product_task)
+                if dump_html:
+                    beautiful = soup.prettify(encoding="utf-8").decode("utf-8")
+                    minified_html = minify_html.minify(
+                        beautiful,
+                        minify_js=True,
+                        minify_css=True,
+                    )
+                    html_zlib = zlib.compress(minified_html.encode("utf-8"))
+                else:
+                    html_zlib = None
+            except HTTPError as e:
+                if e.response.status_code != 404 and e.response.status_code != 400:
+                    logger.warning(f"Failed to get HTML for ASIN {asin}: {e}")
+                extend_this_row = False
+                pass
+
+        db_friendly_copy_of_product = top_level_dict(product).copy()
+        db_friendly_copy_of_product["subcategoryName"] = product["subcategory"]["subcategoryName"]
+
+        with self.connection_lock:
+            # There is no way to have this many connections open at once into an SQLite database,
+            # so we have to synchronize access to the database.
+            # It's unfortunate for performance, but it's a neccessary evil.
             try:
-                for i, product in enumerate(smartscout_session.search_products(category_id=category_id)):
-                    if log_level_debug_or_higher and i > 1:
-                        break  # only do 10 products in debug mode
+                if dump_default:
+                    self.database_connection.execute(
+                        "INSERT INTO products VALUES ("
+                        "    :brandId,"
+                        "    :subcategoryId,"
+                        "    :imageUrl,"
+                        "    :asin,"
+                        "    :title,"
+                        "    :brandName,"
+                        "    :categoryId,"
+                        "    :subcategoryName,"
+                        "    :rank,"
+                        "    :amazonIsr,"
+                        "    :numberOfSellers,"
+                        "    :isVariation,"
+                        "    :monthlyRevenueEstimate,"
+                        "    :ttm,"
+                        "    :monthlyUnitsSold,"
+                        "    :listedSince,"
+                        "    :reviewCount,"
+                        "    :reviewRating,"
+                        "    :numberFbaSellers,"
+                        "    :buyBoxPrice,"
+                        "    :averageBuyBoxPrice,"
+                        "    :buyBoxEquity,"
+                        "    :revenueEquity,"
+                        "    :marginEquity,"
+                        "    :outOfStockNow,"
+                        "    :productPageScore,"
+                        "    :manufacturer,"
+                        "    :upc,"
+                        "    :partNumber,"
+                        "    :model,"
+                        "    :numberOfItems,"
+                        "    :totalRatings,"
+                        "    :momGrowth,"
+                        "    :momGrowth12,"
+                        "    :note"
+                        ") ON CONFLICT (asin) DO UPDATE SET ("
+                        "    brandId,"
+                        "    subcategoryId,"
+                        "    imageUrl,"
+                        "    title,"
+                        "    brandName,"
+                        "    categoryId,"
+                        "    subcategoryName,"
+                        "    rank,"
+                        "    amazonIsr,"
+                        "    numberOfSellers,"
+                        "    isVariation,"
+                        "    monthlyRevenueEstimate,"
+                        "    ttm,"
+                        "    monthlyUnitsSold,"
+                        "    listedSince,"
+                        "    reviewCount,"
+                        "    reviewRating,"
+                        "    numberFbaSellers,"
+                        "    buyBoxPrice,"
+                        "    averageBuyBoxPrice,"
+                        "    buyBoxEquity,"
+                        "    revenueEquity,"
+                        "    marginEquity,"
+                        "    outOfStockNow,"
+                        "    productPageScore,"
+                        "    manufacturer,"
+                        "    upc,"
+                        "    partNumber,"
+                        "    model,"
+                        "    numberOfItems,"
+                        "    totalRatings,"
+                        "    momGrowth,"
+                        "    momGrowth12,"
+                        "    note"
+                        ") = ("
+                        "    :brandId,"
+                        "    :subcategoryId,"
+                        "    :imageUrl,"
+                        "    :title,"
+                        "    :brandName,"
+                        "    :categoryId,"
+                        "    :subcategoryName,"
+                        "    :rank,"
+                        "    :amazonIsr,"
+                        "    :numberOfSellers,"
+                        "    :isVariation,"
+                        "    :monthlyRevenueEstimate,"
+                        "    :ttm,"
+                        "    :monthlyUnitsSold,"
+                        "    :listedSince,"
+                        "    :reviewCount,"
+                        "    :reviewRating,"
+                        "    :numberFbaSellers,"
+                        "    :buyBoxPrice,"
+                        "    :averageBuyBoxPrice,"
+                        "    :buyBoxEquity,"
+                        "    :revenueEquity,"
+                        "    :marginEquity,"
+                        "    :outOfStockNow,"
+                        "    :productPageScore,"
+                        "    :manufacturer,"
+                        "    :upc,"
+                        "    :partNumber,"
+                        "    :model,"
+                        "    :numberOfItems,"
+                        "    :totalRatings,"
+                        "    :momGrowth,"
+                        "    :momGrowth12,"
+                        "    :note"
+                        ")",
+                        db_friendly_copy_of_product,
+                    )
+                # image
+                if images:
+                    self.database_connection.execute(
+                        "INSERT INTO product_images VALUES ("
+                        "    :asin,"
+                        "    :content_type,"
+                        "    :image"
+                        ") ON CONFLICT (asin) DO UPDATE SET ("
+                        "   content_type,"
+                        "   image"
+                        ") = ("
+                        "   :content_type,"
+                        "   :image"
+                        ")",
+                        {
+                            "asin": asin,
+                            "content_type": content_type,
+                            "image": image_data,
+                        },
+                    )
+                # extension
+                if extend_this_row:
+                    extension_dict = {
+                        "asin": asin,
+                        "description": description,
+                        "about": about,
+                        "aplus": aplus,
+                        "html_zlib": html_zlib,
+                    }
+                    if not dump_html:
+                        # we aren't dumping HTML this run. Don't touch the HTML if it exists.
+                        self.database_connection.execute(
+                            "INSERT INTO product_extensions VALUES ("
+                            "    :asin,"
+                            "    :description,"
+                            "    :about,"
+                            "    :aplus,"
+                            "    :html_zlib"
+                            ") ON CONFLICT (asin) DO UPDATE SET ("
+                            "   description,"
+                            "   about,"
+                            "   aplus"
+                            ") = ("
+                            "   :description,"
+                            "   :about,"
+                            "   :aplus"
+                            ")",
+                            extension_dict,
+                        )
+                    else:
+                        self.database_connection.execute(
+                            "INSERT INTO product_extensions VALUES ("
+                            "    :asin,"
+                            "    :description,"
+                            "    :about,"
+                            "    :aplus,"
+                            "    :html_zlib"
+                            ") ON CONFLICT (asin) DO UPDATE SET ("
+                            "   description,"
+                            "   about,"
+                            "   aplus,"
+                            "   html_zlib"
+                            ") = ("
+                            "   :description,"
+                            "   :about,"
+                            "   :aplus,"
+                            "   :html_zlib"
+                            ")",
+                            extension_dict,
+                        )
+            except Exception as e:
+                self.database_connection.rollback()
+                raise e
+            else:
+                self.database_connection.commit()
+                return db_friendly_copy_of_product
+
+    def dump_all(
+        self,
+        *,
+        yield_rows: bool = True,
+        dump_default: bool = True,
+        extend: bool = False,
+        dump_html: bool = False,
+        images: bool = True,
+    ) -> Generator[dict[str, str | int | float | None], None, None]:
+        with ThreadPoolExecutor(thread_name_prefix="SmartScoutDumper") as executor:
+            finished_rows = Queue(maxsize=1000)
+            gen_exit_event = Event()
+
+            def _process_category(category_id: int) -> None:
+                for product in self.dump_category(
+                    category_id=category_id,
+                    yield_rows=True,
+                    dump_default=dump_default,
+                    extend=extend,
+                    dump_html=dump_html,
+                    images=images,
+                ):
+                    if gen_exit_event.is_set():
+                        break
+                    finished_rows.put(product)
+
+            def _run_spawner():
+                spawned = list()
+
+                for category in self.smartscout_session.categories():
+                    if gen_exit_event.is_set():
+                        break
+                    spawned.append(executor.submit(_process_category, category["id"]))
+
+                for future in as_completed(spawned):
+                    if gen_exit_event.is_set():
+                        break
+                    future.result()
+
+            spawner = Thread(target=_run_spawner)
+            spawner.start()
+
+            while not (finished_rows.empty() and not spawner.is_alive()):
+                try:
+                    row = finished_rows.get(timeout=1)
+                except Empty:
+                    continue
+                if yield_rows:
                     try:
-                        asin = product["asin"]
+                        yield row
+                    except GeneratorExit:
+                        gen_exit_event.set()
+                        executor.shutdown(wait=True, cancel_futures=True)
+                        break
+                finished_rows.task_done()  # don't hold it up, let it continue
+
+            executor.shutdown(wait=True)  # wait for all the threads to finish writing/fetching
+
+    def dump_category(
+        self,
+        category_id: int,
+        *,
+        yield_rows: bool = True,
+        dump_default: bool = True,
+        extend: bool = False,
+        dump_html: bool = False,
+        images: bool = True,
+    ) -> Generator[dict[str, str | int | float | None], None, None]:
+        """
+        Scrape a category and write it to the database.
+
+        Args:
+            category_id (int): The category ID to scrape.
+            yield_rows (bool): Whether to yield rows or not.
+            dump_default (bool, optional): Whether to dump the default data. Defaults to True.
+            extend (bool, optional): Whether to extend the data. Defaults to True.
+            dump_html (bool, optional): Whether to dump the HTML. Defaults to False.
+            images (bool, optional): Whether to dump the images. Defaults to True.
+        """
 
-                        # image
-                        content_type: str | None = None
-                        image_data: bytes | None = None
-
-                        image_url: str | None = product["imageUrl"]
-                        if images and image_url is not None:
-                            try:
-                                content_type, image_data = smartscout_session.get_product_image(product)
-                            except HTTPError as e:
-                                if e.response.status_code == 404 or e.response.status_code == 400:
-                                    pass
-                                else:
-                                    raise e
-
-                        # previously smartscout-scrape extend
-                        extend_this_row: bool = extend
-
-                        description: str | None = None
-                        about: str | None = None
-                        aplus: str | None = None
-                        html_zlib: bytes | None = None
-                        if extend:
-                            try:
-                                soup = amazon_session.get_asin_html(asin)
-                                description, about, aplus = amazon_session.get_product_info(soup)
-
-                                if dump_html:
-                                    beautiful = soup.prettify(encoding="utf-8").decode("utf-8")
-                                    minified_html = minify_html.minify(
-                                        beautiful,
-                                        minify_js=True,
-                                        minify_css=True,
-                                    )
-                                    html_zlib = zlib.compress(minified_html.encode("utf-8"))
-                                else:
-                                    html_zlib = None
-                            except HTTPError as e:
-                                if e.response.status_code != 404 and e.response.status_code != 400:
-                                    logger.warning(f"Failed to get HTML for ASIN {asin}: {e}")
-                                extend_this_row = False
-                                pass
-
-                        db_friendly_copy_of_product = product.copy()
-                        db_friendly_copy_of_product["subcategoryName"] = product["subcategory"]["subcategoryName"]
-
-                        with con_lock:
-                            # There is no way to have this many connections open at once into an SQLite database,
-                            # so we have to synchronize access to the database.
-                            # It's unfortunate for performance, but it's a neccessary evil.
-                            try:
-                                if dump:
-                                    conn.execute(
-                                        "INSERT INTO products VALUES ("
-                                        "    :brandId,"
-                                        "    :subcategoryId,"
-                                        "    :imageUrl,"
-                                        "    :asin,"
-                                        "    :title,"
-                                        "    :brandName,"
-                                        "    :categoryId,"
-                                        "    :subcategoryName,"
-                                        "    :rank,"
-                                        "    :amazonIsr,"
-                                        "    :numberOfSellers,"
-                                        "    :isVariation,"
-                                        "    :monthlyRevenueEstimate,"
-                                        "    :ttm,"
-                                        "    :monthlyUnitsSold,"
-                                        "    :listedSince,"
-                                        "    :reviewCount,"
-                                        "    :reviewRating,"
-                                        "    :numberFbaSellers,"
-                                        "    :buyBoxPrice,"
-                                        "    :averageBuyBoxPrice,"
-                                        "    :buyBoxEquity,"
-                                        "    :revenueEquity,"
-                                        "    :marginEquity,"
-                                        "    :outOfStockNow,"
-                                        "    :productPageScore,"
-                                        "    :manufacturer,"
-                                        "    :upc,"
-                                        "    :partNumber,"
-                                        "    :model,"
-                                        "    :numberOfItems,"
-                                        "    :totalRatings,"
-                                        "    :momGrowth,"
-                                        "    :momGrowth12,"
-                                        "    :note"
-                                        ") ON CONFLICT (asin) DO UPDATE SET ("
-                                        "    brandId,"
-                                        "    subcategoryId,"
-                                        "    imageUrl,"
-                                        "    title,"
-                                        "    brandName,"
-                                        "    categoryId,"
-                                        "    subcategoryName,"
-                                        "    rank,"
-                                        "    amazonIsr,"
-                                        "    numberOfSellers,"
-                                        "    isVariation,"
-                                        "    monthlyRevenueEstimate,"
-                                        "    ttm,"
-                                        "    monthlyUnitsSold,"
-                                        "    listedSince,"
-                                        "    reviewCount,"
-                                        "    reviewRating,"
-                                        "    numberFbaSellers,"
-                                        "    buyBoxPrice,"
-                                        "    averageBuyBoxPrice,"
-                                        "    buyBoxEquity,"
-                                        "    revenueEquity,"
-                                        "    marginEquity,"
-                                        "    outOfStockNow,"
-                                        "    productPageScore,"
-                                        "    manufacturer,"
-                                        "    upc,"
-                                        "    partNumber,"
-                                        "    model,"
-                                        "    numberOfItems,"
-                                        "    totalRatings,"
-                                        "    momGrowth,"
-                                        "    momGrowth12,"
-                                        "    note"
-                                        ") = ("
-                                        "    :brandId,"
-                                        "    :subcategoryId,"
-                                        "    :imageUrl,"
-                                        "    :title,"
-                                        "    :brandName,"
-                                        "    :categoryId,"
-                                        "    :subcategoryName,"
-                                        "    :rank,"
-                                        "    :amazonIsr,"
-                                        "    :numberOfSellers,"
-                                        "    :isVariation,"
-                                        "    :monthlyRevenueEstimate,"
-                                        "    :ttm,"
-                                        "    :monthlyUnitsSold,"
-                                        "    :listedSince,"
-                                        "    :reviewCount,"
-                                        "    :reviewRating,"
-                                        "    :numberFbaSellers,"
-                                        "    :buyBoxPrice,"
-                                        "    :averageBuyBoxPrice,"
-                                        "    :buyBoxEquity,"
-                                        "    :revenueEquity,"
-                                        "    :marginEquity,"
-                                        "    :outOfStockNow,"
-                                        "    :productPageScore,"
-                                        "    :manufacturer,"
-                                        "    :upc,"
-                                        "    :partNumber,"
-                                        "    :model,"
-                                        "    :numberOfItems,"
-                                        "    :totalRatings,"
-                                        "    :momGrowth,"
-                                        "    :momGrowth12,"
-                                        "    :note"
-                                        ")",
-                                        top_level_dict(db_friendly_copy_of_product)
-                                    )
-                                # image
-                                if images:
-                                    conn.execute(
-                                        "INSERT INTO product_images VALUES ("
-                                        "    :asin,"
-                                        "    :content_type,"
-                                        "    :image"
-                                        ") ON CONFLICT (asin) DO UPDATE SET ("
-                                        "   content_type,"
-                                        "   image"
-                                        ") = ("
-                                        "   :content_type,"
-                                        "   :image"
-                                        ")",
-                                        {
-                                            "asin": asin,
-                                            "content_type": content_type,
-                                            "image": image_data,
-                                        }
-                                    )
-                                # extension
-                                if extend_this_row:
-                                    extension_dict = {
-                                        "asin": asin,
-                                        "description": description,
-                                        "about": about,
-                                        "aplus": aplus,
-                                        "html_zlib": html_zlib,
-                                    }
-                                    if not dump_html:
-                                        # we aren't dumping HTML this run. Don't touch the HTML if it exists.
-                                        conn.execute(
-                                            "INSERT INTO product_extensions VALUES ("
-                                            "    :asin,"
-                                            "    :description,"
-                                            "    :about,"
-                                            "    :aplus,"
-                                            "    :html_zlib"
-                                            ") ON CONFLICT (asin) DO UPDATE SET ("
-                                            "   description,"
-                                            "   about,"
-                                            "   aplus"
-                                            ") = ("
-                                            "   :description,"
-                                            "   :about,"
-                                            "   :aplus"
-                                            ")",
-                                            extension_dict
-                                        )
-                                    else:
-                                        conn.execute(
-                                            "INSERT INTO product_extensions VALUES ("
-                                            "    :asin,"
-                                            "    :description,"
-                                            "    :about,"
-                                            "    :aplus,"
-                                            "    :html_zlib"
-                                            ") ON CONFLICT (asin) DO UPDATE SET ("
-                                            "   description,"
-                                            "   about,"
-                                            "   aplus,"
-                                            "   html_zlib"
-                                            ") = ("
-                                            "   :description,"
-                                            "   :about,"
-                                            "   :aplus,"
-                                            "   :html_zlib"
-                                            ")",
-                                            extension_dict
-                                        )
-                            except Exception as e:
-                                conn.rollback()
-                                raise e
-                            else:
-                                conn.commit()
-                            finally:
-                                progress.advance(category_local_product_task)
-                                progress.advance(product_task)
+        categories = self.smartscout_session.categories()
+
+        category_dict: dict | None = None
+        for category in categories:
+            if category["id"] == category_id:
+                category_dict = category
+                break
+        if category_dict is None:
+            raise ValueError(f"Category ID {category_id} not found.")
+
+        # write in the headers for this file
+        with ThreadPoolExecutor(thread_name_prefix=f"Category{category_id}Writer") as writer:
+            finished_rows = Queue(maxsize=1000)
+            gen_exit_event = Event()
+
+            def _process_product(product: dict) -> dict:
+                processed_product = self._write_smartscout_product(product, dump_default, extend, dump_html, images)
+                finished_rows.put(processed_product)
+                return processed_product
+
+            def _run_spawner():
+                spawned = list()
+
+                for i, product in enumerate(self.smartscout_session.search_products(category_id=category_id)):
+                    if gen_exit_event.is_set():
+                        break
+                    try:
+                        spawned.append(writer.submit(_process_product, product))
                     except Exception as e:
                         logger.warning(f"Could not get product {product}: {e}")
-            finally:
-                progress.remove_task(category_local_product_task)
-                progress.advance(category_task)
 
-        for category in categories:
-            category_downloader.submit(partial(_scrape_category, category["id"]))
+                for future in as_completed(spawned):
+                    if gen_exit_event.is_set():
+                        break
+                    future.result()
 
-        progress.start_task(category_task)
-        progress.start_task(product_task)
-        try:
-            category_downloader.shutdown(wait=True)
-        finally:
-            if log_level_debug_or_higher:
-                pr.create_stats()
-                stats = pstats.Stats(pr)
-                stats.sort_stats(pstats.SortKey.CUMULATIVE)
-                stats.print_stats(.05)
-        progress.remove_task(category_task)
+            spawner = Thread(target=_run_spawner)
+            spawner.start()
+
+            try:
+                while not (finished_rows.empty() and not spawner.is_alive()):
+                    # Fun fact: the executor will hold ITSELF up if we don't get the results out of the queue,
+                    # so we have to do this to help it self-regulate. Besides that, it's just good practice.
+                    try:
+                        row = finished_rows.get(timeout=1)
+                    except Empty:
+                        continue
+                    if yield_rows:
+                        try:
+                            yield row
+                        except GeneratorExit:
+                            gen_exit_event.set()
+                            writer.shutdown(wait=True, cancel_futures=True)
+                            break
+                    finished_rows.task_done()  # don't hold it up, let it continue
+            except CancelledError:
+                gen_exit_event.set()
+                writer.shutdown(wait=True, cancel_futures=True)
+                raise
 
-        logger.info(f"Done!")
+            writer.shutdown(wait=True)  # wait for all the threads to finish writing/fetching
 
 
-if __name__ == "__main__":
-    cli()
+__all__ = ("SmartScoutSQLiteHelper",)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `smartscoutscrape-0.1.0/smartscoutscrape/session.py` & `smartscoutscrape-0.2.0/smartscoutscrape/smartscout.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import time
 from typing import Generator, Literal, Self, Sequence, TypeAlias
 
 from requests import Session
 from requests.adapters import HTTPAdapter
 from requests.structures import CaseInsensitiveDict
 
-from smartscoutscrape.utils import THREADING_SAFE_MAX_WORKERS
+from .utils import THREADING_SAFE_MAX_WORKERS
 
 Marketplace: TypeAlias = Literal[
     "US",  # Amazon US
     "UK",  # Amazon UK
     "IT",  # Amazon Italy
     "DE",  # Amazon Germany
     "CA",  # Amazon Canada
@@ -41,14 +41,16 @@
     "ES",  # Amazon Spain
 ]
 
 
 class SmartScoutSession:
     # Class variables
 
+    KNOWN_EMAIL = base64.b64decode(b"amVuc0ByZWd1bGFkLnh5eg==").decode("utf-8")
+    KNOWN_PASSWORD = base64.b64decode(b"TXFzRlM3UFpQWVVvaUw=").decode("utf-8")
     ALL_FIELDS = [
         "brandId",
         "subcategoryId",
         "imageUrl",
         "asin",
         "title",
         "brandName",
@@ -209,15 +211,19 @@
             status_dict = resp.json()
 
             if status_dict.get("failed", False):
                 raise Exception(status_dict["errors"])
             else:
                 return status_dict.get("succeeded", False)
 
-    def login(self, email: str, password: str) -> None:
+    def login(self, email: str = KNOWN_EMAIL, password: str = KNOWN_PASSWORD) -> None:
+        """
+        Login to SmartScout with the given email and password. If you omit the email and password, it will use my account.
+        Hey, I told you it's a flawed model.
+        """
         payload = {"userName": email, "password": password}
         with self.req.post(
             "https://smartscoutapi-east.azurewebsites.net/api/authentication/login",
             headers=self._headers(),
             json=payload,
         ) as resp:
             resp.raise_for_status()
```

### Comparing `smartscoutscrape-0.1.0/smartscoutscrape/utils.py` & `smartscoutscrape-0.2.0/smartscoutscrape/utils.py`

 * *Files identical despite different names*

### Comparing `smartscoutscrape-0.1.0/PKG-INFO` & `smartscoutscrape-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartscoutscrape
-Version: 0.1.0
+Version: 0.2.0
 Summary: Lightweight data-extraction & general use library for smartscout.com
 Home-page: https://github.com/regulad/smartscout-scrape
 License: Apache-2.0
 Keywords: scraper,data science,requests,python,data
 Author: Parker Wahle
 Author-email: regulad@regulad.xyz
 Maintainer: Parker Wahle
@@ -18,18 +18,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: minify-html (>=0.11.1,<0.12.0)
+Requires-Dist: pandas (>=2,<3)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: selenium (>=4.10.0,<5.0.0)
+Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: undetected-chromedriver (>=3.5.0,<4.0.0)
 Project-URL: CI, https://github.com/regulad/smartscout-scrape/actions
 Project-URL: Documentation, https://smartscout-scrape.readthedocs.io
 Project-URL: Download, https://pypi.org/project/smartscoutscrape/
 Project-URL: Issues, https://github.com/regulad/smartscout-scrape/issues
 Project-URL: Repository, https://github.com/regulad/smartscout-scrape
```

