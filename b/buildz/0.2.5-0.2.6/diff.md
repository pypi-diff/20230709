# Comparing `tmp/buildz-0.2.5.tar.gz` & `tmp/buildz-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.2.5.tar", last modified: Tue Jun 27 16:03:57 2023, max compression
+gzip compressed data, was "buildz-0.2.6.tar", last modified: Sun Jul  9 06:25:46 2023, max compression
```

## Comparing `buildz-0.2.5.tar` & `buildz-0.2.6.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)    11357 2023-05-10 08:15:22.000000 buildz-0.2.5/LICENSE
--rw-rw-r--   0 zzz       (1000) zzz       (1000)       49 2023-05-10 08:15:22.000000 buildz-0.2.5/MANIFEST.in
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-27 16:03:57.203179 buildz-0.2.5/PKG-INFO
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5193 2023-06-19 17:20:46.000000 buildz-0.2.5/README.md
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1039 2023-06-02 05:54:37.000000 buildz-0.2.5/buildz/__init__.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      336 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/__main__.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      413 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/base.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     7595 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/build.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)    10421 2023-05-10 08:21:53.000000 buildz-0.2.5/buildz/confz.py
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz/demo/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      514 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/demo.confz
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      502 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/demo.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      451 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/run.confz
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      203 2023-06-19 17:24:31.000000 buildz-0.2.5/buildz/demo/test.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1107 2023-06-20 16:06:31.000000 buildz-0.2.5/buildz/demo/testz.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      357 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/demo/value.confz
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5173 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/keys.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      804 2023-05-10 08:15:22.000000 buildz-0.2.5/buildz/tools.py
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz/xconfz/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)       45 2023-06-19 17:22:29.000000 buildz-0.2.5/buildz/xconfz/__init__.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     3397 2023-06-27 15:49:52.000000 buildz-0.2.5/buildz/xconfz/base.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1631 2023-06-19 17:22:23.000000 buildz-0.2.5/buildz/xconfz/buff.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      227 2023-06-19 17:21:53.000000 buildz-0.2.5/buildz/xconfz/fc.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1951 2023-06-19 17:22:20.000000 buildz-0.2.5/buildz/xconfz/fc_item.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1846 2023-06-19 17:22:16.000000 buildz-0.2.5/buildz/xconfz/fc_list.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     2116 2023-06-19 17:22:13.000000 buildz-0.2.5/buildz/xconfz/fc_map.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     1732 2023-06-19 17:22:08.000000 buildz-0.2.5/buildz/xconfz/fc_set.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     2821 2023-06-19 17:22:05.000000 buildz-0.2.5/buildz/xconfz/fc_str.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     2762 2023-06-19 17:21:59.000000 buildz-0.2.5/buildz/xconfz/fc_type.py
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     4067 2023-06-27 15:31:44.000000 buildz-0.2.5/buildz/xconfz/mg.py
-drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-06-27 16:03:57.203179 buildz-0.2.5/buildz.egg-info/
--rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/PKG-INFO
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      661 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/SOURCES.txt
--rw-rw-r--   0 zzz       (1000) zzz       (1000)        1 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/dependency_links.txt
--rw-rw-r--   0 zzz       (1000) zzz       (1000)        7 2023-06-27 16:03:57.000000 buildz-0.2.5/buildz.egg-info/top_level.txt
--rw-rw-r--   0 zzz       (1000) zzz       (1000)       38 2023-06-27 16:03:57.203179 buildz-0.2.5/setup.cfg
--rw-rw-r--   0 zzz       (1000) zzz       (1000)      746 2023-06-27 15:32:44.000000 buildz-0.2.5/setup.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-07-09 06:25:46.589270 buildz-0.2.6/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)    11357 2023-05-10 08:15:22.000000 buildz-0.2.6/LICENSE
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       49 2023-05-10 08:15:22.000000 buildz-0.2.6/MANIFEST.in
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-07-09 06:25:46.589270 buildz-0.2.6/PKG-INFO
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5193 2023-06-19 17:20:46.000000 buildz-0.2.6/README.md
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-07-09 06:25:46.585269 buildz-0.2.6/buildz/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1039 2023-06-02 05:54:37.000000 buildz-0.2.6/buildz/__init__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      336 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/__main__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      413 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/base.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     7595 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/build.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)    10463 2023-07-09 06:16:52.000000 buildz-0.2.6/buildz/confz.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-07-09 06:25:46.589270 buildz-0.2.6/buildz/demo/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      514 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/demo/demo.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      502 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/demo/demo.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      451 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/demo/run.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      441 2023-07-09 06:17:43.000000 buildz-0.2.6/buildz/demo/test.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      203 2023-06-19 17:24:31.000000 buildz-0.2.6/buildz/demo/test.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      734 2023-07-09 06:17:54.000000 buildz-0.2.6/buildz/demo/testf.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1107 2023-06-20 16:06:31.000000 buildz-0.2.6/buildz/demo/testz.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      357 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/demo/value.confz
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5173 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/keys.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      804 2023-05-10 08:15:22.000000 buildz-0.2.6/buildz/tools.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-07-09 06:25:46.589270 buildz-0.2.6/buildz/xconfz/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      543 2023-07-09 06:15:39.000000 buildz-0.2.6/buildz/xconfz/__init__.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     3140 2023-07-09 04:28:13.000000 buildz-0.2.6/buildz/xconfz/base.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1631 2023-06-19 17:22:23.000000 buildz-0.2.6/buildz/xconfz/buff.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      227 2023-06-19 17:21:53.000000 buildz-0.2.6/buildz/xconfz/fc.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2120 2023-07-09 03:22:04.000000 buildz-0.2.6/buildz/xconfz/fc_item.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2620 2023-07-09 05:11:57.000000 buildz-0.2.6/buildz/xconfz/fc_list.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2953 2023-07-09 05:11:52.000000 buildz-0.2.6/buildz/xconfz/fc_map.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1732 2023-06-19 17:22:08.000000 buildz-0.2.6/buildz/xconfz/fc_set.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2821 2023-06-19 17:22:05.000000 buildz-0.2.6/buildz/xconfz/fc_str.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2762 2023-07-09 03:22:13.000000 buildz-0.2.6/buildz/xconfz/fc_type.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      801 2023-07-09 05:54:02.000000 buildz-0.2.6/buildz/xconfz/file.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     3877 2023-07-09 05:11:49.000000 buildz-0.2.6/buildz/xconfz/fmt_base.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     1317 2023-07-09 05:50:15.000000 buildz-0.2.6/buildz/xconfz/fmt_str.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     2035 2023-07-09 04:09:04.000000 buildz-0.2.6/buildz/xconfz/fmt_type.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     4216 2023-07-09 06:14:26.000000 buildz-0.2.6/buildz/xconfz/mg.py
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     4099 2023-07-09 05:51:50.000000 buildz-0.2.6/buildz/xconfz/mg_fmt.py
+drwxrwxr-x   0 zzz       (1000) zzz       (1000)        0 2023-07-09 06:25:46.585269 buildz-0.2.6/buildz.egg-info/
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)     5597 2023-07-09 06:25:46.000000 buildz-0.2.6/buildz.egg-info/PKG-INFO
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      828 2023-07-09 06:25:46.000000 buildz-0.2.6/buildz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)        1 2023-07-09 06:25:46.000000 buildz-0.2.6/buildz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)        7 2023-07-09 06:25:46.000000 buildz-0.2.6/buildz.egg-info/top_level.txt
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)       38 2023-07-09 06:25:46.589270 buildz-0.2.6/setup.cfg
+-rw-rw-r--   0 zzz       (1000) zzz       (1000)      746 2023-07-09 06:18:09.000000 buildz-0.2.6/setup.py
```

### Comparing `buildz-0.2.5/LICENSE` & `buildz-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/PKG-INFO` & `buildz-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.2.5
+Version: 0.2.6
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.2.5/README.md` & `buildz-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/__init__.py` & `buildz-0.2.6/buildz/__init__.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/build.py` & `buildz-0.2.6/buildz/build.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/confz.py` & `buildz-0.2.6/buildz/confz.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,14 +415,16 @@
     if '"' in s and "'" in s or "\n" in s:
         match = '"""'
         if match in s:
             match = "'''"
         return match+s+match
     if not need_qt(s):
         return s
