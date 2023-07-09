# Comparing `tmp/whois-parser-0.1.4.tar.gz` & `tmp/whois_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois-parser-0.1.4.tar", max compression
+gzip compressed data, was "whois_parser-0.2.0.tar", max compression
```

## Comparing `whois-parser-0.1.4.tar` & `whois_parser-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1070 2021-05-29 22:39:35.970026 whois-parser-0.1.4/LICENSE
--rw-r--r--   0        0        0     1952 2021-06-05 06:29:47.529040 whois-parser-0.1.4/README.md
--rw-r--r--   0        0        0      942 2022-02-05 00:41:53.220906 whois-parser-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      221 2021-11-26 20:18:23.176101 whois-parser-0.1.4/whois_parser/__init__.py
--rw-r--r--   0        0        0     1125 2021-06-04 22:34:55.273819 whois-parser-0.1.4/whois_parser/dataclasses.py
--rw-r--r--   0        0        0     1314 2021-06-05 06:27:19.615143 whois-parser-0.1.4/whois_parser/parser.py
--rw-r--r--   0        0        0      136 2021-06-04 22:34:55.275041 whois-parser-0.1.4/whois_parser/parsers/__init__.py
--rw-r--r--   0        0        0    10955 2021-11-26 09:43:10.026572 whois-parser-0.1.4/whois_parser/parsers/abstract.py
--rw-r--r--   0        0        0     6391 2021-06-04 22:34:55.276237 whois-parser-0.1.4/whois_parser/parsers/base.py
--rw-r--r--   0        0        0      406 2021-06-04 22:34:55.276686 whois-parser-0.1.4/whois_parser/parsers/be.py
--rw-r--r--   0        0        0      117 2021-11-26 09:43:10.027133 whois-parser-0.1.4/whois_parser/parsers/constants.py
--rw-r--r--   0        0        0     1873 2021-06-04 22:34:55.276967 whois-parser-0.1.4/whois_parser/parsers/jp.py
--rw-r--r--   0        0        0      399 2021-06-04 22:34:55.277198 whois-parser-0.1.4/whois_parser/parsers/uk.py
--rw-r--r--   0        0        0     1473 2021-11-26 09:39:11.618434 whois-parser-0.1.4/whois_parser/parsers/utils.py
--rw-r--r--   0        0        0     2899 2022-02-05 00:42:05.101512 whois-parser-0.1.4/setup.py
--rw-r--r--   0        0        0     2763 2022-02-05 00:42:05.101924 whois-parser-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-09 01:02:06.011940 whois_parser-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1952 2023-07-09 01:02:06.011940 whois_parser-0.2.0/README.md
+-rw-r--r--   0        0        0      834 2023-07-09 01:02:25.140238 whois_parser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/__init__.py
+-rw-r--r--   0        0        0      978 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/dataclasses.py
+-rw-r--r--   0        0        0     1302 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parser.py
+-rw-r--r--   0        0        0      136 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/__init__.py
+-rw-r--r--   0        0        0    10889 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/abstract.py
+-rw-r--r--   0        0        0     6385 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/base.py
+-rw-r--r--   0        0        0      406 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/be.py
+-rw-r--r--   0        0        0      117 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/constants.py
+-rw-r--r--   0        0        0     1867 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/jp.py
+-rw-r--r--   0        0        0      399 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/uk.py
+-rw-r--r--   0        0        0     1536 2023-07-09 01:02:06.011940 whois_parser-0.2.0/whois_parser/parsers/utils.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 whois_parser-0.2.0/PKG-INFO
```

### Comparing `whois-parser-0.1.4/LICENSE` & `whois_parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whois-parser-0.1.4/README.md` & `whois_parser-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `whois-parser-0.1.4/pyproject.toml` & `whois_parser-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 [tool.poetry]
 name = "whois-parser"
-version = "0.1.4"
+version = "0.2.0"
 description = "Yet another whois parser for Python"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 homepage = "https://github.com/ninoseki/whois-parser"
 repository = "https://github.com/ninoseki/whois-parser"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-dataclasses-json = "^0.5.5"
-dateparser = "^1.1.0"
-importlib-metadata = {version = "^4.8.2", python = "<3.8"}
-pyparsing = "^3.0.7"
+python = ">=3.9,<4.0"
+dateparser = ">=1.1,<2.0"
+pyparsing = ">=3.0,<4.0"
 
 [tool.poetry.dev-dependencies]
-autoflake = "^1.4"
-autopep8 = "^1.6.0"
-black = "^21.11b1"
+black = "^23.3"
 coveralls = "^3.3.1"
-httpx = "^0.21.1"
-isort = "^5.10.1"
-mypy = "^0.910"
-pre-commit = "^2.15.0"
-pytest = "^6.2.5"
-pytest-asyncio = "^0.16.0"
-pytest-cov = "^3.0.0"
-pytest-mock = "^3.6.1"
-pytest-randomly = "^3.10.2"
-pytest-sugar = "^0.9.4"
-pyupgrade = "^2.29.1"
-sh = "^1.14.2"
-loguru = "^0.5.3"
+isort = "^5.12"
+mypy = "^1.4"
+pre-commit = "^3.3"
+pytest = "^7.4"
+pytest-asyncio = "^0.21"
+pytest-cov = "^4.1"
+pytest-mock = "^3.11"
+pytest-randomly = "^3.12"
+pytest-sugar = "^0.9"
+pyupgrade = "^3.9"
+
+[tool.poetry-dynamic-versioning]
+enable = false
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `whois-parser-0.1.4/whois_parser/dataclasses.py` & `whois_parser-0.2.0/whois_parser/dataclasses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,52 @@
 from dataclasses import dataclass, field
 from datetime import datetime
