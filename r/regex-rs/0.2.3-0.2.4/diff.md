# Comparing `tmp/regex_rs-0.2.3.tar.gz` & `tmp/regex_rs-0.2.4.tar.gz`

## Comparing `regex_rs-0.2.3.tar` & `regex_rs-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 regex_rs-0.2.3/Cargo.toml
--rw-r--r--   0     1001      123      109 2023-07-07 21:15:38.000000 regex_rs-0.2.3/.github/dependabot.yml
--rw-r--r--   0     1001      123     2785 2023-07-07 21:15:38.000000 regex_rs-0.2.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-07 21:15:38.000000 regex_rs-0.2.3/.gitignore
--rw-r--r--   0     1001      123      369 2023-07-07 21:15:38.000000 regex_rs-0.2.3/pyproject.toml
--rw-r--r--   0     1001      123     1857 2023-07-07 21:15:38.000000 regex_rs-0.2.3/regex_rs.pyi
--rw-r--r--   0     1001      123     1757 2023-07-07 21:15:38.000000 regex_rs-0.2.3/src/captures.rs
--rw-r--r--   0     1001      123      336 2023-07-07 21:15:38.000000 regex_rs-0.2.3/src/error.rs
--rw-r--r--   0     1001      123      460 2023-07-07 21:15:38.000000 regex_rs-0.2.3/src/lib.rs
--rw-r--r--   0     1001      123     1194 2023-07-07 21:15:38.000000 regex_rs-0.2.3/src/match_struct.rs
--rw-r--r--   0     1001      123     3771 2023-07-07 21:15:38.000000 regex_rs-0.2.3/src/regex.rs
--rw-r--r--   0     1001      123      832 2023-07-07 21:15:38.000000 regex_rs-0.2.3/src/split.rs
--rw-r--r--   0     1001      123    10641 2023-07-07 21:15:38.000000 regex_rs-0.2.3/Cargo.lock
--rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 regex_rs-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 regex_rs-0.2.4/Cargo.toml
+-rw-r--r--   0     1001      123      109 2023-07-08 21:54:16.000000 regex_rs-0.2.4/.github/dependabot.yml
+-rw-r--r--   0     1001      123     2785 2023-07-08 21:54:16.000000 regex_rs-0.2.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-08 21:54:16.000000 regex_rs-0.2.4/.gitignore
+-rw-r--r--   0     1001      123     1069 2023-07-08 21:54:16.000000 regex_rs-0.2.4/LICENSE
+-rw-r--r--   0     1001      123      554 2023-07-08 21:54:16.000000 regex_rs-0.2.4/README.md
+-rw-r--r--   0     1001      123      589 2023-07-08 21:54:16.000000 regex_rs-0.2.4/pyproject.toml
+-rw-r--r--   0     1001      123     1857 2023-07-08 21:54:16.000000 regex_rs-0.2.4/regex_rs.pyi
+-rw-r--r--   0     1001      123     1757 2023-07-08 21:54:16.000000 regex_rs-0.2.4/src/captures.rs
+-rw-r--r--   0     1001      123      336 2023-07-08 21:54:16.000000 regex_rs-0.2.4/src/error.rs
+-rw-r--r--   0     1001      123      460 2023-07-08 21:54:16.000000 regex_rs-0.2.4/src/lib.rs
+-rw-r--r--   0     1001      123     1194 2023-07-08 21:54:16.000000 regex_rs-0.2.4/src/match_struct.rs
+-rw-r--r--   0     1001      123     3771 2023-07-08 21:54:16.000000 regex_rs-0.2.4/src/regex.rs
+-rw-r--r--   0     1001      123      832 2023-07-08 21:54:16.000000 regex_rs-0.2.4/src/split.rs
+-rw-r--r--   0     1001      123    10641 2023-07-08 21:54:23.000000 regex_rs-0.2.4/Cargo.lock
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 regex_rs-0.2.4/PKG-INFO
```

### Comparing `regex_rs-0.2.3/.github/workflows/CI.yml` & `regex_rs-0.2.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `regex_rs-0.2.3/.gitignore` & `regex_rs-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `regex_rs-0.2.3/regex_rs.pyi` & `regex_rs-0.2.4/regex_rs.pyi`

 * *Files identical despite different names*

### Comparing `regex_rs-0.2.3/src/captures.rs` & `regex_rs-0.2.4/src/captures.rs`

 * *Files identical despite different names*

### Comparing `regex_rs-0.2.3/src/match_struct.rs` & `regex_rs-0.2.4/src/match_struct.rs`

 * *Files identical despite different names*

### Comparing `regex_rs-0.2.3/src/regex.rs` & `regex_rs-0.2.4/src/regex.rs`

 * *Files identical despite different names*

### Comparing `regex_rs-0.2.3/src/split.rs` & `regex_rs-0.2.4/src/split.rs`

 * *Files identical despite different names*

### Comparing `regex_rs-0.2.3/Cargo.lock` & `regex_rs-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-rs"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "ouroboros",
  "pyo3",
  "regex",
 ]
 
 [[package]]
```

