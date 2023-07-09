# Comparing `tmp/fastchecks-0.1.0.dev0.tar.gz` & `tmp/fastchecks-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.1.0.dev0.tar", max compression
+gzip compressed data, was "fastchecks-0.1.0rc0.tar", max compression
```

## Comparing `fastchecks-0.1.0.dev0.tar` & `fastchecks-0.1.0rc0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      286 2023-07-07 15:52:57.887512 fastchecks-0.1.0.dev0/README.md
--rw-r--r--   0        0        0      707 2023-07-07 15:33:29.346736 fastchecks-0.1.0.dev0/fastchecks/__init__.py
--rw-r--r--   0        0        0     4714 2023-07-07 15:33:29.346844 fastchecks-0.1.0.dev0/fastchecks/check.py
--rw-r--r--   0        0        0     3996 2023-07-07 15:33:29.346940 fastchecks-0.1.0.dev0/fastchecks/check_quick.py
--rw-r--r--   0        0        0     1471 2023-07-07 15:33:29.347022 fastchecks-0.1.0.dev0/fastchecks/conf.py
--rw-r--r--   0        0        0     1398 2023-07-07 15:33:29.347125 fastchecks-0.1.0.dev0/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     4089 2023-07-07 15:33:29.347229 fastchecks-0.1.0.dev0/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0     1681 2023-07-07 15:33:29.347339 fastchecks-0.1.0.dev0/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     5232 2023-07-07 15:33:29.347434 fastchecks-0.1.0.dev0/fastchecks/types.py
--rw-r--r--   0        0        0     3204 2023-07-07 15:33:29.347516 fastchecks-0.1.0.dev0/fastchecks/util.py
--rw-r--r--   0        0        0     1157 2023-07-07 15:54:52.144726 fastchecks-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 fastchecks-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-07-09 17:17:25.642629 fastchecks-0.1.0rc0/README.md
+-rw-r--r--   0        0        0      707 2023-07-09 17:17:25.642969 fastchecks-0.1.0rc0/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4681 2023-07-09 17:17:25.643240 fastchecks-0.1.0rc0/fastchecks/check.py
+-rw-r--r--   0        0        0     2067 2023-07-09 17:17:25.643588 fastchecks-0.1.0rc0/fastchecks/cli.py
+-rw-r--r--   0        0        0     2754 2023-07-09 17:17:25.643960 fastchecks-0.1.0rc0/fastchecks/conf.py
+-rw-r--r--   0        0        0     5228 2023-07-09 17:17:25.644201 fastchecks-0.1.0rc0/fastchecks/runner.py
+-rw-r--r--   0        0        0     2048 2023-07-09 17:17:25.644600 fastchecks-0.1.0rc0/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     4584 2023-07-09 17:17:25.644821 fastchecks-0.1.0rc0/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      526 2023-07-09 17:17:25.645153 fastchecks-0.1.0rc0/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.1.0rc0/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     5820 2023-07-09 17:17:25.645626 fastchecks-0.1.0rc0/fastchecks/types.py
+-rw-r--r--   0        0        0     4261 2023-07-09 17:17:25.645812 fastchecks-0.1.0rc0/fastchecks/util.py
+-rw-r--r--   0        0        0     1463 2023-07-09 17:17:25.702192 fastchecks-0.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 fastchecks-0.1.0rc0/PKG-INFO
```

### Comparing `fastchecks-0.1.0.dev0/fastchecks/__init__.py` & `fastchecks-0.1.0rc0/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.1.0.dev0/fastchecks/check.py` & `fastchecks-0.1.0rc0/fastchecks/check.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,22 +87,14 @@
                     other_error=True,
                 )
 
     finally:
         response_ftr.close()
 
 
-__ARBITRARY_TOO_BIG_CONTENT_LENGTH = 100000
-"""
-Arbitrary value to consider a response's content length as too big to be read in memory.
-
-For reference, the size of https://python.org is, as of 2023-07-06, 49943 bytes.
-"""
-
-
 async def search_pattern_whole_text_body(regex: str, response: aiohttp.ClientResponse) -> str | bool | None:
     """
     Search for a regex pattern in the response's content (assumed to be in most cases HTML).
 
     WARNING: the whole response's body is read in memory.
 
     To alleviate this:
@@ -113,17 +105,21 @@
 
 
     MAYBE (Alternatives):
     * If regex search can limited to a line, we could use use response.content.readline() instead of response.text().
     * The text body searched is raw HTML (in most cases), not the HTML's text. If we want to search the text of the HTML (or other text-based format) only, we would need a corresponding parser.
     """
     if is_likely_text_based_body(response) and is_content_length_less_than(
-        response, length=__ARBITRARY_TOO_BIG_CONTENT_LENGTH, allow_none_content_length=True
+        response, length=conf.TOO_BIG_CONTENT_LENGTH_KB, allow_none_content_length=True
     ):
         content = await response.text()
         match_opt = re.search(regex, content)