+    if '"' in s:
+        return "'"+s+"'"
     return '"'+s+'"'
 
 pass
 
 
 def output(data, level = 0, simple = True, orders = [], format = False):
     rst = []
```

### Comparing `buildz-0.2.5/buildz/demo/demo.confz` & `buildz-0.2.6/buildz/demo/demo.confz`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/demo/testz.py` & `buildz-0.2.6/buildz/demo/testz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/keys.py` & `buildz-0.2.6/buildz/keys.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/tools.py` & `buildz-0.2.6/buildz/tools.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/xconfz/base.py` & `buildz-0.2.6/buildz/xconfz/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,23 @@
 
 pass
 class Reg:
     def __init__(self):
         self.index = 0
         self.sets = set()
         self.keys = {}
+    def exist(self, s):
+        bts = type(s)==bytes
+        for key in self.keys:
+            val = key
+            if bts:
+                val = val.encode("utf-8")
+            if s.find(val)>=0:
+                return True
+        return False
     def __call__(self, key):
         if key in self.keys:
             return self.keys[key]
         #if key in self.keys:
         #    raise Exception("reg key already regist:"+str(key))
         self.keys[key] = Key(key)
         return self.keys[key]
@@ -113,40 +122,7 @@
         return None
     def prev(self, buff, queue):
         return False
     def deal(self, queue, stack):
         return False
 
 pass
-
-class BaseFormat:
-    def deal(self, data, fc):
-        return None
-
-pass
-
-
-class FormatNode:
-    def init(self):
-        self.childs = []
-        self.value = None
-        self.up = None
-        return self
-    def val(self, value):
-        self.value = value
-    def add(self, node):
-        self.childs.append(node)
-        node.up = self
-    def is_leaf(self):
-        return len(self.childs)==0
-
-pass
-
-class KVFormatNode(FormatNode):
-    pass
-
-pass
-
-class SptFormatNode(FormatNode):
-    pass
-
-pass
```

