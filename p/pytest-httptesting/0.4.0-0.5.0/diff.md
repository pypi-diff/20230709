# Comparing `tmp/pytest_httptesting-0.4.0.tar.gz` & `tmp/pytest_httptesting-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_httptesting-0.4.0.tar", max compression
+gzip compressed data, was "pytest_httptesting-0.5.0.tar", max compression
```

## Comparing `pytest_httptesting-0.4.0.tar` & `pytest_httptesting-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2022-11-13 16:42:42.780000 pytest_httptesting-0.4.0/LICENSE
--rw-r--r--   0        0        0     3419 2023-04-19 19:55:13.180000 pytest_httptesting-0.4.0/README.md
--rw-r--r--   0        0        0      628 2023-06-03 11:58:22.720000 pytest_httptesting-0.4.0/http_testing/__init__.py
--rw-r--r--   0        0        0        0 2022-11-13 15:15:16.890000 pytest_httptesting-0.4.0/http_testing/assertion_elements/__init__.py
--rw-r--r--   0        0        0      567 2022-11-13 15:15:16.890000 pytest_httptesting-0.4.0/http_testing/assertion_elements/assert_element_checker_base.py
--rw-r--r--   0        0        0     1354 2022-11-13 15:15:16.890000 pytest_httptesting-0.4.0/http_testing/assertion_elements/assertion_attribute_base.py
--rw-r--r--   0        0        0     1587 2022-12-08 23:04:34.980000 pytest_httptesting-0.4.0/http_testing/assertion_elements/content_assertion.py
--rw-r--r--   0        0        0     2888 2023-06-03 11:39:49.730000 pytest_httptesting-0.4.0/http_testing/assertion_elements/cookies_assertion.py
--rw-r--r--   0        0        0     1601 2022-12-08 23:04:34.980000 pytest_httptesting-0.4.0/http_testing/assertion_elements/headers_assertion.py
--rw-r--r--   0        0        0      728 2022-11-13 15:15:16.890000 pytest_httptesting-0.4.0/http_testing/assertion_elements/status_code_assertion.py
--rw-r--r--   0        0        0     1316 2022-11-13 15:15:16.890000 pytest_httptesting-0.4.0/http_testing/assertions.py
--rw-r--r--   0        0        0       79 2023-04-19 19:55:13.180000 pytest_httptesting-0.4.0/http_testing/cookie.py
--rw-r--r--   0        0        0      259 2023-04-19 19:55:13.180000 pytest_httptesting-0.4.0/http_testing/http_client_configuration.py
--rw-r--r--   0        0        0     2748 2023-06-03 12:10:16.720000 pytest_httptesting-0.4.0/http_testing/page_checker.py
--rw-r--r--   0        0        0     1217 2023-06-03 11:39:42.590000 pytest_httptesting-0.4.0/http_testing/plugin.py
--rw-r--r--   0        0        0      709 2023-06-03 11:48:20.280000 pytest_httptesting-0.4.0/http_testing/validators.py
--rw-r--r--   0        0        0      705 2023-06-03 12:16:35.190000 pytest_httptesting-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 pytest_httptesting-0.4.0/setup.py
--rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 pytest_httptesting-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-11-13 16:42:42.780000 pytest_httptesting-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4049 2023-06-05 21:03:36.750000 pytest_httptesting-0.5.0/README.md
+-rw-r--r--   0        0        0      628 2023-06-03 11:58:22.720000 pytest_httptesting-0.5.0/http_testing/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/__init__.py
+-rw-r--r--   0        0        0      567 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/assert_element_checker_base.py
+-rw-r--r--   0        0        0     1354 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/assertion_attribute_base.py
+-rw-r--r--   0        0        0     1587 2022-12-08 23:04:34.980000 pytest_httptesting-0.5.0/http_testing/assertion_elements/content_assertion.py
+-rw-r--r--   0        0        0     2888 2023-06-03 11:39:49.730000 pytest_httptesting-0.5.0/http_testing/assertion_elements/cookies_assertion.py
+-rw-r--r--   0        0        0     1601 2022-12-08 23:04:34.980000 pytest_httptesting-0.5.0/http_testing/assertion_elements/headers_assertion.py
+-rw-r--r--   0        0        0      728 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/status_code_assertion.py
+-rw-r--r--   0        0        0     1316 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertions.py
+-rw-r--r--   0        0        0       79 2023-04-19 19:55:13.180000 pytest_httptesting-0.5.0/http_testing/cookie.py
+-rw-r--r--   0        0        0      259 2023-04-19 19:55:13.180000 pytest_httptesting-0.5.0/http_testing/http_client_configuration.py
+-rw-r--r--   0        0        0     2872 2023-07-09 19:31:42.572186 pytest_httptesting-0.5.0/http_testing/page_checker.py
+-rw-r--r--   0        0        0     1217 2023-06-03 11:39:42.590000 pytest_httptesting-0.5.0/http_testing/plugin.py
+-rw-r--r--   0        0        0      709 2023-06-03 11:48:20.280000 pytest_httptesting-0.5.0/http_testing/validators.py
+-rw-r--r--   0        0        0      705 2023-07-09 19:35:09.342186 pytest_httptesting-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 pytest_httptesting-0.5.0/setup.py
+-rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 pytest_httptesting-0.5.0/PKG-INFO
```

### Comparing `pytest_httptesting-0.4.0/LICENSE` & `pytest_httptesting-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/README.md` & `pytest_httptesting-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # HTTP_TESTING
 
+<a href="https://github.com/heqile/http_testing/actions?query=branch%3Amain+event%3Apush+" target="_blank">
+    <img src="https://github.com/heqile/http_testing/workflows/Test/badge.svg?event=push&branch=main" alt="Test">
+</a>
+<a href="https://pypi.org/project/pytest-httptesting" target="_blank">
+    <img src="https://img.shields.io/pypi/v/pytest-httptesting?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/pytest-httptesting" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/pytest-httptesting.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+
 ## Description
 This project aims to help to create e2e tests, by chaining http calls and verifications on target pages.
 
 ## Concept
 This project is built on pytest.
 
 Each .py file in test represents several tests scenario on one target site, we can provide the site's hostname
```

### Comparing `pytest_httptesting-0.4.0/http_testing/__init__.py` & `pytest_httptesting-0.5.0/http_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/assertion_elements/assert_element_checker_base.py` & `pytest_httptesting-0.5.0/http_testing/assertion_elements/assert_element_checker_base.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/assertion_elements/assertion_attribute_base.py` & `pytest_httptesting-0.5.0/http_testing/assertion_elements/assertion_attribute_base.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/assertion_elements/content_assertion.py` & `pytest_httptesting-0.5.0/http_testing/assertion_elements/content_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/assertion_elements/cookies_assertion.py` & `pytest_httptesting-0.5.0/http_testing/assertion_elements/cookies_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/assertion_elements/headers_assertion.py` & `pytest_httptesting-0.5.0/http_testing/assertion_elements/headers_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/assertion_elements/status_code_assertion.py` & `pytest_httptesting-0.5.0/http_testing/assertion_elements/status_code_assertion.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/assertions.py` & `pytest_httptesting-0.5.0/http_testing/assertions.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/page_checker.py` & `pytest_httptesting-0.5.0/http_testing/page_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import json
 from tempfile import NamedTemporaryFile
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 from attrs import define
 from httpx import URL, Client, Response
 
 from .assertions import Assertions, NegativeAssertions
 
 
 @define
 class PageChecker:
-    _base_url: URL
+    _base_url: Union[URL, str]
     _http_client: Client
     _previous_response: Optional[Response] = None
 
     @property
     def previous_response(self) -> Response:
         if self._previous_response is None:
             raise RuntimeError("previous_response should be called following a http request")
         return self._previous_response
 
     def __call__(
         self,
         *,
         path: str,
         title: Optional[str] = None,
-        base_url: Optional[URL] = None,
+        base_url: Union[URL, str, None] = None,
         method: str = "GET",
         data: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         cookies: Optional[Dict[str, str]] = None,
         follow_redirects: bool = False,
         should_find: Optional[Assertions] = None,
         should_not_find: Optional[NegativeAssertions] = None,
         **kwargs: Any,
     ) -> None:
         """
         Call the target url with given arguments, then verify the response against given rules
         Return None if success, otherwise raise AssertionError
         """
-        base_url = base_url or self._base_url
+        if base_url is None:
+            base_url = self._base_url
+        if isinstance(base_url, str):
+            base_url = URL(base_url)
+
         response = self._http_client.request(
             method=method,
             url=base_url.copy_with(raw_path=path.encode("ascii")),
             data=data,
             headers=headers,
             cookies=cookies,
             follow_redirects=follow_redirects,
```

### Comparing `pytest_httptesting-0.4.0/http_testing/plugin.py` & `pytest_httptesting-0.5.0/http_testing/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/http_testing/validators.py` & `pytest_httptesting-0.5.0/http_testing/validators.py`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.4.0/pyproject.toml` & `pytest_httptesting-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-httptesting"
-version = "0.4.0"
+version = "0.5.0"
 description = "http_testing framework on top of pytest"
 authors = ["HE Qile <mr.qile@gmail.com>"]
 readme = "README.md"
 packages = [{include = "http_testing"}]
 
 homepage = "https://github.com/heqile/http_testing"
 repository = "https://github.com/heqile/http_testing"
```

### Comparing `pytest_httptesting-0.4.0/setup.py` & `pytest_httptesting-0.5.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,258 +18,298 @@
 00000110: 3131 273a 205b 2768 7474 705f 7061 6765  11': ['http_page
 00000120: 5f63 6865 636b 6572 203d 2068 7474 705f  _checker = http_
 00000130: 7465 7374 696e 672e 706c 7567 696e 275d  testing.plugin']
 00000140: 7d0a 0a73 6574 7570 5f6b 7761 7267 7320  }..setup_kwargs 
 00000150: 3d20 7b0a 2020 2020 276e 616d 6527 3a20  = {.    'name': 
 00000160: 2770 7974 6573 742d 6874 7470 7465 7374  'pytest-httptest
 00000170: 696e 6727 2c0a 2020 2020 2776 6572 7369  ing',.    'versi
-00000180: 6f6e 273a 2027 302e 342e 3027 2c0a 2020  on': '0.4.0',.  
+00000180: 6f6e 273a 2027 302e 352e 3027 2c0a 2020  on': '0.5.0',.  
 00000190: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
 000001a0: 2027 6874 7470 5f74 6573 7469 6e67 2066   'http_testing f
 000001b0: 7261 6d65 776f 726b 206f 6e20 746f 7020  ramework on top 
 000001c0: 6f66 2070 7974 6573 7427 2c0a 2020 2020  of pytest',.    
 000001d0: 276c 6f6e 675f 6465 7363 7269 7074 696f  'long_descriptio
 000001e0: 6e27 3a20 2723 2048 5454 505f 5445 5354  n': '# HTTP_TEST
-000001f0: 494e 475c 6e5c 6e23 2320 4465 7363 7269  ING\n\n## Descri
-00000200: 7074 696f 6e5c 6e54 6869 7320 7072 6f6a  ption\nThis proj
-00000210: 6563 7420 6169 6d73 2074 6f20 6865 6c70  ect aims to help
-00000220: 2074 6f20 6372 6561 7465 2065 3265 2074   to create e2e t
-00000230: 6573 7473 2c20 6279 2063 6861 696e 696e  ests, by chainin
-00000240: 6720 6874 7470 2063 616c 6c73 2061 6e64  g http calls and
-00000250: 2076 6572 6966 6963 6174 696f 6e73 206f   verifications o
-00000260: 6e20 7461 7267 6574 2070 6167 6573 2e5c  n target pages.\
-00000270: 6e5c 6e23 2320 436f 6e63 6570 745c 6e54  n\n## Concept\nT
-00000280: 6869 7320 7072 6f6a 6563 7420 6973 2062  his project is b
-00000290: 7569 6c74 206f 6e20 7079 7465 7374 2e5c  uilt on pytest.\
-000002a0: 6e5c 6e45 6163 6820 2e70 7920 6669 6c65  n\nEach .py file
-000002b0: 2069 6e20 7465 7374 2072 6570 7265 7365   in test represe
-000002c0: 6e74 7320 7365 7665 7261 6c20 7465 7374  nts several test
-000002d0: 7320 7363 656e 6172 696f 206f 6e20 6f6e  s scenario on on
-000002e0: 6520 7461 7267 6574 2073 6974 652c 2077  e target site, w
-000002f0: 6520 6361 6e20 7072 6f76 6964 6520 7468  e can provide th
-00000300: 6520 7369 7465 5c27 7320 686f 7374 6e61  e site\'s hostna
-00000310: 6d65 5c6e 6173 2061 206c 6f63 616c 2076  me\nas a local v
-00000320: 6172 6961 626c 652c 2074 6865 2066 7261  ariable, the fra
-00000330: 6d65 776f 726b 206b 6e6f 7720 686f 7720  mework know how 
-00000340: 746f 2063 6f6e 7374 7275 6374 2068 7474  to construct htt
-00000350: 7020 6361 6c6c 2066 726f 6d20 7468 6174  p call from that
-00000360: 2e5c 6e5c 6e45 6163 6820 7465 7374 2066  .\n\nEach test f
-00000370: 756e 6374 696f 6e20 696e 2074 6865 202e  unction in the .
-00000380: 7079 2074 6573 7420 6669 6c65 2072 6570  py test file rep
-00000390: 7265 7365 6e74 2061 2073 6365 6e61 7269  resent a scenari
-000003a0: 6f20 6f66 2074 6573 7420 7768 6963 6820  o of test which 
-000003b0: 6973 2063 6f6e 7369 7374 6564 2062 7920  is consisted by 
-000003c0: 7365 7665 7261 6c20 7374 6570 732e 2046  several steps. F
-000003d0: 6f72 2065 7861 6d70 6c65 2c5c 6e74 6573  or example,\ntes
-000003e0: 7420 7573 6572 5c27 7320 6163 636f 756e  t user\'s accoun
-000003f0: 7420 7061 6765 2c20 6669 7273 742c 2077  t page, first, w
-00000400: 6520 6175 7468 656e 7469 6361 7465 2074  e authenticate t
-00000410: 6865 2063 6c69 656e 7420 6279 2070 6f73  he client by pos
-00000420: 7420 7573 6572 5c27 7320 6e61 6d65 2061  t user\'s name a
-00000430: 6e64 2070 6173 7377 6f72 642c 5c6e 7468  nd password,\nth
-00000440: 656e 2061 6363 6573 7320 7468 6520 6163  en access the ac
-00000450: 636f 756e 7420 7061 6765 2074 6f20 7665  count page to ve
-00000460: 7269 6679 2073 6f6d 6520 7661 6c75 6573  rify some values
-00000470: 2e20 4561 6368 2073 7465 7020 6973 2064  . Each step is d
-00000480: 6573 6372 6962 6564 2062 7920 6361 6c6c  escribed by call
-00000490: 696e 6720 7468 6520 7661 7269 6162 6c65  ing the variable
-000004a0: 2060 6368 6563 6b60 5c6e 7768 6963 6820   `check`\nwhich 
-000004b0: 6973 2061 2070 7974 6573 7420 6669 7874  is a pytest fixt
-000004c0: 7572 652e 5c6e 5c6e 2323 2054 7574 6f72  ure.\n\n## Tutor
-000004d0: 6961 6c5c 6e23 2323 2049 6e73 7461 6c6c  ial\n### Install
-000004e0: 5c6e 6060 6062 6173 685c 6e70 6970 2069  \n```bash\npip i
-000004f0: 6e73 7461 6c6c 2070 7974 6573 742d 6874  nstall pytest-ht
-00000500: 7470 7465 7374 696e 675c 6e60 6060 5c6e  tptesting\n```\n
-00000510: 5c6e 2323 2320 4372 6561 7465 2074 6573  \n### Create tes
-00000520: 7420 7375 6974 655c 6e60 6060 7079 7468  t suite\n```pyth
-00000530: 6f6e 5c6e 2320 7465 7374 2f74 6573 745f  on\n# test/test_
-00000540: 6578 616d 706c 652e 7079 5c6e 6672 6f6d  example.py\nfrom
-00000550: 2068 7474 705f 7465 7374 696e 672e 6173   http_testing.as
-00000560: 7365 7274 696f 6e73 2069 6d70 6f72 7420  sertions import 
-00000570: 4173 7365 7274 696f 6e73 2c20 4e65 6761  Assertions, Nega
-00000580: 7469 7665 4173 7365 7274 696f 6e73 5c6e  tiveAssertions\n
-00000590: 6672 6f6d 2068 7474 705f 7465 7374 696e  from http_testin
-000005a0: 672e 636f 6f6b 6965 2069 6d70 6f72 7420  g.cookie import 
-000005b0: 436f 6f6b 6965 5c6e 6672 6f6d 2068 7474  Cookie\nfrom htt
-000005c0: 705f 7465 7374 696e 672e 7061 6765 5f63  p_testing.page_c
-000005d0: 6865 636b 6572 2069 6d70 6f72 7420 5061  hecker import Pa
-000005e0: 6765 4368 6563 6b65 725c 6e66 726f 6d20  geChecker\nfrom 
-000005f0: 6874 7470 5f74 6573 7469 6e67 2e76 616c  http_testing.val
-00000600: 6964 6174 6f72 7320 696d 706f 7274 2052  idators import R
-00000610: 6567 6578 5c6e 5c6e 686f 7374 203d 2022  egex\n\nhost = "
-00000620: 7777 772e 676f 6f67 6c65 2e63 6f6d 2220  www.google.com" 
-00000630: 2023 206d 616e 6461 746f 7279 3a20 7573   # mandatory: us
-00000640: 6564 2069 6e20 7468 6520 6063 6865 636b  ed in the `check
-00000650: 6020 6669 7874 7572 655c 6e73 6368 656d  ` fixture\nschem
-00000660: 6520 3d20 2268 7474 7073 2220 2023 2022  e = "https"  # "
-00000670: 6874 7470 7322 2062 7920 6465 6661 756c  https" by defaul
-00000680: 745c 6e70 6f72 7420 3d20 4e6f 6e65 2020  t\nport = None  
-00000690: 2320 4e6f 6e65 2062 7920 6465 6661 756c  # None by defaul
-000006a0: 745c 6e5c 6e5c 6e64 6566 2074 6573 745f  t\n\n\ndef test_
-000006b0: 7363 656e 6172 696f 5f6f 6e65 2863 6865  scenario_one(che
-000006c0: 636b 3a20 5061 6765 4368 6563 6b65 7229  ck: PageChecker)
-000006d0: 3a5c 6e20 2020 2063 6865 636b 285c 6e20  :\n    check(\n 
-000006e0: 2020 2020 2020 2074 6974 6c65 3d22 5365         title="Se
-000006f0: 6e61 7269 6f20 4f6e 6522 2c5c 6e20 2020  nario One",\n   
-00000700: 2020 2020 2070 6174 683d 222f 222c 5c6e       path="/",\n
-00000710: 2020 2020 2020 2020 7368 6f75 6c64 5f66          should_f
-00000720: 696e 643d 4173 7365 7274 696f 6e73 285c  ind=Assertions(\
-00000730: 6e20 2020 2020 2020 2020 2020 2073 7461  n            sta
-00000740: 7475 735f 636f 6465 3d32 3030 2c5c 6e20  tus_code=200,\n 
-00000750: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00000760: 6e74 3d5b 223c 7469 746c 653e 476f 6f67  nt=["<title>Goog
-00000770: 6c65 3c2f 7469 746c 653e 225d 2c5c 6e20  le</title>"],\n 
-00000780: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-00000790: 7273 3d7b 2243 6f6e 7465 6e74 2d54 7970  rs={"Content-Typ
-000007a0: 6522 3a20 2274 6578 742f 6874 6d6c 3b20  e": "text/html; 
-000007b0: 6368 6172 7365 743d 4953 4f2d 3838 3539  charset=ISO-8859
-000007c0: 2d31 227d 2c5c 6e20 2020 2020 2020 2020  -1"},\n         
-000007d0: 2020 2063 6f6f 6b69 6573 3d5b 436f 6f6b     cookies=[Cook
-000007e0: 6965 286e 616d 653d 2241 4543 222c 2076  ie(name="AEC", v
-000007f0: 616c 7565 3d52 6567 6578 2872 222e 2a22  alue=Regex(r".*"
-00000800: 2929 5d2c 5c6e 2020 2020 2020 2020 292c  ))],\n        ),
-00000810: 5c6e 2020 2020 2020 2020 7368 6f75 6c64  \n        should
-00000820: 5f6e 6f74 5f66 696e 643d 4e65 6761 7469  _not_find=Negati
-00000830: 7665 4173 7365 7274 696f 6e73 285c 6e20  veAssertions(\n 
-00000840: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-00000850: 735f 636f 6465 3d34 3030 2c5c 6e20 2020  s_code=400,\n   
-00000860: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
-00000870: 3d5b 2267 726f 6f74 225d 2c5c 6e20 2020  =["groot"],\n   
-00000880: 2020 2020 2020 2020 2068 6561 6465 7273           headers
-00000890: 3d7b 226e 6f6f 6f6f 6f22 3a20 2222 7d2c  ={"nooooo": ""},
-000008a0: 5c6e 2020 2020 2020 2020 2020 2020 636f  \n            co
-000008b0: 6f6b 6965 733d 5b43 6f6f 6b69 6528 6e61  okies=[Cookie(na
-000008c0: 6d65 3d22 6e6f 7022 2c20 7661 6c75 653d  me="nop", value=
-000008d0: 2261 2229 5d2c 5c6e 2020 2020 2020 2020  "a")],\n        
-000008e0: 292c 5c6e 2020 2020 2020 2020 7469 6d65  ),\n        time
-000008f0: 6f75 743d 3130 2c20 2023 2079 6f75 2063  out=10,  # you c
-00000900: 616e 2070 6173 7320 6164 6469 7469 6f6e  an pass addition
-00000910: 616c 206b 7761 7267 7320 746f 2068 7474  al kwargs to htt
-00000920: 7078 2072 6571 7565 7374 5c6e 2020 2020  px request\n    
-00000930: 295c 6e5c 6e20 2020 2061 7373 6572 7420  )\n\n    assert 
-00000940: 6368 6563 6b2e 7072 6576 696f 7573 5f72  check.previous_r
-00000950: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
-00000960: 6f64 6520 3d3d 2032 3030 2020 2320 696e  ode == 200  # in
-00000970: 7370 6563 7420 7072 6576 696f 7573 2072  spect previous r
-00000980: 6573 706f 6e73 655c 6e60 6060 5c6e 5c6e  esponse\n```\n\n
-00000990: 2323 2320 5275 6e20 7465 7374 5c6e 6060  ### Run test\n``
-000009a0: 6062 6173 685c 6e24 2070 7974 6573 7420  `bash\n$ pytest 
-000009b0: 7465 7374 202d 2d74 623d 6e6f 202d 2d6e  test --tb=no --n
-000009c0: 6f2d 6865 6164 6572 202d 7620 2023 2074  o-header -v  # t
-000009d0: 7261 6365 6261 636b 2069 7320 6469 7361  raceback is disa
-000009e0: 626c 6564 2062 6563 6175 7365 2069 7420  bled because it 
-000009f0: 6973 206e 6f74 2076 6572 7920 7573 6566  is not very usef
-00000a00: 756c 2074 6f20 616e 6179 7365 2074 6865  ul to anayse the
-00000a10: 2066 756e 6374 696f 6e61 6c20 6572 726f   functional erro
-00000a20: 725c 6e3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  r\n=============
-00000a30: 2074 6573 7420 7365 7373 696f 6e20 7374   test session st
-00000a40: 6172 7473 203d 3d3d 3d3d 3d3d 3d3d 3d3d  arts ===========
-00000a50: 3d3d 5c6e 636f 6c6c 6563 7465 6420 3120  ==\ncollected 1 
-00000a60: 6974 656d 5c6e 5c6e 7465 7374 2f74 6573  item\n\ntest/tes
-00000a70: 745f 6578 616d 706c 652e 7079 3a3a 7465  t_example.py::te
-00000a80: 7374 5f73 6365 6e61 7269 6f5f 6f6e 6520  st_scenario_one 
-00000a90: 5041 5353 4544 5c6e 5c6e 3d3d 3d3d 3d3d  PASSED\n\n======
-00000aa0: 3d3d 3d3d 3d3d 3d20 3120 7061 7373 6564  ======= 1 passed
-00000ab0: 2069 6e20 302e 3136 7320 3d3d 3d3d 3d3d   in 0.16s ======
-00000ac0: 3d3d 3d3d 3d3d 3d5c 6e5c 6e60 6060 5c6e  =======\n\n```\n
-00000ad0: 5c6e 2323 2320 4465 6275 675c 6e49 6e20  \n### Debug\nIn 
-00000ae0: 6361 7365 206f 6620 6572 726f 722c 2061  case of error, a
-00000af0: 2074 656d 706f 7261 7279 2066 696c 6520   temporary file 
-00000b00: 7769 6c6c 2062 6520 6765 6e65 7261 7465  will be generate
-00000b10: 642c 2061 7320 7368 6f77 6e20 696e 2074  d, as shown in t
-00000b20: 6865 2060 7368 6f72 7420 7465 7374 2073  he `short test s
-00000b30: 756d 6d61 7279 2069 6e66 6f60 2e20 4974  ummary info`. It
-00000b40: 2069 7320 6120 6a73 6f6e 2066 696c 6520   is a json file 
-00000b50: 636f 6e63 6c75 6469 6e67 5c6e 7265 7370  concluding\nresp
-00000b60: 6f6e 7365 2063 6f6e 7465 6e74 2c20 7374  onse content, st
-00000b70: 6174 7573 2063 6f64 652c 2068 6561 6465  atus code, heade
-00000b80: 7273 2061 6e64 2063 6f6f 6b69 6573 2e5c  rs and cookies.\
-00000b90: 6e60 6060 6261 7368 5c6e 2420 7079 7465  n```bash\n$ pyte
-00000ba0: 7374 2074 6573 7420 2d2d 7462 3d6e 6f20  st test --tb=no 
-00000bb0: 2d2d 6e6f 2d68 6561 6465 7220 2d76 5c6e  --no-header -v\n
-00000bc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 7465  ============= te
-00000bd0: 7374 2073 6573 7369 6f6e 2073 7461 7274  st session start
-00000be0: 7320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5c  s =============\
-00000bf0: 6e63 6f6c 6c65 6374 6564 2031 2069 7465  ncollected 1 ite
-00000c00: 6d5c 6e5c 6e74 6573 742f 7465 7374 5f65  m\n\ntest/test_e
-00000c10: 7861 6d70 6c65 2e70 793a 3a74 6573 745f  xample.py::test_
-00000c20: 7363 656e 6172 696f 5f6f 6e65 2046 4149  scenario_one FAI
-00000c30: 4c45 445c 6e5c 6e3d 3d3d 3d3d 3d3d 3d3d  LED\n\n=========
-00000c40: 3d3d 3d3d 2073 686f 7274 2074 6573 7420  ==== short test 
-00000c50: 7375 6d6d 6172 7920 696e 666f 203d 3d3d  summary info ===
-00000c60: 3d3d 3d3d 3d3d 3d3d 3d3d 5c6e 4641 494c  ==========\nFAIL
-00000c70: 4544 2074 6573 742f 7465 7374 5f65 7861  ED test/test_exa
-00000c80: 6d70 6c65 2e70 793a 3a74 6573 745f 7363  mple.py::test_sc
-00000c90: 656e 6172 696f 5f6f 6e65 202d 2041 7373  enario_one - Ass
-00000ca0: 6572 7469 6f6e 4572 726f 723a 2053 656e  ertionError: Sen
-00000cb0: 6172 696f 204f 6e65 202d 205c 2743 6f6e  ario One - \'Con
-00000cc0: 7465 6e74 2d54 7970 6573 7373 735c 273a  tent-Typessss\':
-00000cd0: 5c27 7465 7874 2f68 746d 6c3b 2063 6861  \'text/html; cha
-00000ce0: 7273 6574 3d49 534f 2d38 3835 392d 315c  rset=ISO-8859-1\
-00000cf0: 2720 6e6f 7420 666f 756e 6420 696e 2068  ' not found in h
-00000d00: 6561 6465 7273 206f 6e20 7061 6765 205c  eaders on page \
-00000d10: 2768 7474 7073 3a2f 2f77 7777 2e67 6f6f  'https://www.goo
-00000d20: 676c 652e 636f 6d2f 5c27 202d 2070 6c65  gle.com/\' - ple
-00000d30: 6173 6520 6368 6563 6b20 6669 6c65 205c  ase check file \
-00000d40: 272f 746d 702f 746d 7074 616f 7764 3275  '/tmp/tmptaowd2u
-00000d50: 355c 275c 6e3d 3d3d 3d3d 3d3d 3d3d 3d3d  5\'\n===========
-00000d60: 3d3d 2031 2066 6169 6c65 6420 696e 2031  == 1 failed in 1
-00000d70: 2e32 3273 203d 3d3d 3d3d 3d3d 3d3d 3d3d  .22s ===========
-00000d80: 3d3d 5c6e 5c6e 6060 605c 6e5c 6e23 2323  ==\n\n```\n\n###
-00000d90: 2041 6476 616e 6365 645c 6e23 2323 2320   Advanced\n#### 
-00000da0: 4375 7374 6f6d 697a 6520 7468 6520 6874  Customize the ht
-00000db0: 7470 2063 6c69 656e 7420 636f 6e66 6967  tp client config
-00000dc0: 7572 6174 696f 6e5c 6e49 7420 6973 2070  uration\nIt is p
-00000dd0: 6f73 7369 626c 6520 746f 2063 7265 6174  ossible to creat
-00000de0: 6520 6120 6669 7874 7572 6520 6068 7474  e a fixture `htt
-00000df0: 705f 636c 6965 6e74 6020 746f 2063 7265  p_client` to cre
-00000e00: 6174 6520 796f 7572 206f 776e 2068 7474  ate your own htt
-00000e10: 7020 636c 6965 6e74 2e5c 6e60 6060 7079  p client.\n```py
-00000e20: 7468 6f6e 5c6e 4070 7974 6573 742e 6669  thon\n@pytest.fi
-00000e30: 7874 7572 655c 6e64 6566 2068 7474 705f  xture\ndef http_
-00000e40: 636c 6965 6e74 2829 3a5c 6e20 2020 2077  client():\n    w
-00000e50: 6974 6820 436c 6965 6e74 2876 6572 6966  ith Client(verif
-00000e60: 793d 4661 6c73 652c 2063 6f6f 6b69 6573  y=False, cookies
-00000e70: 3d7b 2263 6f6f 6b69 655f 3122 3a20 2263  ={"cookie_1": "c
-00000e80: 6f6f 6b69 655f 7661 6c75 655f 3122 7d29  ookie_value_1"})
-00000e90: 2061 7320 636c 6965 6e74 3a5c 6e20 2020   as client:\n   
-00000ea0: 2020 2020 2079 6965 6c64 2063 6c69 656e       yield clien
-00000eb0: 745c 6e60 6060 5c6e 5c6e 2323 2323 2043  t\n```\n\n#### C
-00000ec0: 7573 746f 6d69 7a65 2074 6865 2062 6173  ustomize the bas
-00000ed0: 6520 7572 6c5c 6e49 7420 6973 2070 6f73  e url\nIt is pos
-00000ee0: 7369 626c 6520 746f 2063 7265 6174 6520  sible to create 
-00000ef0: 6120 6669 7874 7572 6520 6062 6173 655f  a fixture `base_
-00000f00: 7572 6c60 2074 6f20 6f76 6572 7269 6465  url` to override
-00000f10: 2074 6865 2064 6566 6175 6c74 2063 6f6e   the default con
-00000f20: 7374 7275 6374 696f 6e20 6f66 2062 6173  struction of bas
-00000f30: 6520 7572 6c2e 5c6e 6060 6070 7974 686f  e url.\n```pytho
-00000f40: 6e5c 6e66 726f 6d20 6874 7470 7820 696d  n\nfrom httpx im
-00000f50: 706f 7274 2055 524c 5c6e 4070 7974 6573  port URL\n@pytes
-00000f60: 742e 6669 7874 7572 655c 6e64 6566 2062  t.fixture\ndef b
-00000f70: 6173 655f 7572 6c28 2920 2d3e 2055 524c  ase_url() -> URL
-00000f80: 3a5c 6e20 2020 2072 6574 7572 6e20 5552  :\n    return UR
-00000f90: 4c28 2268 7474 7073 3a2f 2f77 7777 2e67  L("https://www.g
-00000fa0: 6f6f 676c 652e 636f 6d22 295c 6e60 6060  oogle.com")\n```
-00000fb0: 5c6e 272c 0a20 2020 2027 6175 7468 6f72  \n',.    'author
-00000fc0: 273a 2027 4845 2051 696c 6527 2c0a 2020  ': 'HE Qile',.  
-00000fd0: 2020 2761 7574 686f 725f 656d 6169 6c27    'author_email'
-00000fe0: 3a20 276d 722e 7169 6c65 4067 6d61 696c  : 'mr.qile@gmail
-00000ff0: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
-00001000: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
-00001010: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-00001020: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
-00001030: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
-00001040: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001050: 6865 7169 6c65 2f68 7474 705f 7465 7374  heqile/http_test
-00001060: 696e 6727 2c0a 2020 2020 2770 6163 6b61  ing',.    'packa
-00001070: 6765 7327 3a20 7061 636b 6167 6573 2c0a  ges': packages,.
-00001080: 2020 2020 2770 6163 6b61 6765 5f64 6174      'package_dat
-00001090: 6127 3a20 7061 636b 6167 655f 6461 7461  a': package_data
-000010a0: 2c0a 2020 2020 2769 6e73 7461 6c6c 5f72  ,.    'install_r
-000010b0: 6571 7569 7265 7327 3a20 696e 7374 616c  equires': instal
-000010c0: 6c5f 7265 7175 6972 6573 2c0a 2020 2020  l_requires,.    
-000010d0: 2765 6e74 7279 5f70 6f69 6e74 7327 3a20  'entry_points': 
-000010e0: 656e 7472 795f 706f 696e 7473 2c0a 2020  entry_points,.  
-000010f0: 2020 2770 7974 686f 6e5f 7265 7175 6972    'python_requir
-00001100: 6573 273a 2027 3e3d 332e 382c 3c34 2e30  es': '>=3.8,<4.0
-00001110: 272c 0a7d 0a0a 0a73 6574 7570 282a 2a73  ',.}...setup(**s
-00001120: 6574 7570 5f6b 7761 7267 7329 0a         etup_kwargs).
+000001f0: 494e 475c 6e5c 6e3c 6120 6872 6566 3d22  ING\n\n<a href="
+00000200: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000210: 6f6d 2f68 6571 696c 652f 6874 7470 5f74  om/heqile/http_t
+00000220: 6573 7469 6e67 2f61 6374 696f 6e73 3f71  esting/actions?q
+00000230: 7565 7279 3d62 7261 6e63 6825 3341 6d61  uery=branch%3Ama
+00000240: 696e 2b65 7665 6e74 2533 4170 7573 682b  in+event%3Apush+
+00000250: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000260: 223e 5c6e 2020 2020 3c69 6d67 2073 7263  ">\n    <img src
+00000270: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000280: 2e63 6f6d 2f68 6571 696c 652f 6874 7470  .com/heqile/http
+00000290: 5f74 6573 7469 6e67 2f77 6f72 6b66 6c6f  _testing/workflo
+000002a0: 7773 2f54 6573 742f 6261 6467 652e 7376  ws/Test/badge.sv
+000002b0: 673f 6576 656e 743d 7075 7368 2662 7261  g?event=push&bra
+000002c0: 6e63 683d 6d61 696e 2220 616c 743d 2254  nch=main" alt="T
+000002d0: 6573 7422 3e5c 6e3c 2f61 3e5c 6e3c 6120  est">\n</a>\n<a 
+000002e0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+000002f0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
+00000300: 7974 6573 742d 6874 7470 7465 7374 696e  ytest-httptestin
+00000310: 6722 2074 6172 6765 743d 225f 626c 616e  g" target="_blan
+00000320: 6b22 3e5c 6e20 2020 203c 696d 6720 7372  k">\n    <img sr
+00000330: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000340: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000350: 2f70 7974 6573 742d 6874 7470 7465 7374  /pytest-httptest
+00000360: 696e 673f 636f 6c6f 723d 2532 3333 3444  ing?color=%2334D
+00000370: 3035 3826 6c61 6265 6c3d 7079 7069 2532  058&label=pypi%2
+00000380: 3070 6163 6b61 6765 2220 616c 743d 2250  0package" alt="P
+00000390: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
+000003a0: 5c6e 3c2f 613e 5c6e 3c61 2068 7265 663d  \n</a>\n<a href=
+000003b0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+000003c0: 672f 7072 6f6a 6563 742f 7079 7465 7374  g/project/pytest
+000003d0: 2d68 7474 7074 6573 7469 6e67 2220 7461  -httptesting" ta
+000003e0: 7267 6574 3d22 5f62 6c61 6e6b 223e 5c6e  rget="_blank">\n
+000003f0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000400: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000410: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000420: 696f 6e73 2f70 7974 6573 742d 6874 7470  ions/pytest-http
+00000430: 7465 7374 696e 672e 7376 673f 636f 6c6f  testing.svg?colo
+00000440: 723d 2532 3333 3444 3035 3822 2061 6c74  r=%2334D058" alt
+00000450: 3d22 5375 7070 6f72 7465 6420 5079 7468  ="Supported Pyth
+00000460: 6f6e 2076 6572 7369 6f6e 7322 3e5c 6e3c  on versions">\n<
+00000470: 2f61 3e5c 6e5c 6e23 2320 4465 7363 7269  /a>\n\n## Descri
+00000480: 7074 696f 6e5c 6e54 6869 7320 7072 6f6a  ption\nThis proj
+00000490: 6563 7420 6169 6d73 2074 6f20 6865 6c70  ect aims to help
+000004a0: 2074 6f20 6372 6561 7465 2065 3265 2074   to create e2e t
+000004b0: 6573 7473 2c20 6279 2063 6861 696e 696e  ests, by chainin
+000004c0: 6720 6874 7470 2063 616c 6c73 2061 6e64  g http calls and
+000004d0: 2076 6572 6966 6963 6174 696f 6e73 206f   verifications o
+000004e0: 6e20 7461 7267 6574 2070 6167 6573 2e5c  n target pages.\
+000004f0: 6e5c 6e23 2320 436f 6e63 6570 745c 6e54  n\n## Concept\nT
+00000500: 6869 7320 7072 6f6a 6563 7420 6973 2062  his project is b
+00000510: 7569 6c74 206f 6e20 7079 7465 7374 2e5c  uilt on pytest.\
+00000520: 6e5c 6e45 6163 6820 2e70 7920 6669 6c65  n\nEach .py file
+00000530: 2069 6e20 7465 7374 2072 6570 7265 7365   in test represe
+00000540: 6e74 7320 7365 7665 7261 6c20 7465 7374  nts several test
+00000550: 7320 7363 656e 6172 696f 206f 6e20 6f6e  s scenario on on
+00000560: 6520 7461 7267 6574 2073 6974 652c 2077  e target site, w
+00000570: 6520 6361 6e20 7072 6f76 6964 6520 7468  e can provide th
+00000580: 6520 7369 7465 5c27 7320 686f 7374 6e61  e site\'s hostna
+00000590: 6d65 5c6e 6173 2061 206c 6f63 616c 2076  me\nas a local v
+000005a0: 6172 6961 626c 652c 2074 6865 2066 7261  ariable, the fra
+000005b0: 6d65 776f 726b 206b 6e6f 7720 686f 7720  mework know how 
+000005c0: 746f 2063 6f6e 7374 7275 6374 2068 7474  to construct htt
+000005d0: 7020 6361 6c6c 2066 726f 6d20 7468 6174  p call from that
+000005e0: 2e5c 6e5c 6e45 6163 6820 7465 7374 2066  .\n\nEach test f
+000005f0: 756e 6374 696f 6e20 696e 2074 6865 202e  unction in the .
+00000600: 7079 2074 6573 7420 6669 6c65 2072 6570  py test file rep
+00000610: 7265 7365 6e74 2061 2073 6365 6e61 7269  resent a scenari
+00000620: 6f20 6f66 2074 6573 7420 7768 6963 6820  o of test which 
+00000630: 6973 2063 6f6e 7369 7374 6564 2062 7920  is consisted by 
+00000640: 7365 7665 7261 6c20 7374 6570 732e 2046  several steps. F
+00000650: 6f72 2065 7861 6d70 6c65 2c5c 6e74 6573  or example,\ntes
+00000660: 7420 7573 6572 5c27 7320 6163 636f 756e  t user\'s accoun
+00000670: 7420 7061 6765 2c20 6669 7273 742c 2077  t page, first, w
+00000680: 6520 6175 7468 656e 7469 6361 7465 2074  e authenticate t
+00000690: 6865 2063 6c69 656e 7420 6279 2070 6f73  he client by pos
+000006a0: 7420 7573 6572 5c27 7320 6e61 6d65 2061  t user\'s name a
+000006b0: 6e64 2070 6173 7377 6f72 642c 5c6e 7468  nd password,\nth
+000006c0: 656e 2061 6363 6573 7320 7468 6520 6163  en access the ac
+000006d0: 636f 756e 7420 7061 6765 2074 6f20 7665  count page to ve
+000006e0: 7269 6679 2073 6f6d 6520 7661 6c75 6573  rify some values
+000006f0: 2e20 4561 6368 2073 7465 7020 6973 2064  . Each step is d
+00000700: 6573 6372 6962 6564 2062 7920 6361 6c6c  escribed by call
+00000710: 696e 6720 7468 6520 7661 7269 6162 6c65  ing the variable
+00000720: 2060 6368 6563 6b60 5c6e 7768 6963 6820   `check`\nwhich 
+00000730: 6973 2061 2070 7974 6573 7420 6669 7874  is a pytest fixt
+00000740: 7572 652e 5c6e 5c6e 2323 2054 7574 6f72  ure.\n\n## Tutor
+00000750: 6961 6c5c 6e23 2323 2049 6e73 7461 6c6c  ial\n### Install
+00000760: 5c6e 6060 6062 6173 685c 6e70 6970 2069  \n```bash\npip i
+00000770: 6e73 7461 6c6c 2070 7974 6573 742d 6874  nstall pytest-ht
+00000780: 7470 7465 7374 696e 675c 6e60 6060 5c6e  tptesting\n```\n
+00000790: 5c6e 2323 2320 4372 6561 7465 2074 6573  \n### Create tes
+000007a0: 7420 7375 6974 655c 6e60 6060 7079 7468  t suite\n```pyth
+000007b0: 6f6e 5c6e 2320 7465 7374 2f74 6573 745f  on\n# test/test_
+000007c0: 6578 616d 706c 652e 7079 5c6e 6672 6f6d  example.py\nfrom
+000007d0: 2068 7474 705f 7465 7374 696e 672e 6173   http_testing.as
+000007e0: 7365 7274 696f 6e73 2069 6d70 6f72 7420  sertions import 
+000007f0: 4173 7365 7274 696f 6e73 2c20 4e65 6761  Assertions, Nega
+00000800: 7469 7665 4173 7365 7274 696f 6e73 5c6e  tiveAssertions\n
+00000810: 6672 6f6d 2068 7474 705f 7465 7374 696e  from http_testin
+00000820: 672e 636f 6f6b 6965 2069 6d70 6f72 7420  g.cookie import 
+00000830: 436f 6f6b 6965 5c6e 6672 6f6d 2068 7474  Cookie\nfrom htt
+00000840: 705f 7465 7374 696e 672e 7061 6765 5f63  p_testing.page_c
+00000850: 6865 636b 6572 2069 6d70 6f72 7420 5061  hecker import Pa
+00000860: 6765 4368 6563 6b65 725c 6e66 726f 6d20  geChecker\nfrom 
+00000870: 6874 7470 5f74 6573 7469 6e67 2e76 616c  http_testing.val
+00000880: 6964 6174 6f72 7320 696d 706f 7274 2052  idators import R
+00000890: 6567 6578 5c6e 5c6e 686f 7374 203d 2022  egex\n\nhost = "
+000008a0: 7777 772e 676f 6f67 6c65 2e63 6f6d 2220  www.google.com" 
+000008b0: 2023 206d 616e 6461 746f 7279 3a20 7573   # mandatory: us
+000008c0: 6564 2069 6e20 7468 6520 6063 6865 636b  ed in the `check
+000008d0: 6020 6669 7874 7572 655c 6e73 6368 656d  ` fixture\nschem
+000008e0: 6520 3d20 2268 7474 7073 2220 2023 2022  e = "https"  # "
+000008f0: 6874 7470 7322 2062 7920 6465 6661 756c  https" by defaul
+00000900: 745c 6e70 6f72 7420 3d20 4e6f 6e65 2020  t\nport = None  
+00000910: 2320 4e6f 6e65 2062 7920 6465 6661 756c  # None by defaul
+00000920: 745c 6e5c 6e5c 6e64 6566 2074 6573 745f  t\n\n\ndef test_
+00000930: 7363 656e 6172 696f 5f6f 6e65 2863 6865  scenario_one(che
+00000940: 636b 3a20 5061 6765 4368 6563 6b65 7229  ck: PageChecker)
+00000950: 3a5c 6e20 2020 2063 6865 636b 285c 6e20  :\n    check(\n 
+00000960: 2020 2020 2020 2074 6974 6c65 3d22 5365         title="Se
+00000970: 6e61 7269 6f20 4f6e 6522 2c5c 6e20 2020  nario One",\n   
+00000980: 2020 2020 2070 6174 683d 222f 222c 5c6e       path="/",\n
+00000990: 2020 2020 2020 2020 7368 6f75 6c64 5f66          should_f
+000009a0: 696e 643d 4173 7365 7274 696f 6e73 285c  ind=Assertions(\
+000009b0: 6e20 2020 2020 2020 2020 2020 2073 7461  n            sta
+000009c0: 7475 735f 636f 6465 3d32 3030 2c5c 6e20  tus_code=200,\n 
+000009d0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+000009e0: 6e74 3d5b 223c 7469 746c 653e 476f 6f67  nt=["<title>Goog
+000009f0: 6c65 3c2f 7469 746c 653e 225d 2c5c 6e20  le</title>"],\n 
+00000a00: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+00000a10: 7273 3d7b 2243 6f6e 7465 6e74 2d54 7970  rs={"Content-Typ
+00000a20: 6522 3a20 2274 6578 742f 6874 6d6c 3b20  e": "text/html; 
+00000a30: 6368 6172 7365 743d 4953 4f2d 3838 3539  charset=ISO-8859
+00000a40: 2d31 227d 2c5c 6e20 2020 2020 2020 2020  -1"},\n         
+00000a50: 2020 2063 6f6f 6b69 6573 3d5b 436f 6f6b     cookies=[Cook
+00000a60: 6965 286e 616d 653d 2241 4543 222c 2076  ie(name="AEC", v
+00000a70: 616c 7565 3d52 6567 6578 2872 222e 2a22  alue=Regex(r".*"
+00000a80: 2929 5d2c 5c6e 2020 2020 2020 2020 292c  ))],\n        ),
+00000a90: 5c6e 2020 2020 2020 2020 7368 6f75 6c64  \n        should
+00000aa0: 5f6e 6f74 5f66 696e 643d 4e65 6761 7469  _not_find=Negati
+00000ab0: 7665 4173 7365 7274 696f 6e73 285c 6e20  veAssertions(\n 
+00000ac0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00000ad0: 735f 636f 6465 3d34 3030 2c5c 6e20 2020  s_code=400,\n   
+00000ae0: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+00000af0: 3d5b 2267 726f 6f74 225d 2c5c 6e20 2020  =["groot"],\n   
+00000b00: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+00000b10: 3d7b 226e 6f6f 6f6f 6f22 3a20 2222 7d2c  ={"nooooo": ""},
+00000b20: 5c6e 2020 2020 2020 2020 2020 2020 636f  \n            co
+00000b30: 6f6b 6965 733d 5b43 6f6f 6b69 6528 6e61  okies=[Cookie(na
+00000b40: 6d65 3d22 6e6f 7022 2c20 7661 6c75 653d  me="nop", value=
+00000b50: 2261 2229 5d2c 5c6e 2020 2020 2020 2020  "a")],\n        
+00000b60: 292c 5c6e 2020 2020 2020 2020 7469 6d65  ),\n        time
+00000b70: 6f75 743d 3130 2c20 2023 2079 6f75 2063  out=10,  # you c
+00000b80: 616e 2070 6173 7320 6164 6469 7469 6f6e  an pass addition
+00000b90: 616c 206b 7761 7267 7320 746f 2068 7474  al kwargs to htt
+00000ba0: 7078 2072 6571 7565 7374 5c6e 2020 2020  px request\n    
+00000bb0: 295c 6e5c 6e20 2020 2061 7373 6572 7420  )\n\n    assert 
+00000bc0: 6368 6563 6b2e 7072 6576 696f 7573 5f72  check.previous_r
+00000bd0: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
+00000be0: 6f64 6520 3d3d 2032 3030 2020 2320 696e  ode == 200  # in
+00000bf0: 7370 6563 7420 7072 6576 696f 7573 2072  spect previous r
+00000c00: 6573 706f 6e73 655c 6e60 6060 5c6e 5c6e  esponse\n```\n\n
+00000c10: 2323 2320 5275 6e20 7465 7374 5c6e 6060  ### Run test\n``
+00000c20: 6062 6173 685c 6e24 2070 7974 6573 7420  `bash\n$ pytest 
+00000c30: 7465 7374 202d 2d74 623d 6e6f 202d 2d6e  test --tb=no --n
+00000c40: 6f2d 6865 6164 6572 202d 7620 2023 2074  o-header -v  # t
+00000c50: 7261 6365 6261 636b 2069 7320 6469 7361  raceback is disa
+00000c60: 626c 6564 2062 6563 6175 7365 2069 7420  bled because it 
+00000c70: 6973 206e 6f74 2076 6572 7920 7573 6566  is not very usef
+00000c80: 756c 2074 6f20 616e 6179 7365 2074 6865  ul to anayse the
+00000c90: 2066 756e 6374 696f 6e61 6c20 6572 726f   functional erro
+00000ca0: 725c 6e3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  r\n=============
+00000cb0: 2074 6573 7420 7365 7373 696f 6e20 7374   test session st
+00000cc0: 6172 7473 203d 3d3d 3d3d 3d3d 3d3d 3d3d  arts ===========
+00000cd0: 3d3d 5c6e 636f 6c6c 6563 7465 6420 3120  ==\ncollected 1 
+00000ce0: 6974 656d 5c6e 5c6e 7465 7374 2f74 6573  item\n\ntest/tes
+00000cf0: 745f 6578 616d 706c 652e 7079 3a3a 7465  t_example.py::te
+00000d00: 7374 5f73 6365 6e61 7269 6f5f 6f6e 6520  st_scenario_one 
+00000d10: 5041 5353 4544 5c6e 5c6e 3d3d 3d3d 3d3d  PASSED\n\n======
+00000d20: 3d3d 3d3d 3d3d 3d20 3120 7061 7373 6564  ======= 1 passed
+00000d30: 2069 6e20 302e 3136 7320 3d3d 3d3d 3d3d   in 0.16s ======
+00000d40: 3d3d 3d3d 3d3d 3d5c 6e5c 6e60 6060 5c6e  =======\n\n```\n
+00000d50: 5c6e 2323 2320 4465 6275 675c 6e49 6e20  \n### Debug\nIn 
+00000d60: 6361 7365 206f 6620 6572 726f 722c 2061  case of error, a
+00000d70: 2074 656d 706f 7261 7279 2066 696c 6520   temporary file 
+00000d80: 7769 6c6c 2062 6520 6765 6e65 7261 7465  will be generate
+00000d90: 642c 2061 7320 7368 6f77 6e20 696e 2074  d, as shown in t
+00000da0: 6865 2060 7368 6f72 7420 7465 7374 2073  he `short test s
+00000db0: 756d 6d61 7279 2069 6e66 6f60 2e20 4974  ummary info`. It
+00000dc0: 2069 7320 6120 6a73 6f6e 2066 696c 6520   is a json file 
+00000dd0: 636f 6e63 6c75 6469 6e67 5c6e 7265 7370  concluding\nresp
+00000de0: 6f6e 7365 2063 6f6e 7465 6e74 2c20 7374  onse content, st
+00000df0: 6174 7573 2063 6f64 652c 2068 6561 6465  atus code, heade
+00000e00: 7273 2061 6e64 2063 6f6f 6b69 6573 2e5c  rs and cookies.\
+00000e10: 6e60 6060 6261 7368 5c6e 2420 7079 7465  n```bash\n$ pyte
+00000e20: 7374 2074 6573 7420 2d2d 7462 3d6e 6f20  st test --tb=no 
+00000e30: 2d2d 6e6f 2d68 6561 6465 7220 2d76 5c6e  --no-header -v\n
+00000e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 7465  ============= te
+00000e50: 7374 2073 6573 7369 6f6e 2073 7461 7274  st session start
+00000e60: 7320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5c  s =============\
+00000e70: 6e63 6f6c 6c65 6374 6564 2031 2069 7465  ncollected 1 ite
+00000e80: 6d5c 6e5c 6e74 6573 742f 7465 7374 5f65  m\n\ntest/test_e
+00000e90: 7861 6d70 6c65 2e70 793a 3a74 6573 745f  xample.py::test_
+00000ea0: 7363 656e 6172 696f 5f6f 6e65 2046 4149  scenario_one FAI
+00000eb0: 4c45 445c 6e5c 6e3d 3d3d 3d3d 3d3d 3d3d  LED\n\n=========
+00000ec0: 3d3d 3d3d 2073 686f 7274 2074 6573 7420  ==== short test 
+00000ed0: 7375 6d6d 6172 7920 696e 666f 203d 3d3d  summary info ===
+00000ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 5c6e 4641 494c  ==========\nFAIL
+00000ef0: 4544 2074 6573 742f 7465 7374 5f65 7861  ED test/test_exa
+00000f00: 6d70 6c65 2e70 793a 3a74 6573 745f 7363  mple.py::test_sc
+00000f10: 656e 6172 696f 5f6f 6e65 202d 2041 7373  enario_one - Ass
+00000f20: 6572 7469 6f6e 4572 726f 723a 2053 656e  ertionError: Sen
+00000f30: 6172 696f 204f 6e65 202d 205c 2743 6f6e  ario One - \'Con
+00000f40: 7465 6e74 2d54 7970 6573 7373 735c 273a  tent-Typessss\':
+00000f50: 5c27 7465 7874 2f68 746d 6c3b 2063 6861  \'text/html; cha
+00000f60: 7273 6574 3d49 534f 2d38 3835 392d 315c  rset=ISO-8859-1\
+00000f70: 2720 6e6f 7420 666f 756e 6420 696e 2068  ' not found in h
+00000f80: 6561 6465 7273 206f 6e20 7061 6765 205c  eaders on page \
+00000f90: 2768 7474 7073 3a2f 2f77 7777 2e67 6f6f  'https://www.goo
+00000fa0: 676c 652e 636f 6d2f 5c27 202d 2070 6c65  gle.com/\' - ple
+00000fb0: 6173 6520 6368 6563 6b20 6669 6c65 205c  ase check file \
+00000fc0: 272f 746d 702f 746d 7074 616f 7764 3275  '/tmp/tmptaowd2u
+00000fd0: 355c 275c 6e3d 3d3d 3d3d 3d3d 3d3d 3d3d  5\'\n===========
+00000fe0: 3d3d 2031 2066 6169 6c65 6420 696e 2031  == 1 failed in 1
+00000ff0: 2e32 3273 203d 3d3d 3d3d 3d3d 3d3d 3d3d  .22s ===========
+00001000: 3d3d 5c6e 5c6e 6060 605c 6e5c 6e23 2323  ==\n\n```\n\n###
+00001010: 2041 6476 616e 6365 645c 6e23 2323 2320   Advanced\n#### 
+00001020: 4375 7374 6f6d 697a 6520 7468 6520 6874  Customize the ht
+00001030: 7470 2063 6c69 656e 7420 636f 6e66 6967  tp client config
+00001040: 7572 6174 696f 6e5c 6e49 7420 6973 2070  uration\nIt is p
+00001050: 6f73 7369 626c 6520 746f 2063 7265 6174  ossible to creat
+00001060: 6520 6120 6669 7874 7572 6520 6068 7474  e a fixture `htt
+00001070: 705f 636c 6965 6e74 6020 746f 2063 7265  p_client` to cre
+00001080: 6174 6520 796f 7572 206f 776e 2068 7474  ate your own htt
+00001090: 7020 636c 6965 6e74 2e5c 6e60 6060 7079  p client.\n```py
+000010a0: 7468 6f6e 5c6e 4070 7974 6573 742e 6669  thon\n@pytest.fi
+000010b0: 7874 7572 655c 6e64 6566 2068 7474 705f  xture\ndef http_
+000010c0: 636c 6965 6e74 2829 3a5c 6e20 2020 2077  client():\n    w
+000010d0: 6974 6820 436c 6965 6e74 2876 6572 6966  ith Client(verif
+000010e0: 793d 4661 6c73 652c 2063 6f6f 6b69 6573  y=False, cookies
+000010f0: 3d7b 2263 6f6f 6b69 655f 3122 3a20 2263  ={"cookie_1": "c
+00001100: 6f6f 6b69 655f 7661 6c75 655f 3122 7d29  ookie_value_1"})
+00001110: 2061 7320 636c 6965 6e74 3a5c 6e20 2020   as client:\n   
+00001120: 2020 2020 2079 6965 6c64 2063 6c69 656e       yield clien
+00001130: 745c 6e60 6060 5c6e 5c6e 2323 2323 2043  t\n```\n\n#### C
+00001140: 7573 746f 6d69 7a65 2074 6865 2062 6173  ustomize the bas
+00001150: 6520 7572 6c5c 6e49 7420 6973 2070 6f73  e url\nIt is pos
+00001160: 7369 626c 6520 746f 2063 7265 6174 6520  sible to create 
+00001170: 6120 6669 7874 7572 6520 6062 6173 655f  a fixture `base_
+00001180: 7572 6c60 2074 6f20 6f76 6572 7269 6465  url` to override
+00001190: 2074 6865 2064 6566 6175 6c74 2063 6f6e   the default con
+000011a0: 7374 7275 6374 696f 6e20 6f66 2062 6173  struction of bas
+000011b0: 6520 7572 6c2e 5c6e 6060 6070 7974 686f  e url.\n```pytho
+000011c0: 6e5c 6e66 726f 6d20 6874 7470 7820 696d  n\nfrom httpx im
+000011d0: 706f 7274 2055 524c 5c6e 4070 7974 6573  port URL\n@pytes
+000011e0: 742e 6669 7874 7572 655c 6e64 6566 2062  t.fixture\ndef b
+000011f0: 6173 655f 7572 6c28 2920 2d3e 2055 524c  ase_url() -> URL
+00001200: 3a5c 6e20 2020 2072 6574 7572 6e20 5552  :\n    return UR
+00001210: 4c28 2268 7474 7073 3a2f 2f77 7777 2e67  L("https://www.g
+00001220: 6f6f 676c 652e 636f 6d22 295c 6e60 6060  oogle.com")\n```
+00001230: 5c6e 272c 0a20 2020 2027 6175 7468 6f72  \n',.    'author
+00001240: 273a 2027 4845 2051 696c 6527 2c0a 2020  ': 'HE Qile',.  
+00001250: 2020 2761 7574 686f 725f 656d 6169 6c27    'author_email'
+00001260: 3a20 276d 722e 7169 6c65 4067 6d61 696c  : 'mr.qile@gmail
+00001270: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
+00001280: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
+00001290: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
+000012a0: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
+000012b0: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
+000012c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000012d0: 6865 7169 6c65 2f68 7474 705f 7465 7374  heqile/http_test
+000012e0: 696e 6727 2c0a 2020 2020 2770 6163 6b61  ing',.    'packa
+000012f0: 6765 7327 3a20 7061 636b 6167 6573 2c0a  ges': packages,.
+00001300: 2020 2020 2770 6163 6b61 6765 5f64 6174      'package_dat
+00001310: 6127 3a20 7061 636b 6167 655f 6461 7461  a': package_data
+00001320: 2c0a 2020 2020 2769 6e73 7461 6c6c 5f72  ,.    'install_r
+00001330: 6571 7569 7265 7327 3a20 696e 7374 616c  equires': instal
+00001340: 6c5f 7265 7175 6972 6573 2c0a 2020 2020  l_requires,.    
+00001350: 2765 6e74 7279 5f70 6f69 6e74 7327 3a20  'entry_points': 
+00001360: 656e 7472 795f 706f 696e 7473 2c0a 2020  entry_points,.  
+00001370: 2020 2770 7974 686f 6e5f 7265 7175 6972    'python_requir
+00001380: 6573 273a 2027 3e3d 332e 382c 3c34 2e30  es': '>=3.8,<4.0
+00001390: 272c 0a7d 0a0a 0a73 6574 7570 282a 2a73  ',.}...setup(**s
+000013a0: 6574 7570 5f6b 7761 7267 7329 0a         etup_kwargs).
```