+
         if match_opt:
             return match_opt[0]
         else:
             return False
     else:
+        logging.warning(
+            f"The regex will not be checked because the response's body might be unsafe to read in memory (too big or not text-based), for url: {response.url}"
+        )
         return None
```

### Comparing `fastchecks-0.1.0.dev0/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.1.0rc0/fastchecks/sockets/postgres/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,53 @@
+from typing import AsyncIterator
 from pydantic import PositiveInt
-from fastchecks.types import CheckResult, WebsiteCheck
+from fastchecks.types import CheckResult, WebsiteCheckScheduled, WebsiteCheck
 from fastchecks.sockets import CheckResultSocket, WebsiteCheckSocket
 from psycopg_pool import AsyncConnectionPool
 from psycopg.rows import namedtuple_row
 from psycopg import sql
 
 
 class WebsiteCheckSocketPostgres(WebsiteCheckSocket):
     def __init__(self, conninfo: str) -> None:
         self.__pool = AsyncConnectionPool(conninfo)
 
-    async def upsert(self, check: WebsiteCheck) -> None:
+    def is_closed(self) -> bool:
+        return self.__pool.closed
+
+    async def upsert(self, check: WebsiteCheckScheduled) -> None:
         async with self.__pool.connection() as aconn:
             await aconn.execute(
                 """
             INSERT INTO WebsiteCheck
-            (url, regex)
-            VALUES (%s, %s)
+            (url, regex, interval_seconds)
+            VALUES (%s, %s, %s)
             ON CONFLICT (url) DO UPDATE
                 SET regex = EXCLUDED.regex;
             """,
-                (check.url, check.regex),
+                (check.url, check.regex, check.interval_seconds),
             )
 
-    async def read_last_n(self, n: PositiveInt):
+    async def read_n(self, n: PositiveInt) -> AsyncIterator[WebsiteCheckScheduled]:
         async with self.__pool.connection() as aconn:
             # We format the safe query in 2 steps (also below) to avoid false positives from bandit (B608:hardcoded_sql_expressions)
             # We follow psycopg recommendations for how to escape composed SQL queries: https://www.psycopg.org/psycopg3/docs/advanced/typing.html#checking-literal-strings-in-queries
             query_raw = """
                 SELECT * FROM WebsiteCheck
                 LIMIT {};"""
             query_safe = query_raw.format(n)
 
             acur = await aconn.execute(sql.SQL(query_safe))
 
             acur.row_factory = namedtuple_row
             async for row in acur:
-                yield WebsiteCheck.create_without_validation(row.url, row.regex)
+                # without validation, because we trust the database -- its value were validated before
+                yield WebsiteCheckScheduled.with_check(
+                    WebsiteCheck.without_validation(row.url, row.regex), row.interval_seconds
+                )
 
     async def delete(self, url: str) -> None:
         async with self.__pool.connection() as aconn:
             await aconn.execute(
                 """
             DELETE FROM WebsiteCheck
             WHERE url = %s;""",
@@ -51,14 +58,17 @@
         return await self.__pool.close()
 
 
 class CheckResultSocketPostgres(CheckResultSocket):
     def __init__(self, conninfo: str) -> None:
         self.__pool = AsyncConnectionPool(conninfo)
 
+    def is_closed(self) -> bool:
+        return self.__pool.closed
+
     async def write(self, result: CheckResult) -> None:
         async with self.__pool.connection() as aconn:
             await aconn.execute(
                 """
             INSERT INTO CheckResult
             (url, regex, timestamp_start, response_time, timeout_error, host_error, other_error, response_status, regex_match)
             VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s);""",
@@ -74,28 +84,28 @@
                     result.other_error,
                     #
                     result.response_status,
                     result.regex_match_to_bool_or_none(),
                 ),
             )
 
