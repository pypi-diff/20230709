# Comparing `tmp/hrequests-0.2.0.tar.gz` & `tmp/hrequests-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrequests-0.2.0.tar", max compression
+gzip compressed data, was "hrequests-0.3.0.tar", max compression
```

## Comparing `hrequests-0.2.0.tar` & `hrequests-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.2.0/hrequests/__init__.py
--rw-r--r--   0        0        0      143 2023-07-08 02:07:11.575795 hrequests-0.2.0/hrequests/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.2.0/hrequests/bin/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.2.0/hrequests/bin/LICENSE.txt
--rw-r--r--   0        0        0    23097 2023-07-08 02:07:11.879627 hrequests-0.2.0/hrequests/browser.py
--rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.2.0/hrequests/cffi.py
--rw-r--r--   0        0        0    15622 2023-07-08 00:43:33.012698 hrequests-0.2.0/hrequests/client.py
--rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.2.0/hrequests/cookies.py
--rw-r--r--   0        0        0      582 2023-07-07 01:06:44.367224 hrequests-0.2.0/hrequests/exceptions.py
--rw-r--r--   0        0        0    17489 2023-07-08 03:00:50.611004 hrequests-0.2.0/hrequests/parser.py
--rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.2.0/hrequests/playwright_mock/__init__.py
--rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.2.0/hrequests/playwright_mock/context.py
--rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.2.0/hrequests/playwright_mock/element_handle.py
--rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.2.0/hrequests/playwright_mock/faker.py
--rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.2.0/hrequests/playwright_mock/frame.py
--rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.2.0/hrequests/playwright_mock/frame_locator.py
--rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.2.0/hrequests/playwright_mock/js_handle.py
--rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.2.0/hrequests/playwright_mock/locale.json
--rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.2.0/hrequests/playwright_mock/locator.py
--rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.2.0/hrequests/playwright_mock/mouse.py
--rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.2.0/hrequests/playwright_mock/page.py
--rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.2.0/hrequests/playwright_mock/playwright_mock.py
--rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.2.0/hrequests/playwright_mock/proxy_manager.py
--rw-r--r--   0        0        0    13464 2023-07-08 02:07:11.860477 hrequests-0.2.0/hrequests/reqs.py
--rw-r--r--   0        0        0     7501 2023-07-08 02:07:11.851360 hrequests-0.2.0/hrequests/response.py
--rw-r--r--   0        0        0    11715 2023-07-08 02:54:30.797972 hrequests-0.2.0/hrequests/session.py
--rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.2.0/LICENSE
--rw-r--r--   0        0        0     1022 2023-07-08 01:14:18.341560 hrequests-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    31376 2023-07-08 03:26:00.777238 hrequests-0.2.0/README.md
--rw-r--r--   0        0        0    31848 1970-01-01 00:00:00.000000 hrequests-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.3.0/hrequests/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-09 08:44:09.084639 hrequests-0.3.0/hrequests/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.3.0/hrequests/bin/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.3.0/hrequests/bin/LICENSE.txt
+-rw-r--r--   0        0        0    23097 2023-07-08 02:07:11.879627 hrequests-0.3.0/hrequests/browser.py
+-rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.3.0/hrequests/cffi.py
+-rw-r--r--   0        0        0    15622 2023-07-08 00:43:33.012698 hrequests-0.3.0/hrequests/client.py
+-rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.3.0/hrequests/cookies.py
+-rw-r--r--   0        0        0      723 2023-07-09 08:14:06.945274 hrequests-0.3.0/hrequests/exceptions.py
+-rw-r--r--   0        0        0    19488 2023-07-09 08:47:23.150659 hrequests-0.3.0/hrequests/parser.py
+-rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.3.0/hrequests/playwright_mock/__init__.py
+-rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.3.0/hrequests/playwright_mock/context.py
+-rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.3.0/hrequests/playwright_mock/element_handle.py
+-rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.3.0/hrequests/playwright_mock/faker.py
+-rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.3.0/hrequests/playwright_mock/frame.py
+-rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.3.0/hrequests/playwright_mock/frame_locator.py
+-rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.3.0/hrequests/playwright_mock/js_handle.py
+-rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.3.0/hrequests/playwright_mock/locale.json
+-rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.3.0/hrequests/playwright_mock/locator.py
+-rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.3.0/hrequests/playwright_mock/mouse.py
+-rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.3.0/hrequests/playwright_mock/page.py
+-rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.3.0/hrequests/playwright_mock/playwright_mock.py
+-rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.3.0/hrequests/playwright_mock/proxy_manager.py
+-rw-r--r--   0        0        0    13464 2023-07-08 02:07:11.860477 hrequests-0.3.0/hrequests/reqs.py
+-rw-r--r--   0        0        0     7501 2023-07-08 02:07:11.851360 hrequests-0.3.0/hrequests/response.py
+-rw-r--r--   0        0        0    11715 2023-07-08 02:54:30.797972 hrequests-0.3.0/hrequests/session.py
+-rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1022 2023-07-09 08:44:14.453438 hrequests-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    32070 2023-07-09 08:42:09.963610 hrequests-0.3.0/README.md
+-rw-r--r--   0        0        0    32516 1970-01-01 00:00:00.000000 hrequests-0.3.0/PKG-INFO
```

### Comparing `hrequests-0.2.0/hrequests/bin/LICENSE.txt` & `hrequests-0.3.0/hrequests/bin/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/browser.py` & `hrequests-0.3.0/hrequests/browser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/cffi.py` & `hrequests-0.3.0/hrequests/cffi.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/client.py` & `hrequests-0.3.0/hrequests/client.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/cookies.py` & `hrequests-0.3.0/hrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/parser.py` & `hrequests-0.3.0/hrequests/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import contextlib
+import re
+import weakref
+from functools import partial
 from typing import List, MutableMapping, Optional, Set, Union
 from urllib.parse import urljoin, urlparse, urlunparse
 
 import lxml
 from lxml import etree
 from lxml.html import HtmlElement
 from lxml.html import tostring as lxml_html_tostring
