# Comparing `tmp/mapperr-0.2.2.tar.gz` & `tmp/mapperr-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapperr-0.2.2.tar", last modified: Sat Jul  8 19:32:20 2023, max compression
+gzip compressed data, was "mapperr-0.2.3.tar", last modified: Sun Jul  9 15:27:40 2023, max compression
```

## Comparing `mapperr-0.2.2.tar` & `mapperr-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.989349 mapperr-0.2.2/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.2.2/LICENSE
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 19:32:20.989139 mapperr-0.2.2/PKG-INFO
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2535 2023-07-08 17:53:17.000000 mapperr-0.2.2/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.986659 mapperr-0.2.2/mapperr/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     1080 2023-07-08 17:45:59.000000 mapperr-0.2.2/mapperr/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3702 2023-07-08 19:24:53.000000 mapperr-0.2.2/mapperr/mapper.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      243 2023-07-08 11:49:55.000000 mapperr-0.2.2/mapperr/util.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.987374 mapperr-0.2.2/mapperr.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2905 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      373 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-07-08 19:32:20.000000 mapperr-0.2.2/mapperr.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-08 19:32:20.989401 mapperr-0.2.2/setup.cfg
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-07-08 19:31:47.000000 mapperr-0.2.2/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-08 19:32:20.988712 mapperr-0.2.2/test/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      624 2023-07-08 19:25:31.000000 mapperr-0.2.2/test/test_dict_attributes.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     1889 2023-07-07 23:58:08.000000 mapperr-0.2.2/test/test_nested_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.2.2/test/test_op_required.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      822 2023-07-08 18:28:47.000000 mapperr-0.2.2/test/test_recursive_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      923 2023-07-08 19:31:11.000000 mapperr-0.2.2/test/test_super_classes.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-07-01 05:54:21.000000 mapperr-0.2.2/test/test_unmatched_types.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-09 15:27:40.591137 mapperr-0.2.3/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.2.3/LICENSE
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3001 2023-07-09 15:27:40.590948 mapperr-0.2.3/PKG-INFO
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2631 2023-07-09 15:26:57.000000 mapperr-0.2.3/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-09 15:27:40.588640 mapperr-0.2.3/mapperr/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1080 2023-07-08 17:45:59.000000 mapperr-0.2.3/mapperr/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3752 2023-07-09 15:22:31.000000 mapperr-0.2.3/mapperr/mapper.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      243 2023-07-08 11:49:55.000000 mapperr-0.2.3/mapperr/util.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-09 15:27:40.589558 mapperr-0.2.3/mapperr.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3001 2023-07-09 15:27:40.000000 mapperr-0.2.3/mapperr.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      373 2023-07-09 15:27:40.000000 mapperr-0.2.3/mapperr.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-07-09 15:27:40.000000 mapperr-0.2.3/mapperr.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-07-09 15:27:40.000000 mapperr-0.2.3/mapperr.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-07-09 15:27:40.591186 mapperr-0.2.3/setup.cfg
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-07-09 15:27:07.000000 mapperr-0.2.3/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-07-09 15:27:40.590696 mapperr-0.2.3/test/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      624 2023-07-08 19:25:31.000000 mapperr-0.2.3/test/test_dict_attributes.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     1889 2023-07-07 23:58:08.000000 mapperr-0.2.3/test/test_nested_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.2.3/test/test_op_required.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      822 2023-07-08 18:28:47.000000 mapperr-0.2.3/test/test_recursive_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2193 2023-07-09 15:22:19.000000 mapperr-0.2.3/test/test_super_classes.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-07-01 05:54:21.000000 mapperr-0.2.3/test/test_unmatched_types.py
```

### Comparing `mapperr-0.2.2/LICENSE` & `mapperr-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.2/PKG-INFO` & `mapperr-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.2.2
+Version: 0.2.3
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -97,17 +97,21 @@
 new_book.title = "Alchemy"
 
 lib.book_shelfs[0].books.append(new_book)
 
 send_library_to_the_source( to_dict(lib) )
 ```
 
-You can add your `recursive` type definitions into your class by using string variables.
+You can add your `recursive` type definitions into your class by using string variables and you can also use `superclass`es.
 
 ```python
 class Person:
     name: str
     identity: int
+    age: int
     mother: 'Person'
     father: 'Person'
     friends: List['Person']
+
+class Employee(Person):
+    company_name: str
 ```
```

### Comparing `mapperr-0.2.2/README.md` & `mapperr-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -85,17 +85,21 @@
 new_book.title = "Alchemy"
 
 lib.book_shelfs[0].books.append(new_book)
 
 send_library_to_the_source( to_dict(lib) )
 ```
 
-You can add your `recursive` type definitions into your class by using string variables.
+You can add your `recursive` type definitions into your class by using string variables and you can also use `superclass`es.
 
 ```python
 class Person:
     name: str
     identity: int
+    age: int
     mother: 'Person'
     father: 'Person'
     friends: List['Person']
