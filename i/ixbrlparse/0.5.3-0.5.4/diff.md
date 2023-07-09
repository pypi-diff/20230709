# Comparing `tmp/ixbrlparse-0.5.3.tar.gz` & `tmp/ixbrlparse-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrlparse-0.5.3.tar", last modified: Tue Dec 20 20:23:34 2022, max compression
+gzip compressed data, was "ixbrlparse-0.5.4.tar", last modified: Sun Jul  9 08:52:22 2023, max compression
```

## Comparing `ixbrlparse-0.5.3.tar` & `ixbrlparse-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 20:23:34.371766 ixbrlparse-0.5.3/
--rw-rw-rw-   0        0        0     1088 2020-02-25 22:10:31.000000 ixbrlparse-0.5.3/LICENSE
--rw-rw-rw-   0        0        0     7329 2022-12-20 20:23:34.369772 ixbrlparse-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     6552 2022-12-20 20:14:15.000000 ixbrlparse-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2022-12-20 20:23:34.330769 ixbrlparse-0.5.3/ixbrlparse/
--rw-rw-rw-   0        0        0       97 2022-11-16 21:23:50.000000 ixbrlparse-0.5.3/ixbrlparse/__init__.py
--rw-rw-rw-   0        0        0     1907 2022-11-16 21:16:55.000000 ixbrlparse-0.5.3/ixbrlparse/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 20:23:34.366767 ixbrlparse-0.5.3/ixbrlparse/components/
--rw-rw-rw-   0        0        0      176 2022-12-20 14:20:48.000000 ixbrlparse-0.5.3/ixbrlparse/components/__init__.py
--rw-rw-rw-   0        0        0     1644 2022-12-20 14:20:48.000000 ixbrlparse-0.5.3/ixbrlparse/components/context.py
--rw-rw-rw-   0        0        0      910 2022-12-20 14:20:48.000000 ixbrlparse-0.5.3/ixbrlparse/components/nonnumeric.py
--rw-rw-rw-   0        0        0     2261 2022-12-20 14:20:48.000000 ixbrlparse-0.5.3/ixbrlparse/components/numeric.py
--rw-rw-rw-   0        0        0     4066 2022-11-16 23:59:06.000000 ixbrlparse-0.5.3/ixbrlparse/components/transform.py
--rw-rw-rw-   0        0        0    13938 2022-12-20 20:07:23.000000 ixbrlparse-0.5.3/ixbrlparse/core.py
--rw-rw-rw-   0        0        0        0 2022-11-16 21:16:55.000000 ixbrlparse-0.5.3/ixbrlparse/utils.py
--rw-rw-rw-   0        0        0       23 2022-12-20 20:09:41.000000 ixbrlparse-0.5.3/ixbrlparse/version.py
-drwxrwxrwx   0        0        0        0 2022-12-20 20:23:34.355768 ixbrlparse-0.5.3/ixbrlparse.egg-info/
--rw-rw-rw-   0        0        0     7329 2022-12-20 20:23:34.000000 ixbrlparse-0.5.3/ixbrlparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2022-12-20 20:23:34.000000 ixbrlparse-0.5.3/ixbrlparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 20:23:34.000000 ixbrlparse-0.5.3/ixbrlparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-12-20 20:23:34.000000 ixbrlparse-0.5.3/ixbrlparse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-12-20 20:23:34.000000 ixbrlparse-0.5.3/ixbrlparse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-20 20:23:34.371766 ixbrlparse-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1149 2022-11-16 23:59:06.000000 ixbrlparse-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:52:22.006368 ixbrlparse-0.5.4/
+-rw-rw-rw-   0        0        0     1088 2020-02-25 22:10:31.000000 ixbrlparse-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0     7433 2023-07-09 08:52:22.004371 ixbrlparse-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6656 2023-07-09 08:45:00.000000 ixbrlparse-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 08:52:21.955374 ixbrlparse-0.5.4/ixbrlparse/
+-rw-rw-rw-   0        0        0       97 2022-11-16 21:23:50.000000 ixbrlparse-0.5.4/ixbrlparse/__init__.py
+-rw-rw-rw-   0        0        0     1907 2022-11-16 21:16:55.000000 ixbrlparse-0.5.4/ixbrlparse/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:52:21.994372 ixbrlparse-0.5.4/ixbrlparse/components/
+-rw-rw-rw-   0        0        0      176 2022-12-20 14:20:48.000000 ixbrlparse-0.5.4/ixbrlparse/components/__init__.py
+-rw-rw-rw-   0        0        0     1644 2022-12-20 14:20:48.000000 ixbrlparse-0.5.4/ixbrlparse/components/context.py
+-rw-rw-rw-   0        0        0     1052 2023-07-09 08:39:20.000000 ixbrlparse-0.5.4/ixbrlparse/components/nonnumeric.py
+-rw-rw-rw-   0        0        0     2403 2023-07-09 08:47:05.000000 ixbrlparse-0.5.4/ixbrlparse/components/numeric.py
+-rw-rw-rw-   0        0        0     4066 2022-11-16 23:59:06.000000 ixbrlparse-0.5.4/ixbrlparse/components/transform.py
+-rw-rw-rw-   0        0        0    14082 2023-07-09 08:39:20.000000 ixbrlparse-0.5.4/ixbrlparse/core.py
+-rw-rw-rw-   0        0        0        0 2022-11-16 21:16:55.000000 ixbrlparse-0.5.4/ixbrlparse/utils.py
+-rw-rw-rw-   0        0        0       23 2023-07-09 08:44:24.000000 ixbrlparse-0.5.4/ixbrlparse/version.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:52:21.980367 ixbrlparse-0.5.4/ixbrlparse.egg-info/
+-rw-rw-rw-   0        0        0     7433 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 08:52:21.000000 ixbrlparse-0.5.4/ixbrlparse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 08:52:22.006368 ixbrlparse-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2022-11-16 23:59:06.000000 ixbrlparse-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:52:22.000368 ixbrlparse-0.5.4/tests/
+-rw-rw-rw-   0        0        0     9070 2022-12-20 20:32:07.000000 ixbrlparse-0.5.4/tests/test_classes.py
+-rw-rw-rw-   0        0        0    14270 2023-07-09 08:42:01.000000 ixbrlparse-0.5.4/tests/test_parse.py
```

### Comparing `ixbrlparse-0.5.3/LICENSE` & `ixbrlparse-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ixbrlparse-0.5.3/PKG-INFO` & `ixbrlparse-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrlparse
-Version: 0.5.3
+Version: 0.5.4
 Summary: A python module for getting useful data out of ixbrl files.
 Home-page: https://github.com/drkane/ixbrl-parse
 Author: David Kane
 Author-email: david@dkane.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,14 +24,16 @@
 ![Test status](https://github.com/drkane/ixbrl-parse/workflows/tests/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ixbrlparse)](https://pypi.org/project/ixbrlparse/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ixbrlparse)
 ![PyPI - License](https://img.shields.io/pypi/l/ixbrlparse)
 
 A python module for getting useful data out of ixbrl files. The library is at an early stage - feedback and improvements are very welcome.
 
+**New in version 0.5.4**: Added backreferences to BeautifulSoup objects - thanks to @avyfain for PR.
+
 **New in version 0.5.3**: Support for `exclude` and `continuation` elements within XBRL documents. Thanks to @wcollinscw for adding support for exclude elements.
 
 **New in version 0.5**: Support for Python 3.11 has been added. I've had some problems with Python 3.11 and Windows as lxml binaries aren't yet available. Also new in version 0.5 is type checking - the whole library now has types added. 
 
 **New in version 0.4**: I've added initial support for pure XBRL files as well as tagged HTML iXBRL files. Feedback on this feature is welcome - particularly around getting values out of numeric items.
 
 ## Requirements
```

### Comparing `ixbrlparse-0.5.3/README.md` & `ixbrlparse-0.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ![Test status](https://github.com/drkane/ixbrl-parse/workflows/tests/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ixbrlparse)](https://pypi.org/project/ixbrlparse/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ixbrlparse)
 ![PyPI - License](https://img.shields.io/pypi/l/ixbrlparse)
 
 A python module for getting useful data out of ixbrl files. The library is at an early stage - feedback and improvements are very welcome.
 
+**New in version 0.5.4**: Added backreferences to BeautifulSoup objects - thanks to @avyfain for PR.
+
 **New in version 0.5.3**: Support for `exclude` and `continuation` elements within XBRL documents. Thanks to @wcollinscw for adding support for exclude elements.
 
 **New in version 0.5**: Support for Python 3.11 has been added. I've had some problems with Python 3.11 and Windows as lxml binaries aren't yet available. Also new in version 0.5 is type checking - the whole library now has types added. 
 
 **New in version 0.4**: I've added initial support for pure XBRL files as well as tagged HTML iXBRL files. Feedback on this feature is welcome - particularly around getting values out of numeric items.
 
 ## Requirements
```

### Comparing `ixbrlparse-0.5.3/ixbrlparse/__main__.py` & `ixbrlparse-0.5.4/ixbrlparse/__main__.py`

 * *Files identical despite different names*

### Comparing `ixbrlparse-0.5.3/ixbrlparse/components/context.py` & `ixbrlparse-0.5.4/ixbrlparse/components/context.py`

 * *Files identical despite different names*

### Comparing `ixbrlparse-0.5.3/ixbrlparse/components/nonnumeric.py` & `ixbrlparse-0.5.4/ixbrlparse/components/nonnumeric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Union
 
+from bs4 import Tag
+
 from ixbrlparse.components import ixbrlContext
 
 
 class ixbrlNonNumeric:
     def __init__(
         self,
         context: Union[ixbrlContext, str, None],
         name: str,
         format_: Optional[str],
         value: str,
+        soup_tag: Optional[Tag] = None,
     ) -> None:
-
         name_split: List[str] = name.split(":", maxsplit=1)
         if len(name_split) == 2:
             self.schema = name_split[0]
             self.name = name_split[1]
         else:
             self.schema = "unknown"
             self.name = name_split[0]
 
         self.context = context
         self.format = format_
         self.value = value
+        self.soup_tag = soup_tag
 
     def to_json(self) -> Dict[str, Any]:
-        values = deepcopy(self.__dict__)
+        values = {k: deepcopy(v) for k, v in self.__dict__.items() if k != "soup_tag"}
         if isinstance(self.context, ixbrlContext):
             values["context"] = self.context.to_json()
         return values
```

### Comparing `ixbrlparse-0.5.3/ixbrlparse/components/numeric.py` & `ixbrlparse-0.5.4/ixbrlparse/components/numeric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from copy import deepcopy
 from typing import Dict, Optional, Union
 
+from bs4 import Tag
+
 from .context import ixbrlContext
 from .transform import get_format, ixbrlFormat
 
 
 class ixbrlNumeric:
-
     # contextref
     # decimals
     # format
     # name
     # scale
     # sign
     # text
@@ -19,14 +20,15 @@
     def __init__(
         self,
         name: Optional[str] = None,
         unit: Optional[str] = None,
         value: Optional[Union[str, int, float]] = None,
         text: Optional[Union[str, int, float]] = None,
         context: Union[ixbrlContext, str, None] = None,
+        soup_tag: Optional[Tag] = None,
         **attrs,
     ) -> None:
         self.name: Optional[str] = name
         self.schema: str = "unknown"
         if isinstance(name, str):
             name_value = name.split(":", maxsplit=1)
             if len(name_value) == 2:
@@ -40,14 +42,15 @@
             value = text
         if not isinstance(value, (str, int, float)):
             raise ValueError("Must provide either value or text")
         self.text: Union[str, int, float] = value
         self.context: Union[ixbrlContext, str, None] = context
         self.unit: Optional[str] = unit
         self.value: Optional[Union[int, float]] = None
+        self.soup_tag = soup_tag
 
         format_ = {
             "format_": attrs.get("format"),
             "decimals": attrs.get("decimals", "0"),
             "scale": attrs.get("scale", 0),
             "sign": attrs.get("sign", ""),
         }
@@ -57,13 +60,13 @@
             if isinstance(self.format, ixbrlFormat):
                 self.value = self.format.parse_value(self.text)
         except ValueError:
             print(attrs)
             raise
 
     def to_json(self) -> Dict:
-        values = deepcopy(self.__dict__)
+        values = {k: deepcopy(v) for k, v in self.__dict__.items() if k != "soup_tag"}
         if isinstance(self.format, ixbrlFormat):
             values["format"] = self.format.to_json()
         if isinstance(self.context, ixbrlContext):
             values["context"] = self.context.to_json()
         return values
```

### Comparing `ixbrlparse-0.5.3/ixbrlparse/components/transform.py` & `ixbrlparse-0.5.4/ixbrlparse/components/transform.py`

 * *Files identical despite different names*

### Comparing `ixbrlparse-0.5.3/ixbrlparse/core.py` & `ixbrlparse-0.5.4/ixbrlparse/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,15 @@
                     ixbrlNonNumeric(
                         context=context,
                         name=s["name"] if isinstance(s["name"], str) else "",
                         format_=format_,
                         value=text.strip().replace("\n", "")
                         if isinstance(text, str)
                         else "",
+                        soup_tag=s,
                     )
                 )
             except Exception as e:
                 self.errors.append(
                     {
                         "error": e,
                         "element": s,
@@ -194,14 +195,15 @@
         for s in self.soup.find_all({"nonFraction"}):
             try:
                 self.numeric.append(
                     ixbrlNumeric(
                         text=s.text,
                         context=self.contexts.get(s["contextRef"], s["contextRef"]),
                         unit=self.units.get(s["unitRef"], s["unitRef"]),
+                        soup_tag=s,
                         **s.attrs
                     )
                 )
             except Exception as e:
                 self.errors.append(
                     {
                         "error": e,
@@ -244,14 +246,15 @@
             try:
                 self.numeric.append(
                     ixbrlNumeric(
                         name=s.name,
                         text=s.text,
                         context=self.contexts.get(context_ref, context_ref),
                         unit=self.units.get(unit_ref, unit_ref),
+                        soup_tag=s,
                         **s.attrs
                     )
                 )
             except Exception as e:
                 self.errors.append(
                     {
                         "error": e,
@@ -285,14 +288,15 @@
                 ixbrlNonNumeric(
                     context=context,
                     name=s.name if isinstance(s.name, str) else "",
                     format_=format_,
                     value=text.strip().replace("\n", "")
                     if isinstance(text, str)
                     else "",
+                    soup_tag=s,
                 )
             )
 
 
 class IXBRL:
     def __init__(self, f: IO, raise_on_error: bool = True) -> None:
         self.soup = BeautifulSoup(f.read(), "xml", multi_valued_attributes=None)
```

### Comparing `ixbrlparse-0.5.3/ixbrlparse.egg-info/PKG-INFO` & `ixbrlparse-0.5.4/ixbrlparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixbrlparse
-Version: 0.5.3
+Version: 0.5.4
 Summary: A python module for getting useful data out of ixbrl files.
 Home-page: https://github.com/drkane/ixbrl-parse
 Author: David Kane
 Author-email: david@dkane.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,14 +24,16 @@
 ![Test status](https://github.com/drkane/ixbrl-parse/workflows/tests/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ixbrlparse)](https://pypi.org/project/ixbrlparse/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ixbrlparse)
 ![PyPI - License](https://img.shields.io/pypi/l/ixbrlparse)
 
 A python module for getting useful data out of ixbrl files. The library is at an early stage - feedback and improvements are very welcome.
 
+**New in version 0.5.4**: Added backreferences to BeautifulSoup objects - thanks to @avyfain for PR.
+
 **New in version 0.5.3**: Support for `exclude` and `continuation` elements within XBRL documents. Thanks to @wcollinscw for adding support for exclude elements.
 
 **New in version 0.5**: Support for Python 3.11 has been added. I've had some problems with Python 3.11 and Windows as lxml binaries aren't yet available. Also new in version 0.5 is type checking - the whole library now has types added. 
 
 **New in version 0.4**: I've added initial support for pure XBRL files as well as tagged HTML iXBRL files. Feedback on this feature is welcome - particularly around getting values out of numeric items.
 
 ## Requirements
```

### Comparing `ixbrlparse-0.5.3/setup.py` & `ixbrlparse-0.5.4/setup.py`

 * *Files identical despite different names*