@@ -10,14 +13,15 @@
 from lxml.html.soupparser import fromstring as soup_parse
 from parse import Result, findall
 from parse import search as parse_search
 from pyquery import PyQuery
 from w3lib.encoding import html_to_unicode
 
 import hrequests
+from hrequests.exceptions import NotRenderedException
 
 """
 Based off https://github.com/psf/requests-html/blob/master/requests_html.py
 Copyright 2018 Kenneth Reitz
 
 Used as an alternative to beautifulsoup4:
 ==== Total trials: 100000 =====
@@ -50,29 +54,61 @@
         element: The element from which to base the parsing upon.
         default_encoding: Which encoding to default to.
         html: HTML from which to base the parsing upon (optional).
         url: The URL from which the HTML originated, used for ``absolute_links``.
     """
 
     def __init__(
-        self, *, element, default_encoding: str = None, html: _HTML = None, url: str
+        self,
+        *,
+        element,
+        default_encoding: str = None,
+        html: _HTML = None,
+        url: str,
+        br_session: Optional[weakref.CallableProxyType] = None,
     ) -> None:
         self.element = element
         self.url = url
         self.skip_anchors = True
         self.default_encoding = default_encoding
         self._encoding = None
         self._html = html.encode(DEFAULT_ENCODING) if isinstance(html, str) else html
         self._lxml = None
         self._pq = None
+        self.br_session = br_session
 
         self.cleaner = Cleaner()
         self.cleaner.javascript = True
         self.cleaner.style = True
 
+    # BrowserSession methods that accept a `selector` parameter
+    pass_to_session = {
+        'awaitSelector',
+        'awaitEnabled',
+        'isVisible',
+        'isEnabled',
+        'dragTo',
+        'type',
+        'click',
+    }
+
+    def __getattr__(self, name):
+        if name not in self.pass_to_session:
+            return
+        # pass through to session if it exists
+        if self.br_session is None:
+            raise NotRenderedException(f'Method {name} only allowed in BrowserSession')
+        return partial(getattr(self.br_session, name), self.css_path)
+
+    @property
+    def css_path(self) -> str:
+        # returns css selector of the element
+        xpath = self.element.getroottree().getelementpath(self.element)
+        return re.sub(r'\[(\d+)\]', r':nth-of-type(\1)', ' > '.join(xpath.strip('/').split('/')))
+
     @property
     def raw_html(self) -> bytes:
         """
         Bytes representation of the HTML content.
         (`learn more <http://www.diveintopython3.net/strings.html>`_).
         """
         if self._html:
@@ -162,15 +198,15 @@
     def full_text(self) -> str:
         """
         The full text content (including links) of the
         :class:`Element <Element>` or :class:`HTML <HTML>`.
         """
         return self.lxml.text_content()
 
