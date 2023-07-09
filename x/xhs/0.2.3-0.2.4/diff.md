# Comparing `tmp/xhs-0.2.3.tar.gz` & `tmp/xhs-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.2.3.tar", last modified: Thu Jun 22 02:45:57 2023, max compression
+gzip compressed data, was "xhs-0.2.4.tar", last modified: Sun Jul  9 09:34:15 2023, max compression
```

## Comparing `xhs-0.2.3.tar` & `xhs-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.478889 xhs-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-22 02:45:44.000000 xhs-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-22 02:45:44.000000 xhs-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 02:45:44.000000 xhs-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-22 02:45:57.478889 xhs-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-22 02:45:44.000000 xhs-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 02:45:44.000000 xhs-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 02:45:57.478889 xhs-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-22 02:45:44.000000 xhs-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.474889 xhs-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.478889 xhs-0.2.3/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.478889 xhs-0.2.3/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:34:15.636571 xhs-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-09 09:34:02.000000 xhs-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 09:34:02.000000 xhs-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-09 09:34:02.000000 xhs-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-09 09:34:15.636571 xhs-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-09 09:34:02.000000 xhs-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 09:34:02.000000 xhs-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-09 09:34:15.636571 xhs-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-09 09:34:02.000000 xhs-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:34:15.636571 xhs-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-09 09:34:02.000000 xhs-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-09 09:34:02.000000 xhs-0.2.4/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-07-09 09:34:02.000000 xhs-0.2.4/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 09:34:02.000000 xhs-0.2.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:34:15.636571 xhs-0.2.4/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-09 09:34:02.000000 xhs-0.2.4/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-09 09:34:02.000000 xhs-0.2.4/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-07-09 09:34:02.000000 xhs-0.2.4/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-09 09:34:02.000000 xhs-0.2.4/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-09 09:34:02.000000 xhs-0.2.4/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:34:15.636571 xhs-0.2.4/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-09 09:34:15.000000 xhs-0.2.4/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-09 09:34:15.000000 xhs-0.2.4/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:34:15.000000 xhs-0.2.4/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:34:15.000000 xhs-0.2.4/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 09:34:15.000000 xhs-0.2.4/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 09:34:15.000000 xhs-0.2.4/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.2.3/CHANGELOG.md` & `xhs-0.2.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.2.4
+
+### Added
+
+- add create note api
+
+### Fixed
+
+- fix cookie key with white space error
+
 ## 0.2.3
 
 ### Added
 
 - add get self info v2 api
 - add get home feed categories api
