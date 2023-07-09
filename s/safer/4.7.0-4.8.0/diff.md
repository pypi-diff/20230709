# Comparing `tmp/safer-4.7.0.tar.gz` & `tmp/safer-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safer-4.7.0.tar", max compression
+gzip compressed data, was "safer-4.8.0.tar", max compression
```

## Comparing `safer-4.7.0.tar` & `safer-4.8.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-05-02 09:24:25.348741 safer-4.7.0/LICENSE
--rw-r--r--   0        0        0     4713 2023-05-02 09:24:25.349032 safer-4.7.0/README.md
--rw-r--r--   0        0        0      604 2023-05-05 08:41:09.854840 safer-4.7.0/pyproject.toml
--rw-r--r--   0        0        0    21475 2023-05-04 14:26:28.993404 safer-4.7.0/safer.py
--rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 safer-4.7.0/setup.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 safer-4.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-02 09:24:25.348741 safer-4.8.0/LICENSE
+-rw-r--r--   0        0        0     4713 2023-05-02 09:24:25.349032 safer-4.8.0/README.md
+-rw-r--r--   0        0        0      573 2023-07-09 14:55:28.466497 safer-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0    21475 2023-05-04 14:26:28.993404 safer-4.8.0/safer.py
+-rw-r--r--   0        0        0     5298 1970-01-01 00:00:00.000000 safer-4.8.0/PKG-INFO
```

### Comparing `safer-4.7.0/LICENSE` & `safer-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safer-4.7.0/README.md` & `safer-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `safer-4.7.0/safer.py` & `safer-4.8.0/safer.py`

 * *Files identical despite different names*

