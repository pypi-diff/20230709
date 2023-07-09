# Comparing `tmp/pyromark-0.2.0.tar.gz` & `tmp/pyromark-0.2.1.tar.gz`

## Comparing `pyromark-0.2.0.tar` & `pyromark-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 pyromark-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     1065 2023-06-29 21:42:52.000000 pyromark-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1224 2023-06-29 21:42:52.000000 pyromark-0.2.0/README.md
--rw-r--r--   0     1001      123     3143 2023-06-29 21:42:52.000000 pyromark-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      264 2023-06-29 21:42:52.000000 pyromark-0.2.0/python/pyromark/__init__.py
--rw-r--r--   0     1001      123     1712 2023-06-29 21:42:52.000000 pyromark-0.2.0/python/pyromark/_extensions.py
--rw-r--r--   0     1001      123      271 2023-06-29 21:42:52.000000 pyromark-0.2.0/python/pyromark/_pyromark.pyi
--rw-r--r--   0     1001      123        0 2023-06-29 21:42:52.000000 pyromark-0.2.0/python/pyromark/py.typed
--rw-r--r--   0     1001      123     2893 2023-06-29 21:42:52.000000 pyromark-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     8308 2023-06-29 21:42:52.000000 pyromark-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 pyromark-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 pyromark-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     1065 2023-07-09 12:37:53.000000 pyromark-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     1224 2023-07-09 12:37:53.000000 pyromark-0.2.1/README.md
+-rw-r--r--   0     1001      123     3372 2023-07-09 12:37:53.000000 pyromark-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123      264 2023-07-09 12:37:53.000000 pyromark-0.2.1/python/pyromark/__init__.py
+-rw-r--r--   0     1001      123     1342 2023-07-09 12:37:53.000000 pyromark-0.2.1/python/pyromark/__main__.py
+-rw-r--r--   0     1001      123     1497 2023-07-09 12:37:53.000000 pyromark-0.2.1/python/pyromark/_extensions.py
+-rw-r--r--   0     1001      123      315 2023-07-09 12:37:53.000000 pyromark-0.2.1/python/pyromark/_pyromark.pyi
+-rw-r--r--   0     1001      123        0 2023-07-09 12:37:53.000000 pyromark-0.2.1/python/pyromark/py.typed
+-rw-r--r--   0     1001      123     2785 2023-07-09 12:37:53.000000 pyromark-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123     8309 2023-07-09 12:37:53.000000 pyromark-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 pyromark-0.2.1/PKG-INFO
```

### Comparing `pyromark-0.2.0/LICENSE` & `pyromark-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyromark-0.2.0/README.md` & `pyromark-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyromark-0.2.0/pyproject.toml` & `pyromark-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 name = "pyromark"
 description = "Blazingly fast Markdown parser"
 readme = "README.md"
 keywords = ["converter", "html"]
 authors = [{ name = "monosans", email = "hsyqixco@protonmail.com" }]
 requires-python = ">=3.7"
 classifiers = [
+    "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
@@ -30,14 +32,17 @@
     "Programming Language :: Rust",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
+[project.scripts]
+pyromark = "pyromark.__main__:main"
+
 [project.urls]
 Homepage = "https://github.com/monosans/pyromark"
 Documentation = "https://pyromark.readthedocs.io/"
 Repository = "https://github.com/monosans/pyromark"
 
 [tool.maturin]
 python-source = "python"
@@ -98,14 +103,15 @@
     "D407",
     "D415",
     "D417",
     "DJ008",
     "ERA001",
     "FBT002",
     "PD901",
+    "PERF203",
     "PLR0911",
     "PLR0912",
     "PLR0913",
     "PLR0915",
     "PT012",
     "RUF001",
     "RUF002",
@@ -121,18 +127,24 @@
     "TCH002",
     "TCH003",
     "TID252",
     "TRY400",
 ]
 
 [tool.ruff.per-file-ignores]
-"tests/*" = ["S101", "UP006", "UP007"]
+"tests/*" = ["S101"]
 
 [tool.ruff.flake8-unused-arguments]
 ignore-variadic-names = true
 
 [tool.ruff.isort]
 combine-as-imports = true
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
+
+[tool.ruff.pyupgrade]
+keep-runtime-typing = true
+
+[tool.ruff.flake8-self]
+ignore-names = ["_name_", "_value_"]
```

### Comparing `pyromark-0.2.0/python/pyromark/_extensions.py` & `pyromark-0.2.1/python/pyromark/_extensions.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 class Extensions(IntFlag):
     """IntFlag containing flags for enabling Markdown extensions.
 
     Examples:
         All extensions:
 
         ```python
-        >>> extensions=(
-        ...     pyromark.Extensions.ENABLE_TABLES
-        ...     | pyromark.Extensions.ENABLE_FOOTNOTES
-        ...     | pyromark.Extensions.ENABLE_STRIKETHROUGH
-        ...     | pyromark.Extensions.ENABLE_TASKLISTS
-        ...     | pyromark.Extensions.ENABLE_SMART_PUNCTUATION
-        ...     | pyromark.Extensions.ENABLE_HEADING_ATTRIBUTES
-        ... )
-        >>> extensions
-        <Extensions.ENABLE_TABLES|ENABLE_FOOTNOTES|ENABLE_STRIKETHROUGH|ENABLE_TASKLISTS|ENABLE_SMART_PUNCTUATION|ENABLE_HEADING_ATTRIBUTES: 126>
+        extensions=(
+            pyromark.Extensions.ENABLE_TABLES
+            | pyromark.Extensions.ENABLE_FOOTNOTES
+            | pyromark.Extensions.ENABLE_STRIKETHROUGH
+            | pyromark.Extensions.ENABLE_TASKLISTS
+            | pyromark.Extensions.ENABLE_SMART_PUNCTUATION
+            | pyromark.Extensions.ENABLE_HEADING_ATTRIBUTES
+        )
         ```
-    """  # noqa: E501
+    """
 
     ENABLE_TABLES = 1 << 1
     """<https://github.github.com/gfm/#tables-extension->"""
     ENABLE_FOOTNOTES = 1 << 2
     """<https://www.markdownguide.org/extended-syntax/#footnotes>"""
     ENABLE_STRIKETHROUGH = 1 << 3
     """<https://github.github.com/gfm/#strikethrough-extension->"""