```

### Comparing `xhs-0.2.3/LICENSE` & `xhs-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.2.3/PKG-INFO` & `xhs-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.2.3
+Version: 0.2.4
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xhs-0.2.3/README.md` & `xhs-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `xhs-0.2.3/setup.py` & `xhs-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.3/tests/test_help.py` & `xhs-0.2.4/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.3/tests/test_xhs.py` & `xhs-0.2.4/tests/test_xhs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from time import sleep
 
 import pytest
 from playwright.sync_api import sync_playwright
 
 from xhs import FeedType, IPBlockError, XhsClient
-from xhs.exception import SignError
+from xhs.exception import SignError, DataFetchError
 from . import test_cookie
 from .utils import beauty_print
 
 
 def get_context_page(playwright):
     chromium = playwright.chromium
     browser = chromium.launch(headless=True)
     browser_context = browser.new_context(
         viewport={"width": 1920, "height": 1080},
         user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
     )
-    browser_context.add_init_script(path="stealth.min.js")
+    browser_context.add_init_script(path="/Users/reajason/ReaJason/xhs/tests/stealth.min.js")
     context_page = browser_context.new_page()
     return browser_context, context_page
 
 
 playwright = sync_playwright().start()
 browser_context, context_page = get_context_page(playwright)
 
@@ -268,7 +268,53 @@
     assert info["session"]
 
 
 def test_get_emojis(xhs_client: XhsClient):
     emojis = xhs_client.get_emojis()
     beauty_print(emojis)
     assert len(emojis)
+
+
+def test_get_upload_image_ids(xhs_client: XhsClient):
+    count = 5
+    ids = xhs_client.get_upload_image_ids(count)
+    beauty_print(ids)
+    assert len(ids[0]["fileIds"]) == count
+
+
+def test_upload_image(xhs_client: XhsClient):
+    ids = xhs_client.get_upload_image_ids(1)
+    file_info = ids[0]
+    file_id = file_info["fileIds"][0]
+    file_token = file_info["token"]
+    file_path = "/Users/reajason/Downloads/4538306CF3BDC215721FCC0532AF4D3D.jpg"
+    res = xhs_client.upload_image(file_id, file_token, file_path)
+    assert res.status_code == 200
+    print(res.headers["X-Ros-Preview-Url"])
+
+    with pytest.raises(DataFetchError, match="file already exists"):
+        xhs_client.upload_image(file_id, file_token, file_path)
+
+
+def test_get_suggest_topic(xhs_client: XhsClient):
+    topic_keyword = "Python"
+    topics = xhs_client.get_suggest_topic(topic_keyword)
+    beauty_print(topics)
+    assert topic_keyword.upper() in topics[0]["name"].upper()
+
+
+def test_get_suggest_ats(xhs_client: XhsClient):
+    ats_keyword = "ReaJason"
+    ats = xhs_client.get_suggest_ats(ats_keyword)
+    beauty_print(ats)
+    assert ats_keyword.upper() in ats[0]["user_base_dto"]["user_nickname"].upper()
+
+
+def test_create_note_with_simple_desc(xhs_client: XhsClient):
+    title = "我是通过自动发布脚本发送的笔记"
+    desc = "deployed by GitHub xhs"
+    files = [
+        "/Users/reajason/Downloads/221686462282_.pic.png",
+        "/Users/reajason/Downloads/221686462282_.pic.jpg",
+    ]
+    note = xhs_client.create_note(title, desc, files)
+    beauty_print(note)
```

### Comparing `xhs-0.2.3/xhs/core.py` & `xhs-0.2.4/xhs/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,49 +133,51 @@
     def user_agent(self):
         return self.__session.headers.get("user-agent")
 
     @user_agent.setter
     def user_agent(self, user_agent: str):
         self.__session.headers.update({"user-agent": user_agent})
 
-    def _pre_headers(self, url: str, data=None):
-        if self.sign:
-            self.__session.headers.update(
-                self.sign(url, data, a1=self.cookie_dict.get("a1"),
-                          web_session=self.cookie_dict.get("web_session")))
-        else:
+    def _pre_headers(self, url: str, data=None, is_creator: bool = False):
+        if is_creator:
             signs = sign(url, data, a1=self.cookie_dict.get("a1"))
             self.__session.headers.update({"x-s": signs["x-s"]})
             self.__session.headers.update({"x-t": signs["x-t"]})
             self.__session.headers.update({"x-s-common": signs["x-s-common"]})
+        else:
+            self.__session.headers.update(
+                self.sign(url, data, a1=self.cookie_dict.get("a1"),
+                          web_session=self.cookie_dict.get("web_session")))
 
     def request(self, method, url, **kwargs):
         response = self.__session.request(
             method, url, timeout=self.timeout,
             proxies=self.proxies, **kwargs)
+        if not len(response.text):
+            return response
         data = response.json()
-        if data["success"]:
+        if data.get("success"):
             return data.get("data", data.get("success"))
         elif data["code"] == ErrorEnum.IP_BLOCK.value.code:
             raise IPBlockError(ErrorEnum.IP_BLOCK.value.msg)
         elif data["code"] == ErrorEnum.SIGN_FAULT.value.code:
             raise SignError(ErrorEnum.SIGN_FAULT.value.msg)
         else:
-            raise DataFetchError(data.get("msg", None))
+            raise DataFetchError(data.get("msg", data))
 
-    def get(self, uri: str, params=None):
+    def get(self, uri: str, params=None, is_creator: bool = False):
         final_uri = uri
         if isinstance(params, dict):
             final_uri = (f"{uri}?"
-                         f"{'&'.join([f'{k}={v}'for k,v in params.items()])}")
-        self._pre_headers(final_uri)
+                         f"{'&'.join([f'{k}={v}' for k, v in params.items()])}")
+        self._pre_headers(final_uri, is_creator=is_creator)
         return self.request(method="GET", url=f"{self._host}{final_uri}")
 
