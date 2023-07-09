# Comparing `tmp/avro.py-2023.6.30.tar.gz` & `tmp/avro.py-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro.py-2023.6.30.tar", last modified: Thu Jun 29 18:13:23 2023, max compression
+gzip compressed data, was "avro.py-2023.7.9.tar", last modified: Sun Jul  9 09:54:22 2023, max compression
```

## Comparing `avro.py-2023.6.30.tar` & `avro.py-2023.7.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:13:23.240200 avro.py-2023.6.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 18:13:13.000000 avro.py-2023.6.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 18:13:13.000000 avro.py-2023.6.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-29 18:13:23.240200 avro.py-2023.6.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-29 18:13:13.000000 avro.py-2023.6.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:13:23.240200 avro.py-2023.6.30/avro/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      583 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10649 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:13:23.240200 avro.py-2023.6.30/avro/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32079 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/resources/avrodict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:13:23.240200 avro.py-2023.6.30/avro/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/utils/count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-06-29 18:13:13.000000 avro.py-2023.6.30/avro/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:13:23.240200 avro.py-2023.6.30/avro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-29 18:13:23.000000 avro.py-2023.6.30/avro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 18:13:23.000000 avro.py-2023.6.30/avro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:13:23.000000 avro.py-2023.6.30/avro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 18:13:23.000000 avro.py-2023.6.30/avro.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-29 18:13:13.000000 avro.py-2023.6.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:13:23.240200 avro.py-2023.6.30/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-06-29 18:13:13.000000 avro.py-2023.6.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:13:23.240200 avro.py-2023.6.30/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4658 2023-06-29 18:13:13.000000 avro.py-2023.6.30/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-06-29 18:13:13.000000 avro.py-2023.6.30/tests/test_utils_count.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2653 2023-06-29 18:13:13.000000 avro.py-2023.6.30/tests/test_utils_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:22.160102 avro.py-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-09 09:54:10.000000 avro.py-2023.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-09 09:54:10.000000 avro.py-2023.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-09 09:54:22.160102 avro.py-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-09 09:54:10.000000 avro.py-2023.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:22.160102 avro.py-2023.7.9/avro/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      583 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10618 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:22.160102 avro.py-2023.7.9/avro/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/resources/avrodict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:22.160102 avro.py-2023.7.9/avro/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/utils/count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-07-09 09:54:10.000000 avro.py-2023.7.9/avro/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:22.160102 avro.py-2023.7.9/avro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-09 09:54:22.000000 avro.py-2023.7.9/avro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-09 09:54:22.000000 avro.py-2023.7.9/avro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:54:22.000000 avro.py-2023.7.9/avro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 09:54:22.000000 avro.py-2023.7.9/avro.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-09 09:54:10.000000 avro.py-2023.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:54:22.160102 avro.py-2023.7.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1574 2023-07-09 09:54:10.000000 avro.py-2023.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:54:22.160102 avro.py-2023.7.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4751 2023-07-09 09:54:10.000000 avro.py-2023.7.9/tests/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-09 09:54:10.000000 avro.py-2023.7.9/tests/test_utils_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2660 2023-07-09 09:54:10.000000 avro.py-2023.7.9/tests/test_utils_validate.py
```

### Comparing `avro.py-2023.6.30/LICENSE` & `avro.py-2023.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `avro.py-2023.6.30/PKG-INFO` & `avro.py-2023.7.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.6.30
+Version: 2023.7.9
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,16 @@
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
 <br>
 
 | Checks | Status | 
 |:---|---:|
 | usability | [![Unit Tests](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml) |
-| beauty | [![Style Check](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml) |
+| pretty code | [![Linting](https://github.com/hitblast/avro.py/actions/workflows/linting.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/linting.yml) |
+| style enforcement | [![Formatting](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml) |
 
 <br>
 
 </div>
 
 ## Overview
 
@@ -56,44 +57,41 @@
 <br>
 
 ## Installation
 
 This package requires **Python 3.8 or higher** to be used inside your development environment.
 
 ```bash
