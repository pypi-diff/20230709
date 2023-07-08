# Comparing `tmp/augpathlib-0.0.8.tar.gz` & `tmp/augpathlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/augpathlib-0.0.8.tar", last modified: Fri Jan 24 10:08:33 2020, max compression
+gzip compressed data, was "dist/augpathlib-0.0.9.tar", last modified: Tue Feb 11 02:26:51 2020, max compression
```

## Comparing `augpathlib-0.0.8.tar` & `augpathlib-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-01-24 10:08:33.000000 augpathlib-0.0.8/
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2019-09-20 03:48:25.000000 augpathlib-0.0.8/.gitignore
--rw-r--r--   0 tom       (1000) tom       (1000)      561 2019-11-14 07:50:23.000000 augpathlib-0.0.8/.travis.yml
--rw-r--r--   0 tom       (1000) tom       (1000)     1080 2019-09-20 03:48:25.000000 augpathlib-0.0.8/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     2808 2020-01-24 10:08:33.000000 augpathlib-0.0.8/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      129 2019-09-20 03:48:25.000000 augpathlib-0.0.8/Pipfile
--rw-r--r--   0 tom       (1000) tom       (1000)     1930 2019-09-20 03:48:25.000000 augpathlib-0.0.8/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib/
--rw-r--r--   0 tom       (1000) tom       (1000)     1328 2020-01-24 10:04:22.000000 augpathlib-0.0.8/augpathlib/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    44682 2020-01-24 10:04:22.000000 augpathlib-0.0.8/augpathlib/caches.py
--rw-r--r--   0 tom       (1000) tom       (1000)    40036 2020-01-24 10:04:22.000000 augpathlib-0.0.8/augpathlib/core.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2734 2019-11-25 22:05:00.000000 augpathlib-0.0.8/augpathlib/exceptions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    24868 2019-11-11 23:12:02.000000 augpathlib-0.0.8/augpathlib/meta.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4771 2019-10-29 22:24:56.000000 augpathlib-0.0.8/augpathlib/pyads.py
--rw-r--r--   0 tom       (1000) tom       (1000)    25344 2019-11-14 07:50:23.000000 augpathlib-0.0.8/augpathlib/remotes.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10840 2020-01-24 10:04:22.000000 augpathlib-0.0.8/augpathlib/repo.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7220 2019-11-14 07:50:23.000000 augpathlib-0.0.8/augpathlib/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2808 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      604 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       20 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      150 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2020-01-24 10:08:33.000000 augpathlib-0.0.8/augpathlib.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2020-01-24 10:08:33.000000 augpathlib-0.0.8/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1895 2020-01-24 10:04:22.000000 augpathlib-0.0.8/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-01-24 10:08:33.000000 augpathlib-0.0.8/test/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-09-20 03:48:25.000000 augpathlib-0.0.8/test/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5236 2019-11-11 23:12:02.000000 augpathlib-0.0.8/test/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1479 2019-11-11 23:12:02.000000 augpathlib-0.0.8/test/test_eat.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2668 2019-11-11 23:12:02.000000 augpathlib-0.0.8/test/test_move.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8689 2020-01-24 10:04:22.000000 augpathlib-0.0.8/test/test_path.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2865 2019-11-11 23:12:02.000000 augpathlib-0.0.8/test/test_remotes.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3688 2020-01-24 10:04:22.000000 augpathlib-0.0.8/test/test_repo.py
--rw-r--r--   0 tom       (1000) tom       (1000)      186 2019-09-20 03:48:25.000000 augpathlib-0.0.8/test/test_utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-02-11 02:26:51.000000 augpathlib-0.0.9/
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2019-09-20 03:48:25.000000 augpathlib-0.0.9/.gitignore
+-rw-r--r--   0 tom       (1000) tom       (1000)      561 2019-11-14 07:50:23.000000 augpathlib-0.0.9/.travis.yml
+-rw-r--r--   0 tom       (1000) tom       (1000)     1080 2019-09-20 03:48:25.000000 augpathlib-0.0.9/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     2808 2020-02-11 02:26:51.000000 augpathlib-0.0.9/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      129 2019-09-20 03:48:25.000000 augpathlib-0.0.9/Pipfile
+-rw-r--r--   0 tom       (1000) tom       (1000)     1930 2019-09-20 03:48:25.000000 augpathlib-0.0.9/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1326 2020-02-11 02:25:34.000000 augpathlib-0.0.9/augpathlib/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    44682 2020-01-24 10:04:22.000000 augpathlib-0.0.9/augpathlib/caches.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    40220 2020-02-11 02:25:34.000000 augpathlib-0.0.9/augpathlib/core.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2734 2019-11-25 22:05:00.000000 augpathlib-0.0.9/augpathlib/exceptions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    24868 2019-11-11 23:12:02.000000 augpathlib-0.0.9/augpathlib/meta.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4771 2019-10-29 22:24:56.000000 augpathlib-0.0.9/augpathlib/pyads.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    25344 2019-11-14 07:50:23.000000 augpathlib-0.0.9/augpathlib/remotes.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10840 2020-01-24 10:04:22.000000 augpathlib-0.0.9/augpathlib/repo.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7220 2019-11-14 07:50:23.000000 augpathlib-0.0.9/augpathlib/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2808 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      604 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       20 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      150 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2020-02-11 02:26:51.000000 augpathlib-0.0.9/augpathlib.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2020-02-11 02:26:51.000000 augpathlib-0.0.9/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1895 2020-01-24 10:04:22.000000 augpathlib-0.0.9/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2020-02-11 02:26:51.000000 augpathlib-0.0.9/test/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-09-20 03:48:25.000000 augpathlib-0.0.9/test/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5236 2019-11-11 23:12:02.000000 augpathlib-0.0.9/test/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1683 2020-02-11 02:25:34.000000 augpathlib-0.0.9/test/test_eat.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2668 2019-11-11 23:12:02.000000 augpathlib-0.0.9/test/test_move.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8689 2020-01-24 10:04:22.000000 augpathlib-0.0.9/test/test_path.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2865 2019-11-11 23:12:02.000000 augpathlib-0.0.9/test/test_remotes.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3688 2020-01-24 10:04:22.000000 augpathlib-0.0.9/test/test_repo.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      186 2019-09-20 03:48:25.000000 augpathlib-0.0.9/test/test_utils.py
```

### Comparing `augpathlib-0.0.8/.gitignore` & `augpathlib-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/.travis.yml` & `augpathlib-0.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/LICENSE` & `augpathlib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/PKG-INFO` & `augpathlib-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augpathlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Augmented pathlib. Everything else you could do with a path.
 Home-page: https://github.com/tgbugs/augpathlib
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Description: # augpathlib
         [![PyPI version](https://badge.fury.io/py/augpathlib.svg)](https://pypi.org/project/augpathlib/)
```

### Comparing `augpathlib-0.0.8/README.md` & `augpathlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib/__init__.py` & `augpathlib-0.0.9/augpathlib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from augpathlib.meta import PathMeta
 from augpathlib.core import (AugmentedPath,
                              AugmentedPathPosix,
                              AugmentedPathWindows,
                              XopenPath,
                              LocalPath,
-                             EatHelper)
+                             EatPath)
 from augpathlib.caches import (CachePath,
                                PrimaryCache,
                                SqliteCache,
                                SymlinkCache,
                                EatCache,
                                SshCache)
 from augpathlib.remotes import RemotePath
@@ -46,8 +46,8 @@
     'SymlinkCache',
     'XattrCache',
     'SshCache',
 
     'RemotePath',
 ]
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `augpathlib-0.0.8/augpathlib/caches.py` & `augpathlib-0.0.9/augpathlib/caches.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib/core.py` & `augpathlib-0.0.9/augpathlib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,21 +94,21 @@
 
 
 class EatHelper:
     """ Extended attributes helper """
 
     @staticmethod
     def _base_helpers(pos_helpers, win_helpers):
-        pos_helpers = pos_helpers + (XattrHelper,)
-        win_helpers = win_helpers + (ADSHelper,)
+        pos_helpers = tuple(set(pos_helpers + (XattrHelper,)))
+        win_helpers = tuple(set(win_helpers + (ADSHelper,)))
         return pos_helpers, win_helpers
 
     @classmethod
     def _bind_flavours(cls, pos_helpers=tuple(), win_helpers=tuple()):
-        super()._bind_flavours(*cls._base_helpers(pos_helpers, win_helpers))
+        super()._bind_flavours(*EatHelper._base_helpers(pos_helpers, win_helpers))
 
 
 class ADSHelper(EatHelper):
     """ Windows NTFS equivalent of Xattrs is Alternate Data Streams
         This class allows ADS to pretend to work like xattrs.
     """
 
@@ -627,15 +627,22 @@
 pathlib._WindowsFlavour.drive_letters.update(AugmentedPathWindows._registry_drives)
 pathlib._WindowsFlavour.splitroot = splitroot
 pathlib._windows_flavour.splitroot = pathlib._WindowsFlavour().splitroot
 
 AugmentedPath._bind_flavours()
 
 
-class LocalPath(EatHelper, AugmentedPath):
+class EatPath(EatHelper, AugmentedPath):
+    pass
+
+
+EatPath._bind_flavours()
+
+
+class LocalPath(EatPath, AugmentedPath):
     # local data about remote objects
 
     chunksize = 4096  # make the data generator chunksize visible externally
     _cache_class = None  # must be defined by child classes
     sysid = None  # set below
 
     _bind_sysid = classmethod(_bind_sysid_)
@@ -1036,37 +1043,37 @@
 
         return
 
 
 LocalPath._bind_flavours()
 
 
-class XopenPath(AugmentedPath):
+class XopenHelper:
     @staticmethod
     def _base_helpers(pos_helpers, win_helpers):
         pos_helpers = tuple(set(pos_helpers + (XopenPosixHelper,)))
         win_helpers = tuple(set(win_helpers + (XopenWindowsHelper,)))
         return pos_helpers, win_helpers
 
     @classmethod
     def _bind_flavours(cls, pos_helpers=tuple(), win_helpers=tuple()):
-        super()._bind_flavours(*cls._base_helpers(pos_helpers, win_helpers))
+        super()._bind_flavours(*XopenHelper._base_helpers(pos_helpers, win_helpers))
 
 
-class XopenWindowsHelper:
+class XopenWindowsHelper(XopenHelper):
     _command = 'start'
 
     def xopen(self):
         """ open file using start """
         process = subprocess.Popen([self._command, self],
                                    stdout=subprocess.DEVNULL,
                                    stderr=subprocess.STDOUT)
 
 
-class XopenPosixHelper:
+class XopenPosixHelper(XopenHelper):
     _command = 'open' if sys.platform == 'darwin' else 'xdg-open'
 
     def xopen(self):
         """ open file using xdg-open """
         process = subprocess.Popen([self._command, self.as_posix()],
                                    stdout=subprocess.DEVNULL,
                                    stderr=subprocess.STDOUT)
@@ -1113,11 +1120,15 @@
                 break
                 process_window.set_wm_name(new_name)
                 break
             else:
                 sleep(.01)  # spin a bit more slowly
 
 
+class XopenPath(XopenHelper, AugmentedPath):
+    pass
+
+
 XopenPath._bind_flavours()
 
 # any additional values
 LocalPath._bind_sysid()
```