### Comparing `safer-4.7.0/setup.py` & `safer-4.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,164 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: safer
+Version: 4.8.0
+Summary: 🧿 A safer writer for files and streams 🧿
+License: MIT
+Author: Tom Ritchford
+Author-email: tom@swirly.com
+Requires-Python: >=3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-modules = \
-['safer']
-setup_kwargs = {
-    'name': 'safer',
-    'version': '4.7.0',
-    'description': '🧿 A safer writer for files and streams 🧿',
-    'long_description': "# 🧿 `safer`: A safer writer 🧿\n\nAvoid partial writes or corruption!\n\n`safer` wraps file streams, sockets, or a callable, and offers a drop-in\nreplacement for regular old `open()`.\n\n## Quick summary\n\n### A tiny example\n\n    import safer\n\n    with safer.open(filename, 'w') as fp:\n        fp.write('one')\n        print('two', file=fp)\n        raise ValueError\n        # filename was not written.\n\n\n### How to use\n\nUse [pip](https://pypi.org/project/pip) to install `safer` from the command\nline: `pip install safer`.\n\nTested on Python 3.4 - 3.11.  An old Python 2.7 version\nis [here](https://github.com/rec/safer/tree/v2.0.5).\n\nSee the Medium article [here](https://medium.com/@TomSwirly/%EF%B8%8F-safer-a-safer-file-writer-%EF%B8%8F-5fe267dbe3f5)\n\n### The details\n\n`safer` helps prevent programmer error from corrupting files, socket\nconnections, or generalized streams by writing a whole file or nothing.\n\nIt does not prevent concurrent modification of files from other threads or\nprocesses: if you need atomic file writing, see\nhttps://pypi.org/project/atomicwrites/\n\nIt also has a useful `dry_run` setting to let you test your code without\nactually overwriting the target file.\n\n* `safer.writer()` wraps an existing writer, socket or stream and writes a\n  whole response or nothing\n\n* `safer.open()` is a drop-in replacement for built-in `open` that\n  writes a whole file or nothing\n\n* `safer.closer()` returns a stream like from `safer.write()` that also\n  closes the underlying stream or callable when it closes.\n\n* `safer.dump()` is like a safer `json.dump()` which can be used for any\n  serialization protocol, including Yaml and Toml, and also allows you to\n  write to file streams or any other callable.\n\n* `safer.printer()` is `safer.open()` except that it yields a\n  a function that prints to the stream.\n\nBy default, `safer` buffers the written data in memory in a `io.StringIO`\nor `io.BytesIO`.\n\nFor very large files, `safer.open()` has a `temp_file` argument which\nwrites the data to a temporary file on disk, which is moved over using\n`os.rename` if the operation completes successfully.  This functionality\ndoes not work on Windows.  (In fact, it's unclear if any of this works on\nWindows, but that certainly won't.  Windows developer solicted!)\n\n\n### Example: `safer.writer()`\n\n`safer.writer()` wraps an existing stream - a writer, socket, or callback -\nin a temporary stream which is only copied to the target stream at close(), and\nonly if no exception was raised.\n\nSuppose `sock = socket.socket(*args)`.\n\nThe old, dangerous way goes like this.\n\n    try:\n        write_header(sock)\n        write_body(sock)   # Exception is thrown here\n        write_footer(sock)\n     except Exception:\n        write_error(sock)  # Oops, the header was already written\n\nWith `safer` you write all or nothing:\n\n    try:\n        with safer.writer(sock) as s:\n            write_header(s)\n            write_body(s)  # Exception is thrown here\n            write_footer(s)\n     except Exception:\n        write_error(sock)  # Nothing has been written\n\n### Example: `safer.open()` and json\n\n`safer.open()` is a a drop-in replacement for built-in `open()` except that\nwhen used as a context, it leaves the original file unchanged on failure.\n\nIt's easy to write broken JSON if something within it doesn't serialize.\n\n    with open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is empty or partly written\n\n`safer` prevents this:\n\n    with safer.open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is unchanged.\n\n`safer.open(filename)` returns a file stream `fp` like `open(filename)`\nwould, except that `fp` writes to memory stream or a temporary file in the\nsame directory.\n\nIf `fp` is used as a context manager and an exception is raised, then the\nproperty `fp.safer_failed` on the stream is automatically set to `True`.\n\nAnd when `fp.close()` is called, the cached data is stored in `filename` -\n*unless* `fp.safer_failed` is true.\n\n### Example: `safer.printer()`\n\n`safer.printer()` is similar to `safer.open()` except it yields a function\nthat prints to the open file - it's very convenient for printing text.\n\nLike `safer.open()`, if an exception is raised within its context manager,\nthe original file is left unchanged.\n\nBefore.\n\n    with open(file, 'w') as fp:\n        for item in items:\n            print(item, file=fp)\n        # Prints lines until the first exception\n\nWith `safer`\n\n    with safer.printer(file) as print:\n        for item in items:\n            print(item)\n        # Either the whole file is written, or nothing\n\n\n### [API Documentation](https://rec.github.io/safer#safer--api-documentation)\n",
-    'author': 'Tom Ritchford',
-    'author_email': 'tom@swirly.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'py_modules': modules,
-    'python_requires': '>=3.7,<4.0',
-}
+# 🧿 `safer`: A safer writer 🧿
 
