# Comparing `tmp/langchain_ray-0.0.2.tar.gz` & `tmp/langchain_ray-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ray-0.0.2.tar", last modified: Fri Jul  7 05:23:29 2023, max compression
+gzip compressed data, was "langchain_ray-0.0.4.tar", last modified: Sun Jul  9 03:21:52 2023, max compression
```

## Comparing `langchain_ray-0.0.2.tar` & `langchain_ray-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 langchain_ray-0.0.2/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 langchain_ray-0.0.2/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      127 2023-07-07 04:36:43.000000 langchain_ray-0.0.2/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.793174 langchain_ray-0.0.2/langchain_ray/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     5525 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2153 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/chains.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      914 2023-07-07 04:23:18.000000 langchain_ray-0.0.2/langchain_ray/imports.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/langchain_ray/pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     5342 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/pdf/chains.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     6175 2023-07-07 05:23:22.000000 langchain_ray-0.0.2/langchain_ray/pdf/utils.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/langchain_ray.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      496 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       48 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 03:48:41.000000 langchain_ray-0.0.2/langchain_ray.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       47 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       14 2023-07-07 05:23:29.000000 langchain_ray-0.0.2/langchain_ray.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      722 2023-07-07 05:23:19.000000 langchain_ray-0.0.2/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-07-07 05:23:29.797174 langchain_ray-0.0.2/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 langchain_ray-0.0.2/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 langchain_ray-0.0.4/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 langchain_ray-0.0.4/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      127 2023-07-07 04:36:43.000000 langchain_ray-0.0.4/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/langchain_ray/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     6244 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3575 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/chains.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      984 2023-07-09 02:01:37.000000 langchain_ray-0.0.4/langchain_ray/imports.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/langchain_ray/pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     6120 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/pdf/chains.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     6485 2023-07-09 03:21:35.000000 langchain_ray-0.0.4/langchain_ray/pdf/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/langchain_ray.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      855 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      496 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       48 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-07-07 03:48:41.000000 langchain_ray-0.0.4/langchain_ray.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       85 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       14 2023-07-09 03:21:52.000000 langchain_ray-0.0.4/langchain_ray.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      760 2023-07-09 03:21:30.000000 langchain_ray-0.0.4/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-07-09 03:21:52.383475 langchain_ray-0.0.4/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 langchain_ray-0.0.4/setup.py
```

### Comparing `langchain_ray-0.0.2/LICENSE` & `langchain_ray-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ray-0.0.2/PKG-INFO` & `langchain_ray-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_ray
-Version: 0.0.2
+Version: 0.0.4
 Summary: LangChain leveraging Ray.
 Home-page: https://github.com/HamzaFarhan/langchain_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langchain_ray-0.0.2/langchain_ray/_modidx.py` & `langchain_ray-0.0.4/langchain_ray/_modidx.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,36 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/langchain_ray',
                 'doc_host': 'https://HamzaFarhan.github.io',
                 'git_url': 'https://github.com/HamzaFarhan/langchain_ray',
                 'lib_path': 'langchain_ray'},
   'syms': { 'langchain_ray.chains': { 'langchain_ray.chains.chain_fn': ('chains.html#chain_fn', 'langchain_ray/chains.py'),
+                                      'langchain_ray.chains.chainfn_input': ('chains.html#chainfn_input', 'langchain_ray/chains.py'),
+                                      'langchain_ray.chains.chainfn_output': ('chains.html#chainfn_output', 'langchain_ray/chains.py'),
                                       'langchain_ray.chains.noop_chain': ('chains.html#noop_chain', 'langchain_ray/chains.py'),
                                       'langchain_ray.chains.ray_chain': ('chains.html#ray_chain', 'langchain_ray/chains.py'),
                                       'langchain_ray.chains.ray_chain_fn': ('chains.html#ray_chain_fn', 'langchain_ray/chains.py'),
                                       'langchain_ray.chains.transform_chain': ('chains.html#transform_chain', 'langchain_ray/chains.py')},
             'langchain_ray.imports': {},
-            'langchain_ray.pdf.chains': { 'langchain_ray.pdf.chains.index_query_chain': ( 'pdf/pdf_chains.html#index_query_chain',
+            'langchain_ray.pdf.chains': { 'langchain_ray.pdf.chains.docs_faiss_chain': ( 'pdf/pdf_chains.html#docs_faiss_chain',
+                                                                                         'langchain_ray/pdf/chains.py'),
+                                          'langchain_ray.pdf.chains.index_query_chain': ( 'pdf/pdf_chains.html#index_query_chain',
                                                                                           'langchain_ray/pdf/chains.py'),
                                           'langchain_ray.pdf.chains.pdf_cats_chain': ( 'pdf/pdf_chains.html#pdf_cats_chain',
                                                                                        'langchain_ray/pdf/chains.py'),
                                           'langchain_ray.pdf.chains.pdf_docs_chain': ( 'pdf/pdf_chains.html#pdf_docs_chain',
                                                                                        'langchain_ray/pdf/chains.py'),
                                           'langchain_ray.pdf.chains.pdf_ems_chain': ( 'pdf/pdf_chains.html#pdf_ems_chain',
                                                                                       'langchain_ray/pdf/chains.py'),
                                           'langchain_ray.pdf.chains.pdf_faiss_chain': ( 'pdf/pdf_chains.html#pdf_faiss_chain',
-                                                                                        'langchain_ray/pdf/chains.py'),
-                                          'langchain_ray.pdf.chains.pdf_index_chain': ( 'pdf/pdf_chains.html#pdf_index_chain',
                                                                                         'langchain_ray/pdf/chains.py')},
-            'langchain_ray.pdf.utils': { 'langchain_ray.pdf.utils.cid_to_char': ( 'pdf/pdf_utils.html#cid_to_char',
+            'langchain_ray.pdf.utils': { 'langchain_ray.pdf.utils.bold_text': ( 'pdf/pdf_utils.html#bold_text',
+                                                                                'langchain_ray/pdf/utils.py'),
+                                         'langchain_ray.pdf.utils.cid_to_char': ( 'pdf/pdf_utils.html#cid_to_char',
                                                                                   'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.create_idx_q_df': ( 'pdf/pdf_utils.html#create_idx_q_df',
                                                                                       'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.create_pdf_df': ( 'pdf/pdf_utils.html#create_pdf_df',
                                                                                     'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.df_docs_cat': ( 'pdf/pdf_utils.html#df_docs_cat',
                                                                                   'langchain_ray/pdf/utils.py'),
@@ -41,11 +45,13 @@
                                                                                       'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.df_to_faiss': ( 'pdf/pdf_utils.html#df_to_faiss',
                                                                                   'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.doc_proc_text': ( 'pdf/pdf_utils.html#doc_proc_text',
                                                                                     'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.docs_cat': ('pdf/pdf_utils.html#docs_cat', 'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.docs_ems': ('pdf/pdf_utils.html#docs_ems', 'langchain_ray/pdf/utils.py'),
+                                         'langchain_ray.pdf.utils.print_doc': ( 'pdf/pdf_utils.html#print_doc',
+                                                                                'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.process_text': ( 'pdf/pdf_utils.html#process_text',
                                                                                    'langchain_ray/pdf/utils.py'),
                                          'langchain_ray.pdf.utils.text_cat': ( 'pdf/pdf_utils.html#text_cat',
                                                                                'langchain_ray/pdf/utils.py')}}}
```

### Comparing `langchain_ray-0.0.2/langchain_ray/chains.py` & `langchain_ray-0.0.4/langchain_ray/chains.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,100 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_chains.ipynb.
 
 # %% auto 0
-__all__ = ['chain_fn', 'transform_chain', 'ray_chain_fn', 'ray_chain', 'noop_chain']
+__all__ = ['chainfn_input', 'chainfn_output', 'chain_fn', 'transform_chain', 'ray_chain_fn', 'ray_chain', 'noop_chain']
 
 # %% ../nbs/00_chains.ipynb 2
 from dreamai.imports import *
 from .imports import *
 
 # %% ../nbs/00_chains.ipynb 3
-def chain_fn(data, tfm, tfm_kwargs={}, input_key="df", output_key="df"):
-    return {output_key: tfm(data[input_key], **tfm_kwargs)}
-
-
-def transform_chain(transform, transform_kwargs={}, input_key="df", output_key="df"):
+def chainfn_input(data, tfm, tfm_kwargs={}, input_variables=["df"]):
+    for k in input_variables:
+        tfm_kwargs[k] = data.get(k, None)
+    fn_args = inspect.signature(tfm).parameters
+    pos_args = [k for k in fn_args if fn_args[k].default == inspect._empty]
+    for pk, ik in zip(pos_args, input_variables):
+        if pk != "kwargs":
+            tfm_kwargs[pk] = tfm_kwargs.pop(ik)
+    if 'kwargs' not in fn_args:
+        tfm_kwargs = {k:v for k,v in tfm_kwargs.items() if k in fn_args.keys()}
+    return tfm_kwargs
+
+def chainfn_output(fn_res, output_variables=["df"]):
+    if not list_or_tuple(fn_res):
+        fn_res = [fn_res]
+    return {k: r for k, r in zip(output_variables, fn_res)}
+
+def chain_fn(data, tfm, tfm_kwargs={}, input_variables=["df"], output_variables=["df"]):
+    tfm_kwargs = chainfn_input(data, tfm, tfm_kwargs, input_variables)
+    # print(f'\n\nTFM: {tfm}\n\n')
+    # print(f'\n\nTFM KWARGS: {tfm_kwargs.keys()}\n\n')
+    fn_res = tfm(**tfm_kwargs)
+    return chainfn_output(fn_res, output_variables)
+
+
+def transform_chain(
+    transform,
+    transform_kwargs={},
+    input_variables=["df"],
+    output_variables=["df"],
+):
     return TransformChain(
-        input_variables=[input_key],
-        output_variables=[output_key],
+        input_variables=input_variables,
+        output_variables=output_variables,
         transform=partial(
             chain_fn,
             tfm=transform,
             tfm_kwargs=transform_kwargs,
-            input_key=input_key,
-            output_key=output_key,
+            input_variables=input_variables,
+            output_variables=output_variables,
         ),
     )
 
 
-def ray_chain_fn(data, chain, block_size=1500, cuda=True, max_cpus=8):
-    df = data[chain.input_keys[0]]
-    if not is_df(df):
-        res = chain.run(df)
-    elif block_size is None or len(df) <= block_size:
-        res = chain.run(df)
+def ray_chain_fn(data, chain, block_size=1500, num_cpus=8, num_gpus=1):
+    ray_data = data[chain.input_keys[0]]
+    # if not is_df(df):
+    # res = chain.run(df)
+    if path_or_str(ray_data) or not is_iter(ray_data):
+        res = chain.run(ray_data)
+        # print(f'\n\nRES: {res}\n\n')
+        return {chain.output_keys[0]: res}
+    if block_size is None or len(ray_data) <= block_size:
+        res = chain.run(ray_data)
+        # print(f'\n\nRES: {res}\n\n')
+        return {chain.output_keys[0]: res}
+    ray.init(ignore_reinit_error=True)
+    num_blocks = int(np.ceil(len(ray_data) / block_size))
+    msg.info(f"Running chain on {num_blocks} blocks.", spaced=True)
+    num_cpus = min(ray.available_resources()["CPU"], num_cpus)
+    num_cpus /= num_blocks
+    if num_gpus is not None:
+        num_gpus = min(ray.available_resources()["GPU"], num_gpus)
+        num_gpus /= num_blocks
+        num_cpus = None
+    if not is_df(ray_data):
+        ds = rd.from_items(ray_data).repartition(num_blocks)
     else:
-        num_blocks = int(np.ceil(len(df) / block_size))
-        msg.info(f"Running chain on {num_blocks} blocks.", spaced=True)
-        num_cpus = min(ray.available_resources()["CPU"] - 4, max_cpus)
-        num_cpus /= num_blocks
-        num_gpus = None
-        if cuda:
-            num_gpus = (ray.available_resources()["GPU"] - 0.25) / num_blocks
-            num_cpus = None
-        ds = rd.from_pandas(df).repartition(num_blocks)
-        res = ds.map_batches(
-            lambda x: chain.run(x),
-            batch_size=block_size,
-            num_cpus=num_cpus,
-            num_gpus=num_gpus,
-            batch_format="pandas",
-        ).to_pandas()
+        ds = rd.from_pandas(ray_data).repartition(num_blocks)
+    res = ds.map_batches(
+        lambda x: chain.run(x),
+        batch_size=block_size,
+        num_cpus=num_cpus,
+        num_gpus=num_gpus,
+        batch_format="pandas",
+    ).to_pandas()
     return {chain.output_keys[0]: res}
 
 
-def ray_chain(chain, block_size=1500, cuda=True):
-    tfm = partial(ray_chain_fn, chain=chain, block_size=block_size, cuda=cuda)
+def ray_chain(chain, block_size=1500, num_cpus=8, num_gpus=1):
+    tfm = partial(
+        ray_chain_fn, chain=chain, block_size=block_size, num_cpus=num_cpus, num_gpus=num_gpus
+    )
     input_variables = chain.input_keys
     output_variables = chain.output_keys
     return TransformChain(
         input_variables=input_variables,
         output_variables=output_variables,
         transform=tfm,
     )
```

### Comparing `langchain_ray-0.0.2/langchain_ray/imports.py` & `langchain_ray-0.0.4/langchain_ray/imports.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from dreamai.imports import *
 from dreamai.core import *
 
 import ray
+import inspect
 from ray import serve
 from ray import data as rd
 from transformers import pipeline
+from sentence_transformers import SentenceTransformer
+
 from langchain.schema import Document
 from langchain.llms import HuggingFacePipeline
 from langchain.vectorstores import Chroma, FAISS
 from langchain.document_loaders import PyPDFLoader
 from langchain.document_loaders.pdf import BasePDFLoader
 from langchain.document_loaders.blob_loaders import Blob
 from langchain.document_loaders.base import BaseBlobParser
```

### Comparing `langchain_ray-0.0.2/langchain_ray/pdf/utils.py` & `langchain_ray-0.0.4/langchain_ray/pdf/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/pdf/00_pdf_utils.ipynb.
 
 # %% auto 0
-__all__ = ['cid_to_char', 'process_text', 'create_pdf_df', 'create_idx_q_df', 'doc_proc_text', 'df_pdf_docs_', 'df_pdf_docs',
-           'text_cat', 'docs_cat', 'df_docs_cat', 'docs_ems', 'df_docs_ems', 'df_to_faiss', 'df_search_faiss']
+__all__ = ['cid_to_char', 'process_text', 'bold_text', 'print_doc', 'create_pdf_df', 'create_idx_q_df', 'doc_proc_text',
+           'df_pdf_docs_', 'df_pdf_docs', 'text_cat', 'docs_cat', 'df_docs_cat', 'docs_ems', 'df_docs_ems',
+           'df_to_faiss', 'df_search_faiss']
 
 # %% ../../nbs/pdf/00_pdf_utils.ipynb 2
 from dreamai.imports import *
 from ..imports import *
 from ..chains import *
 
 # %% ../../nbs/pdf/00_pdf_utils.ipynb 3
@@ -55,14 +56,23 @@
     text = re.sub(r"\uf0d8", "", text)
     text = re.sub(r"\u00b7", "", text)
     text = re.sub("\t", " ", text)
     text = re.sub(" +", " ", text)
     return text.strip()
 
 
+def bold_text(text):
+    return "\033[1m" + text + "\033[0m"
+
+
+def print_doc(doc):
+    print(f"{bold_text('Page_Content:')} {doc.page_content}\n")
+    print(f"{bold_text('Metadata:')} {doc.metadata}\n")
+
+
 def create_pdf_df(pdf_folder):
     pdfs = get_files(pdf_folder, extensions=[".pdf"])
     return pd.DataFrame({"pdf_path": pdfs})
 
 
 def create_idx_q_df(query, index_folder, index_name):
     index_names = [
@@ -183,15 +193,16 @@
     if index_path.exists():
         index_path = find_alternate_path(index_path, first_idx=1, verbose=False)
     index_name = index_path.stem
     db.save_local(index_folder, index_name)
     return df
 
 
-def df_search_faiss(df, ems_model, k=2):
+def df_search_faiss(df, ems_model, filter=None, k=2):
     index_folder = str(df["index_folder"])
     index_name = df["index_name"]
     query = df["query"]
     db = FAISS.load_local(index_folder, embeddings=ems_model, index_name=index_name)
-    q_sims = db.similarity_search_with_score(query, k=k)
+    q_sims = db.similarity_search_with_score(query, filter=filter, k=k)
+    # print(f'\n\nQSIMS: {q_sims}\n\n')
     df["results"] = q_sims
     return df
```

### Comparing `langchain_ray-0.0.2/langchain_ray.egg-info/PKG-INFO` & `langchain_ray-0.0.4/langchain_ray.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-ray
-Version: 0.0.2
+Version: 0.0.4
 Summary: LangChain leveraging Ray.
 Home-page: https://github.com/HamzaFarhan/langchain_ray
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langchain_ray-0.0.2/settings.ini` & `langchain_ray-0.0.4/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = langchain_ray
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.4
 min_python = 3.8
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = langchain_ray
 nbs_path = nbs
 recursive = True
@@ -22,9 +22,9 @@
 author_email = thehamza96@gmail.com
 copyright = 2023 onwards, %(author)s
 description = LangChain leveraging Ray.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = HamzaFarhan
-pip_requirements = "ray[air]" dreamai langchain transformers
+pip_requirements = "ray[air]" dreamai langchain transformers pypdf faiss-cpu sentence-transformers
```

### Comparing `langchain_ray-0.0.2/setup.py` & `langchain_ray-0.0.4/setup.py`

 * *Files identical despite different names*

