# Comparing `tmp/kanonym4text-0.2.2.tar.gz` & `tmp/kanonym4text-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanonym4text-0.2.2.tar", last modified: Thu Jul  6 10:51:46 2023, max compression
+gzip compressed data, was "kanonym4text-0.2.3.tar", last modified: Sun Jul  9 15:09:38 2023, max compression
```

## Comparing `kanonym4text-0.2.2.tar` & `kanonym4text-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     5099 2023-07-01 20:45:19.000000 kanonym4text-0.2.2/README.md
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      119 2023-07-06 09:36:30.000000 kanonym4text-0.2.2/kanonym4text/__init__.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/data/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.2.2/kanonym4text/data/5000_most_common_words_by_order.txt
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/objects/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       52 2023-07-06 09:06:10.000000 kanonym4text-0.2.2/kanonym4text/objects/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8013 2023-07-06 10:20:08.000000 kanonym4text-0.2.2/kanonym4text/objects/kanonym.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text/utils/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.2.2/kanonym4text/utils/__init__.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13287 2023-07-06 10:50:11.000000 kanonym4text-0.2.2/kanonym4text/utils/anonym_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-06 10:17:19.000000 kanonym4text-0.2.2/kanonym4text/utils/cluster_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6024 2023-07-06 10:14:17.000000 kanonym4text-0.2.2/kanonym4text/utils/llm_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.2.2/kanonym4text/utils/models.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11168 2023-07-06 08:39:12.000000 kanonym4text-0.2.2/kanonym4text/utils/nlp_utils.py
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3152 2023-07-06 08:40:32.000000 kanonym4text-0.2.2/kanonym4text/utils/utilization_utils.py
-drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/kanonym4text.egg-info/
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/PKG-INFO
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      576 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/SOURCES.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/dependency_links.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/requires.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       13 2023-07-06 10:51:46.000000 kanonym4text-0.2.2/kanonym4text.egg-info/top_level.txt
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-06 10:51:46.337937 kanonym4text-0.2.2/setup.cfg
--rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1571 2023-07-06 10:51:34.000000 kanonym4text-0.2.2/setup.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     4896 2023-07-09 13:23:33.000000 kanonym4text-0.2.3/README.md
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/kanonym4text/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      119 2023-07-06 09:36:30.000000 kanonym4text-0.2.3/kanonym4text/__init__.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/kanonym4text/data/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    35592 2023-07-01 20:45:19.000000 kanonym4text-0.2.3/kanonym4text/data/5000_most_common_words_by_order.txt
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/kanonym4text/objects/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       52 2023-07-06 09:06:10.000000 kanonym4text-0.2.3/kanonym4text/objects/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8210 2023-07-09 14:14:56.000000 kanonym4text-0.2.3/kanonym4text/objects/kanonym.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/kanonym4text/utils/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        0 2023-07-01 20:45:19.000000 kanonym4text-0.2.3/kanonym4text/utils/__init__.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    13287 2023-07-06 10:50:11.000000 kanonym4text-0.2.3/kanonym4text/utils/anonym_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     8723 2023-07-06 10:17:19.000000 kanonym4text-0.2.3/kanonym4text/utils/cluster_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     6355 2023-07-09 14:30:42.000000 kanonym4text-0.2.3/kanonym4text/utils/llm_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      721 2023-07-05 07:09:39.000000 kanonym4text-0.2.3/kanonym4text/utils/models.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)    11168 2023-07-06 08:39:12.000000 kanonym4text-0.2.3/kanonym4text/utils/nlp_utils.py
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     3152 2023-07-06 08:40:32.000000 kanonym4text-0.2.3/kanonym4text/utils/utilization_utils.py
+drwxrwxr-x   0 neumanh   (1000) neumanh   (1001)        0 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/kanonym4text.egg-info/
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      869 2023-07-09 15:09:38.000000 kanonym4text-0.2.3/kanonym4text.egg-info/PKG-INFO
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      576 2023-07-09 15:09:38.000000 kanonym4text-0.2.3/kanonym4text.egg-info/SOURCES.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)        1 2023-07-09 15:09:38.000000 kanonym4text-0.2.3/kanonym4text.egg-info/dependency_links.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)      189 2023-07-09 15:09:38.000000 kanonym4text-0.2.3/kanonym4text.egg-info/requires.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       13 2023-07-09 15:09:38.000000 kanonym4text-0.2.3/kanonym4text.egg-info/top_level.txt
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)       38 2023-07-09 15:09:38.912281 kanonym4text-0.2.3/setup.cfg
+-rw-rw-r--   0 neumanh   (1000) neumanh   (1001)     1571 2023-07-09 15:09:00.000000 kanonym4text-0.2.3/setup.py
```

### Comparing `kanonym4text-0.2.2/PKG-INFO` & `kanonym4text-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kanonym4text
-Version: 0.2.2
+Version: 0.2.3
 Summary: k-anonymity for texts
 Home-page: https://github.com/neumanh/K-anonymity-fot-texts
 Author: Lior Trieman, Hadas Neuman
 Author-email: liortr30@gmail.com, hadas.doron@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.3.tar.gz
 Description: A package that takes a dataframe with a corpus and return an anonymized corpus
 Keywords: python,k-anonymity,privacy,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `kanonym4text-0.2.2/README.md` & `kanonym4text-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,131 +1,107 @@
-# kanon4text K-ANONYMITY GUARANTEE FOR TEXTS
+# kanonym4text K-anonymity guerantee for texts
 
 
 
-K Anonymity for text (or in short - kanon4text) is an open‑sourced library that receives a corpus from the user (*dataframe*) and returns a K-anonymized corpus with additional information about the anonymization process performed.
+K Anonymity for text (or in short - kanonym4text) is an open‑sourced library that receives a corpus from the user (*dataframe*) and returns a K-anonymized corpus with additional information about the anonymization process performed.
 kanon4txet is designed to be easily utilized, to **guarantee** anonymization at a certain level pre-defined by the user (k) while still preserving some of the text utilization properties. 
 This repo and package are part of our Y-Data data science final project, and we would love to hear your feedback and learn from it!
 
 ## Overview
 In this project, we aim to apply data science techniques to anonymize textual data while preserving their utility. K-Anonymity is a technique used to ensure that an individual in a dataset cannot be identified by linking their attributes to external information, by forcing each row to be identical to k-1 other rows The anonymized data can be used for various purposes like data sharing, research, and analysis without compromising privacy. We plan on creating a novel algorithm for k-anonymity. Specifically, we address the case of unstructured data items, such as texts. Using various NLP techniques, from classical to modern DL-based solutions, and testing the utility of the anonymized data.
 We have tested the library on two main datasets:
 1) Amazon dataset,
 2) Enron emails dataset
 
 We show it is able to generate anonymized corpora in both cases.
 
 ## Package High-Level Algorithm:
 
-1) Data Preprocessing: tokenization, stemming, and stop word removal.
+1) Data Preprocessing: tokenization, lemmatization, and stop word removal.
 2) K-Anonymization: Generalization and Reduction.
 3) Evaluation: Utilization is evaluated by embedding distance and semantic scores.
 4) Visualization: dataset properties prior to and post anonymization will be visualized (optional)
 
 
 
 
 # Getting Started
-You can get started with kanon4text immediately by installing it with pip:
+You can get started with kanonym4text immediately by installing it with pip:
 
 ## download package
 
-pip install kanon4text
+```
+pip install kanonym4text
+```
 
-import kanon4text
-
-## step 1 - creat a data frame from your corpus
+## Step 1 - creat a data frame from your corpus
 The code receives a data frame containing the corpus in the following format:
 "txt" - column with the texts (default column name)
 
-## step 2 - import the following: (TBD - need to some how insert to the package)
-
-import kanonym4text
-
-import pandas as pd
-
-import nltk
-
-nltk.download('vader_lexicon')
+## Step 2 - import the following and initializethe object
+Use [gensim word embedding model]([url](https://radimrehurek.com/gensim/models/word2vec.html#pretrained-models)) for you choice (default - *glove-twitter-25*) 
+```
+from kanonym4text import Kanonym
+kan = Kanonym()
+```
 
 ## Step 3 - read the df:
-
+```
+import pandas as pd
 df = pd.read_csv('YOUR_FILE.csv')