+Avoid partial writes or corruption!
+
+`safer` wraps file streams, sockets, or a callable, and offers a drop-in
+replacement for regular old `open()`.
+
+## Quick summary
+
+### A tiny example
+
+    import safer
+
+    with safer.open(filename, 'w') as fp:
+        fp.write('one')
+        print('two', file=fp)
+        raise ValueError
+        # filename was not written.
+
+
+### How to use
+
+Use [pip](https://pypi.org/project/pip) to install `safer` from the command
+line: `pip install safer`.
+
+Tested on Python 3.4 - 3.11.  An old Python 2.7 version
+is [here](https://github.com/rec/safer/tree/v2.0.5).
+
+See the Medium article [here](https://medium.com/@TomSwirly/%EF%B8%8F-safer-a-safer-file-writer-%EF%B8%8F-5fe267dbe3f5)
+
+### The details
+
+`safer` helps prevent programmer error from corrupting files, socket
+connections, or generalized streams by writing a whole file or nothing.
+
+It does not prevent concurrent modification of files from other threads or
+processes: if you need atomic file writing, see
+https://pypi.org/project/atomicwrites/
+
+It also has a useful `dry_run` setting to let you test your code without
+actually overwriting the target file.
+
+* `safer.writer()` wraps an existing writer, socket or stream and writes a
+  whole response or nothing
+
+* `safer.open()` is a drop-in replacement for built-in `open` that
+  writes a whole file or nothing
+
+* `safer.closer()` returns a stream like from `safer.write()` that also
+  closes the underlying stream or callable when it closes.
+
+* `safer.dump()` is like a safer `json.dump()` which can be used for any
+  serialization protocol, including Yaml and Toml, and also allows you to
+  write to file streams or any other callable.
+
+* `safer.printer()` is `safer.open()` except that it yields a
+  a function that prints to the stream.
+
+By default, `safer` buffers the written data in memory in a `io.StringIO`
+or `io.BytesIO`.
+
+For very large files, `safer.open()` has a `temp_file` argument which
+writes the data to a temporary file on disk, which is moved over using
+`os.rename` if the operation completes successfully.  This functionality
+does not work on Windows.  (In fact, it's unclear if any of this works on
+Windows, but that certainly won't.  Windows developer solicted!)
+
+
+### Example: `safer.writer()`
+
+`safer.writer()` wraps an existing stream - a writer, socket, or callback -
+in a temporary stream which is only copied to the target stream at close(), and
+only if no exception was raised.
+
+Suppose `sock = socket.socket(*args)`.
+
+The old, dangerous way goes like this.
+
+    try:
+        write_header(sock)
+        write_body(sock)   # Exception is thrown here
+        write_footer(sock)
+     except Exception:
+        write_error(sock)  # Oops, the header was already written
+
+With `safer` you write all or nothing:
+
+    try:
+        with safer.writer(sock) as s:
+            write_header(s)
+            write_body(s)  # Exception is thrown here
+            write_footer(s)
+     except Exception:
+        write_error(sock)  # Nothing has been written
+
+### Example: `safer.open()` and json
+
+`safer.open()` is a a drop-in replacement for built-in `open()` except that
+when used as a context, it leaves the original file unchanged on failure.
+
+It's easy to write broken JSON if something within it doesn't serialize.
+
+    with open(filename, 'w') as fp:
+        json.dump(data, fp)
+        # If an exception is raised, the file is empty or partly written
+
+`safer` prevents this:
+
+    with safer.open(filename, 'w') as fp:
+        json.dump(data, fp)
+        # If an exception is raised, the file is unchanged.
+
+`safer.open(filename)` returns a file stream `fp` like `open(filename)`
+would, except that `fp` writes to memory stream or a temporary file in the
+same directory.
+
+If `fp` is used as a context manager and an exception is raised, then the
+property `fp.safer_failed` on the stream is automatically set to `True`.
+
+And when `fp.close()` is called, the cached data is stored in `filename` -
+*unless* `fp.safer_failed` is true.
+
+### Example: `safer.printer()`
+
+`safer.printer()` is similar to `safer.open()` except it yields a function
+that prints to the open file - it's very convenient for printing text.
+
+Like `safer.open()`, if an exception is raised within its context manager,
+the original file is left unchanged.
+
+Before.
+
+    with open(file, 'w') as fp:
+        for item in items:
+            print(item, file=fp)
+        # Prints lines until the first exception
+
+With `safer`
+
+    with safer.printer(file) as print:
+        for item in items:
+            print(item)
+        # Either the whole file is written, or nothing
+
+
+### [API Documentation](https://rec.github.io/safer#safer--api-documentation)
 
-setup(**setup_kwargs)
```