-    def post(self, uri: str, data: dict):
-        self._pre_headers(uri, data)
+    def post(self, uri: str, data: dict, is_creator: bool = False):
+        self._pre_headers(uri, data, is_creator=is_creator)
         json_str = json.dumps(data, separators=(',', ':'), ensure_ascii=False)
         return self.request(method="POST", url=f"{self._host}{uri}",
                             data=json_str.encode("utf-8"))
 
     def get_note_by_id(self, note_id: str):
         """
         :param note_id: note_id you want to fetch
@@ -222,15 +224,16 @@
         if state != "{}":
             new_dict = transform_json_keys(state)
             return new_dict["note"]["note"]
         elif self.IP_ERROR_STR in html:
             raise IPBlockError(self.IP_ERROR_STR)
         raise DataFetchError()
 
-    def report_note_metrics(self, note_id: str, note_type: int, note_user_id: str, viewer_user_id: str, followed_author=0, report_type=1, stay_seconds=0):
+    def report_note_metrics(self, note_id: str, note_type: int, note_user_id: str, viewer_user_id: str,
+                            followed_author=0, report_type=1, stay_seconds=0):
         """report note stay seconds and other interaction info
 
         :param note_id: note_id which you want to report
         :type note_id: str
         :param note_type: input value -> 1: note is images, 2: note is video
         :type note_type: int
         :param note_user_id: note author id
@@ -642,7 +645,70 @@
             "cursor": cursor
         }
         return self.get(uri, params)
 
     def get_emojis(self):
         uri = "/api/im/redmoji/detail"
         return self.get(uri)["emoji"]["tabs"][0]["collection"]
+
+    def get_upload_image_ids(self, count):
+        uri = "/api/media/v1/upload/web/permit"
+        params = {
+            "biz_name": "spectrum",
+            "scene": "image",
+            "file_count": count,
+            "version": "1",
+            "source": "web",
+        }
+        return self.get(uri, params)["uploadTempPermits"]
+
+    def upload_image(self, image_id: str, token: str, file_path: str):
+        url = "https://ros-upload.xiaohongshu.com/" + image_id
+        headers = {
+            "X-Cos-Security-Token": token,
+            "Content-Type": "image/jpeg"
+        }
+        with open(file_path, "rb") as f:
+            return self.request("PUT", url, data=f, headers=headers)
+
+    def get_suggest_topic(self, keyword=""):
+        uri = "/web_api/sns/v1/search/topic"
+        data = {"keyword": keyword,
+                "suggest_topic_request": {"title": "", "desc": ""},
+                "page": {"page_size": 20, "page": 1}
+                }
+        return self.post(uri, data)["topic_info_dtos"]
+
+    def get_suggest_ats(self, keyword=""):
+        uri = "/web_api/sns/v1/search/user_info"
+        data = {"keyword": keyword, "search_id": str(time.time() * 1000), "page": {"page_size": 20, "page": 1}}
+        return self.post(uri, data)["user_info_dtos"]
+
+    def create_note(self, title, desc, files: list, ats: list = None, topics: list = None, is_private: bool = False):
+        if ats is None:
+            ats = []
+        if topics is None:
+            topics = []
+
+        image_info = []
+        for file in files:
+            images_ids_res = self.get_upload_image_ids(1)
+            image_id = images_ids_res[0]["fileIds"][0]
+            token = images_ids_res[0]["token"]
+            res = self.upload_image(image_id, token, file)
+            # print(res.headers["X-Ros-Preview-Url"])
+            image_info.append({
+                "file_id": image_id,
+                "width": 1003,
+                "height": 1000,
+                "metadata": {"source": -1}, "stickers": {"version": 2, "floating": []},
+                "extra_info_json": "{\"mimeType\":\"image/jpeg\"}"
+            })
+
+        uri = "/web_api/sns/v2/note"
+        data = {"common": {"type": "normal", "title": title, "note_id": "", "desc": desc,
+                           "source": "{\"type\":\"web\",\"ids\":\"\",\"extraInfo\":\"{\\\"subType\\\":\\\"official\\\"}\"}",
+                           "business_binds": "{\"version\":1,\"noteId\":0,\"bizType\":0,\"noteOrderBind\":{},\"notePostTiming\":{\"postTime\":\"\"},\"noteCollectionBind\":{\"id\":\"\"}}",
+                           "ats": ats, "hash_tag": topics, "post_loc": {},
+                           "privacy_info": {"op_type": 1, "type": int(is_private)}},
+                "image_info": {"images": image_info}, "video_info": None}
+        return self.post(uri, data)
```

### Comparing `xhs-0.2.3/xhs/exception.py` & `xhs-0.2.4/xhs/exception.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.3/xhs/help.py` & `xhs-0.2.4/xhs/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 import requests
 
 
 def sign(uri, data=None, ctime=None, a1="", b1=""):
     """
     takes in a URI (uniform resource identifier), an optional data dictionary, and an optional ctime parameter. It returns a dictionary containing two keys: "x-s" and "x-t".
     """