-# install / upgrade
-$ pip install avro.py
+# Install / upgrade.
+$ pip install -U avro.py
 ```
 
 <br>
 
 ## Usage Guide
 As of now, you can easily use avro.py by importing the module and calling the primary `parse` function.
 
 ```python
+# Imports.
 import avro
 
-# Unicode
+# Parsing some text.
 parsed_text = avro.parse('ami banglay gan gai.')
 print(parsed_text)
-
-# ASCII
-parsed_ascii = avro.parse('srabon dharay', in_ascii=True)
-print(parsed_ascii)
 ```
 
-Also, you can reverse unicode Bengali to English text as well (new, doesn't contain phonetic rules)!
+Also, you can reverse unicode Bengali to English text as well (new, doesn't contain phonetic rules).
 
 ```python
+# Imports.
 import avro
 
+# Reversing some text.
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 print(reversed_text)
-
-# amar sonar bangla.
 ```
 
 Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally! 
 
 <br>
 
 ## Contributing
```

### Comparing `avro.py-2023.6.30/README.md` & `avro.py-2023.7.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
 <br>
 
 | Checks | Status | 
 |:---|---:|
 | usability | [![Unit Tests](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml) |
-| beauty | [![Style Check](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml) |
+| pretty code | [![Linting](https://github.com/hitblast/avro.py/actions/workflows/linting.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/linting.yml) |
+| style enforcement | [![Formatting](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml) |
 
 <br>
 
 </div>
 
 ## Overview
 
@@ -34,44 +35,41 @@
 <br>
 
 ## Installation
 
 This package requires **Python 3.8 or higher** to be used inside your development environment.
 
 ```bash
-# install / upgrade
-$ pip install avro.py
+# Install / upgrade.
+$ pip install -U avro.py
 ```
 
 <br>
 
 ## Usage Guide
 As of now, you can easily use avro.py by importing the module and calling the primary `parse` function.
 
 ```python
+# Imports.
 import avro
 
-# Unicode
+# Parsing some text.
 parsed_text = avro.parse('ami banglay gan gai.')
 print(parsed_text)
-
-# ASCII
-parsed_ascii = avro.parse('srabon dharay', in_ascii=True)
-print(parsed_ascii)
 ```
 
-Also, you can reverse unicode Bengali to English text as well (new, doesn't contain phonetic rules)!
+Also, you can reverse unicode Bengali to English text as well (new, doesn't contain phonetic rules).
 
 ```python
+# Imports.
 import avro
 
+# Reversing some text.
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 print(reversed_text)
-
-# amar sonar bangla.
 ```
 
 Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally! 
 
 <br>
 
 ## Contributing
```

### Comparing `avro.py-2023.6.30/avro/config.py` & `avro.py-2023.7.9/avro/config.py`

 * *Files identical despite different names*

### Comparing `avro.py-2023.6.30/avro/main.py` & `avro.py-2023.7.9/avro/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 # SPDX-License-Identifier: MIT
 
 
-# Import third-party modules.
+# Import first-party Python libraries.
 import re
+from concurrent.futures import ThreadPoolExecutor
 from functools import lru_cache
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 # Import local modules.
 from . import config
 from .utils import validate
 
 # Constants.
-PATTERNS: Any = config.AVRO_DICT['data']['patterns']
-NON_RULE_PATTERNS: list = [p for p in PATTERNS if 'rules' not in p]
-RULE_PATTERNS: list = [p for p in PATTERNS if 'rules' in p]
+PATTERNS = config.AVRO_DICT['data']['patterns']
+NON_RULE_PATTERNS = [p for p in PATTERNS if 'rules' not in p]
+RULE_PATTERNS = [p for p in PATTERNS if 'rules' in p]
+
+
+# The helper function for handling multithreaded workloads.
+def _concurrency_helper(func: Callable, params: Tuple[str]) -> List[str]:
+    output = []
+
+    with ThreadPoolExecutor() as executor:
+        futures = [executor.submit(func, text) for text in params]
+
+        for future in futures:
+            output.append(future.result())
+
+    return output
 
 
 # The primary parse function for the library.
-@lru_cache
-def parse(*texts: str, in_ascii: bool = False) -> Union[str, List[str]]:
+def parse(*texts: str) -> Union[str, List[str]]:
     '''
-    ### Parses input text, matches and replaces using avrodict.
+    #### Parses input text, matches and replaces using the Avro Dictionary.
 
     If a valid replacement is found, then it returns the replaced string.
     If no replacement is found, then it instead returns the input text.
 
     Parameters:
-    - `*texts (str)`: The text to parse.
-    - `in_ascii (bool = False)`: Whether to output in ASCII or not (Unicode).
+    - `*texts: str | Tuple[str]`: The text(s) to parse.
 
     Usage:
     ```python
     import avro
 
-    # Unicode
     parsed = avro.parse('ami banglay gan gai')
     print(parsed)
-
-    # ASCII
-    parsed_ascii = avro.parse('ami banglay gan gai', in_ascii=True)
-    print(parsed_ascii)
     ```
     '''
 
-    def subparse(text: str) -> str:
-        # Sanitize text case to meet phonetic comparison standards.
-        fixed_text = validate.fix_string_case(text)
-
-        # Prepare output list.
-        output = []
-
-        # Cursor end point.
-        cur_end = 0
+    # Internal function for multiple parses.
+    @lru_cache
+    def _parse_backend(text: str) -> str:
+        fixed_text = validate.fix_string_case(
+            text
+        )  # Sanitize text case to meet phonetic comparison standards.
+        output = []  # The output list of strings.
+        cur_end = 0  # Cursor end point.
 
         # Iterate through input text.
         for cur, i in enumerate(fixed_text):
             try:
                 i.encode('utf-8')
             except UnicodeDecodeError:
                 uni_pass = False
@@ -92,47 +98,42 @@
 
                 if not match['matched']:
                     cur_end = cur + 1
                     output.append(i)
 
         return ''.join(output)
 
-    output = []
-    for text in texts:  # Applies to non-keyword arguments.
-        output.append(
-            subparse(text) if not in_ascii else str(subparse(text).encode('ascii', errors='backslashreplace'))
-        )
-
+    # Do the final output.
+    output = _concurrency_helper(_parse_backend, texts)
     return output[0] if len(output) == 1 else output
 
 
-@lru_cache
 def reverse(*texts: str) -> Union[str, List[str]]:
     '''
-    ### Reverses input text to Roman script typed in English.
+    #### Reverses input text to Roman script typed in English.
 
     If a valid replacement is found, then it returns the replaced string.
     If no replacement is found, then it instead returns the input text.
 
     Parameters:
-    - `*texts (str)`: The text to reverse.
+    - `*texts: str | Tuple[str]`: The text(s) to reverse.
 
     Usage:
     ```python
     import avro
 
-    target = avro.reverse('আমার সোনার বাংলা')
-    print(target)
+    reversed = avro.reverse('আমার সোনার বাংলা')
+    print(reversed)
     ```
-    `output: amar sonar bangla`
     '''
 
-    def subparse(text: str) -> str:
-        # Prepare output list.
-        output = []
+    # Internal function for multiple reverses.
+    @lru_cache
+    def _reverse_backend(text: str) -> str:
+        output = []  # The output list of strings.
 
         # Iterate through input text.
         for cur, i in enumerate(text):
             try:
                 i.encode('utf-8')
             except UnicodeDecodeError:
                 uni_pass = False
@@ -154,50 +155,46 @@
                         output.append(match['found'])
 
                 if not match['matched']:
                     output.append(i)
 
         return ''.join(output)
 
-    text_segments = []
-    output = []
-
     # Split using regex to remove noise.
-    regex_pattern = "(\\s|\\.|,|\\?|\\।|\\-|;|')"
-    compiled_regex = re.compile(regex_pattern, re.UNICODE)
+    compiled_regex = re.compile("(\\s|\\.|,|\\?|\\।|\\-|;|')", re.UNICODE)
 
-    for text in texts:  # Applies to non-keyword arguments.
+    # Extension for the _reverse_backend() function.
+    @lru_cache
+    def _reverse_backend_ext(text: str) -> str:
+        text_segments = []
         exceptions = config.EXCEPTIONS.get(text, None)
 
         if not exceptions:
             separated_texts = compiled_regex.split(text)
 
             for separated_text in separated_texts:
-                text_segments.append(subparse(separated_text))
+                text_segments.append(_reverse_backend(separated_text))
 
-            output.append(''.join(text_segments))
-            text_segments = []
+            return ''.join(text_segments)
 
         else:
-            output.append(exceptions)
+            return exceptions
 
+    # Prepare final output.
+    output = _concurrency_helper(_reverse_backend_ext, texts)
     return output[0] if len(output) == 1 else output
 
 
 def match_patterns(
     fixed_text: str, cur: int = 0, rule: bool = False, reversed: bool = False
 ) -> Dict[str, Any]:
     '''
-    ### Matches given text at cursor position with rule / non rule patterns.
+    Matches given text at cursor position with rule / non rule patterns.
 
-    Returns a dictionary of three elements:
-
-    - `matched` - Bool: depending on if match found.
-    - `found` - string/None: Value of matched pattern's 'find' key or none.
-    - `replaced` - string: Replaced string if match found else input string at cursor.
+    Returns a dictionary of three (upto four) elements.
     '''
 
     rule_type = NON_RULE_PATTERNS if not rule else RULE_PATTERNS
     pattern = exact_find_in_pattern(fixed_text, reversed, cur, rule_type)
 
     if len(pattern) > 0:
         if not rule:
@@ -211,25 +208,27 @@
             return {
                 "matched": True,
                 "found": pattern[0]['find'],
                 "replaced": pattern[0]['replace'],
                 "rules": pattern[0]['rules'],
             }
     else:
-        if not rule:
-            return {"matched": False, "found": None, "replaced": fixed_text[cur]}
-        else:
-            return {"matched": False, "found": None, "replaced": fixed_text[cur], "rules": None}
+        result = {"matched": False, "found": None, "replaced": fixed_text[cur]}
+
+        if rule:
+            result['rules'] = None
+
+        return result
 
 
 def exact_find_in_pattern(
     fixed_text: str, reversed: bool, cur: int = 0, patterns: Any = PATTERNS
 ) -> List[Dict[str, Any]]:
     '''
-    ### Returns pattern items that match given text, cursor position and pattern.
+    Returns pattern items that match given text, cursor position and pattern.
     '''
 
     if reversed:
         return [
             x
             for x in patterns
             if (cur + len(x['replace']) <= len(fixed_text))
@@ -244,15 +243,15 @@
         and x['find'] == fixed_text[cur : (cur + len(x['find']))]
     ]
 
 
 @lru_cache
 def reverse_with_rules(cursor: int, fixed_text: str, text_reversed: str) -> str:
     '''
-    ### Enhances the word with rules for reverse-parsing.
+    Enhances the word with rules for reverse-parsing.
     '''
 
     added_suffix = ''
 
     if not (
         fixed_text[cursor] in config.AVRO_KAR
         or fixed_text[cursor] in config.AVRO_SHORBORNO
@@ -271,15 +270,15 @@
         pass
 
     return text_reversed if not text_reversed else text_reversed + added_suffix
 
 
 def process_rules(rules: Dict[str, Any], fixed_text: str, cur: int = 0, cur_end: int = 1) -> Optional[str]:
     '''
-    ### Process rules matched in pattern and returns suitable replacement.
+    Process rules matched in pattern and returns suitable replacement.
 
     If any rule's condition is satisfied, output the rules "replace",
     else output None.
     '''
 
     replaced = ''
 
@@ -298,15 +297,15 @@
             break
 
     return replaced if matched else None
 
 
 def process_match(match: Any, fixed_text: str, cur: int, cur_end: int) -> bool:
     '''
-    ### Processes a single match in rules.
+    Processes a single match in rules.
     '''
 
     # Initial/default value for replace.
     replace = True
 
     # Set check cursor depending on match['type']
     chk = cur - 1 if match['type'] == 'prefix' else cur_end
```

### Comparing `avro.py-2023.6.30/avro/resources/avrodict.py` & `avro.py-2023.7.9/avro/resources/avrodict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: MIT
 
 
-# Imports.
+# Import first-party Python modules.
 from typing import Dict
 
-# The dictionary variable.
+# The Avro Dictionary, implemented in Python.
 AVRO_DICT: Dict[str, str] = {
     "meta": {
         "file_name": "avrodict.py",
         "file_description": "Provides Avro Dictionary in native Python.",
         "package": "avro.py",
         "license": "MIT License",
         "source": "https://github.com/hitblast/avro.py/blob/main/avro/resources/avrodict.py",
```

### Comparing `avro.py-2023.6.30/avro/utils/count.py` & `avro.py-2023.7.9/avro/utils/count.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 # Functions.
 def count_vowels(text) -> int:
     '''
     ### Count number of occurrences of vowels in a given string.
     '''
 
     count = 0
+
     for i in text:
         if i.lower() in config.AVRO_VOWELS:
             count += 1
+
     return count
 
 
 def count_consonants(text) -> int:
     '''
     ### Count number of occurrences of consonants in a given string.
     '''
 
     count = 0
+
     for i in text:
         if i.lower() in config.AVRO_CONSONANTS:
             count += 1
+
     return count
```

### Comparing `avro.py-2023.6.30/avro/utils/validate.py` & `avro.py-2023.7.9/avro/utils/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,13 +61,15 @@
     Case-sensitive characters as defined in config.AVRO_CASESENSITIVES
     retain their case, but others are converted to their lowercase
     equivalents. The result is a string with phonetic-compatible case
     which will the parser will understand without confusion.
     '''
 
     fixed = []
+
     for i in text:
         if is_case_sensitive(i):
             fixed.append(i)
         else:
             fixed.append(i.lower())
+
     return ''.join(fixed)
```

### Comparing `avro.py-2023.6.30/avro.py.egg-info/PKG-INFO` & `avro.py-2023.7.9/avro.py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2023.6.30
+Version: 2023.7.9
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,avro,avro phonetic,bangla,bangla phonetics,bengali,bengali phonetics
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,16 @@
 ![License](https://img.shields.io/pypi/l/avro.py.svg?color=black&label=License)
 
 <br>
 
 | Checks | Status | 
 |:---|---:|
 | usability | [![Unit Tests](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml/badge.svg?branch=main)](https://github.com/hitblast/avro.py/actions/workflows/unit-tests.yml) |
-| beauty | [![Style Check](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/stylecheck.yml) |
+| pretty code | [![Linting](https://github.com/hitblast/avro.py/actions/workflows/linting.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/linting.yml) |
+| style enforcement | [![Formatting](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml/badge.svg)](https://github.com/hitblast/avro.py/actions/workflows/formatting.yml) |
 
 <br>
 
 </div>
 
 ## Overview
 
@@ -56,44 +57,41 @@
 <br>
 
 ## Installation
 
 This package requires **Python 3.8 or higher** to be used inside your development environment.
 
 ```bash
-# install / upgrade
-$ pip install avro.py
+# Install / upgrade.
+$ pip install -U avro.py
 ```
 
 <br>
 
 ## Usage Guide
 As of now, you can easily use avro.py by importing the module and calling the primary `parse` function.
 
 ```python
+# Imports.
 import avro
 
-# Unicode
+# Parsing some text.
 parsed_text = avro.parse('ami banglay gan gai.')
 print(parsed_text)
-
-# ASCII
-parsed_ascii = avro.parse('srabon dharay', in_ascii=True)
-print(parsed_ascii)
 ```
 
-Also, you can reverse unicode Bengali to English text as well (new, doesn't contain phonetic rules)!
+Also, you can reverse unicode Bengali to English text as well (new, doesn't contain phonetic rules).
 
 ```python
+# Imports.
 import avro
 
+# Reversing some text.
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 print(reversed_text)
-
-# amar sonar bangla.
 ```
 
 Other use cases include [your terminal](https://github.com/hitblast/avro.py-cli), literally! 
 
 <br>
 
 ## Contributing
```

### Comparing `avro.py-2023.6.30/setup.py` & `avro.py-2023.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `avro.py-2023.6.30/tests/test_main.py` & `avro.py-2023.7.9/tests/test_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: MIT
 
 
-# Import third-party modules.
+# Import first-party Python modules.
 import os
 import sys
 
 # Add support layer for accessing the primary package.
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), os.path.pardir)))
 
 # Import local modules.
@@ -123,44 +123,37 @@
 def test_words_with_punctuations() -> None:
     '''
     ### Test parsing of words with punctuations.
     '''
 
     words_with_punctuations = {
         'আয়রে,': avro.parse('ayre,'),
-        'ভোলা': avro.parse('bhOla'),
-        'খেয়াল': avro.parse('kheyal'),
-        'খোলা': avro.parse('khOla'),
+        'ভোলা;': avro.parse('bhOla;'),
+        '/খেয়াল': avro.parse('/kheyal'),
+        'খোলা|': avro.parse('khOla|'),
     }
 
     for key, value in words_with_punctuations.items():
         assert key == value
 
 
 def tests_sentences_with_default() -> None:
     '''
     ### Test parsing of sentences (Unicode).
     '''
 
-    assert 'আমি বাংলায় গান গাই' == avro.parse('ami banglay gan gai')
-
-
-def test_sentences_with_ascii_flag() -> None:
-    '''
-    ### Test parsing of sentences (ASCII).
-    '''
-
-    assert str(
-        b'\\u0986\\u09ae\\u09bf \\u09ac\\u09be\\u0982\\u09b2\\u09be\\u09df'
-        + b' \\u0997\\u09be\\u09a8 \\u0997\\u09be\\u0987'
-    ) == avro.parse('ami banglay gan gai', in_ascii=True)
+    assert 'আমি বাংলায় গান গাই;' == avro.parse('ami banglay gan gai;')
+    assert ['আমি বাংলার গান গাই।', 'আমি আমার আমিকে চিরদিন এই বাংলায় খুঁজে পাই।'] == avro.parse(
+        'ami banglar gan gai.', 'ami amar amike cirodin ei banglay khu^je pai.'
+    )
 
 
 def test_reverse_func() -> None:
     '''
     ### Test reverse-parsing with sentences.
     '''
 
-    assert 'ami banglay gan gai' == avro.reverse('আমি বাংলায় গান গাই')
-    assert 'rahim, tomake korim dakche. ekhon ki rowna debe?' == avro.reverse(
-        'রাহিম, তোমাকে করিম ডাকছে। এখন কি রওনা দেবে?'
-    )
+    assert 'ami banglay gan gai.' == avro.reverse('আমি বাংলায় গান গাই।')
+    assert [
+        'rohim, tomake korim dakche. ekhon ki rowna debe?',
+        'rowna dile amake bole zew.',
+    ] == avro.reverse('রহিম, তোমাকে করিম ডাকছে। এখন কি রওনা দেবে?', 'রওনা দিলে আমাকে বলে যেও।')
```

### Comparing `avro.py-2023.6.30/tests/test_utils_count.py` & `avro.py-2023.7.9/tests/test_utils_count.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: MIT
 
 
-# Import third-party modules.
+# Import first-party Python modules.
 import os
 import sys
 
 # Add support layer for accessing the primary package.
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), os.path.pardir)))
 
 # Import local modules.
```

### Comparing `avro.py-2023.6.30/tests/test_utils_validate.py` & `avro.py-2023.7.9/tests/test_utils_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: MIT
 
 
-# Import third-party modules.
+# Import first-party Python modules.
 import os
 import sys
 
 # Add support layer for accessing the primary package.
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), os.path.pardir)))
 
 # Import local modules.
```