### Comparing `buildz-0.2.5/buildz/xconfz/buff.py` & `buildz-0.2.6/buildz/xconfz/buff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.2.5/buildz/xconfz/fc_item.py` & `buildz-0.2.6/buildz/xconfz/fc_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #coding=utf-8
 from buildz.xconfz.base import *
 
+from buildz.xconfz.fmt_base import *
 
 """
 去左空格
 """
 class SpcDeal(BaseDeal):
     def prev(self, buff, stack):
         if buff.remain_size()==0:
@@ -69,7 +70,15 @@
         it = queue[0]
         if self.k_spt(it.val):
             queue.pop(0)
             return True
         return False
 
 pass
+
+class ItemFormat(BaseFormat):
+    def deal(self, data, fc):
+        node = FormatNode().init().val(data)
+        return node
+
+
+pass
```

### Comparing `buildz-0.2.5/buildz/xconfz/fc_list.py` & `buildz-0.2.6/buildz/xconfz/fc_str.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,80 @@
 #coding=utf-8
 from buildz.xconfz.base import *
 
 
-class ListDeal(BaseDeal):
-    def init(self, reg):
-        self.k_l = reg(self.l)
-        self.k_r = reg(self.r)
-    def __init__(self, left, right):
-        self.l = left
-        self.r = right
+class StrDeal(BaseDeal):
+    def __init__(self, left = '"', right= '"', single_line = False, note = False):
+        self.left = left
+        self.right = right
+        self.single_line = single_line
+        self.note = note
+    def init(self,reg):
+        self.k_l = reg(self.left)
+        if self.left == self.right:
+            self.k_r = self.k_l
+        else:
+            self.k_r = reg(self.right)
     def prev(self, buff, queue):
-        #c = buff.curr()
-        if self.check_curr(buff,self.l):
-            if buff.remain_size()>0:
-                raise FormatExp("error string before list:", buff.pos_curr(), buff.full())
-            queue.append(Item(self.k_l, buff.pos_curr()))
-            buff.deal2curr(len(self.l))
-            return True
-        elif self.check_curr(buff, self.r):
-            if buff.remain_size()>0:
-                r = buff.remain().strip()
-                if len(r)>0:
-                    queue.append(Item(r, buff.pos_remain()))
-            queue.append(Item(self.k_r, buff.pos_curr()))
-            buff.deal2curr(len(self.r))
-            return True
-        return False
-    def deal(self, queue, stack):
-        if len(queue)==0:
+        if not self.check_curr(buff, self.left):
             return False