-from typing import List, Optional, Union
+from typing import Optional, Union
 
-from dataclasses_json import dataclass_json
 
-
-@dataclass_json
 @dataclass
 class Contact:
     organization: Optional[str] = None
     email: Optional[str] = None
     name: Optional[str] = None
     telephone: Optional[str] = None
 
 
-@dataclass_json
 @dataclass
 class Tech(Contact):
     pass
 
 
-@dataclass_json
 @dataclass
 class Registrant(Contact):
     pass
 
 
-@dataclass_json
 @dataclass
 class Admin(Contact):
     pass
 
 
-@dataclass_json
 @dataclass
 class Abuse:
     email: Optional[str] = None
     telephone: Optional[str] = None
 
 
-@dataclass_json
 @dataclass
 class WhoisRecord:
     raw_text: str
 
     registrant: Registrant
     admin: Admin
     tech: Tech
     abuse: Abuse
 
-    statuses: List[str] = field(default_factory=list)
-    name_servers: List[str] = field(default_factory=list)
+    statuses: list[str] = field(default_factory=list)
+    name_servers: list[str] = field(default_factory=list)
 
     domain: Optional[str] = None
     registrar: Optional[str] = None
 
     expires_at: Optional[Union[datetime, str]] = None
     registered_at: Optional[Union[datetime, str]] = None
     updated_at: Optional[Union[datetime, str]] = None
```

### Comparing `whois-parser-0.1.4/whois_parser/parser.py` & `whois_parser-0.2.0/whois_parser/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import Dict, Optional, Type
+from typing import Optional
 
 from whois_parser.parsers.be import BeParser
 from whois_parser.parsers.uk import UkParser
 
 from . import dataclasses
 from .parsers import BaseParser, JpParser
 
-PARSERS_MAP: Dict[str, Type[BaseParser]] = {
+PARSERS_MAP: dict[str, type[BaseParser]] = {
     "jp": JpParser,
     "uk": UkParser,
     "be": BeParser,
 }
 
 
-def get_default_parsers_map() -> Dict[str, Type[BaseParser]]:
+def get_default_parsers_map() -> dict[str, type[BaseParser]]:
     return PARSERS_MAP
 
 
 def get_parser(
-    tld: Optional[str], parsers_map: Dict[str, Type[BaseParser]]
-) -> Type[BaseParser]:
+    tld: Optional[str], parsers_map: dict[str, type[BaseParser]]
+) -> type[BaseParser]:
     if tld is None:
         return BaseParser
 
     return parsers_map.get(tld, BaseParser)
 
 
 class WhoisParser:
-    def __init__(self, parsers_map: Dict[str, Type[BaseParser]] = PARSERS_MAP):
+    def __init__(self, parsers_map: dict[str, type[BaseParser]] = PARSERS_MAP):
         self.parsers_map = parsers_map
 
     def parse(
         self, raw_text: str, *, hostname: Optional[str] = None
     ) -> dataclasses.WhoisRecord:
         """Parse a whois record and return it as a data class object
```

### Comparing `whois-parser-0.1.4/whois_parser/parsers/abstract.py` & `whois_parser-0.2.0/whois_parser/parsers/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
-from typing import List, Optional, Type, Union
+from typing import Optional, Union
 
 from pyparsing import ParserElement
 
 from .. import dataclasses
 from .constants import ANY_CHARACTERS, DEILIMITER, SPACE_OR_TAB
 from .utils import build_common_prefix_pattern, find, find_all, parse_datetime
 
@@ -28,15 +28,15 @@
         if line.startswith("#"):
             sharp_index = index + 1
             break
 
     if sharp_index is None:
         return raw_text
 
-    lines: List[str] = []
+    lines: list[str] = []
     for line in reversed_lines[:sharp_index]:
         lines.append(line.strip())
 
     # revert reversed lines
     lines.reverse()
 
     return "\n".join(lines)
@@ -150,35 +150,35 @@
         """Find registrar field
 
         Returns:
             Optional[str]:
         """
 
     @abstractmethod
-    def _find_statuses(self) -> List[str]:
+    def _find_statuses(self) -> list[str]:
         """Find a list of status filed
 
         Returns:
             List[str]: Returns an empty list if found nothing
         """
 
     @abstractmethod
-    def _find_name_servers(self) -> List[str]:
+    def _find_name_servers(self) -> list[str]:
         """Find a list of name server field
 
         Returns:
             List[str]: Returns an empty list if found nothing
         """
 
     def _find(
         self,
-        prefix: Type[ParserElement],
+        prefix: ParserElement,
         *,
-        delimiter: Optional[Type[ParserElement]] = SPACE_OR_TAB,
-        target: Type[ParserElement] = ANY_CHARACTERS
+        delimiter: Optional[ParserElement] = SPACE_OR_TAB,
+        target: ParserElement = ANY_CHARACTERS
     ) -> Optional[str]:
         """Find text which matches with PyParsing expression
 
         Args:
             prefix (Type[ParserElement]): [description]
             delimiter (Optional[Type[ParserElement]], optional): [description]. Defaults to White().
             target (Type[ParserElement], optional): [description]. Defaults to Regex(".+").
@@ -190,18 +190,18 @@
         if delimiter is not None:
             grammar += delimiter
         grammar += target("value")
         return find(text=self._normalized_raw_text, grammar=grammar)
 
     def _find_datetime(
         self,
-        prefix: Type[ParserElement],
+        prefix: ParserElement,
         *,
-        delimiter: Optional[Type[ParserElement]] = SPACE_OR_TAB,
-        target: Type[ParserElement] = ANY_CHARACTERS
+        delimiter: Optional[ParserElement] = SPACE_OR_TAB,
+        target: ParserElement = ANY_CHARACTERS
     ) -> Optional[Union[str, datetime]]:
         """Find text which matches with PyParsing expression and return it as a datetime
 
         Args:
             prefix (Type[ParserElement]): [description]
             delimiter (Optional[Type[ParserElement]], optional): [description]. Defaults to White().
             target (Type[ParserElement], optional): [description]. Defaults to Regex(".+").
@@ -213,19 +213,19 @@
         if value is None:
             return None
 
         return parse_datetime(value)
 
     def _find_all(
         self,
-        prefix: Type[ParserElement],
+        prefix: ParserElement,
         *,
-        delimiter: Optional[Type[ParserElement]] = SPACE_OR_TAB,
-        target: Type[ParserElement] = ANY_CHARACTERS
-    ) -> List[str]:
+        delimiter: Optional[ParserElement] = SPACE_OR_TAB,
+        target: ParserElement = ANY_CHARACTERS
+    ) -> list[str]:
         """Find a list of text which matches with a PyParsing expression
 
         Args:
             prefix (Type[ParserElement]): [description]
             delimiter (Optional[Type[ParserElement]], optional): [description]. Defaults to White().
             target (Type[ParserElement], optional): [description]. Defaults to Regex(".+").
 
@@ -236,15 +236,15 @@
         if delimiter is not None:
             grammar += delimiter
         grammar += target("value")
         return find_all(text=self._normalized_raw_text, grammar=grammar)
 
     def _find_by_keywords(
         self,
-        keywords: List[str],
+        keywords: list[str],
         *,
         delimiter: Optional[str] = DEILIMITER,
         is_case_sensitive: bool = False,
         is_line_start_sensitive: bool = True
     ) -> Optional[str]:
         """Find text which matches with a keyword
 
@@ -269,15 +269,15 @@
             if value is not None:
                 return value
 
         return None
 
     def _find_datetime_by_keywords(
         self,
-        keywords: List[str],
+        keywords: list[str],
         *,
         delimiter: Optional[str] = DEILIMITER,
         is_case_sensitive: bool = False,
         is_line_start_sensitive: bool = True
     ) -> Optional[Union[datetime, str]]:
         """Find text which matches with a keyword and return it as a datetime
 