-    async def read_last_n(self, n: PositiveInt):
+    async def read_last_n(self, n: PositiveInt) -> AsyncIterator[CheckResult]:
         async with self.__pool.connection() as aconn:
             query_raw = """
                 SELECT * FROM CheckResult
                 ORDER BY timestamp_start DESC
                 LIMIT {};"""
             query_safe = query_raw.format(n)
 
             acur = await aconn.execute(sql.SQL(query_safe))
 
             acur.row_factory = namedtuple_row
             async for row in acur:
                 yield CheckResult(
-                    check=WebsiteCheck.create_without_validation(row.url, row.regex),
+                    check=WebsiteCheck.without_validation(row.url, row.regex),
                     #
                     timestamp_start=row.timestamp_start,
                     response_time=row.response_time,
                     #
                     timeout_error=row.timeout_error,
                     host_error=row.host_error,
                     other_error=row.other_error,
```

### Comparing `fastchecks-0.1.0.dev0/fastchecks/types.py` & `fastchecks-0.1.0rc0/fastchecks/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,81 @@
 import datetime
 from pydantic import BaseModel
 
 from fastchecks.util import validate_regex, validate_url
-from fastchecks import require
+from fastchecks import conf, require
 
 
 # We use Pydantic classes for type safety and because they could be handy in the future for de/serialization.
 # See benchmarks with other alternatives (e.g. NamedTuple): https://janhendrikewers.uk/pydantic_vs_protobuf_vs_namedtuple_vs_dataclasses.html
 # Note that Pydantic V2 (released in 2023 June) promises a 5-50x speedup over V1: https://docs.pydantic.dev/2.0/blog/pydantic-v2-alpha/#headlines
 
 
 class WebsiteCheck(BaseModel):
     url: str
     regex: str | None = None
 
     @classmethod
-    def create_with_validation(cls, url: str, regex: str | None = None) -> "WebsiteCheck":
+    def with_validation(cls, url: str, regex: str | None = None) -> "WebsiteCheck":
         """
         Validate the given URL and regex (if any), and return a WebsiteCheck instance.
 
         If the URL or regex are invalid, raise ValueError.
         """
         validate_url(url)
         if regex is not None:
             validate_regex(regex)
         return cls(url=url, regex=regex)
 
     @classmethod
-    def create_without_validation(cls, url: str, regex: str | None = None) -> "WebsiteCheck":
+    def without_validation(cls, url: str, regex: str | None = None) -> "WebsiteCheck":
         """
         Return a WebsiteCheck instance without validating the given URL and regex (if any).
 
         Only use this method if you are sure that the URL and regex are valid (e.g., they were validated before).
         """
         return cls(url=url, regex=regex)
 
 
+class WebsiteCheckScheduled(WebsiteCheck):
+    """
+    WebsiteCheck with an schedule.
+    """
+
+    # url: str
+    # regex: str | None = None
+    interval_seconds: int | None
+    """If None, later a system's default value will be used."""
+
+    @classmethod
+    def with_check(cls, check: WebsiteCheck, interval_seconds: int | None) -> "WebsiteCheckScheduled":
+        if interval_seconds is not None:
+            conf.validate_interval(interval_seconds)
+
+        return cls(url=check.url, regex=check.regex, interval_seconds=interval_seconds)
+
+
 class CheckResult(BaseModel):
-    # The check that generated this result
+    #
     check: WebsiteCheck
+    """The check that generated this result"""
+    #
     # Common values
+    #
     timestamp_start: datetime.datetime
     response_time: float
+    #
     # Connection error values
+    #
     timeout_error: bool
     host_error: bool
     other_error: bool
-    # Response values (OK response, <400, or not)
+    #
+    # Response values (note: OK response, <400, or not)
+    #
     response_status: int | None
     regex_match: str | bool | None
     """
     str: the tested regex matched and the matched string is this value.
     bool True: the tested regex matched but the matched string is not available.
     bool False: the tested regex did not match.
     None: means "not tested" (e.g. there was no regex to test, the response was not OK, or the response body was ignored because it was too big or not text).
```

### Comparing `fastchecks-0.1.0.dev0/PKG-INFO` & `fastchecks-0.1.0rc0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: fastchecks
-Version: 0.1.0.dev0
+Version: 0.1.0rc0
 Summary: 
 Author: Dr. Juan Miguel Cejuela
 Author-email: i@juanmi.rocks
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: apscheduler (==4.0.0a2)
 Requires-Dist: psycopg[binary,pool] (>=3.1.9,<4.0.0)
 Requires-Dist: pydantic (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 🚥 Website monitoring backend service - in Python 🐍 - check results written into PostgreSQL 🐘
 
 [![test & lint](https://github.com/juanmirocks/fastchecks/actions/workflows/test_n_lint.yml/badge.svg)](https://github.com/juanmirocks/fastchecks/actions/workflows/test_n_lint.yml)
 
+[![Coverage Status](https://coveralls.io/repos/github/juanmirocks/fastchecks/badge.svg?branch=develop)](https://coveralls.io/github/juanmirocks/fastchecks?branch=develop)
```