+```
 
 ## Step 4 -  run the anonymization process on your corpus
-
-df, dist = kanonym4text.anonymize(df: pd.DataFrame, k: int, col: str = 'txt', plot: bool = False,
-              wemodel: str = 'fasttext-wiki-news-subwords-300',
-              num_stop: int = 1000, n_jobs: int = 1, verbose: int = 0)
+```
+dfa, dist = kan.anonymize(df, k=2)
+```
 
 **Running instructions:**
 The main function is called *anonymize*. 
 
 It's input parameters are:
 ---------------------------
 
-df - Input Dataframe
-
-k - k
-
-col - The column in df that holds the text to anonymize. Default - txt
-
-wemodel - The word embedding model from Gensim. Default = 'fasttext-wiki-news-subwords-300'
-
-num_stop - Number of stop word to use. Default - 1000
-
-num_jobs - Number of CPUs to utilize. Default - 1. All CPUs - -1.
+* `df` - Input Dataframe
+* `k` - k
+* `col` - The column in df that holds the text to anonymize. Default - txt
+* `num_stop` - Number of stop word to use. Default - 1000
+* `num_jobs` - Number of CPUs to utilize. Default - 1. All CPUs - -1.
+* `verbose` - Output text level. Default - 0.
 
-verbose - Output text level. Default - 0. doesn't work yet
-
-It's output parameters are:
+The function outputs are:    
 ---------------------------
+A tuple with these items:
+1. A dataframe - the same df the user sent with additional columns:
+> 1. general_txt - text after "generalization"
+> 2. anon_txt_history - changes performed on text during annonymization process:    
+>       [] - replaced     
+>       {} - Lemmatize     
+>       () - protected word (stop-word)     
+> 3. anon_txt - resulted anonymized text
+> 4. neighbors - indeces of k neigbors (Bow anonymized)
 
-df - the same df the user insrted with additional columns:
-
-1. num_of_words - number of words in the original text
-2. anon_txt - text after "generalization"
-3. anon_txt_history - changes performed on text during annonymization process:
-    [] - replaced
-    {} - Lemmatize
-    () - protected word (stop-word)
-4. force_anon_txt - resulted anonymized text
-5. neigbors - indeces of k neigbors (Bow anonymized)
-6. num_of_words_after_forcing - number of words in the anonymized text
-7. num_of_deleting_after_forcing - number of words deleted during anonymization process.
+2. An averaged cosine distance of sentence embedding for the documents before and after the anonymizaion
 
 # Running Example
 
 use the following link to run some examples of the package on your own dataframe:
 
 https://colab.research.google.com/drive/1eMSSvBxtsNFMOvKrUXgbsx1g3KOQD56s#scrollTo=ci2qjboGCt0A&uniqifier=1
 
 or use the following code:
-
-import kanonym4text
-
+```
+from kanonym4text import Kanonym
 import pandas as pd
 
