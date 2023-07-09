# Comparing `tmp/kasserver-0.3.0.tar.gz` & `tmp/kasserver-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kasserver-0.3.0.tar", last modified: Wed Aug  3 22:11:42 2022, max compression
+gzip compressed data, was "kasserver-0.4.0.tar", last modified: Sun Jul  9 09:41:54 2023, max compression
```

## Comparing `kasserver-0.3.0.tar` & `kasserver-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 22:11:42.224179 kasserver-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 22:11:42.220179 kasserver-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 22:11:42.220179 kasserver-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-08-03 22:11:30.000000 kasserver-0.3.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-03 22:11:42.000000 kasserver-0.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-03 22:11:42.000000 kasserver-0.3.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-08-03 22:11:30.000000 kasserver-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-08-03 22:11:42.224179 kasserver-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-08-03 22:11:30.000000 kasserver-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 22:11:42.220179 kasserver-0.3.0/kasserver/
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver/KasApi.wsdl
--rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver/kasserver_dns.py
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver/kasserver_dns_certbot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver/kasserver_dns_lego.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 22:11:42.224179 kasserver-0.3.0/kasserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-03 22:11:42.000000 kasserver-0.3.0/kasserver.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1362 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver_dns.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1376 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver_dns_certbot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1328 2022-08-03 22:11:30.000000 kasserver-0.3.0/kasserver_dns_lego.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-08-03 22:11:30.000000 kasserver-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-03 22:11:42.224179 kasserver-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-08-03 22:11:30.000000 kasserver-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 22:11:42.224179 kasserver-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-08-03 22:11:30.000000 kasserver-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-08-03 22:11:30.000000 kasserver-0.3.0/tests/test_kasserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2751 2022-08-03 22:11:30.000000 kasserver-0.3.0/tests/test_kasserver_dns.py
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-08-03 22:11:30.000000 kasserver-0.3.0/tests/test_kasserver_dns_certbot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-08-03 22:11:30.000000 kasserver-0.3.0/tests/test_kasserver_dns_lego.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-08-03 22:11:30.000000 kasserver-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:41:54.298082 kasserver-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:41:54.294082 kasserver-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:41:54.298082 kasserver-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-09 09:41:46.000000 kasserver-0.4.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-09 09:41:54.000000 kasserver-0.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-09 09:41:54.000000 kasserver-0.4.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 09:41:46.000000 kasserver-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-09 09:41:54.298082 kasserver-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-09 09:41:46.000000 kasserver-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:41:54.298082 kasserver-0.4.0/kasserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver/KasApi.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver/kasserver_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver/kasserver_dns_certbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver/kasserver_dns_lego.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:41:54.298082 kasserver-0.4.0/kasserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 09:41:54.000000 kasserver-0.4.0/kasserver.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver_dns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1376 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver_dns_certbot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-09 09:41:46.000000 kasserver-0.4.0/kasserver_dns_lego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-09 09:41:46.000000 kasserver-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 09:41:54.298082 kasserver-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-09 09:41:46.000000 kasserver-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:41:54.298082 kasserver-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-09 09:41:46.000000 kasserver-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-09 09:41:46.000000 kasserver-0.4.0/tests/test_kasserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-09 09:41:46.000000 kasserver-0.4.0/tests/test_kasserver_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-09 09:41:46.000000 kasserver-0.4.0/tests/test_kasserver_dns_certbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-09 09:41:46.000000 kasserver-0.4.0/tests/test_kasserver_dns_lego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-09 09:41:46.000000 kasserver-0.4.0/tox.ini
```

### Comparing `kasserver-0.3.0/.github/workflows/check.yml` & `kasserver-0.4.0/.github/workflows/check.yml`

 * *Files 5% similar despite different names*

```diff
@@ -7,46 +7,47 @@
   test:
     name: Test with Python ${{ matrix.py }}
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         py:
+          - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
     steps:
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.py }}
       - uses: actions/checkout@v2
       - name: Install tox-gh
         run: python -m pip install tox-gh
       - name: Setup test suite
         run: tox
-      - if: ${{ matrix.py == '3.10' }}
+      - if: ${{ matrix.py == '3.11' }}
         name: Generate coverage data
         run: .tox/py310/bin/coverage lcov -o coverage/lcov.info
-      - if: ${{ matrix.py == '3.10' }}
+      - if: ${{ matrix.py == '3.11' }}
         name: Coveralls
         uses: coverallsapp/github-action@master
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
   publish:
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     needs: [test]
     runs-on: ubuntu-latest
     steps:
       - name: Setup python to build package
         uses: actions/setup-python@v2
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install build
         run: python -m pip install build
       - uses: actions/checkout@v2
       - name: Build sdist and wheel
         run: python -m build -s -w . -o dist
       - name: Publish to PyPi
         uses: pypa/gh-action-pypi-publish@master
