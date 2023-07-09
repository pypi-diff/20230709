# Comparing `tmp/zein-0.0.4.tar.gz` & `tmp/zein-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zein-0.0.4.tar", last modified: Tue Jun 27 09:14:50 2023, max compression
+gzip compressed data, was "zein-0.0.5.tar", last modified: Sun Jul  9 12:38:33 2023, max compression
```

## Comparing `zein-0.0.4.tar` & `zein-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.329738 zein-0.0.4/
--rw-rw-rw-   0        0        0     1070 2023-06-27 06:45:13.000000 zein-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      742 2023-06-27 09:14:50.328740 zein-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-06-27 06:53:20.000000 zein-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 09:14:50.329738 zein-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1156 2023-06-27 09:14:14.000000 zein-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.306771 zein-0.0.4/zein/
--rw-rw-rw-   0        0        0       36 2023-06-27 07:49:23.000000 zein-0.0.4/zein/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.325749 zein-0.0.4/zein/data/
--rw-rw-rw-   0        0        0      630 2023-06-25 15:14:01.000000 zein-0.0.4/zein/data/data.csv
--rw-rw-rw-   0        0        0       61 2023-06-27 09:13:02.000000 zein-0.0.4/zein/main.py
--rw-rw-rw-   0        0        0     2100 2023-06-27 09:12:37.000000 zein-0.0.4/zein/text.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:14:50.322759 zein-0.0.4/zein.egg-info/
--rw-rw-rw-   0        0        0      742 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-27 09:14:49.000000 zein-0.0.4/zein.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-27 09:14:50.000000 zein-0.0.4/zein.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.037207 zein-0.0.5/
+-rw-rw-rw-   0        0        0     1070 2023-07-03 16:08:37.000000 zein-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      831 2023-07-09 12:38:33.037207 zein-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1783 2023-07-03 16:08:38.000000 zein-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 12:38:33.037207 zein-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2023-07-09 12:38:23.000000 zein-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.002013 zein-0.0.5/zein/
+-rw-rw-rw-   0        0        0       42 2023-07-03 20:47:55.000000 zein-0.0.5/zein/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.021586 zein-0.0.5/zein/images/
+-rw-rw-rw-   0        0        0       39 2023-07-03 16:08:38.000000 zein-0.0.5/zein/images/__init__.py
+-rw-rw-rw-   0        0        0     2094 2023-07-09 12:05:54.000000 zein-0.0.5/zein/images/_utils.py
+-rw-rw-rw-   0        0        0     4148 2023-07-08 19:32:14.000000 zein-0.0.5/zein/images/images_module.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.021586 zein-0.0.5/zein/text/
+-rw-rw-rw-   0        0        0       35 2023-07-03 16:08:40.000000 zein-0.0.5/zein/text/__init__.py
+-rw-rw-rw-   0        0        0     1650 2023-07-09 12:29:03.000000 zein-0.0.5/zein/text/_utils.py
+-rw-rw-rw-   0        0        0     3271 2023-07-09 12:03:46.000000 zein-0.0.5/zein/text/ar.py
+-rw-rw-rw-   0        0        0      583 2023-07-08 19:30:44.000000 zein-0.0.5/zein/text/text_module.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:38:33.017387 zein-0.0.5/zein.egg-info/
+-rw-rw-rw-   0        0        0      831 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       69 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 12:38:32.000000 zein-0.0.5/zein.egg-info/top_level.txt
```

### Comparing `zein-0.0.4/LICENSE.txt` & `zein-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zein-0.0.4/PKG-INFO` & `zein-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for ensuring the safety and security of ML models
+Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
+License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Provides-Extra: scikit-learn
 License-File: LICENSE.txt
 
 A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community
+
```

### Comparing `zein-0.0.4/README.md` & `zein-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 <div align="center">
   <img src="logo.png" alt="Ather logo" width="400" height="auto" />
-  <h1>aman</h1>
+  <h1>zein</h1>
   <p> A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community.</p>
 
 </div>
 
 ### Library Mission
 - The package includes a module that filters out profane words in Arabic text, using a comprehensive list of swear words and a smart algorithm that can handle variations and misspellings.
 - The package also includes a module that detects offensive sentences that insult or mock any of the Abrahamic religions (Islam, Christianity, Judaism), or any person or institution associated with them. The module uses natural language processing and sentiment analysis to identify the tone and intention of the sentences.
 - The package further includes a module that detects sexual images, or images that disrespect or ridicule any of the prophets or sacred symbols of the Abrahamic religions. The module uses computer vision and deep learning to classify and flag the images.
   
   <!-- About the Project -->
 ## ⬇️: Installation
 Install using `pip <http://www.pip-installer.org/en/latest/>`__ with:
 
-    pip install aman
+    pip install zein
 
 Or, `download a wheel or source archive from
-PyPI <https://pypi.python.org/pypi/aman>`__.
+PyPI <https://pypi.python.org/pypi/zein>`__.
 
 ## 🧑‍🤝‍🧑: Call for Contributions
-<p>We Need Your Help The aman project values your skills and passion!</p>
+<p>We Need Your Help The zein project values your skills and passion!</p>
 <p>We appreciate any small enhancements or fixes you can make. If you want to make bigger changes to the source code, please let us know through the mailing list first.</p>
 
 There are many other ways to contribute to NumPy besides writing code. You can also:
 - Help us manage new and old issues
 - Create tutorials, presentations, and other learning materials
 - Evaluate pull requests