-import nltk
-
 df = pd.read_csv('YOUR_FILE.csv')
 
-nltk.download('vader_lexicon')
-
-
-
-%%time
-
-k=4
-
-df, dist = kanonym4text.anonymize(df, k=k, verbose=1, wemodel = 'glove-twitter-25')
-
-print(k, dist)
-
-
+kan = Kanonym('glove-twitter-25') # creating an object from class
+dfa, dist = kan.anonymize(df, k=k, n_jobs=-1, plot=True)
+```
 
 # Support
 
 ## Create a Bug Report
 If you see an error message or run into an issue, please create a bug report. This effort is valued and helps all users.
 
 ## Submit a Feature Request
```

### Comparing `kanonym4text-0.2.2/kanonym4text/data/5000_most_common_words_by_order.txt` & `kanonym4text-0.2.3/kanonym4text/data/5000_most_common_words_by_order.txt`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.2/kanonym4text/objects/kanonym.py` & `kanonym4text-0.2.3/kanonym4text/objects/kanonym.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,44 +142,49 @@
         col - colom name in the df contains the documents (default: 'txt')
         plot - True if user want's to get visuales during the process (default: False)
         n_jobs - The number of parallel jobs to run for neighbors search (default: -1, means all processors)
         verbose - The verbosity level: if non zero, progress messages are printed (default: 0)
 
         Returns
         -------
