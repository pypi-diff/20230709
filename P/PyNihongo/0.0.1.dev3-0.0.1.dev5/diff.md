# Comparing `tmp/PyNihongo-0.0.1.dev3.tar.gz` & `tmp/PyNihongo-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNihongo-0.0.1.dev3.tar", last modified: Fri Jul  7 12:50:16 2023, max compression
+gzip compressed data, was "PyNihongo-0.0.1.dev5.tar", last modified: Sun Jul  9 11:10:45 2023, max compression
```

## Comparing `PyNihongo-0.0.1.dev3.tar` & `PyNihongo-0.0.1.dev5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/pynihongo/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/pynihongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/pynihongo/kana.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/pynihongo/method.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:10:45.180934 PyNihongo-0.0.1.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 11:10:35.000000 PyNihongo-0.0.1.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-09 11:10:45.180934 PyNihongo-0.0.1.dev5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:10:45.180934 PyNihongo-0.0.1.dev5/PyNihongo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-09 11:10:45.000000 PyNihongo-0.0.1.dev5/PyNihongo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 11:10:45.000000 PyNihongo-0.0.1.dev5/PyNihongo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 11:10:45.000000 PyNihongo-0.0.1.dev5/PyNihongo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 11:10:45.000000 PyNihongo-0.0.1.dev5/PyNihongo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-09 11:10:35.000000 PyNihongo-0.0.1.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 11:10:45.180934 PyNihongo-0.0.1.dev5/pynihongo/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-09 11:10:35.000000 PyNihongo-0.0.1.dev5/pynihongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-09 11:10:35.000000 PyNihongo-0.0.1.dev5/pynihongo/kana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-09 11:10:35.000000 PyNihongo-0.0.1.dev5/pynihongo/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 11:10:45.180934 PyNihongo-0.0.1.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-09 11:10:35.000000 PyNihongo-0.0.1.dev5/setup.py
```

### Comparing `PyNihongo-0.0.1.dev3/LICENSE` & `PyNihongo-0.0.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNihongo-0.0.1.dev3/PKG-INFO` & `PyNihongo-0.0.1.dev5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNihongo
-Version: 0.0.1.dev3
+Version: 0.0.1.dev5
 Summary: A Python package about japanese.
 Author: Koushoken
 Author-email: kskjcx-dev@yahoo.co.jp
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynihongo
```

### Comparing `PyNihongo-0.0.1.dev3/PyNihongo.egg-info/PKG-INFO` & `PyNihongo-0.0.1.dev5/PyNihongo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNihongo
-Version: 0.0.1.dev3
+Version: 0.0.1.dev5
 Summary: A Python package about japanese.
 Author: Koushoken
 Author-email: kskjcx-dev@yahoo.co.jp
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynihongo
```

### Comparing `PyNihongo-0.0.1.dev3/README.md` & `PyNihongo-0.0.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `PyNihongo-0.0.1.dev3/pynihongo/__init__.py` & `PyNihongo-0.0.1.dev5/pynihongo/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,7 +26,15 @@
     romaji_list = __kana.romaji_list
 
     # 現代仮名（戦前の仮名はない, 清音のみ）
     kendai_hiragana_list = []
 
     '''地理'''
     todofuken = JapanCountries()
+
+
+gojyuon_table = Get.gojyuon_table
+hiragana_list = Get.hiragana_list
+katagana_list = Get.katagana_list
+romaji_list = Get.romaji_list
+kendai_hiragana_list = []
+todofuken = Get.todofuken
```

### Comparing `PyNihongo-0.0.1.dev3/pynihongo/kana.py` & `PyNihongo-0.0.1.dev5/pynihongo/kana.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         # 現代仮名（戦前の仮名は含まない, 清音のみ）
         self.kendai_hiragana_list = []
 
     @staticmethod
     def __gojyuon_table(only_seion=True) -> list:
         """
             Returns:
-                [('', 'た', 'タ'), ('ti', 'ち', 'チ'), ('tu', 'つ', 'ツ'), ('te', 'て', 'テ'), ('to', 'と', 'ト')]
+                [('ta', 'た', 'タ'), ('ti', 'ち', 'チ'), ('tu', 'つ', 'ツ'), ('te', 'て', 'テ'), ('to', 'と', 'ト')]
         """
         table = []
         X = "akstnhmyrw"
         Y = "aiueo"
 
         h = "あいうえおかきくけこさしすせそたちつてとなにぬねのはひふへほまみむめもやいゆえよらりるれろわゐうゑをん"
         k = "アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤイユエヨラリルレロワヰウヱヲン"
@@ -39,14 +39,16 @@
             row = []
             x = x if x != "a" else ""
             for index_y, y in enumerate(Y):
                 row.append((x + y, h[p], k[p]))
                 p += 1
             table.append(row)
 
+        table.append([('n', 'ん', 'ン')])
+
         return table
 
     def __kana_list(self, kana_type: str = "hira") -> list:
         gojyuon = self.gojyuon_table
 
         if kana_type.lower() == "hira":
             flag = 1
```

### Comparing `PyNihongo-0.0.1.dev3/pynihongo/method.py` & `PyNihongo-0.0.1.dev5/pynihongo/method.py`

 * *Files identical despite different names*

### Comparing `PyNihongo-0.0.1.dev3/setup.py` & `PyNihongo-0.0.1.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     long_description=long_description,
     long_description_content_type='text/markdown',
     name='PyNihongo',
-    version='0.0.1dev3',
+    version='0.0.1dev5',
     author='Koushoken',
     author_email='kskjcx-dev@yahoo.co.jp',
     description='A Python package about japanese.',
     packages=['pynihongo'],
     install_requires=[
     ],
 )
```