+
     def h(n):
         m = ""
         d = "A4NjFqYu5wPHsO0XTdDgMa2r1ZQocVte9UJBvk6/7=yRnhISGKblCWi+LpfE8xzm3"
         for i in range(0, 32, 3):
             o = ord(n[i])
-            g = ord(n[i+1]) if i+1 < 32 else 0
-            h = ord(n[i+2]) if i+2 < 32 else 0
+            g = ord(n[i + 1]) if i + 1 < 32 else 0
+            h = ord(n[i + 2]) if i + 2 < 32 else 0
             x = ((o & 3) << 4) | (g >> 4)
             p = ((15 & g) << 2) | (h >> 6)
             v = o >> 2
             b = h & 63 if h else 64
             if not g:
                 p = b = 64
             m += d[v] + d[x] + d[p] + d[b]
@@ -62,14 +63,15 @@
 
 
 def get_a1_and_web_id():
     """generate a1 and webid cookie str, the first return value is a1, second is webId
 
     for example: a1, web_id = get_a1_and_web_id()
     """
+
     def random_str(length):
         alphabet = string.ascii_letters + string.digits
         return ''.join(random.choice(alphabet) for _ in range(length))
 
     d = hex(int(time.time() * 1000))[2:] + random_str(30) + "5" + "0" + "000"
     g = (d + str(binascii.crc32(str(d).encode('utf-8'))))[:52]
     return g, hashlib.md5(g.encode('utf-8')).hexdigest()
@@ -266,18 +268,18 @@
     "X",
     "5",
 ]
 
 
 def tripletToBase64(e):
     return (
-        lookup[63 & (e >> 18)] +
-        lookup[63 & (e >> 12)] +
-        lookup[(e >> 6) & 63] +
-        lookup[e & 63]
+            lookup[63 & (e >> 18)] +
+            lookup[63 & (e >> 12)] +
+            lookup[(e >> 6) & 63] +
+            lookup[e & 63]
     )
 
 
 def encodeChunk(e, t, r):
     m = []
     for b in range(t, r, 3):
         n = (16711680 & (e[b] << 16)) + \
@@ -354,15 +356,15 @@
     t = int(random.uniform(0, 2147483646))
     return base36encode((e + t))
 
 
 def cookie_str_to_cookie_dict(cookie_str: str):
     cookie_blocks = [cookie_block.split("=")
                      for cookie_block in cookie_str.split(";") if cookie_block]
-    return {cookie[0]: cookie[1] for cookie in cookie_blocks}
+    return {cookie[0].strip(): cookie[1].strip() for cookie in cookie_blocks}
 
 
 def cookie_jar_to_cookie_str(cookie_jar):
     cookie_dict = requests.utils.dict_from_cookiejar(cookie_jar)
     return ";".join([f"{key}={value}" for key, value in cookie_dict.items()])
```

### Comparing `xhs-0.2.3/xhs.egg-info/PKG-INFO` & `xhs-0.2.4/xhs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.2.3
+Version: 0.2.4
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