-
+        Anonymized dataframe
+        Average semantic distance
         """
 
         from ..utils import llm_utils
 
-        self.init_logger(verbose)
+        self._init_logger(verbose)
         logging.info(f'{os.path.basename(__file__)} LLM pipeline')
 
         # Adding number of characters
         num_chars_col = 'Num_characters'
         df[num_chars_col] = df[col].str.len()
         docs = df[col]
         
         logging.info(f'Number of documents: {len(docs)}')
         logging.info(f'Average number of characters in documents: {df[num_chars_col].mean()} '
                     f'maximum characters in a document {df[num_chars_col].max()}')
+        
+        # Removing the Num_characters column
+        df.drop([num_chars_col], axis=1, inplace=True)
 
         # Running the anonymization
         annon_docs, _ = llm_utils.run_anonymization_on_txt(docs, k, n_jobs)
-        df['llm_anonym_text'] = annon_docs
+        anonum_col = 'llm_anonym_text'
+        df[anonum_col] = annon_docs
 
         curr_k, non_anon_indexes = anonym_utils.get_anonym_degree(docs=annon_docs, min_k=k)
         logging.info(f'Anonymity after reduction:{curr_k}  number of un-anonymized documents: {len(non_anon_indexes)}')  # Logging
 
         # Logging the un-anonymized documents
         if len(non_anon_indexes) > 0: 
             logging.info(f'Un-anonymized documents: {non_anon_indexes}')  # Logging
 
         # Utilization test
-        mean_dist = utilization_utils.get_mean_semantice_distance_for_corpus(df[col], df['anonymized_text'],
+        mean_dist = utilization_utils.get_mean_semantice_distance_for_corpus(df[col], df[anonum_col],
                                                                             plot=plot)
         logging.info(f'Mean semantic distance before and after the anonymization process: {mean_dist}')  # Logging
 
         logging.info('Done')  # Logging
         return df, mean_dist
```

### Comparing `kanonym4text-0.2.2/kanonym4text/utils/anonym_utils.py` & `kanonym4text-0.2.3/kanonym4text/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.2/kanonym4text/utils/cluster_utils.py` & `kanonym4text-0.2.3/kanonym4text/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.2/kanonym4text/utils/llm_utils.py` & `kanonym4text-0.2.3/kanonym4text/utils/llm_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
 from sentence_transformers import SentenceTransformer
 import logging
+import torch
 from . import anonym_utils
 
 
 def print_example(indexes, origina_docs, new_docs):
     print('Before:')
     for i in indexes:
         print(origina_docs[i])
     print('\nAfter:')
     for i in indexes:
         print(new_docs[i])
 
 
-def sum_text_basic(doc_list, tokenizer, gen_model):
+def sum_text_basic(doc_list, tokenizer, gen_model, device):
     # define the input sentences
     # input_text = '. '.join(doc_list)
     input_text = ''
     for doc in doc_list:
        input_text = f'{input_text}\n- {doc}. ' 
 
     # preprocess the input sentences
     input_ids = tokenizer.encode(f'Generate a general form of these sentences: \n{input_text}', return_tensors="pt")
 
+    # Moving to device
+    input_ids = input_ids.to(device)
+    gen_model = gen_model.to(device)
+
     # generate the summary sentence
     output_ids = gen_model.generate(input_ids=input_ids, max_length=32, num_beams=4, early_stopping=True)
     output = tokenizer.decode(output_ids[0], skip_special_tokens=True)
 
     return output
 
 
-def sum_text(doc_list, tokenizer, gen_model):
+def sum_text(doc_list, tokenizer, gen_model, device):
     # define the input sentences
     # input_text = '. '.join(doc_list)
     input_text = ''
     i = 1
     for doc in doc_list:
        input_text = f'{input_text}{i}: {doc}. ' 
        i += 1
     
     # print('doc_list:', doc_list)
     # preprocess the input sentences
     prompt = prompt_builder(doc_list)
     input_ids = tokenizer.encode(prompt, return_tensors="pt")
 
+    # Moving to device
+    input_ids = input_ids.to(device)
+    gen_model = gen_model.to(device)
+
     # generate the summary sentence
     output_ids = gen_model.generate(input_ids=input_ids, max_length=32, num_beams=4, early_stopping=True)
     output = tokenizer.decode(output_ids[0], skip_special_tokens=True)
 
     return output
 
 
@@ -80,16 +89,17 @@
     logging.info(f'Generating alternative documents...')
     for n in neighbor_list:
         # print('n:', n)
         curr_docs = []
         for doc_index in n:
             # Adding the document to the similar doc list
             curr_docs.append(docs[doc_index])
-        sum_doc = sum_text(curr_docs, tokenizer, gen_model)
-        # sum_doc = sum_text_0(curr_docs, tokenizer, gen_model)
+        device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        sum_doc = sum_text(curr_docs, tokenizer, gen_model, device)
+        # sum_doc = sum_text_0(curr_docs, tokenizer, gen_model, device)
         # print('similar_doc_ind', n, '\tSummary:', sum_doc)
         for doc_index in n:
             annon_docs[doc_index] = sum_doc
 
     logging.info(f'Generation completed.')
 
     return annon_docs, neighbor_list
```

### Comparing `kanonym4text-0.2.2/kanonym4text/utils/models.py` & `kanonym4text-0.2.3/kanonym4text/utils/models.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.2/kanonym4text/utils/nlp_utils.py` & `kanonym4text-0.2.3/kanonym4text/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.2/kanonym4text/utils/utilization_utils.py` & `kanonym4text-0.2.3/kanonym4text/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.2/kanonym4text.egg-info/PKG-INFO` & `kanonym4text-0.2.3/kanonym4text.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kanonym4text
-Version: 0.2.2
+Version: 0.2.3
 Summary: k-anonymity for texts
 Home-page: https://github.com/neumanh/K-anonymity-fot-texts
 Author: Lior Trieman, Hadas Neuman
 Author-email: liortr30@gmail.com, hadas.doron@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.3.tar.gz
 Description: A package that takes a dataframe with a corpus and return an anonymized corpus
 Keywords: python,k-anonymity,privacy,NLP
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `kanonym4text-0.2.2/kanonym4text.egg-info/SOURCES.txt` & `kanonym4text-0.2.3/kanonym4text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kanonym4text-0.2.2/setup.py` & `kanonym4text-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'k-anonymity for texts'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="kanonym4text",
     version=VERSION,
     author="Lior Trieman, Hadas Neuman",
     author_email="liortr30@gmail.com, hadas.doron@gmail.com",
     url='https://github.com/neumanh/K-anonymity-fot-texts',
 
-    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.2.tar.gz',
+    download_url='https://github.com/neumanh/K-anonymity-fot-texts/archive/refs/tags/0.2.3.tar.gz',
 
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # package_dir={'kanonym4text': 'kanonym4text'},
     install_requires=[
```

