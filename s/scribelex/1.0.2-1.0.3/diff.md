# Comparing `tmp/scribelex-1.0.2.tar.gz` & `tmp/scribelex-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribelex-1.0.2.tar", last modified: Sat Jul  8 21:06:39 2023, max compression
+gzip compressed data, was "scribelex-1.0.3.tar", last modified: Sat Jul  8 21:59:01 2023, max compression
```

## Comparing `scribelex-1.0.2.tar` & `scribelex-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 21:06:39.838863 scribelex-1.0.2/
--rw-rw-rw-   0        0        0     1086 2023-07-08 20:43:01.000000 scribelex-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1595 2023-07-08 21:06:39.837863 scribelex-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-08 21:06:39.838863 scribelex-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1289 2023-07-08 21:06:36.000000 scribelex-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 21:06:39.826862 scribelex-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 21:06:39.837863 scribelex-1.0.2/src/scribelex.egg-info/
--rw-rw-rw-   0        0        0     1595 2023-07-08 21:06:39.000000 scribelex-1.0.2/src/scribelex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-07-08 21:06:39.000000 scribelex-1.0.2/src/scribelex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 21:06:39.000000 scribelex-1.0.2/src/scribelex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 21:06:39.000000 scribelex-1.0.2/src/scribelex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:59:01.026227 scribelex-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-08 21:58:57.000000 scribelex-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-08 21:59:01.026227 scribelex-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-08 21:58:57.000000 scribelex-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:59:01.026227 scribelex-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-08 21:58:57.000000 scribelex-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:59:01.026227 scribelex-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:59:01.026227 scribelex-1.0.3/src/scribelex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-08 21:59:01.000000 scribelex-1.0.3/src/scribelex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-08 21:59:01.000000 scribelex-1.0.3/src/scribelex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:59:01.000000 scribelex-1.0.3/src/scribelex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:59:01.000000 scribelex-1.0.3/src/scribelex.egg-info/top_level.txt
```

### Comparing `scribelex-1.0.2/PKG-INFO` & `scribelex-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1
-Name: scribelex
-Version: 1.0.2
-Summary: Scribelex is a lightweight Python library for building parser combinators.
-Home-page: https://github.com/UncleDrema/scribelex
-Author: UncleDrema
-Author-email: missl.wipiece@gmail.com
-License: MIT
-Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# scribelex
-scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
-
-## Установка
-
-Вы можете установить scribelex с помощью pip:
-
-```bash
-pip install scribelex
-```
-
-## Лицензия
-
-Этот проект лицензирован под лицензией MIT. Подробнее смотрите файл [LICENSE](LICENSE).
+Metadata-Version: 2.1
+Name: scribelex
+Version: 1.0.3
+Summary: Scribelex is a lightweight Python library for building parser combinators.
+Home-page: https://github.com/UncleDrema/scribelex
+Author: UncleDrema
+Author-email: missl.wipiece@gmail.com
+License: MIT
+Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# scribelex
+scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
+
+## Установка
+
+Вы можете установить scribelex с помощью pip:
+
+```bash
+pip install scribelex
+```
+
+## Лицензия
+
+Этот проект лицензирован под лицензией MIT.
+Подробнее смотрите файл [LICENSE](LICENSE).
```

### Comparing `scribelex-1.0.2/setup.py` & `scribelex-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setup(
-    name="scribelex",
-    version="1.0.2",
-    author="UncleDrema",
-    author_email="missl.wipiece@gmail.com",
-    description="Scribelex is a lightweight Python library for building parser combinators.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    keywords=["parser", "parsing", "combinator", "library", "Python", "structured data", "grammar", "syntax", "parsing toolkit"],
-    url="https://github.com/UncleDrema/scribelex",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
-    license="MIT",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setup(
+    name="scribelex",
+    version="1.0.3",
+    author="UncleDrema",
+    author_email="missl.wipiece@gmail.com",
+    description="Scribelex is a lightweight Python library for building parser combinators.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    keywords=["parser", "parsing", "combinator", "library", "Python", "structured data", "grammar", "syntax", "parsing toolkit"],
+    url="https://github.com/UncleDrema/scribelex",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    license="MIT",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
 )
```

### Comparing `scribelex-1.0.2/src/scribelex.egg-info/PKG-INFO` & `scribelex-1.0.3/src/scribelex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1
-Name: scribelex
-Version: 1.0.2
-Summary: Scribelex is a lightweight Python library for building parser combinators.
-Home-page: https://github.com/UncleDrema/scribelex
-Author: UncleDrema
-Author-email: missl.wipiece@gmail.com
-License: MIT
-Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# scribelex
-scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
-
-## Установка
-
-Вы можете установить scribelex с помощью pip:
-
-```bash
-pip install scribelex
-```
-
-## Лицензия
-
-Этот проект лицензирован под лицензией MIT. Подробнее смотрите файл [LICENSE](LICENSE).
+Metadata-Version: 2.1
+Name: scribelex
+Version: 1.0.3
+Summary: Scribelex is a lightweight Python library for building parser combinators.
+Home-page: https://github.com/UncleDrema/scribelex
+Author: UncleDrema
+Author-email: missl.wipiece@gmail.com
+License: MIT
+Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# scribelex
+scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
+
+## Установка
+
+Вы можете установить scribelex с помощью pip:
+
+```bash
+pip install scribelex
+```
+
+## Лицензия
+
+Этот проект лицензирован под лицензией MIT.
+Подробнее смотрите файл [LICENSE](LICENSE).
```

