# Comparing `tmp/lbvh-0.0.11.tar.gz` & `tmp/lbvh-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbvh-0.0.11.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "lbvh-0.0.12.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `lbvh-0.0.11.tar` & `lbvh-0.0.12.tar`

### file list

```diff
@@ -1,25 +1,22 @@
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 lbvh-0.0.11/.gitignore
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 lbvh-0.0.11/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 lbvh-0.0.11/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 lbvh-0.0.11/.pytest_cache/README.md
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 lbvh-0.0.11/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 lbvh-0.0.11/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 lbvh-0.0.11/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 lbvh-0.0.11/.vscode/settings.json
--rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 lbvh-0.0.11/CMakeLists.txt
--rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 lbvh-0.0.11/LICENSE
--rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 lbvh-0.0.11/README.md
--rw-r--r--   0        0        0     1619 2022-11-09 12:37:21.000000 lbvh-0.0.11/cpp/AABB.hpp
--rw-r--r--   0        0        0     4305 2022-11-09 12:37:21.000000 lbvh-0.0.11/cpp/BVH.cpp
--rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 lbvh-0.0.11/cpp/BVH.hpp
--rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 lbvh-0.0.11/cpp/morton.hpp
--rw-r--r--   0        0        0     1524 2022-11-09 12:37:21.000000 lbvh-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     1099 2022-11-09 12:37:21.000000 lbvh-0.0.11/python/CMakeLists.txt
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 lbvh-0.0.11/python/numpy_test.py
--rw-r--r--   0        0        0     2789 2022-11-09 12:37:21.000000 lbvh-0.0.11/python/python_bindings.cpp
--rw-r--r--   0        0        0     1040 2022-11-09 12:37:21.000000 lbvh-0.0.11/tests/CMakeLists.txt
--rw-r--r--   0        0        0     2459 2022-11-09 12:37:21.000000 lbvh-0.0.11/tests/aabb_correctness_test.cpp
--rw-r--r--   0        0        0     1497 2022-11-09 12:37:21.000000 lbvh-0.0.11/tests/bvh_correctness_test.cpp
--rw-r--r--   0        0        0     2014 2022-11-09 12:37:21.000000 lbvh-0.0.11/tests/bvh_performance_test.cpp
--rw-r--r--   0        0        0   127890 2022-11-09 12:37:21.000000 lbvh-0.0.11/tests/nanobench.h
--rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 lbvh-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 lbvh-0.0.12/.github/dependabot.yml
+-rw-r--r--   0        0        0      768 2022-11-09 12:37:21.000000 lbvh-0.0.12/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1949 2022-11-09 12:37:21.000000 lbvh-0.0.12/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 lbvh-0.0.12/.gitignore
+-rw-r--r--   0        0        0     1215 2022-11-09 12:37:21.000000 lbvh-0.0.12/.vscode/settings.json
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 lbvh-0.0.12/CMakeLists.txt
+-rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 lbvh-0.0.12/LICENSE
+-rw-r--r--   0        0        0      404 2022-11-09 12:37:21.000000 lbvh-0.0.12/README.md
+-rw-r--r--   0        0        0     1619 2022-11-09 12:37:21.000000 lbvh-0.0.12/cpp/AABB.hpp
+-rw-r--r--   0        0        0     4305 2022-11-09 12:37:21.000000 lbvh-0.0.12/cpp/BVH.cpp
+-rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 lbvh-0.0.12/cpp/BVH.hpp
+-rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 lbvh-0.0.12/cpp/morton.hpp
+-rw-r--r--   0        0        0     1702 2022-11-09 12:37:21.000000 lbvh-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0     1103 2022-11-09 12:37:21.000000 lbvh-0.0.12/python/CMakeLists.txt
+-rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 lbvh-0.0.12/python/numpy_test.py
+-rw-r--r--   0        0        0     2789 2022-11-09 12:37:21.000000 lbvh-0.0.12/python/python_bindings.cpp
+-rw-r--r--   0        0        0      689 2022-11-09 12:37:21.000000 lbvh-0.0.12/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     2459 2022-11-09 12:37:21.000000 lbvh-0.0.12/tests/aabb_correctness_test.cpp
+-rw-r--r--   0        0        0     1447 2022-11-09 12:37:21.000000 lbvh-0.0.12/tests/bvh_correctness_test.cpp
+-rw-r--r--   0        0        0     2014 2022-11-09 12:37:21.000000 lbvh-0.0.12/tests/bvh_performance_test.cpp
+-rw-r--r--   0        0        0   127890 2022-11-09 12:37:21.000000 lbvh-0.0.12/tests/nanobench.h
+-rw-r--r--   0        0        0      896 2022-11-09 12:37:21.000000 lbvh-0.0.12/PKG-INFO
```