### Comparing `augpathlib-0.0.8/augpathlib/exceptions.py` & `augpathlib-0.0.9/augpathlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib/meta.py` & `augpathlib-0.0.9/augpathlib/meta.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib/pyads.py` & `augpathlib-0.0.9/augpathlib/pyads.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib/remotes.py` & `augpathlib-0.0.9/augpathlib/remotes.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib/repo.py` & `augpathlib-0.0.9/augpathlib/repo.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib/utils.py` & `augpathlib-0.0.9/augpathlib/utils.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/augpathlib.egg-info/PKG-INFO` & `augpathlib-0.0.9/augpathlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augpathlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Augmented pathlib. Everything else you could do with a path.
 Home-page: https://github.com/tgbugs/augpathlib
 Author: Tom Gillespie
 Author-email: tgbugs@gmail.com
 License: MIT
 Description: # augpathlib
         [![PyPI version](https://badge.fury.io/py/augpathlib.svg)](https://pypi.org/project/augpathlib/)
```

### Comparing `augpathlib-0.0.8/augpathlib.egg-info/SOURCES.txt` & `augpathlib-0.0.9/augpathlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/setup.py` & `augpathlib-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/test/common.py` & `augpathlib-0.0.9/test/common.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/test/test_eat.py` & `augpathlib-0.0.9/test/test_eat.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 import pytest
 import augpathlib as aug
 from .common import test_base, onerror
 
 sandbox = test_base / 'eat-sandbox'
 
 
-class EatPath(aug.EatHelper, aug.AugmentedPath): pass
+class EatPath(aug.EatPath, aug.AugmentedPath): pass
 EatPath._bind_flavours()
 
 
+class EatXopenPath(aug.EatPath, aug.XopenPath, aug.AugmentedPath): pass
+EatXopenPath._bind_flavours()
+
+
 class TestEat(unittest.TestCase):
+    test_class = EatPath
     @classmethod
     def setUpClass(cls):
         sandbox.mkdir(parents=True)
 
     @classmethod
     def tearDownClass(cls):
         sandbox.rmtree(onerror=onerror)
     
     def setUp(self):
-        self.dir = EatPath(sandbox, 'some-dir')
+        self.dir = self.test_class(sandbox, 'some-dir')
         if self.dir.exists():
             self.dir.rmtree(onerror=onerror)
         self.dir.mkdir()
 
-        self.file = EatPath(sandbox, 'some-file')
+        self.file = self.test_class(sandbox, 'some-file')
         if self.file.exists() :
             self.file.unlink()
         self.file.touch()
 
     def tearDown(self):
         self.dir.rmtree(onerror=onerror)
         self.file.unlink()
@@ -54,7 +59,11 @@
         test = self.dir.xattrs()
         assert test
 
     def test_file(self):
         self.file.setxattr('key', b'value')
         test = self.file.xattrs()
         assert test
+
+
+class TestEatXopen(TestEat):
+    test_class = EatXopenPath
```

### Comparing `augpathlib-0.0.8/test/test_move.py` & `augpathlib-0.0.9/test/test_move.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/test/test_path.py` & `augpathlib-0.0.9/test/test_path.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/test/test_remotes.py` & `augpathlib-0.0.9/test/test_remotes.py`

 * *Files identical despite different names*

### Comparing `augpathlib-0.0.8/test/test_repo.py` & `augpathlib-0.0.9/test/test_repo.py`

 * *Files identical despite different names*

