# Comparing `tmp/text2text-1.2.5.tar.gz` & `tmp/text2text-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.2.5.tar", last modified: Sun Jul  9 03:12:43 2023, max compression
+gzip compressed data, was "text2text-1.2.6.tar", last modified: Sun Jul  9 03:23:34 2023, max compression
```

## Comparing `text2text-1.2.5.tar` & `text2text-1.2.6.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:12:43.085440 text2text-1.2.5/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-07-09 02:37:27.000000 text2text-1.2.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    56262 2023-07-09 03:12:43.084440 text2text-1.2.5/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    55448 2023-07-09 02:37:27.000000 text2text-1.2.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 03:12:43.085440 text2text-1.2.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1283 2023-07-09 02:39:42.000000 text2text-1.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:12:43.081440 text2text-1.2.5/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      603 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:12:43.083440 text2text-1.2.5/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:12:43.084440 text2text-1.2.5/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-07-09 02:37:27.000000 text2text-1.2.5/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:12:43.082440 text2text-1.2.5/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    56262 2023-07-09 03:12:42.000000 text2text-1.2.5/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2023-07-09 03:12:42.000000 text2text-1.2.5/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 03:12:42.000000 text2text-1.2.5/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-09 03:12:42.000000 text2text-1.2.5/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-09 03:12:42.000000 text2text-1.2.5/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:23:34.989676 text2text-1.2.6/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-07-09 03:20:10.000000 text2text-1.2.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-07-09 03:23:34.988675 text2text-1.2.6/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    55448 2023-07-09 03:20:10.000000 text2text-1.2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 03:23:34.989676 text2text-1.2.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1283 2023-07-09 03:20:24.000000 text2text-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:23:34.984675 text2text-1.2.6/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      603 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:23:34.986675 text2text-1.2.6/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/indexer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:23:34.987676 text2text-1.2.6/text2text/langchain/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-09 03:21:56.000000 text2text-1.2.6/text2text/langchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/langchain/stfidf.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-09 03:21:32.000000 text2text-1.2.6/text2text/langchain/test_stfidf.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-09 03:21:49.000000 text2text-1.2.6/text2text/langchain/test_text2text_assistant.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/langchain/text2text_assistant.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:23:34.988675 text2text-1.2.6/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-07-09 03:21:25.000000 text2text-1.2.6/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-07-09 03:20:10.000000 text2text-1.2.6/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:23:34.985675 text2text-1.2.6/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-07-09 03:23:34.000000 text2text-1.2.6/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-07-09 03:23:34.000000 text2text-1.2.6/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 03:23:34.000000 text2text-1.2.6/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-09 03:23:34.000000 text2text-1.2.6/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-09 03:23:34.000000 text2text-1.2.6/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.2.5/LICENSE.txt` & `text2text-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/PKG-INFO` & `text2text-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.5
+Version: 1.2.6
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.2.5/README.md` & `text2text-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/setup.py` & `text2text-1.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.2.5",
+  version="1.2.6",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.2.5/text2text/__init__.py` & `text2text-1.2.6/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/abstractor.py` & `text2text-1.2.6/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/answerer.py` & `text2text-1.2.6/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/assistant.py` & `text2text-1.2.6/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/biunilm/loader_utils.py` & `text2text-1.2.6/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/biunilm/seq2seq_loader.py` & `text2text-1.2.6/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/bm25er.py` & `text2text-1.2.6/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/counter.py` & `text2text-1.2.6/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/fitter.py` & `text2text-1.2.6/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/handler.py` & `text2text-1.2.6/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/identifier.py` & `text2text-1.2.6/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/indexer.py` & `text2text-1.2.6/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/measurer.py` & `text2text-1.2.6/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.2.6/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.2.6/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.2.6/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.2.6/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.2.6/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/questioner.py` & `text2text-1.2.6/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/server.py` & `text2text-1.2.6/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/summarizer.py` & `text2text-1.2.6/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/tfidfer.py` & `text2text-1.2.6/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/tokenizer.py` & `text2text-1.2.6/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/transformer.py` & `text2text-1.2.6/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/translator.py` & `text2text-1.2.6/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text/vectorizer.py` & `text2text-1.2.6/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.5/text2text.egg-info/PKG-INFO` & `text2text-1.2.6/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.5
+Version: 1.2.6
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.2.5/text2text.egg-info/SOURCES.txt` & `text2text-1.2.6/text2text.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -25,13 +25,18 @@
 text2text.egg-info/SOURCES.txt
 text2text.egg-info/dependency_links.txt
 text2text.egg-info/requires.txt
 text2text.egg-info/top_level.txt
 text2text/biunilm/__init__.py
 text2text/biunilm/loader_utils.py
 text2text/biunilm/seq2seq_loader.py
+text2text/langchain/__init__.py
+text2text/langchain/stfidf.py
+text2text/langchain/test_stfidf.py
+text2text/langchain/test_text2text_assistant.py
+text2text/langchain/text2text_assistant.py
 text2text/pytorch_pretrained_bert/__init__.py
 text2text/pytorch_pretrained_bert/__main__.py
 text2text/pytorch_pretrained_bert/file_utils.py
 text2text/pytorch_pretrained_bert/loss.py
 text2text/pytorch_pretrained_bert/modeling.py
 text2text/pytorch_pretrained_bert/tokenization.py
```