```

### Comparing `kasserver-0.3.0/LICENSE.txt` & `kasserver-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/PKG-INFO` & `kasserver-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kasserver
-Version: 0.3.0
+Version: 0.4.0
 Summary: Manage domains hosted on All-Inkl.com through the KAS server API
 Home-page: https://github.com/fetzerch/kasserver
 Author: Christian Fetzer
 Author-email: fetzer.ch@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `kasserver-0.3.0/README.md` & `kasserver-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver/KasApi.wsdl` & `kasserver-0.4.0/kasserver/KasApi.wsdl`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver/__init__.py` & `kasserver-0.4.0/kasserver/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,21 @@
 
 LOGGER = logging.getLogger(__name__)
 
 
 class KasServer:
     """Manage domains hosted on All-Inkl.com through the KAS server API"""
 
-    FLOOD_TIMEOUT = 1
-
     def __init__(self):
         wsdl_file = os.path.join(
             os.path.dirname(os.path.realpath(__file__)), "KasApi.wsdl"
         )
         self._client = zeep.Client(wsdl_file)
         self._get_credentials()
+        self._flood_timeout = 0
 
     def _get_credentials(self):
         self._username = os.environ.get("KASSERVER_USER", None)
         self._password = os.environ.get("KASSERVER_PASSWORD", None)
         if self._username:
             return
 
@@ -72,23 +71,22 @@
             "KasAuthType": "plain",
             "KasAuthData": self._password,
             "KasRequestType": request,
             "KasRequestParams": params,
         }
 
         def _send_request(request):
+            time.sleep(self._flood_timeout)
             try:
                 result = self._client.service.KasApi(json.dumps(request))
-                time.sleep(KasServer.FLOOD_TIMEOUT)
+                self._flood_timeout = result[1]["value"]["item"][0]["value"]
                 return result
             except zeep.exceptions.Fault as exc:
                 if exc.message == "flood_protection":
-                    timeout = (
-                        math.ceil(float(exc.detail.text)) + KasServer.FLOOD_TIMEOUT
-                    )
+                    timeout = math.ceil(float(exc.detail.text))
                     LOGGER.warning("Hit flood protection, retrying in %ds", timeout)
                     time.sleep(timeout)
                     return _send_request(request)
                 raise
 
         return _send_request(request)
```

### Comparing `kasserver-0.3.0/kasserver/kasserver_dns.py` & `kasserver-0.4.0/kasserver/kasserver_dns.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver/kasserver_dns_certbot.py` & `kasserver-0.4.0/kasserver/kasserver_dns_certbot.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver/kasserver_dns_lego.py` & `kasserver-0.4.0/kasserver/kasserver_dns_lego.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver.egg-info/PKG-INFO` & `kasserver-0.4.0/kasserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kasserver
-Version: 0.3.0
+Version: 0.4.0
 Summary: Manage domains hosted on All-Inkl.com through the KAS server API
 Home-page: https://github.com/fetzerch/kasserver
 Author: Christian Fetzer
 Author-email: fetzer.ch@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `kasserver-0.3.0/kasserver.egg-info/SOURCES.txt` & `kasserver-0.4.0/kasserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver_dns.py` & `kasserver-0.4.0/kasserver_dns.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver_dns_certbot.py` & `kasserver-0.4.0/kasserver_dns_certbot.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/kasserver_dns_lego.py` & `kasserver-0.4.0/kasserver_dns_lego.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/requirements.txt` & `kasserver-0.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/setup.cfg` & `kasserver-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/setup.py` & `kasserver-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/tests/__init__.py` & `kasserver-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/tests/test_kasserver.py` & `kasserver-0.4.0/tests/test_kasserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     RESPONSE = [
         {},
         {
             "key": "Response",
             "value": {
                 "item": [
-                    {},
+                    {"key": "KasFloodDelay", "value": 0},
                     {},
                     {
                         "key": "ReturnInfo",
                         "value": {
                             "_value_1": [
                                 {
                                     "item": [
```

### Comparing `kasserver-0.3.0/tests/test_kasserver_dns.py` & `kasserver-0.4.0/tests/test_kasserver_dns.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/tests/test_kasserver_dns_certbot.py` & `kasserver-0.4.0/tests/test_kasserver_dns_certbot.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/tests/test_kasserver_dns_lego.py` & `kasserver-0.4.0/tests/test_kasserver_dns_lego.py`

 * *Files identical despite different names*

### Comparing `kasserver-0.3.0/tox.ini` & `kasserver-0.4.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 [tox]
-envlist = py37,py38,py39,py310
+envlist = py37,py38,py39,py310,py311
 
 [testenv]
 deps = pytest-mock
        pytest-cov
        pytest-black
        pytest-pylint
 commands = pytest {posargs} --black --pylint \
```

