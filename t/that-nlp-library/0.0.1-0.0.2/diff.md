# Comparing `tmp/that-nlp-library-0.0.1.tar.gz` & `tmp/that-nlp-library-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that-nlp-library-0.0.1.tar", last modified: Mon May 15 09:59:25 2023, max compression
+gzip compressed data, was "that-nlp-library-0.0.2.tar", last modified: Sun Jul  9 15:50:26 2023, max compression
```

## Comparing `that-nlp-library-0.0.1.tar` & `that-nlp-library-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-05-15 09:59:25.669292 that-nlp-library-0.0.1/
--rw-rw-r--   0 quan      (1000) quan      (1000)    11337 2023-04-27 10:12:58.000000 that-nlp-library-0.0.1/LICENSE
--rw-rw-r--   0 quan      (1000) quan      (1000)      111 2023-04-27 10:12:58.000000 that-nlp-library-0.0.1/MANIFEST.in
--rw-rw-r--   0 quan      (1000) quan      (1000)     2757 2023-05-15 09:59:25.665292 that-nlp-library-0.0.1/PKG-INFO
--rw-rw-r--   0 quan      (1000) quan      (1000)     1870 2023-05-15 09:58:01.000000 that-nlp-library-0.0.1/README.md
--rw-rw-r--   0 quan      (1000) quan      (1000)     1215 2023-05-10 09:21:55.000000 that-nlp-library-0.0.1/settings.ini
--rw-rw-r--   0 quan      (1000) quan      (1000)       38 2023-05-15 09:59:25.669292 that-nlp-library-0.0.1/setup.cfg
--rw-rw-r--   0 quan      (1000) quan      (1000)     2596 2023-04-27 10:12:58.000000 that-nlp-library-0.0.1/setup.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-05-15 09:59:25.665292 that-nlp-library-0.0.1/that_nlp_library/
--rw-rw-r--   0 quan      (1000) quan      (1000)       22 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/__init__.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    29783 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/_modidx.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     4707 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/evaluations.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    18126 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/model_main.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-05-15 09:59:25.665292 that-nlp-library-0.0.1/that_nlp_library/models/
--rw-rw-r--   0 quan      (1000) quan      (1000)        0 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/models/__init__.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    18943 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/models/classifiers.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     5288 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/models/conditional_prob_classifiers.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    12378 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/models/deep_hierarchical_classifiers.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     2694 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/text_augmentation.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    20266 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/text_main.py
--rw-rw-r--   0 quan      (1000) quan      (1000)      857 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/text_transformation.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     4723 2023-05-15 08:11:22.000000 that-nlp-library-0.0.1/that_nlp_library/utils.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-05-15 09:59:25.665292 that-nlp-library-0.0.1/that_nlp_library.egg-info/
--rw-rw-r--   0 quan      (1000) quan      (1000)     2757 2023-05-15 09:59:25.000000 that-nlp-library-0.0.1/that_nlp_library.egg-info/PKG-INFO
--rw-rw-r--   0 quan      (1000) quan      (1000)      774 2023-05-15 09:59:25.000000 that-nlp-library-0.0.1/that_nlp_library.egg-info/SOURCES.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)        1 2023-05-15 09:59:25.000000 that-nlp-library-0.0.1/that_nlp_library.egg-info/dependency_links.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)       54 2023-05-15 09:59:25.000000 that-nlp-library-0.0.1/that_nlp_library.egg-info/entry_points.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)        1 2023-05-10 04:37:10.000000 that-nlp-library-0.0.1/that_nlp_library.egg-info/not-zip-safe
--rw-rw-r--   0 quan      (1000) quan      (1000)      145 2023-05-15 09:59:25.000000 that-nlp-library-0.0.1/that_nlp_library.egg-info/requires.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)       17 2023-05-15 09:59:25.000000 that-nlp-library-0.0.1/that_nlp_library.egg-info/top_level.txt
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-07-09 15:50:26.312929 that-nlp-library-0.0.2/
+-rw-rw-r--   0 quan      (1000) quan      (1000)    11337 2023-04-27 10:12:58.000000 that-nlp-library-0.0.2/LICENSE
+-rw-rw-r--   0 quan      (1000) quan      (1000)      111 2023-04-27 10:12:58.000000 that-nlp-library-0.0.2/MANIFEST.in
+-rw-rw-r--   0 quan      (1000) quan      (1000)     2757 2023-07-09 15:50:26.312929 that-nlp-library-0.0.2/PKG-INFO
+-rw-rw-r--   0 quan      (1000) quan      (1000)     1870 2023-07-09 15:14:43.000000 that-nlp-library-0.0.2/README.md
+-rw-rw-r--   0 quan      (1000) quan      (1000)     1222 2023-07-09 15:16:17.000000 that-nlp-library-0.0.2/settings.ini
+-rw-rw-r--   0 quan      (1000) quan      (1000)       38 2023-07-09 15:50:26.312929 that-nlp-library-0.0.2/setup.cfg
+-rw-rw-r--   0 quan      (1000) quan      (1000)     2596 2023-04-27 10:12:58.000000 that-nlp-library-0.0.2/setup.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-07-09 15:50:26.312929 that-nlp-library-0.0.2/that_nlp_library/
+-rw-rw-r--   0 quan      (1000) quan      (1000)       22 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/__init__.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    30953 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/_modidx.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     4707 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/evaluations.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    25828 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/model_main.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-07-09 15:50:26.312929 that-nlp-library-0.0.2/that_nlp_library/models/
+-rw-rw-r--   0 quan      (1000) quan      (1000)        0 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/models/__init__.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-07-09 15:50:26.312929 that-nlp-library-0.0.2/that_nlp_library/models/roberta/
+-rw-rw-r--   0 quan      (1000) quan      (1000)        0 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/models/roberta/__init__.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    12610 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/models/roberta/classifiers.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     5148 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/models/roberta/conditional_prob_classifiers.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    12677 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/models/roberta/deep_hierarchical_classifiers.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     2694 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/text_augmentation.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    20516 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/text_main.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)      857 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/text_transformation.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     4723 2023-07-09 15:42:36.000000 that-nlp-library-0.0.2/that_nlp_library/utils.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2023-07-09 15:50:26.312929 that-nlp-library-0.0.2/that_nlp_library.egg-info/
+-rw-rw-r--   0 quan      (1000) quan      (1000)     2757 2023-07-09 15:50:26.000000 that-nlp-library-0.0.2/that_nlp_library.egg-info/PKG-INFO
+-rw-rw-r--   0 quan      (1000) quan      (1000)      842 2023-07-09 15:50:26.000000 that-nlp-library-0.0.2/that_nlp_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)        1 2023-07-09 15:50:26.000000 that-nlp-library-0.0.2/that_nlp_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)       54 2023-07-09 15:50:26.000000 that-nlp-library-0.0.2/that_nlp_library.egg-info/entry_points.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)        1 2023-05-10 04:37:10.000000 that-nlp-library-0.0.2/that_nlp_library.egg-info/not-zip-safe
+-rw-rw-r--   0 quan      (1000) quan      (1000)      153 2023-07-09 15:50:26.000000 that-nlp-library-0.0.2/that_nlp_library.egg-info/requires.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)       17 2023-07-09 15:50:26.000000 that-nlp-library-0.0.2/that_nlp_library.egg-info/top_level.txt
```

### Comparing `that-nlp-library-0.0.1/LICENSE` & `that-nlp-library-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.0.1/PKG-INFO` & `that-nlp-library-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-nlp-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Aim to be a convenient NLP library with the help from HuggingFace
 Home-page: https://github.com/anhquan0412/that-nlp-library
 Author: Quan Tran
 Author-email: anhquan0412@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev,jupyter,notebook,python,nlp,natural language processing,transformer,fastai,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `that-nlp-library-0.0.1/README.md` & `that-nlp-library-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.0.1/settings.ini` & `that-nlp-library-0.0.2/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = that-nlp-library
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = that_nlp_library
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 
 ### Docs ###
 branch = main
-custom_sidebar = False
+custom_sidebar = True
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 
 ### PyPI ###
 audience = Developers
@@ -34,11 +34,11 @@
 description = Aim to be a convenient NLP library with the help from HuggingFace
 keywords = nbdev, jupyter, notebook, python, nlp, natural language processing, transformer, fastai, deep learning
 language = English
 status = 3
 user = anhquan0412
 
 ### Optional ###
-requirements = matplotlib pandas requests tqdm scikit-learn datasets underthesea dill transformers sentencepiece pyarrow unidecode wandb
+requirements = matplotlib pandas requests tqdm scikit-learn datasets underthesea dill transformers==4.28.1 sentencepiece pyarrow unidecode wandb
 pip_requirements = torch>=1.7,<2.1
 # dev_requirements =
 # console_scripts =
```

