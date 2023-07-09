# Comparing `tmp/learn-diffusion-0.0.1.tar.gz` & `tmp/learn-diffusion-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learn-diffusion-0.0.1.tar", last modified: Sun Jul  9 17:20:56 2023, max compression
+gzip compressed data, was "learn-diffusion-0.0.2.tar", last modified: Sun Jul  9 17:48:26 2023, max compression
```

## Comparing `learn-diffusion-0.0.1.tar` & `learn-diffusion-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 17:20:56.831314 learn-diffusion-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-09 16:22:05.000000 learn-diffusion-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-07-09 17:14:12.000000 learn-diffusion-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1119 2023-07-09 17:20:56.832300 learn-diffusion-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-07-09 16:42:50.000000 learn-diffusion-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 17:20:56.812355 learn-diffusion-0.0.1/learn-diffusion/
--rw-rw-rw-   0        0        0       22 2023-07-09 17:18:14.000000 learn-diffusion-0.0.1/learn-diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:20:56.827341 learn-diffusion-0.0.1/learn_diffusion.egg-info/
--rw-rw-rw-   0        0        0     1119 2023-07-09 17:20:56.000000 learn-diffusion-0.0.1/learn_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-09 17:20:56.000000 learn-diffusion-0.0.1/learn_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 17:20:56.000000 learn-diffusion-0.0.1/learn_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      262 2023-07-09 17:20:56.000000 learn-diffusion-0.0.1/learn_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 17:20:56.000000 learn-diffusion-0.0.1/learn_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-09 17:14:23.000000 learn-diffusion-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       13 2023-07-09 17:19:29.000000 learn-diffusion-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      207 2023-07-09 17:20:56.834294 learn-diffusion-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2232 2023-07-09 17:18:14.000000 learn-diffusion-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:20:56.829310 learn-diffusion-0.0.1/tests/
--rw-rw-rw-   0        0        0      851 2023-07-09 17:20:50.000000 learn-diffusion-0.0.1/tests/test_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:48:26.631898 learn-diffusion-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-09 16:22:05.000000 learn-diffusion-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-07-09 17:14:12.000000 learn-diffusion-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1023 2023-07-09 17:48:26.631898 learn-diffusion-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-07-09 16:42:50.000000 learn-diffusion-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 17:48:26.627910 learn-diffusion-0.0.2/learn_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     1023 2023-07-09 17:48:26.000000 learn-diffusion-0.0.2/learn_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-07-09 17:48:26.000000 learn-diffusion-0.0.2/learn_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 17:48:26.000000 learn-diffusion-0.0.2/learn_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-09 17:48:26.000000 learn-diffusion-0.0.2/learn_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 17:48:26.000000 learn-diffusion-0.0.2/learn_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-09 17:14:23.000000 learn-diffusion-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       64 2023-07-09 17:46:34.000000 learn-diffusion-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      207 2023-07-09 17:48:26.639877 learn-diffusion-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-07-09 17:48:01.000000 learn-diffusion-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:48:26.629904 learn-diffusion-0.0.2/tests/
+-rw-rw-rw-   0        0        0      851 2023-07-09 17:20:50.000000 learn-diffusion-0.0.2/tests/test_diffusion.py
```

### Comparing `learn-diffusion-0.0.1/LICENSE` & `learn-diffusion-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `learn-diffusion-0.0.1/PKG-INFO` & `learn-diffusion-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: learn-diffusion
-Version: 0.0.1
-Summary: Easy to use class-balanced cross-entropy and focal loss implementation for Pytorch.
-Home-page: https://github.com/fcakyon/learn-diffusion
+Version: 0.0.2
+Summary: Learn Diffusion
+Home-page: https://github.com/kadirnar/learn-diffusion
 Author: 
-License: MIT
+License: Apache License 2.0
 Keywords: diffusion,stable-diffusion,midjourney
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,12 +17,10 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: dev
 License-File: LICENSE
 
 # learn-diffusion
```

### Comparing `learn-diffusion-0.0.1/learn_diffusion.egg-info/PKG-INFO` & `learn-diffusion-0.0.2/learn_diffusion.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: learn-diffusion
-Version: 0.0.1
-Summary: Easy to use class-balanced cross-entropy and focal loss implementation for Pytorch.
-Home-page: https://github.com/fcakyon/learn-diffusion
+Version: 0.0.2
+Summary: Learn Diffusion
+Home-page: https://github.com/kadirnar/learn-diffusion
 Author: 
-License: MIT
+License: Apache License 2.0
 Keywords: diffusion,stable-diffusion,midjourney
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,12 +17,10 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: dev
 License-File: LICENSE
 
 # learn-diffusion
```

### Comparing `learn-diffusion-0.0.1/setup.py` & `learn-diffusion-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,38 +19,25 @@
 def get_version():
     current_dir = os.path.abspath(os.path.dirname(__file__))
     version_file = os.path.join(current_dir, "learn-diffusion", "__init__.py")
     with io.open(version_file, encoding="utf-8") as f:
         return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
 
 
-_DEV_REQUIREMENTS = [
-    "black==21.7b0",
-    "flake8==3.9.2",
-    "isort==5.9.2",
-    "click==8.0.4",
-    "importlib-metadata>=1.1.0,<4.3;python_version<'3.8'",
-]
-
-extras = {"tests": _DEV_REQUIREMENTS, "dev": _DEV_REQUIREMENTS}
-
-
 setuptools.setup(
     name="learn-diffusion",
     version=get_version(),
     author="",
-    license="MIT",
-    description="Easy to use class-balanced cross-entropy and focal loss implementation for Pytorch.",
+    license="Apache License 2.0",
+    description="Learn Diffusion",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
-    url="https://github.com/fcakyon/learn-diffusion",
-    packages=setuptools.find_packages(exclude=["tests"]),
+    url="https://github.com/kadirnar/learn-diffusion",
     python_requires=">=3.7",
     install_requires=get_requirements(),
-    extras_require=extras,
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
```

### Comparing `learn-diffusion-0.0.1/tests/test_diffusion.py` & `learn-diffusion-0.0.2/tests/test_diffusion.py`

 * *Files identical despite different names*