-        it = queue[0]
-        rst = False
-        if self.k_r.equal(it.val):
-            tmp = []
-            find_l = False
-            while len(stack)>0:
-                it_1 =  stack.pop(-1)
-                if self.k_l.equal(it_1.val):
-                    find_l = True
-                    break
-                tmp.append(it_1.val)
-            if not find_l:
-                print("queue:", queue)
-                print("stack:", stack)
-                print("list:", tmp)
-                raise FormatExp("can't  find list left side for right side",it.pos)
-            tmp.reverse()
-            stack.append(Item(tmp, it_1.pos))
-            rst = True
-        elif self.k_l.equal(it.val):
-            stack.append(it)
-            rst = True
-        if rst:
-            queue.pop(0)
-        return rst
+        rm = buff.remain().strip()
+        if len(rm)>0 and not self.note:
+            raise FormatExp("str: unexcept char before symbol:", buff.pos_remain(), rm)
+        left_pos = buff.pos_curr()
+        buff.deal2curr(len(self.left))
+        lr = len(self.right)
+        curr = buff.curr(lr)
+        while len(curr)>=lr:
+            if curr == self.right:
+                s = buff.remain()
+                if not self.note:
+                    queue.append(Item(s, left_pos))
+                elif len(rm)>0:
+                    queue.append(Item(rm, left_pos))
+                buff.deal2curr(lr)
+                return True
+            if self.single_line and curr.find("\n")>=0:
+                raise FormatExp("str|note: unexcept enter for string", buff.pos_remain())
+            buff.add_remain(1)
+            curr = buff.curr(lr)
+        print(buff.remain())
+        err = "str|note: can't find right symbol {right} for left symbol {left}".format(right =  self.right, left = self.left)
+        raise FormatExp(err, left_pos)
 
 pass
+
+class TranslateStrDeal(StrDeal):
+    def prev(self, buff, queue):
+        if not self.check_curr(buff, self.left):
+            return False
+        rm = buff.remain().strip()
+        if len(rm)>0:
+            raise FormatExp("str|note: unexcept char before symbol:", buff.pos_remain())
+        left_pos = buff.pos_curr()
+        buff.deal2curr(len(self.left))
+        lr = len(self.right)
+        cnt = 0
+        curr = buff.curr(1)
+        mark = False
+        while len(curr)>0:
+            cnt += 1
+            if curr in ["\\", b"\\"] and not mark:
+                mark = True
+            else:
+                rm += curr
+                if mark:
+                    cnt = 0
+                mark = False
+            if not mark and cnt >= lr:
+                if rm[-lr:] == self.right:
+                    rm = rm[:-lr]
+                    if not self.note:
+                        queue.append(Item(rm, left_pos))
+                    buff.deal2curr(1)
+                    return True
+            buff.add_remain(1)
+            curr = buff.curr(1)
+        err = "str|note: can't find right symbol {right} for left symbol {left}".format(right =  self.right, left = self.left)
+        raise FormatExp(err, left_pos)
+
+pass
```

### Comparing `buildz-0.2.5/buildz/xconfz/fc_map.py` & `buildz-0.2.6/buildz/xconfz/fc_set.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 #coding=utf-8
 from buildz.xconfz.base import *
 
+class TypeSet:
+    def __str__(self):
+        return "@@TypeSet"
+    def __repr__(self):
+        return str(self)
 
-class MapDeal(BaseDeal):
+pass
+class SetDeal(BaseDeal):
+    Type = TypeSet()
+    def __str__(self):
+        return "@@SetDeal"
+    def __repr__(self):
+        return str(self)
+    def find(self, buff):
+        for spt in self.spts:
+            if self.check_curr(buff, spt):
+                return spt
+        return None
+    def __init__(self, *spts):
+        if len(spts)==0:
+            raise Exception("at least one symbol")
+        self.spts= spts
     def init(self, reg):
