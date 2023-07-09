# Comparing `tmp/dek-1.1.0.tar.gz` & `tmp/dek-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dek-1.1.0.tar", max compression
+gzip compressed data, was "dek-1.2.0.tar", max compression
```

## Comparing `dek-1.1.0.tar` & `dek-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1067 2020-07-04 13:16:09.000000 dek-1.1.0/LICENSE
--rw-r--r--   0        0        0     4074 2023-02-23 19:48:33.047881 dek-1.1.0/README.md
--rw-r--r--   0        0        0     8199 2023-02-23 19:35:43.462518 dek-1.1.0/dek.py
--rw-r--r--   0        0        0      530 2023-02-23 19:58:53.117242 dek-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 dek-1.1.0/setup.py
--rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 dek-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2020-07-04 13:16:09.000000 dek-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4074 2023-02-23 19:48:33.047881 dek-1.2.0/README.md
+-rw-r--r--   0        0        0     8138 2023-02-28 13:35:49.446938 dek-1.2.0/dek.py
+-rw-r--r--   0        0        0      511 2023-07-09 14:47:19.652371 dek-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4613 1970-01-01 00:00:00.000000 dek-1.2.0/PKG-INFO
```

### Comparing `dek-1.1.0/LICENSE` & `dek-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dek-1.1.0/README.md` & `dek-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dek-1.1.0/dek.py` & `dek-1.2.0/dek.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,35 +252,29 @@
     * If `methods` is `True`, then only public, non-magic methods - methods
       whose names do *not* start with `_` - are decorated.
 
     * If `methods` is `False`, then methods are not decorated (and neither
       are classes).
     """
 
-    def is_public_non_magic(m):
-        return not m.__name__.startswith('_')
-
-    def is_named(m):
-        return m.__name__.startswith(methods)
-
-    def no(m):
-        return False
-
     if methods is not None:
         if callable(methods):
             accept = methods
 
         elif methods is True:
-            accept = is_public_non_magic
+            def accept(m):
+                return not m.__name__.startswith('_')
 
         elif methods is False:
-            accept = no
+            def accept(m):
+                return False
 
         elif isinstance(methods, str):
-            accept = is_named
+            def accept(m):
+                return m.__name__.startswith(methods)
 
         else:
             raise TypeError('Do not understand methods=%s' % methods)
 
     def decorate(func, *args, **kwargs):
         is_type = isinstance(func, type)
```

### Comparing `dek-1.1.0/setup.py` & `dek-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,182 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dek
+Version: 1.2.0
+Summary: 🎴 The decorator-decorator 🎴
+License: MIT
+Author: Tom Ritchford
+Author-email: tom@swirly.com
+Requires-Python: >3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: xmod
+Description-Content-Type: text/markdown
 
-modules = \
-['dek']
-install_requires = \
-['xmod>=1.3.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'dek',
-    'version': '1.1.0',
-    'description': '🎴 The decorator-decorator 🎴',
-    'long_description': "🗃 `dek` - the decorator-decorator 🗃\n\n`dek` decorates your decorators to diminish defects and drudgery.\n\nWriting a Python decorator which takes no parameters isn't hard.\n\nBut writing a decorator with parameters is less easy - and more work\nif you want to decorate classes, like `unittest.mock.patch` does.\n\n`dek` is a decorator for decorators that does this deftly with a\nsingle tiny function.\n\n## Example 1: a simple decorator with dek\n\nTASK: write a decorator `before` that prints a function's name and its\narguments before it executes.\n\nWith `dek`, it's a few lines:\n\n    import dek\n\n    @dek\n    def before(pfunc):\n        print(pfunc)\n        return pfunc()\n\nDone! To use your new decorator:\n\n    @before\n    def phone(two, four=4):\n        print('Calling', two + two, four * four)\n\n    one(32, four=3)\n\n    # That prints something like:\n    #\n    # functools.partial(<function phone at 0x7fafa8072b00>, 32, four=3)\n    # Calling 64 9\n\n`pfunc` is a [`functools.partial`](\nhttps://docs.python.org/3/library/functools.html#functools.partial),\nwhich represents the function call that `dek` intercepted.  Your code\ncan call `pfunc` as often as you like, or add or change parameters.\n\n## Example 2: same, without `dek`\n\n    import functools\n\n    def before(func):\n        @functools.wraps(func)\n        def wrapped(*args, **kwargs):\n            print(func, args, kwargs)\n            return func(*args, **kwargs)\n\n        return wrapped\n\nWith `dek` it's a bit less work, but the real advantage comes when you have\na decorator with a parameter.\n\n## Example 3: a decorator with a single optional parameter\n\nWrite a decorator `before` that prints a function's name, arguments\n_and a label_ before it executes.\n\nWith `dek`, it's a trivial change from the previous solution.\n\n    import dek\n\n    @dek\n    def before(pfunc, label='dull'):\n        print(label, pfunc.func, *pfunc.args)\n        return pfunc()\n\n    @before\n    def add(x, y):\n        return x + y\n\n    @before(label='Exciting!')\n    def times(x, y):\n        return x * y\n\n    print('Result', add(2, times(2, 3)))\n\n    # Prints:\n    #   Exciting! times 2 3\n    #   dull add 2 6\n    #   Result 8\n\n\n## Example 4: same, without `dek`\n\nWithout `dek` it's actual work that's easy to get wrong.\n\n    import functools\n\n    def before(func=None, label='dull'):\n        if func is not None:\n            @functools.wraps(func)\n            def wrapped(*args, **kwargs):\n                print(label, func.__name, *args)\n                return func(*args, **kwargs)\n\n            return wrapped\n\n        return functools.partial(before, label=label)\n\n\n## Example 5: Deferred mode\n\nFor finer control over function signatures there is deferred mode, which\nlets you select what sort of signature you want to expose with a `wrapped`\nfunction that you create.\n\n    @dek(defer=True)\n    def before(func, label='debug'):\n        def wrapped(foo, bar):\n            print(label, foo, bar)\n            return func(foo, bar)\n\n        return wrapped\n\n## Example 6: Decorating a class\n\nIf you need to decorate methods on a class, there's a `methods` parameter to\nselect which methods get decorated.\n\n\n    import dek\n\n    @dek(methods='test')\n    def before(pfunc):\n        print('HERE', *pfunc.args)\n        return pfunc()\n\n    @before\n    class Class:\n        def test_one(self):\n            return 1\n\n        def test_two(self):\n            return 2\n\n        def three(self):  # This won't get decorated\n            return 1\n\n\n    # Test at the command line:\n    >>> cl = Class()\n    >>> cl.test_one(), cl.test_two(), cl.three()\n    HERE 1\n    HERE 2\n    (1, 2, 3)\n\nNOTES:\n\n[This article](https://medium.com/p/1277a9ed34dc/) talks more about\ndecorators that take parameters and about `dek` in general.\n\nFor your advanced decorator desires, the PyPi module\n[`decorator`](https://github.com/micheles/decorator/blob/master/docs/documentation.md) does not duplicate duties that `dek` does, but does\npretty anything else you could conceive of in a decorator library.\n\n\n### [API Documentation](https://rec.github.io/dek#dek--api-documentation)\n",
-    'author': 'Tom Ritchford',
-    'author_email': 'tom@swirly.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+🗃 `dek` - the decorator-decorator 🗃
 
+`dek` decorates your decorators to diminish defects and drudgery.
+
+Writing a Python decorator which takes no parameters isn't hard.
+
+But writing a decorator with parameters is less easy - and more work
+if you want to decorate classes, like `unittest.mock.patch` does.
+
+`dek` is a decorator for decorators that does this deftly with a
+single tiny function.
+
+## Example 1: a simple decorator with dek
+
+TASK: write a decorator `before` that prints a function's name and its
+arguments before it executes.
+
+With `dek`, it's a few lines:
+
+    import dek
+
+    @dek
+    def before(pfunc):
+        print(pfunc)
+        return pfunc()
+
+Done! To use your new decorator:
+
+    @before
+    def phone(two, four=4):
+        print('Calling', two + two, four * four)
+
+    one(32, four=3)
+
+    # That prints something like:
+    #
+    # functools.partial(<function phone at 0x7fafa8072b00>, 32, four=3)
+    # Calling 64 9
+
+`pfunc` is a [`functools.partial`](
+https://docs.python.org/3/library/functools.html#functools.partial),
+which represents the function call that `dek` intercepted.  Your code
+can call `pfunc` as often as you like, or add or change parameters.
+
+## Example 2: same, without `dek`
+
+    import functools
+
+    def before(func):
+        @functools.wraps(func)
+        def wrapped(*args, **kwargs):
+            print(func, args, kwargs)
+            return func(*args, **kwargs)
+
+        return wrapped
+
+With `dek` it's a bit less work, but the real advantage comes when you have
+a decorator with a parameter.
+
+## Example 3: a decorator with a single optional parameter
+
+Write a decorator `before` that prints a function's name, arguments
+_and a label_ before it executes.
+
+With `dek`, it's a trivial change from the previous solution.
+
+    import dek
+
+    @dek
+    def before(pfunc, label='dull'):
+        print(label, pfunc.func, *pfunc.args)
+        return pfunc()
+
+    @before
+    def add(x, y):
+        return x + y
+
+    @before(label='Exciting!')
+    def times(x, y):
+        return x * y
+
+    print('Result', add(2, times(2, 3)))
+
+    # Prints:
+    #   Exciting! times 2 3
+    #   dull add 2 6
+    #   Result 8
+
+
+## Example 4: same, without `dek`
+
+Without `dek` it's actual work that's easy to get wrong.
+
+    import functools
+
+    def before(func=None, label='dull'):
+        if func is not None:
+            @functools.wraps(func)
+            def wrapped(*args, **kwargs):
+                print(label, func.__name, *args)
+                return func(*args, **kwargs)
+
+            return wrapped
+
+        return functools.partial(before, label=label)
+
+
+## Example 5: Deferred mode
+
+For finer control over function signatures there is deferred mode, which
+lets you select what sort of signature you want to expose with a `wrapped`
+function that you create.
+
+    @dek(defer=True)
+    def before(func, label='debug'):
+        def wrapped(foo, bar):
+            print(label, foo, bar)
+            return func(foo, bar)
+
+        return wrapped
+
+## Example 6: Decorating a class
+
+If you need to decorate methods on a class, there's a `methods` parameter to
+select which methods get decorated.
+
+
+    import dek
+
+    @dek(methods='test')
+    def before(pfunc):
+        print('HERE', *pfunc.args)
+        return pfunc()
+
+    @before
+    class Class:
+        def test_one(self):
+            return 1
+
+        def test_two(self):
+            return 2
+
+        def three(self):  # This won't get decorated
+            return 1
+
+
+    # Test at the command line:
+    >>> cl = Class()
+    >>> cl.test_one(), cl.test_two(), cl.three()
+    HERE 1
+    HERE 2
+    (1, 2, 3)
+
+NOTES:
+
+[This article](https://medium.com/p/1277a9ed34dc/) talks more about
+decorators that take parameters and about `dek` in general.
+
+For your advanced decorator desires, the PyPi module
+[`decorator`](https://github.com/micheles/decorator/blob/master/docs/documentation.md) does not duplicate duties that `dek` does, but does
+pretty anything else you could conceive of in a decorator library.
+
+
+### [API Documentation](https://rec.github.io/dek#dek--api-documentation)
 
-setup(**setup_kwargs)
```