```

### Comparing `zein-0.0.4/setup.py` & `zein-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+
+VERSION = '0.0.5'
 DESCRIPTION = 'A python library for ensuring the safety and security of ML models'
 LONG_DESCRIPTION = 'A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community'
 
 # Setting up
 setup(
     name="zein",
     version=VERSION,
@@ -17,18 +18,25 @@
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     package_data= {
       'zein': ['data/*.csv'],
     },
     include_package_data=True,
     zip_safe=False,
-    install_requires=['pandas'],
+    install_requires=['pandas', 'pickle', 'tensorflow==2.6.0'],
+    extras_require={
+        "scikit-learn": ["scikit-learn>=0.24.2"],
+    },
     keywords=['python','arabic filtering', 'text filtering', 'profanity check'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
+
+
+
+
```

### Comparing `zein-0.0.4/zein/text.py` & `zein-0.0.5/zein/text/ar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,84 @@
+from pandas.io.formats.style import format_table_styles
+from ._utils import clean_txt, check_text
 import pandas as pd
 import re
 import pkg_resources
+import os
+import pickle
+from sklearn.feature_extraction.text import TfidfVectorizer
 
 
-class ArabicFilter():
-    def __init__(self, path: object = pkg_resources.resource_filename('zein', 'data/data.csv')) -> object:  # default argument
-        # instance variable
+class ar():
+    def __init__(self, path: object = os.path.join(
+            os.path.dirname(__file__), "data/data.csv")) -> object:  # default argument
         self.insulting_words = pd.read_csv(path)
-
-    def censor(self, text: str) -> str:
-        # compile a regular expression pattern
-        pattern = re.compile('|'.join(self.insulting_words['words']), re.IGNORECASE)
-
-        # replace the matching words with asterisks
-        censored = re.sub(pattern, lambda m: '*' * len(m.group()), text)
-        return censored
+        # load the vectorizer and the model
+        self.prompt_vectorizer = pickle.load(open("models/prompt_vectorizer.pkl", "rb"))
+        self.prompt_model = pickle.load(open("models/prompt_svm_model.pkl", "rb"))
+
+    def censor(self, text: str, symbol='*') -> str:
+        if check_text(text) == 'OFF':
+            # Compile a regular expression pattern.
+            pattern = re.compile('|'.join(self.insulting_words['words']), re.IGNORECASE)
+
+            # Replace the matching words with asterisks.
+            censored_text = re.sub(pattern, lambda match: symbol * len(match.group()), text)
+
+            # Return the censored text.
+            return censored_text
+        else:
+            return text
 
     def is_profane(self, text: str) -> bool:
-        # compile a regular expression pattern
-        pattern = re.compile('|'.join(self.insulting_words['words']), re.IGNORECASE)
-
-        # check if the text matches the pattern
-        match = re.search(pattern, text)
-
-        # return True if there is a match, False otherwise
-        return bool(match)
+        if check_text(text) == 'OFF':
+            # compile a regular expression pattern
+            pattern = re.compile('|'.join(self.insulting_words['words']), re.IGNORECASE)
+
+            # check if the text matches the pattern
+            match = re.search(pattern, text)
+
+            # return True if there is a match, False otherwise
+            return bool(match)
+        else:
+            return False
 
     def find_insulting_words(self, text: str) -> list:
         # create an empty list to store the results
         results = []
 
         # split the text into words
         words = text.split()
 
         # loop through the words and their indices
         for index, word in enumerate(words):
-            # loop through the insulting words
-            for insult in self.insulting_words['words']:
-                # create a regular expression pattern with some variations
-                # for example, allow optional spaces and punctuation around the word
-                pattern = re.compile(r'\s*[.,:;!?]*\s*' + insult + r'\s*[.,:;!?]*\s*', re.IGNORECASE)
-                # check if the word matches the pattern
-                match = re.search(pattern, word)
-                # if there is a match, append a tuple of the word and the index to the results list
-                if match:
-                    results.append((word, index))
-                    # break the inner loop to avoid duplicate matches
-                    break
+            if check_text(text) == 'OFF':
+                # loop through the insulting words
+                for insult in self.insulting_words['words']:
+                    # create a regular expression pattern with some variations
+                    # for example, allow optional spaces and punctuation around the word
+                    pattern = re.compile(r'\s*[.,:;!?]*\s*' + insult + r'\s*[.,:;!?]*\s*', re.IGNORECASE)
+                    # check if the word matches the pattern
+                    match = re.search(pattern, word)
+                    # if there is a match, append a tuple of the word and the index to the results list
+                    if match:
+                        results.append((word, index))
+                        # break the inner loop to avoid duplicate matches
+                        break
+            else:
+                return None
 
         # return the results list
-        return results
+        return results
+    
+    def check_prompt(self, text: str) -> bool:
+      # transform the text into features using the vectorizer
+      features = self.prompt_vectorizer.transform([clean_txt(text)])
+      # predict the label using the model
+      label = self.prompt_model.predict(features)[0]
+
+      if label == 1:
+        return True
+      else:
+        return False
+
+
```

### Comparing `zein-0.0.4/zein.egg-info/PKG-INFO` & `zein-0.0.5/zein.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: zein
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for ensuring the safety and security of ML models
+Home-page: UNKNOWN
 Author: Mohamed Elsayed
 Author-email: <mohamedelsayed3487@gmail.com>
+License: UNKNOWN
 Keywords: python,arabic filtering,text filtering,profanity check
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Provides-Extra: scikit-learn
 License-File: LICENSE.txt
 
 A python library for ensuring the safety and security of ML models and their outputs for the Arabic and Islamic community
+
```