-        self.k_l = reg(self.l)
-        self.k_r = reg(self.r)
-    def __init__(self, left, right):
-        self.l = left
-        self.r = right
+        self.k_spts = [reg(k) for k in self.spts]
+        self.k_spt = self.k_spts[0]
     def prev(self, buff, queue):
-        if self.check_curr(buff,self.l):
-            if buff.remain_size()>0:
-                raise FormatExp("error string before map:", buff.pos_curr(), buff.full())
-            queue.append(Item(self.k_l, buff.pos_curr()))
-            buff.deal2curr(len(self.l))
-            return True
-        elif self.check_curr(buff, self.r):
-            if buff.remain_size()>0:
-                r = buff.remain().strip()
-                if len(r)>0:
-                    queue.append(Item(r, buff.pos_remain()))
-            queue.append(Item(self.k_r, buff.pos_curr()))
-            buff.deal2curr(len(self.r))
-            return True
-        return False
+        find = self.find(buff)
+        if find is None:
+            return False
+        lf = len(find)
+        rm = buff.remain().strip()
+        pos = buff.pos_remain()
+        c_pos = buff.pos_curr()
+        if len(queue)==0 or len(rm)>0:
+            queue.append(Item(rm, pos))
+        queue.append(Item(self.k_spt, c_pos, find, SetDeal.Type))
+        buff.deal2curr(lf)
+        return True
     def deal(self, queue, stack):
-        if len(queue)==0:
+        if len(stack)<3:
             return False
-        it = queue[0]
-        rst = False
-        if self.k_r.equal(it.val):
-            tmp = []
-            find_l = False
-            while len(stack)>0:
-                it_1 =  stack.pop(-1)
-                if self.k_l.equal(it_1.val):
-                    find_l = True
-                    break
-                val = it_1.val
-                if not KeyVal.is_inst(val):
-                    #print("it_1:", it_1)
-                    #print("queue:", queue)
-                    #print("stack:", stack)
-                    #print("map:", tmp)
-                    raise FormatExp("an not key-val item found in map:"+str(val), it_1.pos)
-                tmp.append(val)
-            tmp.reverse()
-            tmp = {k.key:k.val for k in tmp}
-            #tmp[val.key] = val.val
-            if not find_l:
-                raise FormatExp("can't find map left side for right side",it.pos)
-            stack.append(Item(tmp, it_1.pos))
-            rst = True
-        elif self.k_l.equal(it.val):
-            stack.append(it)
-            rst = True
-        if rst:
-            queue.pop(0)
-        return rst
-
-pass
+        if self.k_spt(stack[-2].val):
+            if len(queue)>0:
+                val = queue[0]
+                if val.type == SetDeal.Type:
+                    return False
+            val = stack[-1]
+            if Key.is_inst(val.val):
+                return False
+            val = stack.pop(-1)
+            tmp = stack.pop(-1)
+            key = stack.pop(-1)
+            kv = KeyVal(key.val,val.val)
+            item = Item(kv, key.pos)
+            stack.append(item)
+            return True
+        return False
```

### Comparing `buildz-0.2.5/buildz/xconfz/fc_set.py` & `buildz-0.2.6/buildz/xconfz/fc_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,100 @@
 #coding=utf-8
 from buildz.xconfz.base import *
+from buildz.xconfz.fc_list import *
+from buildz.xconfz.fc_set import *
 
-class TypeSet:
-    def __str__(self):
-        return "@@TypeSet"
-    def __repr__(self):
-        return str(self)
 
-pass
-class SetDeal(BaseDeal):
-    Type = TypeSet()
-    def __str__(self):
-        return "@@SetDeal"
-    def __repr__(self):
-        return str(self)
-    def find(self, buff):
-        for spt in self.spts:
-            if self.check_curr(buff, spt):
-                return spt
-        return None
-    def __init__(self, *spts):
-        if len(spts)==0:
-            raise Exception("at least one symbol")
-        self.spts= spts
-    def init(self, reg):
-        self.k_spts = [reg(k) for k in self.spts]
-        self.k_spt = self.k_spts[0]
-    def prev(self, buff, queue):
-        find = self.find(buff)
-        if find is None:
+"""
+二元符<val, type>
+
+"""
+
+class TypeDealA(ListDeal):
+    def __init__(self, left, right):
+        super(TypeDealA, self).__init__(left, right)
+        self._types = {}
+    def types(self, maps):
+        self._types = dict(maps)
+    def deal(self, queue, stack):
+        rst = super(TypeDealA, self).deal(queue, stack)
+        if not rst:
             return False