-    def find(
+    def find_all(
         self,
         selector: str = "*",
         *,
         containing: _Containing = None,
         clean: bool = False,
         first: bool = False,
         _encoding: str = None,
@@ -203,15 +239,17 @@
 
         # Convert a single containing into a list.
         if isinstance(containing, str):
             containing = [containing]
 
         encoding = _encoding or self.encoding
         elements = [
-            Element(element=found, url=self.url, default_encoding=encoding)
+            Element(
+                element=found, url=self.url, default_encoding=encoding, br_session=self.br_session
+            )
             for found in self.pq(selector)
         ]
 
         if containing:
             elements_copy = elements.copy()
             elements = [
                 element
@@ -227,14 +265,27 @@
 
             for element in elements_copy:
                 element.raw_html = lxml_html_tostring(self.cleaner.clean_html(element.lxml))
                 elements.append(element)
 
         return _get_first_or_list(elements, first)
 
+    def find(
+        self,
+        selector: str = "*",
+        *,
+        containing: _Containing = None,
+        clean: bool = False,
+        _encoding: str = None,
+    ) -> _Find:
+        # Wrapper around find_all with first=True.
+        return self.find_all(
+            selector=selector, containing=containing, clean=clean, first=True, _encoding=_encoding
+        )
+
     def xpath(
         self, selector: str, *, clean: bool = False, first: bool = False, _encoding: str = None
     ) -> _XPath:
         """
         Given an XPath selector, returns a list of Element objects or a single one.
 
         Args:
@@ -253,15 +304,18 @@
         """
         selected = self.lxml.xpath(selector)
 
         elements = [
             str(selection)
             if isinstance(selection, etree._ElementUnicodeResult)
             else Element(
-                element=selection, url=self.url, default_encoding=_encoding or self.encoding
+                element=selection,
+                url=self.url,
+                default_encoding=_encoding or self.encoding,
+                br_session=self.br_session,
             )
             for selection in selected
         ]
 
         # Sanitize the found HTML.
         if clean:
             elements_copy = elements.copy()
@@ -298,15 +352,15 @@
         return list(findall(template, self.html))
 
     @property
     def links(self) -> _Links:
         """All found links on page, in as-is form."""
 
         def gen():
-            for link in self.find('a'):
+            for link in self.find_all('a'):
                 with contextlib.suppress(KeyError):
                     href = link.attrs['href'].strip()
                     if (
                         href
                         and not (href.startswith('#') and self.skip_anchors)
                         and not href.startswith(('javascript:', 'mailto:'))
                     ):
@@ -350,15 +404,15 @@
 
     @property
     def base_url(self) -> str:
         """
         The base URL for the page. Supports the ``<base>`` tag
         (`learn more <https://www.w3schools.com/tags/tag_base.asp>`_)."""
 
-        if base := self.find('base', first=True):
+        if base := self.find_all('base', first=True):
             if result := base.attrs.get('href', '').strip():
                 return result
 
         # Parse the url to separate out the path
         parsed = urlparse(self.url)._asdict()
 
         # Remove any part of the path after the last '/'
@@ -390,16 +444,25 @@
         '_html',
         '_lxml',
         '_pq',
         '_attrs',
         'session',
     ]
 
-    def __init__(self, *, element, url: str, default_encoding: str = None) -> None:
-        super(Element, self).__init__(element=element, url=url, default_encoding=default_encoding)
+    def __init__(
+        self,
+        *,
+        element,
+        url: str,
+        default_encoding: str = None,
+        br_session: Optional[weakref.CallableProxyType] = None,
+    ) -> None:
+        super(Element, self).__init__(
+            element=element, url=url, default_encoding=default_encoding, br_session=br_session
+        )
         self.element = element
         self.tag = element.tag
         self.lineno = element.sourceline
         self._attrs = None
 
     def __repr__(self) -> str:
         attrs = [f'{attr}={repr(self.attrs[attr])}' for attr in self.attrs]
@@ -433,29 +496,34 @@
     Attributes:
         session (Union[hrequests.session.TLSSession, hrequests.browser.BrowserSession]): The session used for the HTML request.
     """
 
     def __init__(
         self,
         *,
-        session: Optional[Union[hrequests.session.TLSSession, hrequests.browser.BrowserSession]] = None,
+        session: Optional[
+            Union[hrequests.session.TLSSession, hrequests.browser.BrowserSession]
+        ] = None,
         url: str = DEFAULT_URL,
         html: _HTML,
         default_encoding: str = DEFAULT_ENCODING,
     ) -> None:
         # Convert incoming unicode HTML into bytes.
         if isinstance(html, str):
             html = html.encode(DEFAULT_ENCODING)
 
         pq = PyQuery(html)
         super(HTML, self).__init__(
             element=pq('html') or pq.wrapAll('<html></html>')('html'),
             html=html,
             url=url,
             default_encoding=default_encoding,
+            br_session=weakref.proxy(session)
+            if isinstance(session, hrequests.browser.BrowserSession)
+            else None,
         )
         self.session = session or hrequests.firefox.Session(temp=True)
         self.page = None
         self.next_symbol = DEFAULT_NEXT_SYMBOL
 
     def __repr__(self) -> str:
         return f"<HTML url={self.url!r}>"
@@ -466,15 +534,15 @@
         is ``True`` (default), returns :class:`HTML <HTML>` object of
         next page. If ``fetch`` is ``False``, simply returns the next URL.
         """
         if next_symbol is None:
             next_symbol = DEFAULT_NEXT_SYMBOL
 
         def get_next():
-            candidates = self.find('a', containing=next_symbol)
+            candidates = self.find_all('a', containing=next_symbol)
 
             for candidate in candidates:
                 if candidate.attrs.get('href'):
                     # Support 'next' rel (e.g. reddit).
                     if 'next' in candidate.attrs.get('rel', []):
                         return candidate.attrs['href']
```

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/context.py` & `hrequests-0.3.0/hrequests/playwright_mock/context.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/element_handle.py` & `hrequests-0.3.0/hrequests/playwright_mock/element_handle.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/faker.py` & `hrequests-0.3.0/hrequests/playwright_mock/faker.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/frame.py` & `hrequests-0.3.0/hrequests/playwright_mock/frame.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/frame_locator.py` & `hrequests-0.3.0/hrequests/playwright_mock/frame_locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/locale.json` & `hrequests-0.3.0/hrequests/playwright_mock/locale.json`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/locator.py` & `hrequests-0.3.0/hrequests/playwright_mock/locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/mouse.py` & `hrequests-0.3.0/hrequests/playwright_mock/mouse.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/page.py` & `hrequests-0.3.0/hrequests/playwright_mock/page.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/playwright_mock.py` & `hrequests-0.3.0/hrequests/playwright_mock/playwright_mock.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/playwright_mock/proxy_manager.py` & `hrequests-0.3.0/hrequests/playwright_mock/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/reqs.py` & `hrequests-0.3.0/hrequests/reqs.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/response.py` & `hrequests-0.3.0/hrequests/response.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/hrequests/session.py` & `hrequests-0.3.0/hrequests/session.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/LICENSE` & `hrequests-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hrequests-0.2.0/pyproject.toml` & `hrequests-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hrequests"
-version = "0.2.0"
+version = "0.3.0"
 description = "Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library."
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/daijro/hrequests"
 keywords = ["tls", "client", "http", "scraping", "requests", "humans", "playwright"]
 classifiers = [
```

### Comparing `hrequests-0.2.0/README.md` & `hrequests-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,47 +6,63 @@
 
 <h4 align="center">
 <p align="center">
     <a href="https://github.com/daijro/hrequests/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/daijro/hrequests.svg">
     </a>
     <a href="https://python.org/">
-        <img src="https://img.shields.io/badge/python-3.6&#8208;3.10-blue">
+        <img src="https://img.shields.io/badge/python-3.6&#8208;3.11-blue">
     </a>
     <a href="https://pypi.org/project/hrequests/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests.svg">
     </a>
     <a href="https://github.com/ambv/black">
         <img src="https://img.shields.io/badge/code%20style-black-black.svg">
     </a>
     <a href="https://github.com/PyCQA/isort">
         <img src="https://img.shields.io/badge/imports-isort-yellow.svg">
     </a>
 </p>
-    Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
+    Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library. 
 </h4>
 
-- TLS client fingerprinting 🚀
-- Javascript rendering 🚀
-- Human-like browsing emulation 🚀
-- Fast built-in HTML parsing 🚀
-- Asynchronous requests with gevent *(without monkey-paching!)* 🚀
-- Realistic browser header spoofing 🚀
+### ✨ Features
+
+- Seamless transition between HTTP and headless browsing 💻
+- Integrated fast HTML parser 🚀
+- High performance concurrency with gevent (*without monkey-patching!*)  🚀
+- Replication of browser TLS fingerprints 🚀
+- JavaScript rendering 🚀
 - Supports HTTP/2 🚀
-- High performance 🚀
-- 100% thread-safe 🚀
+- Realistic browser header generation 🚀
+- JSON serializing up to 10x faster than the standard library 🚀
+
+### 💻 Browser crawling
+
+- Simple & uncomplicated browser automation
+- Human-like cursor movement and typing
+- Full page screenshots
+- Headless and headful support
+- No CORS restrictions
+
+### ⚡ More
+- High performance ✨
+- Minimal dependence on the python standard libraries
+- Written with type safety
+- 100% threadsafe ❤️
 
 ---
 
 # Installation
 
 Install via pip:
 
 ```bash
 pip install hrequests
+playwright install
 ```
 
 Other depedencies will be downloaded on the first import:
 
 ```py
 >>> import hrequests
 ```
@@ -55,15 +71,15 @@
 
 # Documentation
 
 1. [Simple Usage](https://github.com/daijro/hrequests#simple-usage)
 2. [Sessions](https://github.com/daijro/hrequests#sessions)
 3. [Concurrent & Lazy Requests](https://github.com/daijro/hrequests#concurrent--lazy-requests)
 4. [HTML Parsing](https://github.com/daijro/hrequests#html-parsing)
-5. [Page Rendering](https://github.com/daijro/hrequests#page-rendering)
+5. [Browser Automation](https://github.com/daijro/hrequests#browser-automation)
 
 <hr width=50>
 
 ## Simple Usage
 
 Here is an example of a simple `get` request:
 
@@ -497,15 +513,15 @@
 ```
 
 ### Selecting elements
 
 Select an element using a CSS Selector:
 
 ```py
->>> about = resp.html.find('#about', first=True)
+>>> about = resp.html.find('#about')
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Given a CSS Selector, returns a list of
 :class:`Element <Element>` objects or a single one.
@@ -588,44 +604,56 @@
 '<li aria-haspopup="true" class="tier-1 element-1 " id="about">\n<a class="" href="/about/" title="">About</a>\n<ul aria-hidden="true" class="subnav menu" role="menu">\n<li class="tier-2 element-1" role="treeitem"><a href="/about/apps/" title="">Applications</a></li>\n<li class="tier-2 element-2" role="treeitem"><a href="/about/quotes/" title="">Quotes</a></li>\n<li class="tier-2 element-3" role="treeitem"><a href="/about/gettingstarted/" title="">Getting Started</a></li>\n<li class="tier-2 element-4" role="treeitem"><a href="/about/help/" title="">Help</a></li>\n<li class="tier-2 element-5" role="treeitem"><a href="http://brochure.getpython.info/" title="">Python Brochure</a></li>\n</ul>\n</li>'
 ```
 
 
 Select Elements within Elements:
 
 ```py
->>> about.find('a')
+>>> about.find_all('a')
 [<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>, <Element 'a' href='/about/quotes/' title=''>, <Element 'a' href='/about/gettingstarted/' title=''>, <Element 'a' href='/about/help/' title=''>, <Element 'a' href='http://brochure.getpython.info/' title=''>]
+>>> about.find('a')
+<Element 'a' href='/about/' title='' class=''>
 ```
 
 Search for links within an element:
 
 ```py
 >>> about.absolute_links
 {'http://brochure.getpython.info/', 'https://www.python.org/about/gettingstarted/', 'https://www.python.org/about/', 'https://www.python.org/about/quotes/', 'https://www.python.org/about/help/', 'https://www.python.org/about/apps/'}
 ```
 
 
 <hr width=50>
 
-## Page Rendering
+## Browser Automation
 
-The `.render()` method returns a `BrowserSession` object. This will render the contents of the request in a browser. Once the context manager is exited, the browser will close and the session data will be updated.
 
-Although the backend uses Playwright, `BrowserSession` is still entirely safe to use across threads.
+You can spawn a `BrowserSession` instance by calling it:
 
-**Example - submitting a login form:**
+```py
+>>> page = hrequests.BrowserSession()  # headless=True by default
+```
+
+`BrowserSession` is entirely safe to use across threads.
+
+### Render an existing Response
 
+Responses have a `.render()` method. This will render the contents of the response in a browser page.
+
+Once the page is closed, the Response content and the Response's session cookies will be updated.
+
+**Example - submitting a login form:**
 
 ```py
 >>> resp = session.get('https://www.somewebsite.com/')
 >>> with resp.render(mock_human=True) as page:
 ...     page.type('.input#username', 'myuser')
 ...     page.type('.input#password', 'p4ssw0rd')
 ...     page.click('#submit')
-# session & resp now have updated cookies, content, etc.
+# `session` & `resp` now have updated cookies, content, etc.
 ```
 
 <details>
 
 <summary><strong>Or, without a context manager</strong></summary>
 
 ```py
@@ -635,28 +663,27 @@
 >>> page.type('.input#password', 'p4ssw0rd')
 >>> page.click('#submit')
 >>> page.close()  # must close the page when done!
 ```
 
 </details>
 
+The `mock_human` parameter will emulate human-like behavior. This includes easing and randomizing mouse movements, and randomizing typing speed. This functionality is based on [botright](https://github.com/Vinyzu/botright/).
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
     mock_human (bool, optional): Whether to emulate human behavior. Defaults to False.
     allow_styling (bool, optional): Allow loading images, fonts, styles, etc. Defaults to True
 ```
 </details>
 
-The `mock_human` parameter will emulate human-like behavior. This includes easing mouse movements, randomizing typing speed, and randomizing mouse movements. This functionality is based on [botright](https://github.com/Vinyzu/botright/).
-
 ### Properties
 
 Cookies are inherited from the session:
 
 ```py
 >>> page.cookies: RequestsCookieJar  # cookies are inherited from the session
 <RequestsCookieJar[Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None, port_specified=False, domain='.somewebsite.com', domain_specified=True...
@@ -685,16 +712,18 @@
 >>> page.content: bytes
 b'<!doctype html><html itemscope="" itemtype="http://schema.org/WebPage" lang="en"><head><meta content="Search the world\'s information, including webpag'
 ```
 
 Parsing HTML from the page content:
 
 ```py
->>> page.html.find('a')
+>>> page.html.find_all('a')
 [<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>, ...]
+>>> page.html.find('a')
+<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>
 ```
 
 Take a screenshot of the page:
 ```py
 page.screenshot('screenshot.png')
 ```
 <details>
@@ -723,14 +752,16 @@
 >>> page.forward()
 ```
 
 ### Controlling elements
 Click an element:
 ```py
 >>> page.click('#my-button')
+# or through the html parser
+>>> page.html.find('#my-button').click()
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     selector (str): CSS selector to click.
@@ -740,14 +771,16 @@
     wait_after (bool, optional): Wait for a page event before continuing. Defaults to True.
 ```
 </details>
 
 Type text into an element:
 ```py
 >>> page.type('#my-input', 'Hello world!')
+# or through the html parser
+>>> page.html.find('#my-input').type('Hello world!')
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     selector (str): CSS selector to type in
@@ -756,14 +789,16 @@
     timeout (float, optional): Timeout in seconds. Defaults to 30.
 ```
 </details>
 
 Drag and drop an element:
 ```py
 >>> page.dragTo('#source-selector', '#target-selector')
+# or through the html parser
+>>> page.html.find('#source-selector').dragTo('#target-selector')
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     source (str): Source to drag from
@@ -955,31 +990,22 @@
 'https://www.bing.com/?toWww=1&redig=823778234657823652376438'
 >>> resp.content: Union[bytes, str]
 '<!DOCTYPE html><html lang="en" dir="ltr"><head><meta name="theme-color" content="#4F4F4F"><meta name="description" content="Bing helps you turn inform...
 ```
 
 #### Other ways to create a Browser Session
 
-If you don't want to use the data from an existing response, you can also create a `BrowserSession` object directly from a `Session`:
+You can use `.render` to spawn a `BrowserSession` object directly from a url:
 
 ```py
->>> # render a url using cookies and headers from a session object:
->>> page1 = session.render('https://google.com')
-```
-
-Or without a session at all:
-```py
->>> # render a url without a session:
->>> page2 = hrequests.render('https://google.com')
->>> # or just call BrowserSession directly:
->>> page3 = hrequests.BrowserSession()
->>> page3.url = 'https://google.com'
+# Using a Session:
+>>> page = session.render('https://google.com')
+# Or without a session at all:
+>>> page = hrequests.render('https://google.com')
 ```
 
 Make sure to close all `BrowserSession` objects when done!
 ```py
->>> page1.close()
->>> page2.close()
->>> page3.close()
+>>> page.close()
 ```
 
 ---
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_hed4raw9_/tmp6ot8o4eg_TarContainer/0/28.md", line 985, column 3: CDATA terminal not found*

 * *File "/tmp/diffoscope_hed4raw9_/tmp6ot8o4eg_TarContainer/0/28.md", line 985, column 3: CDATA terminal not found*

```diff
@@ -1,26 +1,32 @@
 [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-       img.shields.io/badge/python-3.6&#8208;3.10-blue] [PyPI] [https://
+       img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [https://
   img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
     badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
  configurable, feature-rich, replacement for the Python requests library. ***
-- TLS client fingerprinting ð - Javascript rendering ð - Human-like
-browsing emulation ð - Fast built-in HTML parsing ð - Asynchronous
-requests with gevent *(without monkey-paching!)* ð - Realistic browser
-header spoofing ð - Supports HTTP/2 ð - High performance ð - 100%
-thread-safe ð --- # Installation Install via pip: ```bash pip install
-hrequests ``` Other depedencies will be downloaded on the first import: ```py
->>> import hrequests ``` --- # Documentation 1. [Simple Usage](https://
-github.com/daijro/hrequests#simple-usage) 2. [Sessions](https://github.com/
-daijro/hrequests#sessions) 3. [Concurrent & Lazy Requests](https://github.com/
-daijro/hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://
-github.com/daijro/hrequests#html-parsing) 5. [Page Rendering](https://
-github.com/daijro/hrequests#page-rendering)
+### â¨ Features - Seamless transition between HTTP and headless browsing ð»
+- Integrated fast HTML parser ð - High performance concurrency with gevent
+(*without monkey-patching!*) ð - Replication of browser TLS fingerprints
+ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
+header generation ð - JSON serializing up to 10x faster than the standard
+library ð ### ð» Browser crawling - Simple & uncomplicated browser
+automation - Human-like cursor movement and typing - Full page screenshots -
+Headless and headful support - No CORS restrictions ### â¡ More - High
+performance â¨ - Minimal dependence on the python standard libraries - Written
+with type safety - 100% threadsafe â¤ï¸ --- # Installation Install via pip:
+```bash pip install hrequests playwright install ``` Other depedencies will be
+downloaded on the first import: ```py >>> import hrequests ``` --- #
+Documentation 1. [Simple Usage](https://github.com/daijro/hrequests#simple-
+usage) 2. [Sessions](https://github.com/daijro/hrequests#sessions) 3.
+[Concurrent & Lazy Requests](https://github.com/daijro/hrequests#concurrent--
+lazy-requests) 4. [HTML Parsing](https://github.com/daijro/hrequests#html-
+parsing) 5. [Browser Automation](https://github.com/daijro/hrequests#browser-
+automation)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
@@ -208,11 +214,11 @@
 apps/', 'https://github.com/python/pythondotorg/issues', '/accounts/login/', '/
 dev/peps/', '/about/legal/',... ``` Grab a list of all links on the page, in
 absolute form (anchors excluded): ```py >>> resp.html.absolute_links {'https://
 github.com/python/pythondotorg/issues', 'https://docs.python.org/3/tutorial/',
 'https://www.python.org/about/success/', 'http://feedproxy.g... ``` Search for
 text on the page: ```py >>> resp.html.search('Python is a {} language')[0]
 programming ``` ### Selecting elements Select an element using a CSS Selector:
-```py >>> about = resp.html.find('#about', first=True) ```  Parameters ```
-Given a CSS Selector, returns a list of :class:`Element ` objects or a single
-one. Parameters: selector: CSS Selector to use. clean: Whether or not to
-sanitize the found HTML of ``
+```py >>> about = resp.html.find('#about') ```  Parameters ``` Given a CSS
+Selector, returns a list of :class:`Element ` objects or a single one.
+Parameters: selector: CSS Selector to use. clean: Whether or not to sanitize
+the found HTML of ``
```

### Comparing `hrequests-0.2.0/PKG-INFO` & `hrequests-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrequests
-Version: 0.2.0
+Version: 0.3.0
 Summary: Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 Home-page: https://github.com/daijro/hrequests
 License: Apache-2.0
 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -45,47 +45,63 @@
 
 <h4 align="center">
 <p align="center">
     <a href="https://github.com/daijro/hrequests/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/daijro/hrequests.svg">
     </a>
     <a href="https://python.org/">
-        <img src="https://img.shields.io/badge/python-3.6&#8208;3.10-blue">
+        <img src="https://img.shields.io/badge/python-3.6&#8208;3.11-blue">
     </a>
     <a href="https://pypi.org/project/hrequests/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests.svg">
     </a>
     <a href="https://github.com/ambv/black">
         <img src="https://img.shields.io/badge/code%20style-black-black.svg">
     </a>
     <a href="https://github.com/PyCQA/isort">
         <img src="https://img.shields.io/badge/imports-isort-yellow.svg">
     </a>
 </p>
-    Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
+    Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library. 
 </h4>
 
-- TLS client fingerprinting 🚀
-- Javascript rendering 🚀
-- Human-like browsing emulation 🚀
-- Fast built-in HTML parsing 🚀
-- Asynchronous requests with gevent *(without monkey-paching!)* 🚀
-- Realistic browser header spoofing 🚀
+### ✨ Features
+
+- Seamless transition between HTTP and headless browsing 💻
+- Integrated fast HTML parser 🚀
+- High performance concurrency with gevent (*without monkey-patching!*)  🚀
+- Replication of browser TLS fingerprints 🚀
+- JavaScript rendering 🚀
 - Supports HTTP/2 🚀
-- High performance 🚀
-- 100% thread-safe 🚀
+- Realistic browser header generation 🚀
+- JSON serializing up to 10x faster than the standard library 🚀
+
+### 💻 Browser crawling
+
+- Simple & uncomplicated browser automation
+- Human-like cursor movement and typing
+- Full page screenshots
+- Headless and headful support
+- No CORS restrictions
+
+### ⚡ More
+- High performance ✨
+- Minimal dependence on the python standard libraries
+- Written with type safety
+- 100% threadsafe ❤️
 
 ---
 
 # Installation
 
 Install via pip:
 
 ```bash
 pip install hrequests
+playwright install
 ```
 
 Other depedencies will be downloaded on the first import:
 
 ```py
 >>> import hrequests
 ```
@@ -94,15 +110,15 @@
 
 # Documentation
 
 1. [Simple Usage](https://github.com/daijro/hrequests#simple-usage)
 2. [Sessions](https://github.com/daijro/hrequests#sessions)
 3. [Concurrent & Lazy Requests](https://github.com/daijro/hrequests#concurrent--lazy-requests)
 4. [HTML Parsing](https://github.com/daijro/hrequests#html-parsing)
-5. [Page Rendering](https://github.com/daijro/hrequests#page-rendering)
+5. [Browser Automation](https://github.com/daijro/hrequests#browser-automation)
 
 <hr width=50>
 
 ## Simple Usage
 
 Here is an example of a simple `get` request:
 
@@ -536,15 +552,15 @@
 ```
 
 ### Selecting elements
 
 Select an element using a CSS Selector:
 
 ```py
->>> about = resp.html.find('#about', first=True)
+>>> about = resp.html.find('#about')
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Given a CSS Selector, returns a list of
 :class:`Element <Element>` objects or a single one.
@@ -627,44 +643,56 @@
 '<li aria-haspopup="true" class="tier-1 element-1 " id="about">\n<a class="" href="/about/" title="">About</a>\n<ul aria-hidden="true" class="subnav menu" role="menu">\n<li class="tier-2 element-1" role="treeitem"><a href="/about/apps/" title="">Applications</a></li>\n<li class="tier-2 element-2" role="treeitem"><a href="/about/quotes/" title="">Quotes</a></li>\n<li class="tier-2 element-3" role="treeitem"><a href="/about/gettingstarted/" title="">Getting Started</a></li>\n<li class="tier-2 element-4" role="treeitem"><a href="/about/help/" title="">Help</a></li>\n<li class="tier-2 element-5" role="treeitem"><a href="http://brochure.getpython.info/" title="">Python Brochure</a></li>\n</ul>\n</li>'
 ```
 
 
 Select Elements within Elements:
 
 ```py
->>> about.find('a')
+>>> about.find_all('a')
 [<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>, <Element 'a' href='/about/quotes/' title=''>, <Element 'a' href='/about/gettingstarted/' title=''>, <Element 'a' href='/about/help/' title=''>, <Element 'a' href='http://brochure.getpython.info/' title=''>]
+>>> about.find('a')
+<Element 'a' href='/about/' title='' class=''>
 ```
 
 Search for links within an element:
 
 ```py
 >>> about.absolute_links
 {'http://brochure.getpython.info/', 'https://www.python.org/about/gettingstarted/', 'https://www.python.org/about/', 'https://www.python.org/about/quotes/', 'https://www.python.org/about/help/', 'https://www.python.org/about/apps/'}
 ```
 
 
 <hr width=50>
 
-## Page Rendering
+## Browser Automation
 
-The `.render()` method returns a `BrowserSession` object. This will render the contents of the request in a browser. Once the context manager is exited, the browser will close and the session data will be updated.
 
-Although the backend uses Playwright, `BrowserSession` is still entirely safe to use across threads.
+You can spawn a `BrowserSession` instance by calling it:
 
-**Example - submitting a login form:**
+```py
+>>> page = hrequests.BrowserSession()  # headless=True by default
+```
+
+`BrowserSession` is entirely safe to use across threads.
+
+### Render an existing Response
 
+Responses have a `.render()` method. This will render the contents of the response in a browser page.
+
+Once the page is closed, the Response content and the Response's session cookies will be updated.
+
+**Example - submitting a login form:**
 
 ```py
 >>> resp = session.get('https://www.somewebsite.com/')
 >>> with resp.render(mock_human=True) as page:
 ...     page.type('.input#username', 'myuser')
 ...     page.type('.input#password', 'p4ssw0rd')
 ...     page.click('#submit')
-# session & resp now have updated cookies, content, etc.
+# `session` & `resp` now have updated cookies, content, etc.
 ```
 
 <details>
 
 <summary><strong>Or, without a context manager</strong></summary>
 
 ```py
@@ -674,28 +702,27 @@
 >>> page.type('.input#password', 'p4ssw0rd')
 >>> page.click('#submit')
 >>> page.close()  # must close the page when done!
 ```
 
 </details>
 
+The `mock_human` parameter will emulate human-like behavior. This includes easing and randomizing mouse movements, and randomizing typing speed. This functionality is based on [botright](https://github.com/Vinyzu/botright/).
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
     mock_human (bool, optional): Whether to emulate human behavior. Defaults to False.
     allow_styling (bool, optional): Allow loading images, fonts, styles, etc. Defaults to True
 ```
 </details>
 
-The `mock_human` parameter will emulate human-like behavior. This includes easing mouse movements, randomizing typing speed, and randomizing mouse movements. This functionality is based on [botright](https://github.com/Vinyzu/botright/).
-
 ### Properties
 
 Cookies are inherited from the session:
 
 ```py
 >>> page.cookies: RequestsCookieJar  # cookies are inherited from the session
 <RequestsCookieJar[Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None, port_specified=False, domain='.somewebsite.com', domain_specified=True...
@@ -724,16 +751,18 @@
 >>> page.content: bytes
 b'<!doctype html><html itemscope="" itemtype="http://schema.org/WebPage" lang="en"><head><meta content="Search the world\'s information, including webpag'
 ```
 
 Parsing HTML from the page content:
 
 ```py
->>> page.html.find('a')
+>>> page.html.find_all('a')
 [<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>, ...]
+>>> page.html.find('a')
+<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>
 ```
 
 Take a screenshot of the page:
 ```py
 page.screenshot('screenshot.png')
 ```
 <details>
@@ -762,14 +791,16 @@
 >>> page.forward()
 ```
 
 ### Controlling elements
 Click an element:
 ```py
 >>> page.click('#my-button')
+# or through the html parser
+>>> page.html.find('#my-button').click()
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     selector (str): CSS selector to click.
@@ -779,14 +810,16 @@
     wait_after (bool, optional): Wait for a page event before continuing. Defaults to True.
 ```
 </details>
 
 Type text into an element:
 ```py
 >>> page.type('#my-input', 'Hello world!')
+# or through the html parser
+>>> page.html.find('#my-input').type('Hello world!')
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     selector (str): CSS selector to type in
@@ -795,14 +828,16 @@
     timeout (float, optional): Timeout in seconds. Defaults to 30.
 ```
 </details>
 
 Drag and drop an element:
 ```py
 >>> page.dragTo('#source-selector', '#target-selector')
+# or through the html parser
+>>> page.html.find('#source-selector').dragTo('#target-selector')
 ```
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     source (str): Source to drag from
@@ -994,31 +1029,22 @@
 'https://www.bing.com/?toWww=1&redig=823778234657823652376438'
 >>> resp.content: Union[bytes, str]
 '<!DOCTYPE html><html lang="en" dir="ltr"><head><meta name="theme-color" content="#4F4F4F"><meta name="description" content="Bing helps you turn inform...
 ```
 
 #### Other ways to create a Browser Session
 
-If you don't want to use the data from an existing response, you can also create a `BrowserSession` object directly from a `Session`:
+You can use `.render` to spawn a `BrowserSession` object directly from a url:
 
 ```py
->>> # render a url using cookies and headers from a session object:
->>> page1 = session.render('https://google.com')
-```
-
-Or without a session at all:
-```py
->>> # render a url without a session:
->>> page2 = hrequests.render('https://google.com')
->>> # or just call BrowserSession directly:
->>> page3 = hrequests.BrowserSession()
->>> page3.url = 'https://google.com'
+# Using a Session:
+>>> page = session.render('https://google.com')
+# Or without a session at all:
+>>> page = hrequests.render('https://google.com')
 ```
 
 Make sure to close all `BrowserSession` objects when done!
 ```py
->>> page1.close()
->>> page2.close()
->>> page3.close()
+>>> page.close()
 ```
 
 ---
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_hed4raw9_/tmp6ot8o4eg_TarContainer/0/29", line 1025, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_hed4raw9_/tmp6ot8o4eg_TarContainer/0/29", line 1025, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hrequests Version: 0.2.0 Summary: Hrequests (human
+Metadata-Version: 2.1 Name: hrequests Version: 0.3.0 Summary: Hrequests (human
 requests) is a simple, configurable, feature-rich, replacement for the Python
 requests library. Home-page: https://github.com/daijro/hrequests License:
 Apache-2.0 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -16,30 +16,36 @@
 runtime ; sys_platform == "win32" Requires-Dist: numpy Requires-Dist: orjson
 Requires-Dist: parse Requires-Dist: playwright Requires-Dist: playwright-
 stealth Requires-Dist: pyquery Requires-Dist: w3lib Requires-Dist: wget
 Project-URL: Repository, https://github.com/daijro/hrequests Description-
 Content-Type: text/markdown [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-       img.shields.io/badge/python-3.6&#8208;3.10-blue] [PyPI] [https://
+       img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [https://
   img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
     badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
  configurable, feature-rich, replacement for the Python requests library. ***
-- TLS client fingerprinting ð - Javascript rendering ð - Human-like
-browsing emulation ð - Fast built-in HTML parsing ð - Asynchronous
-requests with gevent *(without monkey-paching!)* ð - Realistic browser
-header spoofing ð - Supports HTTP/2 ð - High performance ð - 100%
-thread-safe ð --- # Installation Install via pip: ```bash pip install
-hrequests ``` Other depedencies will be downloaded on the first import: ```py
->>> import hrequests ``` --- # Documentation 1. [Simple Usage](https://
-github.com/daijro/hrequests#simple-usage) 2. [Sessions](https://github.com/
-daijro/hrequests#sessions) 3. [Concurrent & Lazy Requests](https://github.com/
-daijro/hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://
-github.com/daijro/hrequests#html-parsing) 5. [Page Rendering](https://
-github.com/daijro/hrequests#page-rendering)
+### â¨ Features - Seamless transition between HTTP and headless browsing ð»
+- Integrated fast HTML parser ð - High performance concurrency with gevent
+(*without monkey-patching!*) ð - Replication of browser TLS fingerprints
+ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
+header generation ð - JSON serializing up to 10x faster than the standard
+library ð ### ð» Browser crawling - Simple & uncomplicated browser
+automation - Human-like cursor movement and typing - Full page screenshots -
+Headless and headful support - No CORS restrictions ### â¡ More - High
+performance â¨ - Minimal dependence on the python standard libraries - Written
+with type safety - 100% threadsafe â¤ï¸ --- # Installation Install via pip:
+```bash pip install hrequests playwright install ``` Other depedencies will be
+downloaded on the first import: ```py >>> import hrequests ``` --- #
+Documentation 1. [Simple Usage](https://github.com/daijro/hrequests#simple-
+usage) 2. [Sessions](https://github.com/daijro/hrequests#sessions) 3.
+[Concurrent & Lazy Requests](https://github.com/daijro/hrequests#concurrent--
+lazy-requests) 4. [HTML Parsing](https://github.com/daijro/hrequests#html-
+parsing) 5. [Browser Automation](https://github.com/daijro/hrequests#browser-
+automation)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
@@ -227,11 +233,11 @@
 apps/', 'https://github.com/python/pythondotorg/issues', '/accounts/login/', '/
 dev/peps/', '/about/legal/',... ``` Grab a list of all links on the page, in
 absolute form (anchors excluded): ```py >>> resp.html.absolute_links {'https://
 github.com/python/pythondotorg/issues', 'https://docs.python.org/3/tutorial/',
 'https://www.python.org/about/success/', 'http://feedproxy.g... ``` Search for
 text on the page: ```py >>> resp.html.search('Python is a {} language')[0]
 programming ``` ### Selecting elements Select an element using a CSS Selector:
-```py >>> about = resp.html.find('#about', first=True) ```  Parameters ```
-Given a CSS Selector, returns a list of :class:`Element ` objects or a single
-one. Parameters: selector: CSS Selector to use. clean: Whether or not to
-sanitize the found HTML of ``
+```py >>> about = resp.html.find('#about') ```  Parameters ``` Given a CSS
+Selector, returns a list of :class:`Element ` objects or a single one.
+Parameters: selector: CSS Selector to use. clean: Whether or not to sanitize
+the found HTML of ``
```