+
+class Employee(Person):
+    company_name: str
 ```
```

### Comparing `mapperr-0.2.2/mapperr/__init__.py` & `mapperr-0.2.3/mapperr/__init__.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.2/mapperr/mapper.py` & `mapperr-0.2.3/mapperr/mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         elif class_definition.__module__ not in ["typing", "builtins"]:
             self.__all_classes.add(class_definition)
         return local_classs_definition
 
     def __get_all_annotations(self, class_definition: type) -> dict:
         classes = [class_definition]
         while classes[0].__name__ != 'object':
+            self.__add_class(classes[0].__base__)
             classes.insert(0, classes[0].__base__)
         del classes[0]
 
         annotations = {}
         for a_class in classes:
             annotations.update(a_class.__annotations__)
```

### Comparing `mapperr-0.2.2/mapperr.egg-info/PKG-INFO` & `mapperr-0.2.3/mapperr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.2.2
+Version: 0.2.3
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -97,17 +97,21 @@
 new_book.title = "Alchemy"
 
 lib.book_shelfs[0].books.append(new_book)
 
 send_library_to_the_source( to_dict(lib) )
 ```
 
-You can add your `recursive` type definitions into your class by using string variables.
+You can add your `recursive` type definitions into your class by using string variables and you can also use `superclass`es.
 
 ```python
 class Person:
     name: str
     identity: int
+    age: int
     mother: 'Person'
     father: 'Person'
     friends: List['Person']
+
+class Employee(Person):
+    company_name: str
 ```
```

### Comparing `mapperr-0.2.2/setup.py` & `mapperr-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="mapperr",
-    version="0.2.2",
+    version="0.2.3",
     description="mapperr for mapping across dict and object, recursively",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/mapperr",
     keywords=["python", "mapper", "recursive mapping"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `mapperr-0.2.2/test/test_dict_attributes.py` & `mapperr-0.2.3/test/test_dict_attributes.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.2/test/test_nested_objects.py` & `mapperr-0.2.3/test/test_nested_objects.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.2/test/test_op_required.py` & `mapperr-0.2.3/test/test_op_required.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.2/test/test_recursive_objects.py` & `mapperr-0.2.3/test/test_recursive_objects.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.2.2/test/test_super_classes.py` & `mapperr-0.2.3/test/test_super_classes.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,31 +7,80 @@
 
 class B(A):
     b1: str
 
 class C(A):
     a1: int
 
+class D(A):
+    d1: str
+    d2: 'D'
+
+class E(D):
+    e1: str
+
 class TestSuperClasses(TestCase):
     def setUp(self) -> None:
         self.b = B()
         self.b.a1, self.b.b1 = "texta1", "textb1"
         self.bd = {"a1": "texta1", "b1": "textb1"}
 
         self.c = C()
         self.c.a1 = 1
         self.cd = {"a1": 1}
 
+        self.d_inner = D()
+        self.d_inner.a1 = "texta1_inner"
+        self.d_inner.d1 = "textd1_inner"
+
+        self.d = D()
+        self.d.a1 = "texta1"
+        self.d.d1 = "textd1"
+        self.d.d2 = self.d_inner
+
+        self.d_dict = {
+            "a1": "texta1",
+            "d1": "textd1",
+            "d2": {
+                "a1": "texta1_inner",
+                "d1": "textd1_inner",
+                "d2": None
+            }
+        }
+
+        self.e = E()
+        self.e.a1, self.e.e1, self.e.d1, self.e.d2 = "texta1", "texte1", "textd1", self.d_inner
+        self.ed = {
+            "a1": "texta1",
+            "e1": "texte1",
+            "d1": "textd1",
+            "d2": {
+                "a1": "texta1_inner",
+                "d1": "textd1_inner",
+                "d2": None
+            }
+        }
+
     def test__to_dict__when_superClassExists(self):
         actual = to_dict(self.b)
         expected = self.bd
         self.assertEqual(actual, expected)
 
     def test__to_obj__when_superClassExists(self):
         actual = to_dict(to_obj(self.bd, B))
         expected = self.bd
         self.assertEqual(actual, expected)
 
     def test__to_obj__when_classOverridesAttrOfSuperClass(self):
         actual = to_dict(to_obj(self.cd, C))
         expected = self.cd
+        self.assertEqual(actual, expected)
+
+    def test__to_obj__to_dict__when_classHasRecursiveAttribute(self):
+        actual = to_dict(to_obj(self.d_dict, D))
+        expected = to_dict(self.d)
+        self.assertEqual(actual, expected)
+
+    def test__to_obj__when_superClassHasRecursiveAttribute(self):
+        actual = to_dict(to_obj(self.ed, E))
+        expected = to_dict(self.e)
         self.assertEqual(actual, expected)
```

### Comparing `mapperr-0.2.2/test/test_unmatched_types.py` & `mapperr-0.2.3/test/test_unmatched_types.py`

 * *Files identical despite different names*