-        lf = len(find)
-        rm = buff.remain().strip()
-        pos = buff.pos_remain()
-        c_pos = buff.pos_curr()
-        if len(queue)==0 or len(rm)>0:
-            queue.append(Item(rm, pos))
-        queue.append(Item(self.k_spt, c_pos, find, SetDeal.Type))
-        buff.deal2curr(lf)
+        item = stack[-1]
+        vals = item.val
+        if Key.is_inst(vals):
+            return True
+        stack.pop(-1)
+        if len(vals)!=2:
+            raise FormatExp("type error: requires two elements", item.pos)
+        val, _type = vals
+        if _type not in self._types:
+            raise FormatExp("type error: can't deal with type {type}".format(type = _type), item.pos)
+        try:
+            val = self._types[_type](val)
+        except Exception as exp:
+            raise FormatExp("type error: "+str(exp), item.pos)
+        stack.append(Item(val, item.pos))
         return True
+
+pass
+
+"""
+二元符val|type
+"""
+class TypeDealB(SetDeal):
+    def __init__(self, *args):
+        super(TypeDealB, self).__init__(*args)
+        self._types = {}
+    def types(self, maps):
+        self._types = dict(maps)
     def deal(self, queue, stack):
-        if len(stack)<3:
+        rst = super(TypeDealB, self).deal(queue, stack)
+        if not rst:
             return False
-        if self.k_spt(stack[-2].val):
-            if len(queue)>0:
-                val = queue[0]
-                if val.type == SetDeal.Type:
-                    return False
-            val = stack[-1]
-            if Key.is_inst(val.val):
-                return False
-            val = stack.pop(-1)
-            tmp = stack.pop(-1)
-            key = stack.pop(-1)
-            kv = KeyVal(key.val,val.val)
-            item = Item(kv, key.pos)
-            stack.append(item)
-            return True
-        return False
+        item = stack.pop(-1)
+        vals = item.val
+        val = vals.key
+        _type = vals.val
+        if _type not in self._types:
+            raise FormatExp("type error: can't deal with type {type}".format(type = _type), item.pos)
+        try:
+            val = self._types[_type](val)
+        except Exception as exp:
+            raise FormatExp("type error: "+str(exp), item.pos)
+        stack.append(Item(val, item.pos))
+        return True
+
+pass
+
+
+class TypesDeal:
+    def __init__(self):
+        self.deals = []
+        self.types = {}
+    def add_deal(self, deal):
+        self.deals.append(deal)
+        return self
+    def add_type(self, key, fc):
+        self.types[key] = fc
+        return self
+    def add(self, obj, fc = None):
+        if isinstance(obj, BaseDeal):
+            return self.add_deal(obj)
+        else:
+            return self.add_type(obj, fc)
+    def init(self, reg):
+        for deal in self.deals:
+            deal.types(self.types)
+            deal.init(reg)
+    def prev(self, buff, queue):
+        for deal in self.deals:
+            if deal.prev(buff, queue):
+                return True
+        return False
+    def deal(self, queue, stack):
+        for deal in self.deals:
+            if deal.deal(queue, stack):
+                return True
+        return False
+
+pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buildz-0.2.5/buildz/xconfz/fc_type.py` & `buildz-0.2.6/buildz/xconfz/fc_map.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,91 @@
 #coding=utf-8
 from buildz.xconfz.base import *
-from buildz.xconfz.fc_list import *
-from buildz.xconfz.fc_set import *
 
+from buildz.xconfz.fmt_base import *
 
-"""
-二元符<val, type>
-
-"""
-
-class TypeDealA(ListDeal):
+class MapDeal(BaseDeal):
+    def init(self, reg):
+        self.k_l = reg(self.l)
+        self.k_r = reg(self.r)
     def __init__(self, left, right):