```

### Comparing `pyromark-0.2.0/src/lib.rs` & `pyromark-0.2.1/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 use pyo3::prelude::*;
 
 /// Examples:
 ///     ```python
-///     >>> md = pyromark.Markdown(
-///     ...     # Optional, include the ones you want
-///     ...     extensions=(
-///     ...         pyromark.Extensions.ENABLE_TABLES
-///     ...         | pyromark.Extensions.ENABLE_FOOTNOTES
-///     ...         | pyromark.Extensions.ENABLE_STRIKETHROUGH
-///     ...         | pyromark.Extensions.ENABLE_TASKLISTS
-///     ...         | pyromark.Extensions.ENABLE_SMART_PUNCTUATION
-///     ...         | pyromark.Extensions.ENABLE_HEADING_ATTRIBUTES
-///     ...     )
-///     ... )
+///     md = pyromark.Markdown(
+///         # Optional, include the ones you want
+///         extensions=(
+///             pyromark.Extensions.ENABLE_TABLES
+///             | pyromark.Extensions.ENABLE_FOOTNOTES
+///             | pyromark.Extensions.ENABLE_STRIKETHROUGH
+///             | pyromark.Extensions.ENABLE_TASKLISTS
+///             | pyromark.Extensions.ENABLE_SMART_PUNCTUATION
+///             | pyromark.Extensions.ENABLE_HEADING_ATTRIBUTES
+///         )
+///     )
 ///     ```
 #[pyclass(frozen, module = "pyromark._pyromark")]
 struct Markdown {
     options: pulldown_cmark::Options,
 }
 
 #[pymethods]
@@ -25,42 +25,40 @@
     #[pyo3(signature = (*, extensions = None))]
     fn new(extensions: Option<u32>) -> Self {
         Self { options: get_options(extensions) }
     }
 
     /// Examples:
     ///     ```python
-    ///     >>> html = md.convert("# Hello world")
-    ///     >>> html
-    ///     '<h1>Hello world</h1>\n'
+    ///     html = md.convert("# Hello world")
+    ///     print(html)  # <h1>Hello world</h1>\n
     ///     ```
     fn convert(&self, py: Python, text: &str) -> String {
         py.allow_threads(move || {
             let parser = pulldown_cmark::Parser::new_ext(text, self.options);
             html_from_parser(parser)
         })
     }
 }
 
 /// Examples:
 ///     ```python
-///     >>> html = pyromark.markdown(
-///     ...     "# Hello world",
-///     ...     # Optional, include the ones you want
-///     ...     extensions=(
-///     ...         pyromark.Extensions.ENABLE_TABLES
-///     ...         | pyromark.Extensions.ENABLE_FOOTNOTES
-///     ...         | pyromark.Extensions.ENABLE_STRIKETHROUGH
-///     ...         | pyromark.Extensions.ENABLE_TASKLISTS
-///     ...         | pyromark.Extensions.ENABLE_SMART_PUNCTUATION
-///     ...         | pyromark.Extensions.ENABLE_HEADING_ATTRIBUTES
-///     ...     )
-///     ... )
-///     >>> html
-///     '<h1>Hello world</h1>\n'
+///     html = pyromark.markdown(
+///         "# Hello world",
+///         # Optional, include the ones you want
+///         extensions=(
+///             pyromark.Extensions.ENABLE_TABLES
+///             | pyromark.Extensions.ENABLE_FOOTNOTES
+///             | pyromark.Extensions.ENABLE_STRIKETHROUGH
+///             | pyromark.Extensions.ENABLE_TASKLISTS
+///             | pyromark.Extensions.ENABLE_SMART_PUNCTUATION
+///             | pyromark.Extensions.ENABLE_HEADING_ATTRIBUTES
+///         )
+///     )
+///     print(html)  # <h1>Hello world</h1>\n
 ///     ```
 #[pyfunction]
 #[pyo3(signature = (text, *, extensions = None))]
 fn markdown(py: Python, text: &str, extensions: Option<u32>) -> String {
     py.allow_threads(move || {
         let options = get_options(extensions);
         let parser = pulldown_cmark::Parser::new_ext(text, options);
```

### Comparing `pyromark-0.2.0/Cargo.lock` & `pyromark-0.2.1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -84,17 +84,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulldown-cmark"
 version = "0.9.3"
@@ -104,75 +104,75 @@
  "bitflags",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyromark"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "pulldown-cmark",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -196,17 +196,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
@@ -228,17 +228,17 @@
 checksum = "50f37be617794602aabbeee0be4f259dc1778fabe05e2d67ee8f79326d5cb4f6"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

### Comparing `pyromark-0.2.0/PKG-INFO` & `pyromark-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: pyromark
-Version: 0.2.0
+Version: 0.2.1
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