@@ -302,20 +302,20 @@
             if value is not None:
                 return value
 
         return None
 
     def _find_all_by_keywords(
         self,
-        keywords: List[str],
+        keywords: list[str],
         *,
         delimiter: Optional[str] = DEILIMITER,
         is_case_sensitive: bool = False,
         is_line_start_sensitive: bool = True
-    ) -> List[str]:
+    ) -> list[str]:
         """Find a list of text which matches with a keyword
 
         Args:
             keywords (List[str]): [description] A list of keyword for prefix. A keyword is converted to a PyPyarsing expression.
             delimiter (Optional[str], optional): Defaults to ":".
             is_case_sensitive (bool, optional): Defaults to False.
             is_line_start_sensitive (bool, optional): Defaults to True.
```

### Comparing `whois-parser-0.1.4/whois_parser/parsers/base.py` & `whois_parser-0.2.0/whois_parser/parsers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from .. import dataclasses
 from .abstract import AbstractParser
 
 
 class BaseParser(AbstractParser):
     def _find_domain(self) -> Optional[str]:
@@ -194,13 +194,13 @@
         return dataclasses.Tech(
             name=self._find_tech_name(),
             email=self._find_tech_email(),
             telephone=self._find_tech_telephone(),
             organization=self._find_tech_organization(),
         )
 
-    def _find_statuses(self) -> List[str]:
+    def _find_statuses(self) -> list[str]:
         return self._find_all_by_keywords(["Domain Status", "domaintype"])
 
-    def _find_name_servers(self) -> List[str]:
+    def _find_name_servers(self) -> list[str]:
         values = self._find_all_by_keywords(["Name server", "Nserver", "Host Name"])
         return [value.lower() for value in values]
```

### Comparing `whois-parser-0.1.4/whois_parser/parsers/jp.py` & `whois_parser-0.2.0/whois_parser/parsers/jp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from .base import BaseParser
 from .utils import build_common_prefix_pattern
 
 
 class JpParser(BaseParser):
     def _find_domain(self) -> Optional[str]:
@@ -38,22 +38,22 @@
         prefix = build_common_prefix_pattern(
             "[最終更新]",
             is_line_start_sensitive=False,
             delimiter=None,
         )
         return self._find_datetime(prefix, delimiter=None)
 
-    def _find_statuses(self) -> List[str]:
+    def _find_statuses(self) -> list[str]:
         prefix = build_common_prefix_pattern(
             "[状態]",
             is_line_start_sensitive=False,
             delimiter=None,
         )
         return self._find_all(prefix, delimiter=None)
 
-    def _find_name_servers(self) -> List[str]:
+    def _find_name_servers(self) -> list[str]:
         prefix = build_common_prefix_pattern(
             "[ネームサーバ]",
             is_line_start_sensitive=False,
             delimiter=None,
         )
         return self._find_all(prefix, delimiter=None)
```

### Comparing `whois-parser-0.1.4/PKG-INFO` & `whois_parser-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: whois-parser
-Version: 0.1.4
+Version: 0.2.0
 Summary: Yet another whois parser for Python
 Home-page: https://github.com/ninoseki/whois-parser
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: dataclasses-json (>=0.5.5,<0.6.0)
-Requires-Dist: dateparser (>=1.1.0,<2.0.0)
-Requires-Dist: importlib-metadata (>=4.8.2,<5.0.0); python_version < "3.8"
-Requires-Dist: pyparsing (>=3.0.7,<4.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dateparser (>=1.1,<2.0)
+Requires-Dist: pyparsing (>=3.0,<4.0)
 Project-URL: Repository, https://github.com/ninoseki/whois-parser
 Description-Content-Type: text/markdown
 
 # whois-parser
 
 [![PyPI version](https://badge.fury.io/py/whois-parser.svg)](https://badge.fury.io/py/whois-parser)
 [![Python CI](https://github.com/ninoseki/whois-parser/actions/workflows/test.yml/badge.svg)](https://github.com/ninoseki/whois-parser/actions/workflows/test.yml)
```