-        super(TypeDealA, self).__init__(left, right)
-        self._types = {}
-    def types(self, maps):
-        self._types = dict(maps)
-    def deal(self, queue, stack):
-        rst = super(TypeDealA, self).deal(queue, stack)
-        if not rst:
-            return False
-        item = stack[-1]
-        vals = item.val
-        if Key.is_inst(vals):
+        self.l = left
+        self.r = right
+    def prev(self, buff, queue):
+        if self.check_curr(buff,self.l):
+            if buff.remain_size()>0:
+                raise FormatExp("error string before map:", buff.pos_curr(), buff.full())
+            queue.append(Item(self.k_l, buff.pos_curr()))
+            buff.deal2curr(len(self.l))
             return True
-        stack.pop(-1)
-        if len(vals)!=2:
-            raise FormatExp("type error: requires two elements", item.pos)
-        val, _type = vals
-        if _type not in self._types:
-            raise FormatExp("type error: can't deal with type {type}".format(type = _type), item.pos)
-        try:
-            val = self._types[_type](val)
-        except Exception as exp:
-            raise FormatExp("type error: "+str(exp), item.pos)
-        stack.append(Item(val, item.pos))
-        return True
-
-pass
-
-"""
-二元符val|type
-"""
-class TypeDealB(SetDeal):
-    def __init__(self, *args):
-        super(TypeDealB, self).__init__(*args)
-        self._types = {}
-    def types(self, maps):
-        self._types = dict(maps)
+        elif self.check_curr(buff, self.r):
+            if buff.remain_size()>0:
+                r = buff.remain().strip()
+                if len(r)>0:
+                    queue.append(Item(r, buff.pos_remain()))
+            queue.append(Item(self.k_r, buff.pos_curr()))
+            buff.deal2curr(len(self.r))
+            return True
+        return False
     def deal(self, queue, stack):
-        rst = super(TypeDealB, self).deal(queue, stack)
-        if not rst:
+        if len(queue)==0:
             return False
-        item = stack.pop(-1)
-        vals = item.val
-        val = vals.key
-        _type = vals.val
-        if _type not in self._types:
-            raise FormatExp("type error: can't deal with type {type}".format(type = _type), item.pos)
-        try:
-            val = self._types[_type](val)
-        except Exception as exp:
-            raise FormatExp("type error: "+str(exp), item.pos)
-        stack.append(Item(val, item.pos))
-        return True
+        it = queue[0]
+        rst = False
+        if self.k_r.equal(it.val):
+            tmp = []
+            find_l = False
+            while len(stack)>0:
+                it_1 =  stack.pop(-1)
+                if self.k_l.equal(it_1.val):
+                    find_l = True
+                    break
+                val = it_1.val
+                if not KeyVal.is_inst(val):
+                    #print("it_1:", it_1)
+                    #print("queue:", queue)
+                    #print("stack:", stack)
+                    #print("map:", tmp)
+                    raise FormatExp("an not key-val item found in map:"+str(val), it_1.pos)
+                tmp.append(val)
+            tmp.reverse()
+            tmp = {k.key:k.val for k in tmp}
+            #tmp[val.key] = val.val
+            if not find_l:
+                raise FormatExp("can't find map left side for right side",it.pos)
+            stack.append(Item(tmp, it_1.pos))
+            rst = True
+        elif self.k_l.equal(it.val):
+            stack.append(it)
+            rst = True
+        if rst:
+            queue.pop(0)
+        return rst
 
 pass
 
+class MapFormat(BaseFormat):
+    def __init__(self, left, right):
+        self.l = left
+        self.r = right 
+    def deal(self, data, fc):
+        if type(data) !=dict:
+            raise FormatExp("not dict found:"+type(data), [-1,-1])
+        node = FormatNode().init()
+        node.add(SymbolFormatNode().init().val(self.l))
+        #_node = FormatNode().init()
+        #node.add(_node)
+        nds = []
+        for key in data:
+            nds.append(SpcFormatNode(0,1))
+            nds.append(fc(key))
+            nds.append(KVFormatNode())
+            nds.append(fc(data[key]))
+            nds.append(SptFormatNode())
+        for nd in nds[:-1]:
+            node.add(nd)
+        node.add(SpcFormatNode(0, 0))
+        node.add(SymbolFormatNode().init().val(self.r))
+        return node
 