### Comparing `that-nlp-library-0.0.1/setup.py` & `that-nlp-library-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.0.1/that_nlp_library/_modidx.py` & `that-nlp-library-0.0.2/that_nlp_library/_modidx.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,86 +21,86 @@
                                                                                                   'that_nlp_library/model_main.py'),
                                              'that_nlp_library.model_main.ModelController.predict_ddict': ( 'model_main.html#modelcontroller.predict_ddict',
                                                                                                             'that_nlp_library/model_main.py'),
                                              'that_nlp_library.model_main.ModelController.predict_raw_text': ( 'model_main.html#modelcontroller.predict_raw_text',
                                                                                                                'that_nlp_library/model_main.py'),
                                              'that_nlp_library.model_main._forward_pass_for_predictions': ( 'model_main.html#_forward_pass_for_predictions',
                                                                                                             'that_nlp_library/model_main.py'),
+                                             'that_nlp_library.model_main.compute_metrics_classification': ( 'model_main.html#compute_metrics_classification',
+                                                                                                             'that_nlp_library/model_main.py'),
+                                             'that_nlp_library.model_main.compute_metrics_separate_singleheads': ( 'model_main.html#compute_metrics_separate_singleheads',
+                                                                                                                   'that_nlp_library/model_main.py'),
                                              'that_nlp_library.model_main.finetune': ( 'model_main.html#finetune',
-                                                                                       'that_nlp_library/model_main.py')},
-            'that_nlp_library.models.classifiers': { 'that_nlp_library.models.classifiers.RobertaBaseForSequenceClassification': ( 'models.classifiers.html#robertabaseforsequenceclassification',
-                                                                                                                                   'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaBaseForSequenceClassification.__init__': ( 'models.classifiers.html#robertabaseforsequenceclassification.__init__',
-                                                                                                                                            'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaBaseForSequenceClassification.forward': ( 'models.classifiers.html#robertabaseforsequenceclassification.forward',
-                                                                                                                                           'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaClassificationHeadCustom': ( 'models.classifiers.html#robertaclassificationheadcustom',
-                                                                                                                              'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaClassificationHeadCustom.__init__': ( 'models.classifiers.html#robertaclassificationheadcustom.__init__',
-                                                                                                                                       'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaClassificationHeadCustom.forward': ( 'models.classifiers.html#robertaclassificationheadcustom.forward',
-                                                                                                                                      'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaConcatHeadExtended': ( 'models.classifiers.html#robertaconcatheadextended',
-                                                                                                                        'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaConcatHeadExtended.__init__': ( 'models.classifiers.html#robertaconcatheadextended.__init__',
-                                                                                                                                 'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaConcatHeadExtended.forward': ( 'models.classifiers.html#robertaconcatheadextended.forward',
-                                                                                                                                'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaConcatHeadSimple': ( 'models.classifiers.html#robertaconcatheadsimple',
-                                                                                                                      'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaConcatHeadSimple.__init__': ( 'models.classifiers.html#robertaconcatheadsimple.__init__',
-                                                                                                                               'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaConcatHeadSimple.forward': ( 'models.classifiers.html#robertaconcatheadsimple.forward',
-                                                                                                                              'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaHiddenStateConcatForSequenceClassification': ( 'models.classifiers.html#robertahiddenstateconcatforsequenceclassification',
-                                                                                                                                                'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaHiddenStateConcatForSequenceClassification.__init__': ( 'models.classifiers.html#robertahiddenstateconcatforsequenceclassification.__init__',
-                                                                                                                                                         'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.RobertaHiddenStateConcatForSequenceClassification.forward': ( 'models.classifiers.html#robertahiddenstateconcatforsequenceclassification.forward',
-                                                                                                                                                        'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.compute_metrics_classification': ( 'models.classifiers.html#compute_metrics_classification',
-                                                                                                                             'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.compute_metrics_separate_singleheads': ( 'models.classifiers.html#compute_metrics_separate_singleheads',
-                                                                                                                                   'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.loss_for_classification': ( 'models.classifiers.html#loss_for_classification',
-                                                                                                                      'that_nlp_library/models/classifiers.py'),
-                                                     'that_nlp_library.models.classifiers.model_init_classification': ( 'models.classifiers.html#model_init_classification',
-                                                                                                                        'that_nlp_library/models/classifiers.py')},
-            'that_nlp_library.models.conditional_prob_classifiers': { 'that_nlp_library.models.conditional_prob_classifiers.RobertaHSCCProbSequenceClassification': ( 'models.conditional_prob_classifiers.html#robertahsccprobsequenceclassification',
-                                                                                                                                                                      'that_nlp_library/models/conditional_prob_classifiers.py'),
-                                                                      'that_nlp_library.models.conditional_prob_classifiers.RobertaHSCCProbSequenceClassification.__init__': ( 'models.conditional_prob_classifiers.html#robertahsccprobsequenceclassification.__init__',
-                                                                                                                                                                               'that_nlp_library/models/conditional_prob_classifiers.py'),
-                                                                      'that_nlp_library.models.conditional_prob_classifiers.RobertaHSCCProbSequenceClassification.forward': ( 'models.conditional_prob_classifiers.html#robertahsccprobsequenceclassification.forward',
-                                                                                                                                                                              'that_nlp_library/models/conditional_prob_classifiers.py'),
-                                                                      'that_nlp_library.models.conditional_prob_classifiers.build_standard_condition_mask': ( 'models.conditional_prob_classifiers.html#build_standard_condition_mask',
-                                                                                                                                                              'that_nlp_library/models/conditional_prob_classifiers.py')},
-            'that_nlp_library.models.deep_hierarchical_classifiers': { 'that_nlp_library.models.deep_hierarchical_classifiers.RobertaConcatHeadDHCRoot': ( 'models.deep_hierarchical_classifiers.html#robertaconcatheaddhcroot',
-                                                                                                                                                           'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaConcatHeadDHCRoot.__init__': ( 'models.deep_hierarchical_classifiers.html#robertaconcatheaddhcroot.__init__',
-                                                                                                                                                                    'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaConcatHeadDHCRoot.forward': ( 'models.deep_hierarchical_classifiers.html#robertaconcatheaddhcroot.forward',
-                                                                                                                                                                   'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaHSCDHCSequenceClassification': ( 'models.deep_hierarchical_classifiers.html#robertahscdhcsequenceclassification',
-                                                                                                                                                                      'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaHSCDHCSequenceClassification.__init__': ( 'models.deep_hierarchical_classifiers.html#robertahscdhcsequenceclassification.__init__',
-                                                                                                                                                                               'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaHSCDHCSequenceClassification.forward': ( 'models.deep_hierarchical_classifiers.html#robertahscdhcsequenceclassification.forward',
-                                                                                                                                                                              'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaHSCSimpleDHCSequenceClassification': ( 'models.deep_hierarchical_classifiers.html#robertahscsimpledhcsequenceclassification',
-                                                                                                                                                                            'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaHSCSimpleDHCSequenceClassification.__init__': ( 'models.deep_hierarchical_classifiers.html#robertahscsimpledhcsequenceclassification.__init__',
-                                                                                                                                                                                     'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.RobertaHSCSimpleDHCSequenceClassification.forward': ( 'models.deep_hierarchical_classifiers.html#robertahscsimpledhcsequenceclassification.forward',
-                                                                                                                                                                                    'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers._check_hierarchy': ( 'models.deep_hierarchical_classifiers.html#_check_hierarchy',
-                                                                                                                                                   'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.build_DHC_conditional_mask': ( 'models.deep_hierarchical_classifiers.html#build_dhc_conditional_mask',
-                                                                                                                                                             'that_nlp_library/models/deep_hierarchical_classifiers.py'),
-                                                                       'that_nlp_library.models.deep_hierarchical_classifiers.loss_for_DHC': ( 'models.deep_hierarchical_classifiers.html#loss_for_dhc',
-                                                                                                                                               'that_nlp_library/models/deep_hierarchical_classifiers.py')},
+                                                                                       'that_nlp_library/model_main.py'),
+                                             'that_nlp_library.model_main.loss_for_classification': ( 'model_main.html#loss_for_classification',
+                                                                                                      'that_nlp_library/model_main.py'),
+                                             'that_nlp_library.model_main.model_init_classification': ( 'model_main.html#model_init_classification',
+                                                                                                        'that_nlp_library/model_main.py')},
+            'that_nlp_library.models.roberta.classifiers': { 'that_nlp_library.models.roberta.classifiers.ConcatHeadExtended': ( 'models.roberta.classifiers.html#concatheadextended',
+                                                                                                                                 'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.ConcatHeadExtended.__init__': ( 'models.roberta.classifiers.html#concatheadextended.__init__',
+                                                                                                                                          'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.ConcatHeadExtended.forward': ( 'models.roberta.classifiers.html#concatheadextended.forward',
+                                                                                                                                         'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.ConcatHeadSimple': ( 'models.roberta.classifiers.html#concatheadsimple',
+                                                                                                                               'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.ConcatHeadSimple.__init__': ( 'models.roberta.classifiers.html#concatheadsimple.__init__',
+                                                                                                                                        'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.ConcatHeadSimple.forward': ( 'models.roberta.classifiers.html#concatheadsimple.forward',
+                                                                                                                                       'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaBaseForSequenceClassification': ( 'models.roberta.classifiers.html#robertabaseforsequenceclassification',
+                                                                                                                                                   'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaBaseForSequenceClassification.__init__': ( 'models.roberta.classifiers.html#robertabaseforsequenceclassification.__init__',
+                                                                                                                                                            'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaBaseForSequenceClassification.forward': ( 'models.roberta.classifiers.html#robertabaseforsequenceclassification.forward',
+                                                                                                                                                           'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaClassificationHeadCustom': ( 'models.roberta.classifiers.html#robertaclassificationheadcustom',
+                                                                                                                                              'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaClassificationHeadCustom.__init__': ( 'models.roberta.classifiers.html#robertaclassificationheadcustom.__init__',
+                                                                                                                                                       'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaClassificationHeadCustom.forward': ( 'models.roberta.classifiers.html#robertaclassificationheadcustom.forward',
+                                                                                                                                                      'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaHiddenStateConcatForSequenceClassification': ( 'models.roberta.classifiers.html#robertahiddenstateconcatforsequenceclassification',
+                                                                                                                                                                'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaHiddenStateConcatForSequenceClassification.__init__': ( 'models.roberta.classifiers.html#robertahiddenstateconcatforsequenceclassification.__init__',
+                                                                                                                                                                         'that_nlp_library/models/roberta/classifiers.py'),
+                                                             'that_nlp_library.models.roberta.classifiers.RobertaHiddenStateConcatForSequenceClassification.forward': ( 'models.roberta.classifiers.html#robertahiddenstateconcatforsequenceclassification.forward',
+                                                                                                                                                                        'that_nlp_library/models/roberta/classifiers.py')},
+            'that_nlp_library.models.roberta.conditional_prob_classifiers': { 'that_nlp_library.models.roberta.conditional_prob_classifiers.RobertaHSCCProbSequenceClassification': ( 'models.roberta.conditional_prob_classifiers.html#robertahsccprobsequenceclassification',
+                                                                                                                                                                                      'that_nlp_library/models/roberta/conditional_prob_classifiers.py'),
+                                                                              'that_nlp_library.models.roberta.conditional_prob_classifiers.RobertaHSCCProbSequenceClassification.__init__': ( 'models.roberta.conditional_prob_classifiers.html#robertahsccprobsequenceclassification.__init__',
+                                                                                                                                                                                               'that_nlp_library/models/roberta/conditional_prob_classifiers.py'),
+                                                                              'that_nlp_library.models.roberta.conditional_prob_classifiers.RobertaHSCCProbSequenceClassification.forward': ( 'models.roberta.conditional_prob_classifiers.html#robertahsccprobsequenceclassification.forward',
+                                                                                                                                                                                              'that_nlp_library/models/roberta/conditional_prob_classifiers.py'),
+                                                                              'that_nlp_library.models.roberta.conditional_prob_classifiers.build_standard_condition_mask': ( 'models.roberta.conditional_prob_classifiers.html#build_standard_condition_mask',
+                                                                                                                                                                              'that_nlp_library/models/roberta/conditional_prob_classifiers.py')},
+            'that_nlp_library.models.roberta.deep_hierarchical_classifiers': { 'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaConcatHeadDHCRoot': ( 'models.roberta.deep_hierarchical_classifiers.html#robertaconcatheaddhcroot',
+                                                                                                                                                                           'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaConcatHeadDHCRoot.__init__': ( 'models.roberta.deep_hierarchical_classifiers.html#robertaconcatheaddhcroot.__init__',
+                                                                                                                                                                                    'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaConcatHeadDHCRoot.forward': ( 'models.roberta.deep_hierarchical_classifiers.html#robertaconcatheaddhcroot.forward',
+                                                                                                                                                                                   'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaHSCDHCSequenceClassification': ( 'models.roberta.deep_hierarchical_classifiers.html#robertahscdhcsequenceclassification',
+                                                                                                                                                                                      'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaHSCDHCSequenceClassification.__init__': ( 'models.roberta.deep_hierarchical_classifiers.html#robertahscdhcsequenceclassification.__init__',
+                                                                                                                                                                                               'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaHSCDHCSequenceClassification.forward': ( 'models.roberta.deep_hierarchical_classifiers.html#robertahscdhcsequenceclassification.forward',
+                                                                                                                                                                                              'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaSimpleHSCDHCSequenceClassification': ( 'models.roberta.deep_hierarchical_classifiers.html#robertasimplehscdhcsequenceclassification',
+                                                                                                                                                                                            'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaSimpleHSCDHCSequenceClassification.__init__': ( 'models.roberta.deep_hierarchical_classifiers.html#robertasimplehscdhcsequenceclassification.__init__',
+                                                                                                                                                                                                     'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.RobertaSimpleHSCDHCSequenceClassification.forward': ( 'models.roberta.deep_hierarchical_classifiers.html#robertasimplehscdhcsequenceclassification.forward',
+                                                                                                                                                                                                    'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers._check_hierarchy': ( 'models.roberta.deep_hierarchical_classifiers.html#_check_hierarchy',
+                                                                                                                                                                   'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.build_DHC_conditional_mask': ( 'models.roberta.deep_hierarchical_classifiers.html#build_dhc_conditional_mask',
+                                                                                                                                                                             'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py'),
+                                                                               'that_nlp_library.models.roberta.deep_hierarchical_classifiers.loss_for_DHC': ( 'models.roberta.deep_hierarchical_classifiers.html#loss_for_dhc',
+                                                                                                                                                               'that_nlp_library/models/roberta/deep_hierarchical_classifiers.py')},
             'that_nlp_library.text_augmentation': { 'that_nlp_library.text_augmentation._remove_kwargs': ( 'text_augmentation.html#_remove_kwargs',
                                                                                                            'that_nlp_library/text_augmentation.py'),
                                                     'that_nlp_library.text_augmentation._sampling_content': ( 'text_augmentation.html#_sampling_content',
                                                                                                               'that_nlp_library/text_augmentation.py'),
                                                     'that_nlp_library.text_augmentation.remove_vnmese_accent': ( 'text_augmentation.html#remove_vnmese_accent',
                                                                                                                  'that_nlp_library/text_augmentation.py'),
                                                     'that_nlp_library.text_augmentation.sampling_with_condition': ( 'text_augmentation.html#sampling_with_condition',
```

### Comparing `that-nlp-library-0.0.1/that_nlp_library/evaluations.py` & `that-nlp-library-0.0.2/that_nlp_library/evaluations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/08_evaluations.ipynb.
 
-# %% ../nbs/08_evaluations.ipynb 23
+# %% ../nbs/08_evaluations.ipynb 26
 from __future__ import annotations
 from .utils import *
 from sklearn.metrics import classification_report,ConfusionMatrixDisplay
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 # %% auto 0
 __all__ = ['evaluate_classification_model_metadata', 'show_top_n_predictions', 'evaluate_classification_model']
 
-# %% ../nbs/08_evaluations.ipynb 24
+# %% ../nbs/08_evaluations.ipynb 27
 def _show_metrics(label,pred,metric_funcs):
     results=''
     for m_func in metric_funcs:
         m_name=callable_name(m_func)
         results+=f'{m_name}: {m_func(label,pred):.4f} . '
     return results
 
-# %% ../nbs/08_evaluations.ipynb 25
+# %% ../nbs/08_evaluations.ipynb 28
 def evaluate_classification_model_metadata(df:pd.DataFrame, # The main dataframe containing the predictions
                                            metadatas:str|list, # Metadata(s) to perform analysis
                                            label_name:str, # Label's column name
                                            pred_name:str, # Prediction's column name
                                            metric_funcs:list, # Metric(s) to calculate
                                           ):
     metadatas = val2iterable(metadatas)
@@ -38,15 +38,15 @@
         print_msg(f'Metrics for each value in {metadata}',10)
         print(f'- For all data:\n{_show_metrics(df[label_name].values,df[pred_name].values,metric_funcs)}')
         for val in np.sort(df[metadata].unique()):
             y_true=df.loc[df[metadata]==val,label_name].values
             y_pred=df.loc[df[metadata]==val,pred_name].values
             print(f'- For {val}:\n{_show_metrics(y_true,y_pred,metric_funcs)}')
 
-# %% ../nbs/08_evaluations.ipynb 29
+# %% ../nbs/08_evaluations.ipynb 32
 def show_top_n_predictions(df:pd.DataFrame, # The main dataframe containing the predictions
                           text_name:str, # Text's column name
                           label_name:str, # Label's column name
                           pred_name:str, # Prediction's column name
                           prob_name:str, # Prediction probability's column name
                           is_incorrect=True, # To show top correct or incorrect sentences
                           ascending=False, # To sort by prob_name ascendingly or descendingly
@@ -58,15 +58,15 @@
         df = df[df[pred_name]==df[label_name]]
     df = df.sort_values(prob_name,ascending=ascending)[[text_name,label_name,pred_name,prob_name]].head(n_show).values
     for row in df:
         print(f'Text: {row[0]}')
         print(f'True label: {row[1]}, {"but" if is_incorrect else ""} predict {row[2]}, with confidence {row[3]:.4f}')
         print('-'*60)
 
-# %% ../nbs/08_evaluations.ipynb 33
+# %% ../nbs/08_evaluations.ipynb 36
 def evaluate_classification_model(df:pd.DataFrame, # The main dataframe containing the predictions
                               text_name:str, # Text's column name
                               label_name:str, # Label's column name
                               pred_name:str, # Prediction's column name
                               prob_name:str, # Prediction probability's column name
                               metric_funcs:list=[], # Metric(s) to calculate
                               metadatas:str|list=[], # Metadata(s) to perform analysis
```

### Comparing `that-nlp-library-0.0.1/that_nlp_library/model_main.py` & `that-nlp-library-0.0.2/that_nlp_library/model_main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,181 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_model_main.ipynb.
 
-# %% ../nbs/03_model_main.ipynb 4
+# %% ../nbs/03_model_main.ipynb 3
 from __future__ import annotations
 import os, sys
-from transformers import Trainer, TrainingArguments
+from transformers import Trainer, TrainingArguments, AutoConfig
 from datasets import DatasetDict,Dataset
 from pathlib import Path
 import torch
 import gc
 from sklearn.metrics import accuracy_score
 from functools import partial
 import pandas as pd
 import numpy as np
 from .utils import *
 from .text_main import TextDataMain
 
 # %% auto 0
-__all__ = ['finetune', 'ModelController']
+__all__ = ['model_init_classification', 'compute_metrics_classification', 'compute_metrics_separate_singleheads',
+           'loss_for_classification', 'finetune', 'ModelController']
+
+# %% ../nbs/03_model_main.ipynb 4
+def model_init_classification(
+                              model_class, # Model's class object, e.g. RobertaHiddenStateConcatForSequenceClassification
+                              cpoint_path, # Either model string name on HuggingFace, or the path to model checkpoint
+                              output_hidden_states:bool, # To whether output the model hidden states or not. Useful when you try to build a custom classification head 
+                              device=None, # Device to train on
+                              seed=42, # Random seed
+                              body_model=None, # If not none, we use this to initialize model's body. If you only want to load the model checkpoint in cpoint_path, leave this as none
+                              model_kwargs={} # Keyword arguments for model (both head and body)
+                             ):
+    """To initialize a classification model, either from an existing HuggingFace model or custom architecture
+    
+    Can be used for binary, multi-class single-head, multi-class "two-head", and multi-label clasisifcation
+    """
+    if device is None: device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+
+    config = AutoConfig.from_pretrained(
+        cpoint_path,
+        output_hidden_states=output_hidden_states,
+    )
+    
+    seed_everything(seed)
+    if body_model is not None:
+        model = model_class(config=config,**model_kwargs)
+        layers = list(model.children())
+        print('Loading body weights. This assumes the body is the very first first-layer block of your custom architecture')
+        body_name, _ = next(iter(model.named_children()))
+        setattr(model, body_name, body_model)
+        model = model.to(device)
+        
+    else:
+        model = model_class.from_pretrained(cpoint_path,config=config,**model_kwargs).to(device)
+    return model
+
+# %% ../nbs/03_model_main.ipynb 6
+def compute_metrics_classification(pred, # An EvalPrediction object from HuggingFace (which is a named tuple with ```predictions``` and ```label_ids``` attributes)
+                                   metric_funcs=[], # A list of metric functions to evaluate
+                                   head_sizes=[], # Class size for each head,
+                                   label_names=[], # Names of the label (dependent variable) columns
+                                   is_multilabel=False, # Whether this is a multilabel classification
+                                   multilabel_threshold=0.5 # Threshold for multilabel (>= threshold is positive)
+                                  ):
+    """
+    Return a dictionary of metric name and its values. Can handle both multiclass and multilabel    
+    
+    Reference: https://github.com/huggingface/transformers/blob/dbc12269ed5546b2da9236b9f1078b95b6a4d3d5/src/transformers/trainer_utils.py#LL100C22-L100C22
+    """
+    assert len(head_sizes)==len(label_names)
+    labels = pred.label_ids 
+    if isinstance(pred.predictions,tuple):
+        preds = pred.predictions[0]
+    else:
+        preds = pred.predictions
+    results={}
+    metric_funcs = val2iterable(metric_funcs)
+    
+    for i,(_size,_name) in enumerate(zip(head_sizes,label_names)):
+        start= 0 if i==0 else start+head_sizes[i-1]
+        end = start + _size
+        _pred = preds[:,start:end]
+        if is_multilabel:
+            # sigmoid and threshold
+            _pred = (sigmoid(_pred)>=multilabel_threshold).astype(int)
+        else:
+            _pred = _pred.argmax(-1)
+        _label = labels[:,i] if len(head_sizes)>1 else labels
+        for m_func in metric_funcs:
+            m_name = callable_name(m_func)
+            results[f'{m_name}_{_name}']=m_func(_label,_pred)
+    return results
+
+# %% ../nbs/03_model_main.ipynb 8
+def compute_metrics_separate_singleheads(pred, # An EvalPrediction object from HuggingFace (which is a named tuple with ```predictions``` and ```label_ids``` attributes)
+                              metric_funcs=[], # A list of metric functions to evaluate
+                              label_names=[], # Names of the label (dependent variable) columns
+                              **kwargs
+                             ):
+    """
+    Return a dictionary of metric name and its values. Can handle both multiclass and multilabel
+    """
+    # pred: EvalPrediction object 
+    # (which is a named tuple with predictions and label_ids attributes)
+    labels = pred.label_ids # (bs,number of head separately)
+    assert labels.shape[1]==len(label_names)
+    
+    results={}
+    metric_funcs = val2iterable(metric_funcs)
+    
+    for i in range(len(label_names)):
+        _label = labels[:,i]
+        _pred = pred.predictions[i].argmax(-1)
+        for m_func in metric_funcs:
+            m_name = callable_name(m_func)
+            results[f'{m_name}_{label_names[i]}']=m_func(_label,_pred)
+    
+    return results
 
-# %% ../nbs/03_model_main.ipynb 5
+# %% ../nbs/03_model_main.ipynb 10
+def loss_for_classification(logits, # output of the last linear layer, before any softmax/sigmoid. Size: (bs,class_size)
+                            labels, # determined by your datasetdict. Size: (bs,number_of_head)
+                            is_multilabel=False, # Whether this is a multilabel classification
+                            is_multihead=False, # Whether this is a multihead (multi-level) classification
+                            head_sizes=[], # class size for each head
+                            head_weights=[], # loss weight for each head
+                           ):
+    """
+    The general loss function for classification
+    
+    - If is_multilabel is ```False``` and is_multihead is ```False```: One-Head Classification, e.g. You predict 1 out of n class
+    
+    - If is_multilabel is ```False``` and is_multihead is ```True```: Multi-Head Classification, e.g. You predict 1 out of n classes at Level 1, 
+    and 1 out of m classes at Level 2
+    
+    - If is_multilabel is ```True``` and is_multihead is ```False```: One-Head Multi-Label Classification, e.g. You predict x out of n class (x>=1)
+    
+    - If is_multilabel is ```True``` and is_multihead is ```True```: Not supported!
+    
+    """
+    if is_multilabel and is_multihead: raise ValueError('Multi-Label and Multi-Head problem is not supported')
+    head_sizes = val2iterable(head_sizes)
+    loss=0
+    if not is_multilabel:
+        if not is_multihead:
+            loss_fct = torch.nn.CrossEntropyLoss()
+            loss = loss_fct(logits.view(-1, head_sizes[0]), labels.view(-1))
+        else:
+            assert len(head_sizes)==len(head_weights),"For MultiHead, make sure len of head_sizes and head_weights equal"
+            for i,(_size,_weight) in enumerate(zip(head_sizes,head_weights)):
+                start= 0 if i==0 else start+head_sizes[i-1]
+                end = start + _size
+                loss_fct = torch.nn.CrossEntropyLoss()
+                loss = loss + _weight*loss_fct(logits[:,start:end].view(-1,_size),
+                                               labels[:,i].view(-1))
+    else:
+        if not is_multihead:
+            loss_fct = torch.nn.BCEWithLogitsLoss()
+#             label_1hot = torch.nn.functional.one_hot(labels.view(-1),num_classes=head_sizes[0])
+            loss = loss_fct(logits,
+                            labels.float())
+        else:
+            raise ValueError('Multi-Head with Multi-Label classification is not supported. Have you lost your mind?')
+#             assert len(head_sizes)==len(head_weights),"For MultiHead, make sure len of head_sizes and head_weights equal"
+#             for i,(_size,_weight) in enumerate(zip(head_sizes,head_weights)):
+#                 start= 0 if i==0 else start+head_sizes[i-1]
+#                 end = start + _size
+#                 loss_fct = torch.nn.BCEWithLogitsLoss()
+#                 loss = loss + _weight*loss_fct(logits[:,start:end].view(-1,_size),
+#                                                torch.nn.functional.one_hot(labels[:,i].view(-1),num_classes=_size).float()
+#                                               )
+            
+    return loss
+
+# %% ../nbs/03_model_main.ipynb 12
 def finetune(lr, # Learning rate
              bs, # Batch size
              wd, # Weight decay
              epochs, # Number of epochs
              ddict, # The HuggingFace datasetdict
              tokenizer,# HuggingFace tokenizer
              o_dir = './tmp_weights', # Directory to save weights
@@ -73,15 +226,15 @@
         compute_metrics=compute_metrics,
     )
     
     
     trainer.train()
     return trainer
 
-# %% ../nbs/03_model_main.ipynb 7
+# %% ../nbs/03_model_main.ipynb 14
 def _forward_pass_for_predictions(batch,
                                  model=None, # NLP model
                                  topk=1, # Number of labels to return for each head
                                  is_multilabel=False, # Is this a multilabel classification?
                                  multilabel_threshold=0.5, # The threshold for multilabel classification
                                  tokenizer=None, # HuggingFace tokenizer
                                  data_collator=None, # HuggingFace data collator
@@ -114,14 +267,17 @@
         batch = data_collator(collator_inp)
     
     inputs = {k:v.to(device) for k,v in batch.items()
               if k in tokenizer.model_input_names}
     
     _f = partial(torch.nn.functional.softmax,dim=1) if not is_multilabel else torch.sigmoid
     
+    # switch to eval mode for evaluation
+    if model.training:
+        model.eval()
     with torch.no_grad():
         outputs = model(**inputs)
         outputs_logits = outputs.logits
         outputs_list=[]
         if is_dhc:
             # outputs_logits will be a list of n (typically 2) heads' logits, each has shape (bs,class_size)
             for i in range(len(label_names)):
@@ -146,26 +302,26 @@
         else:
             for i in range(len(label_names)):
                 _p,_l = torch.topk(outputs_list[i],topk,dim=-1)
                 if topk==1:
                     _l,_p = _l[:,0],_p[:,0]
                 pred_label_list.append(_l)
                 pred_prob_list.append(_p)
-#             if topk==1:
-#                 for i in range(len(label_names)):
-#                     pred_label_list[i]=pred_label_list[i][:,0]
-#                     pred_prob_list[i]=pred_prob_list[i][:,0]
-                
+    
+    # Switch back to train mode
+    if not model.training:
+        model.train()
+        
     results={}
     for i in range(len(label_names)):
         results[f'pred_{label_names[i]}']= pred_label_list[i].numpy()
         results[f'pred_prob_{label_names[i]}']= pred_prob_list[i].numpy()
     return results
 
-# %% ../nbs/03_model_main.ipynb 8
+# %% ../nbs/03_model_main.ipynb 15
 class ModelController():
     def __init__(self,
                  model, # NLP model
                  data_store:TextDataMain=None, # a TextDataMain object
                  metric_funcs=[accuracy_score], # Metric function (can be from Sklearn)
                  seed=42, # Random seed
                 ):
@@ -319,14 +475,9 @@
                     for j in range(1,topk+1):
                         df1[f'pred_{label_names[i]}_top{j}'] =  df1[f'pred_{label_names[i]}_top{j}'].apply(lambda x: label_lists[i][int(x)])
 
                     df_result = pd.concat([df_result,df1,df1_prob],axis=1)
             else:
                 get_label_str_multilabel = lambda row: ','.join([label_lists[i][int(j)] for j in np.where(row==True)[0]])
                 df_result[f'pred_{label_names[i]}_string'] = df_result[f'pred_{label_names[i]}'].apply(get_label_str_multilabel)
-#                 # Broadcasting the label list, then perform np.where on mask result from ddict
-#                 label_broadcast = np.tile(np.array(label_lists[i]),(df_result.shape[0],1))
-#                 _mask = np.vstack(df_result[f'pred_{label_names[i]}'].values)
-#                 label_pass_thres= np.where(_mask==True,label_broadcast,'')
-#                 _result = [','.join(row[row != '']) for row in label_pass_thres]
-#                 df_result[f'pred_{label_names[i]}'] = _result
+
         return df_result
```

### Comparing `that-nlp-library-0.0.1/that_nlp_library/models/conditional_prob_classifiers.py` & `that-nlp-library-0.0.2/that_nlp_library/models/roberta/conditional_prob_classifiers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/06_models.conditional_prob_classifiers.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/06_models.roberta.conditional_prob_classifiers.ipynb.
 
-# %% ../../nbs/06_models.conditional_prob_classifiers.ipynb 3
+# %% ../../../nbs/06_models.roberta.conditional_prob_classifiers.ipynb 3
 from __future__ import annotations
 from collections import defaultdict
 import numpy as np
 import torch
 from transformers.models.roberta.configuration_roberta import RobertaConfig
 from transformers.models.roberta.modeling_roberta import RobertaModel
-from .classifiers import RobertaConcatHeadSimple
+from .classifiers import ConcatHeadSimple
 from sklearn.preprocessing import MultiLabelBinarizer
 from transformers.modeling_outputs import SequenceClassifierOutput
 from transformers.models.roberta.modeling_roberta import RobertaPreTrainedModel
-from .classifiers import loss_for_classification
+from ...model_main import loss_for_classification
 
 # %% auto 0
 __all__ = ['build_standard_condition_mask', 'RobertaHSCCProbSequenceClassification']
 
-# %% ../../nbs/06_models.conditional_prob_classifiers.ipynb 5
+# %% ../../../nbs/06_models.roberta.conditional_prob_classifiers.ipynb 5
 def build_standard_condition_mask(df_labels,
                                   label1,label2):
     L1_SIZE = df_labels[label1].nunique()
     L2_SIZE = df_labels[label2].nunique()
 
     
     df_labels = df_labels.drop_duplicates().sort_values([label1,label2])
@@ -31,62 +31,60 @@
     mlb.fit([np.arange(L2_SIZE)])
     mask_l2 = torch.tensor(mlb.transform(list(_d.values())) == 1)
     
     mask_final= torch.cat((mask_l1,mask_l2),1)
     
     return mask_final
 
-# %% ../../nbs/06_models.conditional_prob_classifiers.ipynb 8
+# %% ../../../nbs/06_models.roberta.conditional_prob_classifiers.ipynb 8
 class RobertaHSCCProbSequenceClassification(RobertaPreTrainedModel):
     """
     Roberta Conditional Probability Architecture with Hidden-State-Concatenation for Sequence Classification task
     """
     config_class = RobertaConfig
 
     def __init__(self, 
                  config, # HuggingFace model configuration
-                 pretrained_roberta=None, # HuggingFace Roberta Body (useful for knowledge transfering task)
-                 concathead_class=RobertaConcatHeadSimple,
-                 classifier_dropout=0.1, # Dropout ratio (for dropout layer right before the last nn.Linear)
-                 last_hidden_size=768, # Last hidden size (before the last nn.Linear)
                  size_l1=None, # Number of classes for head 1
                  size_l2=None, # Number of classes for head 2
                  standard_mask=None, # Mask for conditional probability
-                 device=None # CPU or GPU
+                 layer2concat=4, # number of hidden layer to concatenate (counting from top)
+                 device=None, # CPU or GPU
+                 head_class=None, # The class object of the head. You can use RobertaClassificationHeadCustom as default
+                 **head_class_kwargs, # Keyword arguments for the head class
                 ):
         super().__init__(config)
         self.training_device = device if device is not None else torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         self.size_l1 = size_l1
         self.size_l2 = size_l2
+        self.layer2concat=layer2concat
+        self.head_class_sizes=[size_l1,size_l2] # will be useful for metric calculation later
         
         # set num_labels for config
         num_labels = size_l1+size_l2
         config.num_labels = num_labels
         
-        self.roberta = RobertaModel(config, add_pooling_layer=False) if pretrained_roberta is None else pretrained_roberta
+        self.body_model = RobertaModel(config, add_pooling_layer=False)
         self.standard_mask = standard_mask.to(self.training_device)
-        self.classification_head = concathead_class(config=config,classifier_dropout=classifier_dropout,
-                                                    last_hidden_size=last_hidden_size,
-                                                    n_output=num_labels) 
+        self.classification_head = head_class(config=config,
+                                              **head_class_kwargs) 
 
-        if pretrained_roberta is None:
-            self.init_weights()
 
     def forward(self, input_ids=None, attention_mask=None, token_type_ids=None,
                 labels=None, **kwargs):
         # Use model body to get encoder representations
         # the only ones we need for now are input_ids and attention_mask
-        outputs = self.roberta(input_ids, attention_mask=attention_mask,
+        outputs = self.body_model(input_ids, attention_mask=attention_mask,
                                token_type_ids=token_type_ids, **kwargs)
         
         hidden_states = outputs['hidden_states'] # tuples with len 13 (number of layer/block)
         # each with shape: (bs,seq_len,hidden_size_len), e.g. for phobert: (bs,256, 768)
         # Note: hidden_size_len = embedding_size
         
-        hidden_concat = torch.cat([hidden_states[i][:,0] for i in range(-1,-4-1,-1)],
+        hidden_concat = torch.cat([hidden_states[i][:,0] for i in range(-1,-self.layer2concat-1,-1)],
                                   -1) # (bs,768*4)
         
         # classification head
         logits = self.classification_head(hidden_concat)
 
         loss = None
         if labels is not None:
```

### Comparing `that-nlp-library-0.0.1/that_nlp_library/models/deep_hierarchical_classifiers.py` & `that-nlp-library-0.0.2/that_nlp_library/models/roberta/deep_hierarchical_classifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/05_models.deep_hierarchical_classifiers.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb.
 
-# %% ../../nbs/05_models.deep_hierarchical_classifiers.ipynb 3
+# %% ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb 3
 from __future__ import annotations
 import torch
 from transformers.models.roberta.configuration_roberta import RobertaConfig
 from transformers.models.roberta.modeling_roberta import RobertaModel
 from transformers.modeling_outputs import SequenceClassifierOutput
 from transformers.models.roberta.modeling_roberta import RobertaPreTrainedModel
 from sklearn.preprocessing import MultiLabelBinarizer
 
 # %% auto 0
-__all__ = ['build_DHC_conditional_mask', 'loss_for_DHC', 'RobertaConcatHeadDHCRoot', 'RobertaHSCSimpleDHCSequenceClassification',
+__all__ = ['build_DHC_conditional_mask', 'loss_for_DHC', 'RobertaConcatHeadDHCRoot', 'RobertaSimpleHSCDHCSequenceClassification',
            'RobertaHSCDHCSequenceClassification']
 
-# %% ../../nbs/05_models.deep_hierarchical_classifiers.ipynb 5
+# %% ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb 5
 def build_DHC_conditional_mask(df_labels,
                                   label1,label2):
     """
     This is really similar to `build_standard_condition_mask`, 
     but we don't concatenate l1 1-hot matrix and l2 1-hot matrix
     """
     df_labels = df_labels.drop_duplicates().sort_values([label1,label2])
     _d = df_labels.groupby([label1])[label2].apply(list).to_dict()
     
     mlb = MultiLabelBinarizer()
     results = mlb.fit_transform([v for k,v in sorted(_d.items())])
     return torch.from_numpy(results).float()
 
-# %% ../../nbs/05_models.deep_hierarchical_classifiers.ipynb 10
+# %% ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb 10
 def _check_hierarchy(l1_pred,l2_pred,dhc_mask,size_l2):
     # Check if the predicted class at L2 is a children of the class predicted at L1 for the entire batch
     # if is a children return 0, else 1
     _l1_pred = dhc_mask[l1_pred] # bs,size_l2
     _l2_pred = torch.nn.functional.one_hot(l2_pred, num_classes=size_l2) # bs, size_l2
     return (~torch.mul(_l1_pred,_l2_pred).sum(axis=1).bool()).float()
 
-# %% ../../nbs/05_models.deep_hierarchical_classifiers.ipynb 11
+# %% ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb 11
 def loss_for_DHC(l1_repr_logits, # Head 1's logit output
                  l2_repr_logits, # Head 2's logit output
                  labels_l1, # True label for head 1
                  labels_l2, # True label for head 2
                  dhc_mask, # A one-hot matrix between classes of head 1 and 2
                  lloss_weight=1.0, # Weight for Layer Loss (lloss)
                  dloss_weight=0.8 # Weight for Dependence Loss (dloss)
@@ -65,85 +65,88 @@
     dloss = dloss_weight*(dloss_l1 + dloss_l2)  
     
     
     loss = lloss + dloss
     
     return loss
 
-# %% ../../nbs/05_models.deep_hierarchical_classifiers.ipynb 13
+# %% ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb 13
 class RobertaConcatHeadDHCRoot(torch.nn.Module):
     """
     Concatenated head for Roberta DHC Classification Model. 
     """
     def __init__(self,
                  config, # HuggingFace model configuration
                  classifier_dropout=0.1, # Dropout ratio (for dropout layer right before the last nn.Linear)
                  last_hidden_size=768, # Last hidden size (before the last nn.Linear)
+                 layer2concat=4, # number of hidden layer to concatenate (counting from top)
                  **kwargs
                 ):
         super().__init__()
         self.classifier_dropout=classifier_dropout
         self.last_hidden_size=last_hidden_size
         self.dropout = torch.nn.Dropout(classifier_dropout)
-        self.pre_classifier = torch.nn.Linear(4*config.hidden_size,last_hidden_size)    
+        self.pre_classifier = torch.nn.Linear(layer2concat*config.hidden_size,
+                                              last_hidden_size)    
     def forward(self, inp, **kwargs):
         x = inp
         x = self.dropout(x)
         x = self.pre_classifier(x)
         x = torch.tanh(x)
 #         x = torch.relu(x)
         return x
 
-# %% ../../nbs/05_models.deep_hierarchical_classifiers.ipynb 15
-class RobertaHSCSimpleDHCSequenceClassification(RobertaPreTrainedModel):
+# %% ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb 15
+class RobertaSimpleHSCDHCSequenceClassification(RobertaPreTrainedModel):
     """
     Roberta Simple-DHC Architecture with Hidden-State-Concatenation for Sequence Classification task
     """
     config_class = RobertaConfig
 
     def __init__(self, 
                  config, # HuggingFace model configuration
                  dhc_mask, # A one-hot matrix between classes of head 1 and 2
-                 pretrained_roberta=None, # HuggingFace Roberta Body (useful for knowledge transfering task)
                  lloss_weight=1.0, # Weight for Layer Loss (lloss)
                  dloss_weight=0.8, # Weight for Dependence Loss (dloss)
+                 layer2concat=4, # number of hidden layer to concatenate (counting from top)
                  device=None # CPU or GPU
                 ):
         
         super().__init__(config)
         self.training_device = device if device is not None else torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         self.size_l1 = dhc_mask.shape[0]
         self.size_l2 = dhc_mask.shape[1]
+        self.head_class_sizes=[self.size_l1,self.size_l2] # will be useful for metric calculation later
+
         self.dhc_mask = dhc_mask.to(self.training_device)
-            
+        self.layer2concat=layer2concat
+    
         self.lloss_weight = lloss_weight
         self.dloss_weight = dloss_weight
         
-        self.roberta = RobertaModel(config, add_pooling_layer=False) if pretrained_roberta is None else pretrained_roberta
+        self.body_model = RobertaModel(config, add_pooling_layer=False)
         
-        self.linear_L1_logit = torch.nn.Linear(4*config.hidden_size,self.size_l1)
+        self.linear_L1_logit = torch.nn.Linear(layer2concat*config.hidden_size,self.size_l1)
 
-        self.linear_L2 = torch.nn.Linear(4*config.hidden_size, abs(self.size_l2-self.size_l1))
+        self.linear_L2 = torch.nn.Linear(layer2concat*config.hidden_size, abs(self.size_l2-self.size_l1))
         self.linear_L2_logit = torch.nn.Linear(self.size_l2,self.size_l2)
         
-        if pretrained_roberta is None:
-            self.init_weights()
     
     def forward(self, input_ids=None, attention_mask=None, token_type_ids=None,
                 labels=None, **kwargs):
         # Use model body to get encoder representations
         # the only ones we need for now are input_ids and attention_mask
-        outputs = self.roberta(input_ids, attention_mask=attention_mask,
+        outputs = self.body_model(input_ids, attention_mask=attention_mask,
                                token_type_ids=token_type_ids, **kwargs)
         
         hidden_states = outputs['hidden_states'] # tuples with len 13 (number of layer/block)
         # each with shape: (bs,seq_len,hidden_size_len), e.g. for phobert: (bs,256, 768)
         # Note: hidden_size_len = embedding_size
         
-        hidden_concat = torch.cat([hidden_states[i][:,0] for i in range(-1,-4-1,-1)],
+        hidden_concat = torch.cat([hidden_states[i][:,0] for i in range(-1,-self.layer2concat-1,-1)],
                                   -1) # (bs,768*4)
         
         # root_representation
         root_repr = hidden_concat # (bs,768*4) 
         
         l1_repr_logits = self.linear_L1_logit(root_repr) # (bs,size_l1)
         
@@ -164,74 +167,75 @@
                                 self.lloss_weight,self.dloss_weight)
             
         # Return model output object
         return SequenceClassifierOutput(loss=loss, logits=(l1_repr_logits,l2_repr_logits),
                                      hidden_states=None,
                                      attentions=outputs.attentions)
 
-# %% ../../nbs/05_models.deep_hierarchical_classifiers.ipynb 17
+# %% ../../../nbs/05_models.roberta.deep_hierarchical_classifiers.ipynb 17
 class RobertaHSCDHCSequenceClassification(RobertaPreTrainedModel):
     """
     Roberta DHC Architecture with Hidden-State-Concatenation for Sequence Classification task
     """    
     config_class = RobertaConfig
 
     def __init__(self, 
                  config, # HuggingFace model configuration
                  dhc_mask, # A one-hot matrix between classes of head 1 and 2
-                 pretrained_roberta=None, # HuggingFace Roberta Body (useful for knowledge transfering task)
                  classifier_dropout=0.1, # Dropout ratio (for dropout layer right before the last nn.Linear)
                  last_hidden_size=768, # Last hidden size (before the last nn.Linear)
                  linear_l1_size=None, # last hidden size for head 1
                  linear_l2_size=None, # last hidden size for head 2
                  lloss_weight=1.0, # Weight for Layer Loss (lloss)
                  dloss_weight=0.8, # Weight for Dependence Loss (dloss)
+                 layer2concat=4, # number of hidden layer to concatenate (counting from top)
                  device=None # CPU or GPU
                 ):
         
         super().__init__(config)
         self.training_device = device if device is not None else torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         self.size_l1 = dhc_mask.shape[0]
         self.size_l2 = dhc_mask.shape[1]
-        
+        self.head_class_sizes=[self.size_l1,self.size_l2] # will be useful for metric calculation later
+
         self.dhc_mask = dhc_mask.to(self.training_device)
-    
+        self.layer2concat=layer2concat
+
+        
         if linear_l1_size is None: linear_l1_size = (last_hidden_size+self.size_l1)//2 # 389
         if linear_l2_size is None: linear_l2_size = (last_hidden_size+self.size_l2)//2 # 417
             
         self.lloss_weight = lloss_weight
         self.dloss_weight = dloss_weight
         
-        self.roberta = RobertaModel(config, add_pooling_layer=False) if pretrained_roberta is None else pretrained_roberta
+        self.body_model = RobertaModel(config, add_pooling_layer=False)
         self.root_representation = RobertaConcatHeadDHCRoot(config=config,
                                                             classifier_dropout=classifier_dropout,
                                                             last_hidden_size=last_hidden_size)
         
         self.linear_L1 = torch.nn.Linear(last_hidden_size, linear_l1_size)
         self.linear_L2 = torch.nn.Linear(last_hidden_size, linear_l2_size)
         
         self.linear_L1_logit = torch.nn.Linear(linear_l1_size,self.size_l1)
         self.linear_L2_logit = torch.nn.Linear(linear_l1_size + linear_l2_size,self.size_l2)
         
-        if pretrained_roberta is None:
-            self.init_weights()
 
     
     def forward(self, input_ids=None, attention_mask=None, token_type_ids=None,
                 labels=None, **kwargs):
         # Use model body to get encoder representations
         # the only ones we need for now are input_ids and attention_mask
-        outputs = self.roberta(input_ids, attention_mask=attention_mask,
+        outputs = self.body_model(input_ids, attention_mask=attention_mask,
                                token_type_ids=token_type_ids, **kwargs)
         
         hidden_states = outputs['hidden_states'] # tuples with len 13 (number of layer/block)
         # each with shape: (bs,seq_len,hidden_size_len), e.g. for phobert: (bs,256, 768)
         # Note: hidden_size_len = embedding_size
         
-        hidden_concat = torch.cat([hidden_states[i][:,0] for i in range(-1,-4-1,-1)],
+        hidden_concat = torch.cat([hidden_states[i][:,0] for i in range(-1,-self.layer2concat-1,-1)],
                                   -1) # (bs,768*4)
         
         # root_representation
         root_repr = self.root_representation(hidden_concat) # (bs,768) 
         
         l1_repr = self.linear_L1(root_repr) # (bs,linear_L1_size)
         l1_repr_logits = self.linear_L1_logit(l1_repr) # (bs,size_l1)
```

### Comparing `that-nlp-library-0.0.1/that_nlp_library/text_augmentation.py` & `that-nlp-library-0.0.2/that_nlp_library/text_augmentation.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.0.1/that_nlp_library/text_main.py` & `that-nlp-library-0.0.2/that_nlp_library/text_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,18 @@
     else:
         main_ddict['train'] = all_dataset.select(trn_idx)
 
     if val_idx is not None:  
         main_ddict['validation'] = all_dataset.select(val_idx)
     
     print_msg("Map Tokenize Function",20)
-    main_ddict_tokenized = main_ddict.map(partial(tokenize_function,tok=tokenizer,is_split_into_words=is_split_into_words,max_length=max_length))
+    main_ddict_tokenized = main_ddict.map(partial(tokenize_function,
+                                                  tok=tokenizer,
+                                                  is_split_into_words=is_split_into_words,
+                                                  max_length=max_length),batched=True)
     
     return main_ddict_tokenized
 
 # %% ../nbs/00_text_main.ipynb 45
 class TextDataMain():
     def __init__(self,
                  df: pd.DataFrame, # The main dataframe
@@ -366,15 +369,15 @@
                        is_split_into_words=False, # Is text split into list or not
                        max_length=None, # pad to model's allowed max length (default is max_sequence_length)
                        trn_ratio=1., # Portion of training data to be converted to datasetdict. Useful for sample experiments
                        seed=42 # Random seed
                       ):
         if not self._main_called:
             self._main_text_processing()
-        val_idx = self.df[self.df['is_valid']].index.values if self.val_ratio else None
+        val_idx = self.df[self.df['is_valid']].index.values if self.val_ratio is not None else None
         trn_idx = self.df[~self.df['is_valid']].index.values
         if trn_ratio<1. and trn_ratio>0.:
             rng = np.random.default_rng(self.seed)
             _idxs = rng.permutation(len(trn_idx))
             _cutoff = int(trn_ratio*len(trn_idx)) 
             trn_idx = _idxs[:_cutoff]
             
@@ -440,10 +443,11 @@
         for c in self.cols_to_keep:
             if c not in self.label_names+[self.main_content]: kv_pairs[c] = df_test[c].tolist()
         
         test_dataset = Dataset.from_dict(kv_pairs)
         test_ddict = DatasetDict()
         test_ddict['test'] = test_dataset
         test_ddict_tokenized = test_ddict.map(partial(tokenize_function,tok=self.tokenizer,
-                                                  is_split_into_words=self.is_split_into_words,max_length=self.max_length))
+                                                      is_split_into_words=self.is_split_into_words,
+                                                      max_length=self.max_length),batched=True)
         
         return test_ddict_tokenized
```

### Comparing `that-nlp-library-0.0.1/that_nlp_library/text_transformation.py` & `that-nlp-library-0.0.2/that_nlp_library/text_transformation.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.0.1/that_nlp_library/utils.py` & `that-nlp-library-0.0.2/that_nlp_library/utils.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.0.1/that_nlp_library.egg-info/PKG-INFO` & `that-nlp-library-0.0.2/that_nlp_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-nlp-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Aim to be a convenient NLP library with the help from HuggingFace
 Home-page: https://github.com/anhquan0412/that-nlp-library
 Author: Quan Tran
 Author-email: anhquan0412@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev,jupyter,notebook,python,nlp,natural language processing,transformer,fastai,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `that-nlp-library-0.0.1/that_nlp_library.egg-info/SOURCES.txt` & `that-nlp-library-0.0.2/that_nlp_library.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 that_nlp_library.egg-info/SOURCES.txt
 that_nlp_library.egg-info/dependency_links.txt
 that_nlp_library.egg-info/entry_points.txt
 that_nlp_library.egg-info/not-zip-safe
 that_nlp_library.egg-info/requires.txt
 that_nlp_library.egg-info/top_level.txt
 that_nlp_library/models/__init__.py
-that_nlp_library/models/classifiers.py
-that_nlp_library/models/conditional_prob_classifiers.py
-that_nlp_library/models/deep_hierarchical_classifiers.py
+that_nlp_library/models/roberta/__init__.py
+that_nlp_library/models/roberta/classifiers.py
+that_nlp_library/models/roberta/conditional_prob_classifiers.py
+that_nlp_library/models/roberta/deep_hierarchical_classifiers.py
```

