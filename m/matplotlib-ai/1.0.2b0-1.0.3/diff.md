# Comparing `tmp/matplotlib_ai-1.0.2b0.tar.gz` & `tmp/matplotlib_ai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_ai-1.0.2b0.tar", last modified: Sun Jul  9 21:18:44 2023, max compression
+gzip compressed data, was "matplotlib_ai-1.0.3.tar", last modified: Sun Jul  9 21:21:05 2023, max compression
```

## Comparing `matplotlib_ai-1.0.2b0.tar` & `matplotlib_ai-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 21:18:44.657092 matplotlib_ai-1.0.2b0/
--rw-r--r--   0 yorio      (501) staff       (20)     1066 2023-07-07 06:14:42.000000 matplotlib_ai-1.0.2b0/LICENSE
--rw-r--r--   0 yorio      (501) staff       (20)      856 2023-07-09 21:18:44.656902 matplotlib_ai-1.0.2b0/PKG-INFO
--rw-r--r--   0 yorio      (501) staff       (20)     2353 2023-07-08 19:26:28.000000 matplotlib_ai-1.0.2b0/README.md
-drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 21:18:44.656050 matplotlib_ai-1.0.2b0/matplotlib_ai/
--rw-rw-r--   0 yorio      (501) staff       (20)        0 2023-07-07 00:49:48.000000 matplotlib_ai-1.0.2b0/matplotlib_ai/__init__.py
--rw-rw-r--   0 yorio      (501) staff       (20)     4614 2023-07-09 21:17:50.000000 matplotlib_ai-1.0.2b0/matplotlib_ai/matplotlib_ai.py
-drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 21:18:44.656680 matplotlib_ai-1.0.2b0/matplotlib_ai.egg-info/
--rw-r--r--   0 yorio      (501) staff       (20)      856 2023-07-09 21:18:44.000000 matplotlib_ai-1.0.2b0/matplotlib_ai.egg-info/PKG-INFO
--rw-r--r--   0 yorio      (501) staff       (20)      231 2023-07-09 21:18:44.000000 matplotlib_ai-1.0.2b0/matplotlib_ai.egg-info/SOURCES.txt
--rw-r--r--   0 yorio      (501) staff       (20)        1 2023-07-09 21:18:44.000000 matplotlib_ai-1.0.2b0/matplotlib_ai.egg-info/dependency_links.txt
--rw-r--r--   0 yorio      (501) staff       (20)       14 2023-07-09 21:18:44.000000 matplotlib_ai-1.0.2b0/matplotlib_ai.egg-info/top_level.txt
--rw-r--r--   0 yorio      (501) staff       (20)       38 2023-07-09 21:18:44.657150 matplotlib_ai-1.0.2b0/setup.cfg
--rw-r--r--   0 yorio      (501) staff       (20)     1007 2023-07-09 21:18:37.000000 matplotlib_ai-1.0.2b0/setup.py
+drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 21:21:05.322446 matplotlib_ai-1.0.3/
+-rw-r--r--   0 yorio      (501) staff       (20)     1066 2023-07-07 06:14:42.000000 matplotlib_ai-1.0.3/LICENSE
+-rw-r--r--   0 yorio      (501) staff       (20)      854 2023-07-09 21:21:05.322167 matplotlib_ai-1.0.3/PKG-INFO
+-rw-r--r--   0 yorio      (501) staff       (20)     2353 2023-07-08 19:26:28.000000 matplotlib_ai-1.0.3/README.md
+drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 21:21:05.321069 matplotlib_ai-1.0.3/matplotlib_ai/
+-rw-rw-r--   0 yorio      (501) staff       (20)        0 2023-07-07 00:49:48.000000 matplotlib_ai-1.0.3/matplotlib_ai/__init__.py
+-rw-rw-r--   0 yorio      (501) staff       (20)     4614 2023-07-09 21:17:50.000000 matplotlib_ai-1.0.3/matplotlib_ai/matplotlib_ai.py
+drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 21:21:05.321866 matplotlib_ai-1.0.3/matplotlib_ai.egg-info/
+-rw-r--r--   0 yorio      (501) staff       (20)      854 2023-07-09 21:21:05.000000 matplotlib_ai-1.0.3/matplotlib_ai.egg-info/PKG-INFO
+-rw-r--r--   0 yorio      (501) staff       (20)      231 2023-07-09 21:21:05.000000 matplotlib_ai-1.0.3/matplotlib_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 yorio      (501) staff       (20)        1 2023-07-09 21:21:05.000000 matplotlib_ai-1.0.3/matplotlib_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 yorio      (501) staff       (20)       14 2023-07-09 21:21:05.000000 matplotlib_ai-1.0.3/matplotlib_ai.egg-info/top_level.txt
+-rw-r--r--   0 yorio      (501) staff       (20)       38 2023-07-09 21:21:05.322532 matplotlib_ai-1.0.3/setup.cfg
+-rw-r--r--   0 yorio      (501) staff       (20)     1002 2023-07-09 21:20:50.000000 matplotlib_ai-1.0.3/setup.py
```

### Comparing `matplotlib_ai-1.0.2b0/LICENSE` & `matplotlib_ai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_ai-1.0.2b0/PKG-INFO` & `matplotlib_ai-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib_ai
-Version: 1.0.2b0
+Version: 1.0.3
 Summary: A GPT-powered tool to bring no-code data visualization to life!
 Home-page: https://github.com/notY0rick/mpl_ai
 Author: Yorick Chern
 Author-email: yorichek.007@gmail.com
 License: MIT
 Keywords: python,gpt,matplotlib,no code,LLM
 Platform: UNKNOWN
```

### Comparing `matplotlib_ai-1.0.2b0/README.md` & `matplotlib_ai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib_ai-1.0.2b0/matplotlib_ai/matplotlib_ai.py` & `matplotlib_ai-1.0.3/matplotlib_ai/matplotlib_ai.py`

 * *Files identical despite different names*

### Comparing `matplotlib_ai-1.0.2b0/matplotlib_ai.egg-info/PKG-INFO` & `matplotlib_ai-1.0.3/matplotlib_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib-ai
-Version: 1.0.2b0
+Version: 1.0.3
 Summary: A GPT-powered tool to bring no-code data visualization to life!
 Home-page: https://github.com/notY0rick/mpl_ai
 Author: Yorick Chern
 Author-email: yorichek.007@gmail.com
 License: MIT
 Keywords: python,gpt,matplotlib,no code,LLM
 Platform: UNKNOWN
```

### Comparing `matplotlib_ai-1.0.2b0/setup.py` & `matplotlib_ai-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 The package dependencies require openai and matplotlib, and it is unbelievably easy to use. 
 Calling OpenAI's GPT API, prompt engineering, and using few-shot learning, matplotlib_ai is capable 
 of generating graphs without requiring you to write a single line of matplotlib code! Check out this GitHub link:
 https://github.com/notY0rick/matplotlib_ai
 """
 
 setup(name='matplotlib_ai',
-      version='1.0.2-beta',
+      version='1.0.3',
       description='A GPT-powered tool to bring no-code data visualization to life!',
       long_description=LONG_DESC,
       author='Yorick Chern',
       author_email='yorichek.007@gmail.com',
       url='https://github.com/notY0rick/mpl_ai',
       packages=find_packages(),
       keywords=['python', 'gpt', 'matplotlib', 'no code', 'LLM'],
```