-class TypesDeal:
-    def __init__(self):
-        self.deals = []
-        self.types = {}
-    def add_deal(self, deal):
-        self.deals.append(deal)
-        return self
-    def add_type(self, key, fc):
-        self.types[key] = fc
-        return self
-    def add(self, obj, fc = None):
-        if isinstance(obj, BaseDeal):
-            return self.add_deal(obj)
-        else:
-            return self.add_type(obj, fc)
-    def init(self, reg):
-        for deal in self.deals:
-            deal.types(self.types)
-            deal.init(reg)
-    def prev(self, buff, queue):
-        for deal in self.deals:
-            if deal.prev(buff, queue):
-                return True
-        return False
-    def deal(self, queue, stack):
-        for deal in self.deals:
-            if deal.deal(queue, stack):
-                return True
-        return False
 
-pass
+pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `buildz-0.2.5/buildz/xconfz/mg.py` & `buildz-0.2.6/buildz/xconfz/mg.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 impl in class
 """
 
 import io
 # io.StringIO("asdf")
 from buildz.xconfz.buff import *
 from buildz.xconfz.fc import *
-
+from buildz.xconfz.fmt_base import *
 
 class Confz:
     def fcs(self, fc, *args, **maps):
         return fc(*self.cs(*args), **maps)
     def add_fc(self, fc, *args, **maps):
         obj = self.fcs(fc, *args, **maps)
         self.add(obj)
@@ -22,15 +22,15 @@
         obj = self.fcs(fc, *args, **maps)
         self.add_top(obj)
         return self
     def cs(self, *args):
         return [self.c(k) for k in args]
     def c(self, s):
         if self.bts:
-            s = s.encode("ascii")
+            s = s.encode("utf-8")
         return s
     def add(self,obj):
         obj.init(self.reg)
         self.prevs.append(obj.prev)
         self.deals.append(obj.deal)
         return self
     def add_top(self, obj):
@@ -65,14 +65,15 @@
             raise Exception("ERROR not data")
         if len(stack)==1:
             return stack[0].val
         else:
             return [it.val for it in stack]
 
 pass
+
 class Map:
     def __init__(self):
         self.maps = {}
     def set(self, key, val):
         self.maps[key] = val
     def __call__(self, s):
         if s not in self.maps:
@@ -149,7 +150,14 @@
 pass
 import io
 def loads(s):
     cfz = build(type(s)==bytes)
     return cfz.load(io.StringIO(s).read)
 
 pass
+
+from buildz.xconfz.file import *
+
+def loadfile(fp, coding = 'utf-8'):
+    return loads(fread(fp, coding))
+
+pass
```

### Comparing `buildz-0.2.5/buildz.egg-info/PKG-INFO` & `buildz-0.2.6/buildz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.2.5
+Version: 0.2.6
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.2.5/buildz.egg-info/SOURCES.txt` & `buildz-0.2.6/buildz.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,28 @@
 buildz.egg-info/PKG-INFO
 buildz.egg-info/SOURCES.txt
 buildz.egg-info/dependency_links.txt
 buildz.egg-info/top_level.txt
 buildz/demo/demo.confz
 buildz/demo/demo.py
 buildz/demo/run.confz
+buildz/demo/test.confz
 buildz/demo/test.py
+buildz/demo/testf.py
 buildz/demo/testz.py
 buildz/demo/value.confz
 buildz/xconfz/__init__.py
 buildz/xconfz/base.py
 buildz/xconfz/buff.py
 buildz/xconfz/fc.py
 buildz/xconfz/fc_item.py
 buildz/xconfz/fc_list.py
 buildz/xconfz/fc_map.py
 buildz/xconfz/fc_set.py
 buildz/xconfz/fc_str.py
 buildz/xconfz/fc_type.py
-buildz/xconfz/mg.py
+buildz/xconfz/file.py
+buildz/xconfz/fmt_base.py
+buildz/xconfz/fmt_str.py
+buildz/xconfz/fmt_type.py
+buildz/xconfz/mg.py
+buildz/xconfz/mg_fmt.py
```

### Comparing `buildz-0.2.5/setup.py` & `buildz-0.2.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.2.5',
+    version = '0.2.6',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-like file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

