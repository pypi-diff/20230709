# Comparing `tmp/Texo-0.0.3.tar.gz` & `tmp/Texo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Texo-0.0.3.tar", last modified: Mon Jun 26 16:50:20 2023, max compression
+gzip compressed data, was "Texo-0.0.4.tar", last modified: Sun Jul  9 15:33:34 2023, max compression
```

## Comparing `Texo-0.0.3.tar` & `Texo-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:50:20.196105 Texo-0.0.3/
--rw-rw-rw-   0        0        0     2958 2023-06-26 16:50:20.194106 Texo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2149 2023-06-26 16:41:59.000000 Texo-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 16:50:20.196105 Texo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-06-26 16:49:15.000000 Texo-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:50:20.179057 Texo-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 16:50:20.182449 Texo-0.0.3/src/Texo/
--rw-rw-rw-   0        0        0     3462 2023-06-26 16:35:17.000000 Texo-0.0.3/src/Texo/Unet.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:50:20.192109 Texo-0.0.3/src/Texo.egg-info/
--rw-rw-rw-   0        0        0     2958 2023-06-26 16:50:19.000000 Texo-0.0.3/src/Texo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-26 16:50:20.000000 Texo-0.0.3/src/Texo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:50:19.000000 Texo-0.0.3/src/Texo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-26 16:50:19.000000 Texo-0.0.3/src/Texo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-26 16:50:19.000000 Texo-0.0.3/src/Texo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 15:33:34.787469 Texo-0.0.4/
+-rw-rw-rw-   0        0        0     3567 2023-07-09 15:33:34.786468 Texo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2758 2023-07-09 15:30:56.000000 Texo-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:33:34.788471 Texo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-09 15:31:49.000000 Texo-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:33:34.754080 Texo-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 15:33:34.761676 Texo-0.0.4/src/Texo/
+-rw-rw-rw-   0        0        0     3462 2023-06-26 16:35:17.000000 Texo-0.0.4/src/Texo/Unet.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:33:34.784466 Texo-0.0.4/src/Texo.egg-info/
+-rw-rw-rw-   0        0        0     3567 2023-07-09 15:33:34.000000 Texo-0.0.4/src/Texo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-09 15:33:34.000000 Texo-0.0.4/src/Texo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:33:34.000000 Texo-0.0.4/src/Texo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-09 15:33:34.000000 Texo-0.0.4/src/Texo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 15:33:34.000000 Texo-0.0.4/src/Texo.egg-info/top_level.txt
```

### Comparing `Texo-0.0.3/PKG-INFO` & `Texo-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: Texo
-Version: 0.0.3
-Summary: Sentiment Analysis Multiple language and for all products
-Home-page: https://github.com/Sourabh20022002/Texo
-Download-URL: https://github.com/Sourabh20022002/Texo/archive/refs/tags/python.tar.gz
-Author: Sourabh singh
-Author-email: Sourabh52.singh@gmail.com
-Keywords: python,Sentiment,NLP,Tokenizer,Text-Analyzer,sockets,torch,PIL,torchvision
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
 # Texo
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 Developed by Sourabh Singh from Neuroins(c) 2023
 
 ## Examples of How To Use (Buggy Alpha Version)
@@ -79,7 +61,32 @@
 from Texo.Unet import UnetM
 im = UnetM()
 im.Imageprepocess('image_path')
 
 #Display image
 im.show()
 ```
+
+Tokenize of Text and pos
+```python
+from Texo.Word.texo import tex
+
+#tokenize text without stop-words
+tokenize = tex()
+words = tokenize.tokenize('This is going Awesome')
+print(words)
+
+#tokenize text with stop-words
+tokenize = tex()
+words = tokenize.tokenize_stopwords('This is going Awesome')
+print(words)
+
+#find POS from tokens and return pos in form of array
+tokenize = tex()
+tokens = ['Running', 'dogs', 'are', 'happier', 'than', 'walked', 'dogs', 'in', 'parks.']
+words = tokenize.pos_tag(tokens)
+print(words)
+
+#return output in form of token of array
+#Display image
+im.show()
+```
```

### Comparing `Texo-0.0.3/setup.py` & `Texo-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md","r") as fh:
     long_desc = fh.read()
 
 
 setup(
     name='Texo',
-    version='0.0.3',
+    version='0.0.4',
     description='Sentiment Analysis Multiple language and for all products',
     author='Sourabh singh',
     author_email='Sourabh52.singh@gmail.com',
     long_description=long_desc,
     long_description_content_type = "text/markdown",
     package_dir={'':'src'},
     url='https://github.com/Sourabh20022002/Texo',
```

### Comparing `Texo-0.0.3/src/Texo/Unet.py` & `Texo-0.0.4/src/Texo/Unet.py`

 * *Files identical despite different names*

### Comparing `Texo-0.0.3/src/Texo.egg-info/PKG-INFO` & `Texo-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Texo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sentiment Analysis Multiple language and for all products
 Home-page: https://github.com/Sourabh20022002/Texo
 Download-URL: https://github.com/Sourabh20022002/Texo/archive/refs/tags/python.tar.gz
 Author: Sourabh singh
 Author-email: Sourabh52.singh@gmail.com
 Keywords: python,Sentiment,NLP,Tokenizer,Text-Analyzer,sockets,torch,PIL,torchvision
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,7 +79,32 @@
 from Texo.Unet import UnetM
 im = UnetM()
 im.Imageprepocess('image_path')
 
 #Display image
 im.show()
 ```
+
+Tokenize of Text and pos
+```python
+from Texo.Word.texo import tex
+
+#tokenize text without stop-words
+tokenize = tex()
+words = tokenize.tokenize('This is going Awesome')
+print(words)
+
+#tokenize text with stop-words
+tokenize = tex()
+words = tokenize.tokenize_stopwords('This is going Awesome')
+print(words)
+
+#find POS from tokens and return pos in form of array
+tokenize = tex()
+tokens = ['Running', 'dogs', 'are', 'happier', 'than', 'walked', 'dogs', 'in', 'parks.']
+words = tokenize.pos_tag(tokens)
+print(words)
+
+#return output in form of token of array
+#Display image
+im.show()
+```
```