### Comparing `lbvh-0.0.11/.vscode/settings.json` & `lbvh-0.0.12/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/CMakeLists.txt` & `lbvh-0.0.12/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 file(GLOB lbvh_headers ${PROJECT_SOURCE_DIR}/cpp/*.hpp)
 file(GLOB lbvh_sources ${PROJECT_SOURCE_DIR}/cpp/*.cpp)
 add_library(libLBVH ${lbvh_sources} ${lbvh_headers})
 target_include_directories(libLBVH PUBLIC ${PROJECT_SOURCE_DIR}/cpp)
 set_target_properties(libLBVH PROPERTIES PREFIX "")
 
+if(UNIX AND NOT APPLE)
+  set_property(TARGET libLBVH PROPERTY POSITION_INDEPENDENT_CODE ON)
+endif()
+
 if (LBVH_ENABLE_PYTHON_BINDINGS)
   add_subdirectory(python)
 endif()
 
 if (LBVH_ENABLE_MATHEMATICA_BINDINGS)
   add_subdirectory(mathematica)
 endif()
```

### Comparing `lbvh-0.0.11/LICENSE` & `lbvh-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/cpp/AABB.hpp` & `lbvh-0.0.12/cpp/AABB.hpp`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/cpp/BVH.cpp` & `lbvh-0.0.12/cpp/BVH.cpp`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/cpp/BVH.hpp` & `lbvh-0.0.12/cpp/BVH.hpp`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/cpp/morton.hpp` & `lbvh-0.0.12/cpp/morton.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,25 @@
   return (n == 0) ? 64 : __builtin_clzll(n); 
 }
 
 inline uint32_t clz(uint32_t n) {
   return (n == 0) ? 32 : __builtin_clzll(n); 
 }
 #else
-//#ifdef _WIN32
+// windows
+inline uint64_t unpack64_msb(uint64_t ab, uint64_t shift = 32) {
+  uint64_t mask = (uint64_t(1) << shift) - 1;
+  return ((ab >> shift) & mask);
+}
+
+inline uint64_t unpack64_lsb(uint64_t ab, uint32_t shift = 32) {
+  uint64_t mask = (uint64_t(1) << shift) - 1;
+  return (ab & mask);
+}
+
 inline uint32_t clz(uint32_t n) {
   uint32_t index;
   uint8_t isNonzero = _BitScanReverse((unsigned long *)&index, n);
   return uint32_t(isNonzero ? 31 - index : 32);
 }
 
 inline uint32_t clz(uint64_t n) {
@@ -74,8 +84,8 @@
   uint64_t x = uint64_t(v[0] * scale);
   uint64_t y = uint64_t(v[1] * scale);
   uint64_t z = uint64_t(v[2] * scale);
 
   return (expand3(z) << 2) + (expand3(y) << 1) + expand3(x);
 } 
 
-}  // namespace morton
+}  // namespace morton
```

### Comparing `lbvh-0.0.11/pyproject.toml` & `lbvh-0.0.12/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 #requires = ["scikit-build-core >=0.4.3", "nanobind >=1.3.2"]
-requires = ["scikit-build-core >=0.4.3"]
+requires = ["scikit-build-core >=0.4.3", "numpy"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "LBVH"
-version = "0.0.11"
+version = "0.0.12"
 authors = [
   { name="Sam Mish", email="samuelpmish@gmail.com" },
 ]
 description = "A small bounding volume hierarchy implementation"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
@@ -44,14 +44,20 @@
 sdist.exclude = ["mathematica"]
 
 
 [tool.cibuildwheel]
 # Necessary to see build output from the actual compilation
 build-verbosity = 1
 
+# Skip PyPy, CPython 3.12, see https://github.com/pypa/pip/issues/11501
+skip = ["cp312-*", "pp*"]
+
+# Only target 64 bit architectures
+archs = ["auto64"] 
+
 # Run pytest to ensure that the package was correctly built
-test-command = "pytest {project}/tests"
-test-requires = "pytest"
+test-command = "python {project}/python/numpy_test.py"
+test-requires = "numpy"
 
 # Needed for full C++17 support
 [tool.cibuildwheel.macos.environment]
 MACOSX_DEPLOYMENT_TARGET = "10.14"
```

### Comparing `lbvh-0.0.11/python/CMakeLists.txt` & `lbvh-0.0.12/python/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 include(FetchContent)
 FetchContent_Declare(
   nanobind
-  GIT_REPOSITORY git@github.com:wjakob/nanobind.git
+  GIT_REPOSITORY https://github.com/wjakob/nanobind.git
 )
 FetchContent_MakeAvailable(nanobind)
 
 find_package(Python COMPONENTS Interpreter Development.Module REQUIRED)
 nanobind_add_module(
     
   # name, must match module name in python_bindings.cpp
```

### Comparing `lbvh-0.0.11/python/python_bindings.cpp` & `lbvh-0.0.12/python/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/tests/aabb_correctness_test.cpp` & `lbvh-0.0.12/tests/aabb_correctness_test.cpp`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/tests/bvh_correctness_test.cpp` & `lbvh-0.0.12/tests/bvh_correctness_test.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -46,17 +46,15 @@
 
   EXPECT_EQ(pairs1.size(), pairs2.size());
 
   std::sort(pairs1.begin(), pairs1.end());
   std::sort(pairs2.begin(), pairs2.end());
 
   for (int i = 0; i < pairs1.size(); i++) {
-    for (int d = 0; d < dim; d++) {
-      EXPECT_EQ(pairs1[i][d], pairs2[i][d]);
-    }
+    EXPECT_EQ(pairs1[i], pairs2[i]);
   }
 
 }
 
 TEST(UnitTest, BVHIntersection2D) {
   run_test<2>(1000);
 }
```

### Comparing `lbvh-0.0.11/tests/bvh_performance_test.cpp` & `lbvh-0.0.12/tests/bvh_performance_test.cpp`

 * *Files identical despite different names*

### Comparing `lbvh-0.0.11/tests/nanobench.h` & `lbvh-0.0.12/tests/nanobench.h`

 * *Files identical despite different names*

