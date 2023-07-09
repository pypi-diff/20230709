# Comparing `tmp/mac_voice_assistant-0.3.1.tar.gz` & `tmp/mac_voice_assistant-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/manishraj/Documents/pycharm_projects/mac_voice_assistant/dist/.tmp-6h7j9mqz/mac_voice_assistant-0.3.1.tar", last modified: Fri Feb 17 19:03:11 2023, max compression
+gzip compressed data, was "mac_voice_assistant-0.3.2.tar", last modified: Sun Jul  9 15:54:00 2023, max compression
```

## Comparing `mac_voice_assistant-0.3.1.tar` & `mac_voice_assistant-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 manishraj   (501) staff       (20)        0 2023-02-17 19:03:11.552927 mac_voice_assistant-0.3.1/
--rw-r--r--   0 manishraj   (501) staff       (20)     1067 2022-12-25 03:52:58.000000 mac_voice_assistant-0.3.1/LICENSE
--rw-r--r--   0 manishraj   (501) staff       (20)     2571 2023-02-17 19:03:11.552354 mac_voice_assistant-0.3.1/PKG-INFO
--rw-r--r--   0 manishraj   (501) staff       (20)     1686 2022-12-27 17:29:51.000000 mac_voice_assistant-0.3.1/README.md
-drwxr-xr-x   0 manishraj   (501) staff       (20)        0 2023-02-17 19:03:11.527961 mac_voice_assistant-0.3.1/mac_voice_assistant/
--rw-r--r--   0 manishraj   (501) staff       (20)    13729 2023-02-17 18:18:51.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/AI.py
-drwxr-xr-x   0 manishraj   (501) staff       (20)        0 2023-02-17 19:03:11.534675 mac_voice_assistant-0.3.1/mac_voice_assistant/IA/
--rw-r--r--   0 manishraj   (501) staff       (20)     7877 2023-02-17 18:33:58.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/IA/IA.py
--rw-r--r--   0 manishraj   (501) staff       (20)        0 2022-12-26 03:36:25.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/IA/__init__.py
--rw-r--r--   0 manishraj   (501) staff       (20)     1901 2023-02-17 18:18:51.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/IA/default_intents.json
--rw-r--r--   0 manishraj   (501) staff       (20)        1 2022-12-25 05:52:56.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/__init__.py
-drwxr-xr-x   0 manishraj   (501) staff       (20)        0 2023-02-17 19:03:11.537825 mac_voice_assistant-0.3.1/mac_voice_assistant/audio_samples/
--rw-r--r--   0 manishraj   (501) staff       (20)        1 2022-12-25 05:52:56.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/audio_samples/__init__.py
--rw-r--r--   0 manishraj   (501) staff       (20)   100558 2022-12-25 03:52:58.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/audio_samples/beep.wav
-drwxr-xr-x   0 manishraj   (501) staff       (20)        0 2023-02-17 19:03:11.541716 mac_voice_assistant-0.3.1/mac_voice_assistant/utils/
--rw-r--r--   0 manishraj   (501) staff       (20)        0 2023-01-16 20:10:47.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/utils/__init__.py
--rw-r--r--   0 manishraj   (501) staff       (20)      325 2023-01-16 20:10:47.000000 mac_voice_assistant-0.3.1/mac_voice_assistant/utils/logger.py
-drwxr-xr-x   0 manishraj   (501) staff       (20)        0 2023-02-17 19:03:11.532457 mac_voice_assistant-0.3.1/mac_voice_assistant.egg-info/
--rw-r--r--   0 manishraj   (501) staff       (20)     2571 2023-02-17 19:03:11.000000 mac_voice_assistant-0.3.1/mac_voice_assistant.egg-info/PKG-INFO
--rw-r--r--   0 manishraj   (501) staff       (20)      673 2023-02-17 19:03:11.000000 mac_voice_assistant-0.3.1/mac_voice_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 manishraj   (501) staff       (20)        1 2023-02-17 19:03:11.000000 mac_voice_assistant-0.3.1/mac_voice_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 manishraj   (501) staff       (20)      130 2023-02-17 19:03:11.000000 mac_voice_assistant-0.3.1/mac_voice_assistant.egg-info/requires.txt
--rw-r--r--   0 manishraj   (501) staff       (20)       26 2023-02-17 19:03:11.000000 mac_voice_assistant-0.3.1/mac_voice_assistant.egg-info/top_level.txt
--rw-r--r--   0 manishraj   (501) staff       (20)     1076 2023-02-17 19:02:01.000000 mac_voice_assistant-0.3.1/pyproject.toml
--rw-r--r--   0 manishraj   (501) staff       (20)       38 2023-02-17 19:03:11.553139 mac_voice_assistant-0.3.1/setup.cfg
--rw-r--r--   0 manishraj   (501) staff       (20)      592 2023-02-17 19:02:01.000000 mac_voice_assistant-0.3.1/setup.py
-drwxr-xr-x   0 manishraj   (501) staff       (20)        0 2023-02-17 19:03:11.550594 mac_voice_assistant-0.3.1/tests/
--rw-r--r--   0 manishraj   (501) staff       (20)        0 2022-12-25 04:26:02.000000 mac_voice_assistant-0.3.1/tests/__init__.py
--rw-r--r--   0 manishraj   (501) staff       (20)     2001 2022-12-25 03:52:58.000000 mac_voice_assistant-0.3.1/tests/example.py
--rw-r--r--   0 manishraj   (501) staff       (20)      189 2023-02-17 18:47:47.000000 mac_voice_assistant-0.3.1/tests/my_hotkey.py
--rw-r--r--   0 manishraj   (501) staff       (20)      673 2023-01-15 15:23:55.000000 mac_voice_assistant-0.3.1/tests/test.py
--rw-r--r--   0 manishraj   (501) staff       (20)      659 2022-12-25 03:52:58.000000 mac_voice_assistant-0.3.1/tests/text_typing.py
+drwxr-xr-x   0 hogwarts   (501) staff       (20)        0 2023-07-09 15:54:00.005457 mac_voice_assistant-0.3.2/
+-rw-r--r--   0 hogwarts   (501) staff       (20)     1067 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/LICENSE
+-rw-r--r--   0 hogwarts   (501) staff       (20)     3771 2023-07-09 15:54:00.004891 mac_voice_assistant-0.3.2/PKG-INFO
+-rw-r--r--   0 hogwarts   (501) staff       (20)     2886 2023-07-09 15:45:39.000000 mac_voice_assistant-0.3.2/README.md
+drwxr-xr-x   0 hogwarts   (501) staff       (20)        0 2023-07-09 15:53:59.993319 mac_voice_assistant-0.3.2/mac_voice_assistant/
+-rw-r--r--   0 hogwarts   (501) staff       (20)    13599 2023-07-09 15:20:47.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/AI.py
+drwxr-xr-x   0 hogwarts   (501) staff       (20)        0 2023-07-09 15:53:59.996965 mac_voice_assistant-0.3.2/mac_voice_assistant/IA/
+-rw-r--r--   0 hogwarts   (501) staff       (20)     7286 2023-07-09 14:19:35.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/IA/IA.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)        0 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/IA/__init__.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)        1 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/__init__.py
+drwxr-xr-x   0 hogwarts   (501) staff       (20)        0 2023-07-09 15:53:59.997933 mac_voice_assistant-0.3.2/mac_voice_assistant/audio_samples/
+-rw-r--r--   0 hogwarts   (501) staff       (20)        1 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/audio_samples/__init__.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)   100558 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/audio_samples/beep.wav
+-rw-r--r--   0 hogwarts   (501) staff       (20)     1901 2023-07-09 13:59:08.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/default_intents.json
+drwxr-xr-x   0 hogwarts   (501) staff       (20)        0 2023-07-09 15:53:59.999802 mac_voice_assistant-0.3.2/mac_voice_assistant/utils/
+-rw-r--r--   0 hogwarts   (501) staff       (20)        0 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/utils/__init__.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)      325 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/mac_voice_assistant/utils/logger.py
+drwxr-xr-x   0 hogwarts   (501) staff       (20)        0 2023-07-09 15:53:59.995641 mac_voice_assistant-0.3.2/mac_voice_assistant.egg-info/
+-rw-r--r--   0 hogwarts   (501) staff       (20)     3771 2023-07-09 15:53:59.000000 mac_voice_assistant-0.3.2/mac_voice_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 hogwarts   (501) staff       (20)      686 2023-07-09 15:53:59.000000 mac_voice_assistant-0.3.2/mac_voice_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 hogwarts   (501) staff       (20)        1 2023-07-09 15:53:59.000000 mac_voice_assistant-0.3.2/mac_voice_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 hogwarts   (501) staff       (20)      130 2023-07-09 15:53:59.000000 mac_voice_assistant-0.3.2/mac_voice_assistant.egg-info/requires.txt
+-rw-r--r--   0 hogwarts   (501) staff       (20)       26 2023-07-09 15:53:59.000000 mac_voice_assistant-0.3.2/mac_voice_assistant.egg-info/top_level.txt
+-rw-r--r--   0 hogwarts   (501) staff       (20)     1076 2023-07-09 15:52:30.000000 mac_voice_assistant-0.3.2/pyproject.toml
+-rw-r--r--   0 hogwarts   (501) staff       (20)       38 2023-07-09 15:54:00.005642 mac_voice_assistant-0.3.2/setup.cfg
+-rw-r--r--   0 hogwarts   (501) staff       (20)      589 2023-07-09 15:52:30.000000 mac_voice_assistant-0.3.2/setup.py
+drwxr-xr-x   0 hogwarts   (501) staff       (20)        0 2023-07-09 15:54:00.004111 mac_voice_assistant-0.3.2/tests/
+-rw-r--r--   0 hogwarts   (501) staff       (20)        0 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/tests/__init__.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)     2001 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/tests/example.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)      189 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/tests/my_hotkey.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)      673 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/tests/test.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)      659 2023-07-05 11:58:10.000000 mac_voice_assistant-0.3.2/tests/text_typing.py
+-rw-r--r--   0 hogwarts   (501) staff       (20)      773 2023-07-09 15:11:14.000000 mac_voice_assistant-0.3.2/tests/voices.py
```

### Comparing `mac_voice_assistant-0.3.1/LICENSE` & `mac_voice_assistant-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mac_voice_assistant-0.3.1/mac_voice_assistant/AI.py` & `mac_voice_assistant-0.3.2/mac_voice_assistant/AI.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from time import sleep
 from queue import Empty
 from .IA.IA import GenericAssistant
 from playsound import playsound
 
 
 class Assistant(GenericAssistant):
-    def __init__(self, intents, intent_methods=None, model_name="assistant_model"):
+    def __init__(self, intents, intent_methods={}, model_name="assistant_model"):
         super().__init__(intents, intent_methods, model_name)
 
         # Initialize Recognizer and Microphone instances
         self.recognizer = sr.Recognizer()
         self.microphone = sr.Microphone()
         self.recognizer.energy_threshold = 100
         self.recognizer.dynamic_energy_threshold = True
@@ -25,38 +25,36 @@
         self.recognizer.dynamic_energy_adjustment_ratio = 1.5
         self.recognizer.pause_threshold = 0.5
 
         # Initialize speech engine instance
         self.engine = tts.init()
         rate = self.engine.getProperty('rate')
         self.default_speak_rate = rate - 40
-        self.default_voice = 2
+        self.default_voice = 83
         self.engine.setProperty('rate', self.default_speak_rate)
         self.speech_voices = self.engine.getProperty('voices')
         self.engine.setProperty('voice', self.speech_voices[self.default_voice].id)
 
         # Initialize Refs
         self.CALIBRATED = False
         self.SPEAKING = False
         self.LISTENING = False
         self.STOP_LISTENING = False
         self.audio_file_path = 'mac_voice_assistant/audio_samples/beep.wav'
-        self.set_audio_file_path()
 
         self.mappings = {
             'set_volume' : self.set_volume,
             'set_voice'  : self.set_voice,
             'set_rate'   : self.set_rate,
             'set_name'   : self.set_name,
             'calibrate'  : self.recalibrate,
             'speak_time' : self.speak_time,
             'tell_joke'  : self.tell_joke,
             'stop_assist': self.quit_program
         }
-        self.set_default_intent_methods()
 
     #  +++++++++++++++++++ Core methods  +++++++++++++++++++++++ #
     def set_intent_methods(self, intent_methods):
         for key, value in intent_methods.items():
             self.intent_methods[key] = value
 
     def set_default_intent_methods(self):
@@ -68,17 +66,15 @@
         if os.path.exists(default_audio_path):
             return default_audio_path
         else:
             for path in sys.path:
                 if 'site-packages' in path:
                     return path + '/mac_voice_assistant/audio_samples/beep.wav'
 
-    def set_audio_file_path(self, path='default'):
-        if path == 'default':  # for custom audio sounds, override this path with the file of your choice during setup
-            path = self.get_audio_files_path()
+    def set_audio_file_path(self, path):
         self.audio_file_path = path
 
     def calibrate(self):
         print('Adjusting for ambient noise')
         with self.microphone as source:
             print("Please do not speak during calibration")
             sleep(2)
@@ -232,15 +228,18 @@
             self.tasks.task_done()
         else:
             result = task()
         self.log.debug('worker thread ended')
         return result
 
     def assist(self):
+        path = self.get_audio_files_path()
+        self.set_audio_file_path(path)
         self.calibrate()
+        self.set_default_intent_methods()
         self.run()
 
     def set_name(self):
         self.speak("What shall I set my name as?")
         audio = self.listen_for_audio()
         name = self.transcribe(audio)
         self.model_name = name
```

### Comparing `mac_voice_assistant-0.3.1/mac_voice_assistant/IA/IA.py` & `mac_voice_assistant-0.3.2/mac_voice_assistant/IA/IA.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Intelligent Assistant"""
 import random
 import json
 import pickle
 import numpy as np
 import os
-import sys
 
 # If you're using TensorFlow => 2.0, make sure to put these lines before importing tensorflow to be effective.
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'  # Change 3 to values (0, 1, 2, 3) according to the messages you want avoid.
 
 import nltk
 from abc import ABCMeta, abstractmethod
 from queue import Queue
@@ -16,17 +15,17 @@
 from ..utils.logger import log
 from nltk.stem import WordNetLemmatizer
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import Dense, Dropout
 from tensorflow.keras.optimizers import SGD
 from tensorflow.keras.models import load_model
 
+nltk.download('punkt', quiet=True)
+nltk.download('wordnet', quiet=True)
 
-# nltk.download('punkt', quiet=True)
-# nltk.download('wordnet', quiet=True)
 
 class IAssistant(metaclass=ABCMeta):
 
     @abstractmethod
     def train_model(self):
         """ Implemented in child class """
 
@@ -45,56 +44,39 @@
     @abstractmethod
     def request(self, message):
         """ Implemented in child class """
 
 
 class GenericAssistant(IAssistant):
 
-    def __init__(self, intents, intent_methods=None, model_name="assistant_model"):
+    def __init__(self, intents, intent_methods={}, model_name="assistant_model"):
+        self.intents = intents
+        self.default_intents = json.loads(open('mac_voice_assistant/default_intents.json').read())
+        self.intent_methods = intent_methods
         self.model_name = model_name
         self.log = log
 
         # Initialize queue instances
         self.tasks = Queue(maxsize=20)
         self.audio_queue = Queue(maxsize=20)
         self.commands = Queue(maxsize=20)
         self.responses = Queue(maxsize=20)
 
         # Initialize thread pool instance
         self.thread_pool = ThreadPool(processes=10)
 
-        # Initialize intents files
-        if intent_methods is None:
-            intent_methods = {}
-        self.intents = intents
-        self.intent_methods = intent_methods
-        self.default_intents_file_path = 'mac_voice_assistant/IA/default_intents.json'
-
-        self.load_default_intents()
-        self.load_custom_intents(intents)
+        if intents.endswith(".json"):
+            self.load_json_intents(intents)
 
         self.lemmatizer = WordNetLemmatizer()
 
-    def get_default_intents_file_path(self):
-        default_file_path = self.default_intents_file_path
-        if os.path.exists(default_file_path):
-            return default_file_path
-        else:
-            for path in sys.path:
-                if 'site-packages' in path:
-                    return path + '/mac_voice_assistant/IA/default_intents.json'
-
-    def load_default_intents(self):
-        path = self.get_default_intents_file_path()
-        self.intents = json.loads(open(path).read())
-
-    def load_custom_intents(self, intents):
-        custom_intents = json.loads(open(intents).read())
-        for intent in custom_intents['intents']:
-            self.intents['intents'].append(intent)
+    def load_json_intents(self, intents):
+        self.intents = json.loads(open(intents).read())
+        for my_dict in self.default_intents['intents']:
+            self.intents['intents'].append(my_dict)
 
     def train_model(self):
 
         self.words = []
         self.classes = []
         documents = []
         ignore_letters = ['!', '?', ',', '.']
@@ -141,31 +123,31 @@
 
         sgd = SGD(learning_rate=0.01, weight_decay=1e-6, momentum=0.9, nesterov=True)
         self.model.compile(loss='categorical_crossentropy', optimizer=sgd, metrics=['accuracy'])
         self.hist = self.model.fit(np.array(train_x), np.array(train_y), epochs=50, batch_size=5, verbose=0)
 
     def save_model(self, model_name=None):
         if model_name is None:
-            self.model.save(f"{self.model_name}.h5", self.hist)
+            self.model.save(f"{self.model_name}.keras", self.hist)
             pickle.dump(self.words, open(f'{self.model_name}_words.pkl', 'wb'))
             pickle.dump(self.classes, open(f'{self.model_name}_classes.pkl', 'wb'))
         else:
-            self.model.save(f"{model_name}.h5", self.hist)
+            self.model.save(f"{model_name}.keras", self.hist)
             pickle.dump(self.words, open(f'{model_name}_words.pkl', 'wb'))
             pickle.dump(self.classes, open(f'{model_name}_classes.pkl', 'wb'))
 
     def load_model(self, model_name=None):
         if model_name is None:
             self.words = pickle.load(open(f'{self.model_name}_words.pkl', 'rb'))
             self.classes = pickle.load(open(f'{self.model_name}_classes.pkl', 'rb'))
-            self.model = load_model(f'{self.model_name}.h5')
+            self.model = load_model(f'{self.model_name}.keras')
         else:
             self.words = pickle.load(open(f'{model_name}_words.pkl', 'rb'))
             self.classes = pickle.load(open(f'{model_name}_classes.pkl', 'rb'))
-            self.model = load_model(f'{model_name}.h5')
+            self.model = load_model(f'{model_name}.keras')
 
     def _clean_up_sentence(self, sentence):
         sentence_words = nltk.word_tokenize(sentence)
         sentence_words = [self.lemmatizer.lemmatize(word.lower()) for word in sentence_words]
         return sentence_words
 
     def _bag_of_words(self, sentence, words):
```

### Comparing `mac_voice_assistant-0.3.1/mac_voice_assistant/IA/default_intents.json` & `mac_voice_assistant-0.3.2/mac_voice_assistant/default_intents.json`

 * *Files identical despite different names*

### Comparing `mac_voice_assistant-0.3.1/mac_voice_assistant/audio_samples/beep.wav` & `mac_voice_assistant-0.3.2/mac_voice_assistant/audio_samples/beep.wav`

 * *Files identical despite different names*

### Comparing `mac_voice_assistant-0.3.1/mac_voice_assistant.egg-info/SOURCES.txt` & `mac_voice_assistant-0.3.2/mac_voice_assistant.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 mac_voice_assistant/AI.py
 mac_voice_assistant/__init__.py
+mac_voice_assistant/default_intents.json
 mac_voice_assistant.egg-info/PKG-INFO
 mac_voice_assistant.egg-info/SOURCES.txt
 mac_voice_assistant.egg-info/dependency_links.txt
 mac_voice_assistant.egg-info/requires.txt
 mac_voice_assistant.egg-info/top_level.txt
 mac_voice_assistant/IA/IA.py
 mac_voice_assistant/IA/__init__.py
-mac_voice_assistant/IA/default_intents.json
 mac_voice_assistant/audio_samples/__init__.py
 mac_voice_assistant/audio_samples/beep.wav
 mac_voice_assistant/utils/__init__.py
 mac_voice_assistant/utils/logger.py
 tests/__init__.py
 tests/example.py
 tests/my_hotkey.py
 tests/test.py
-tests/text_typing.py
+tests/text_typing.py
+tests/voices.py
```

### Comparing `mac_voice_assistant-0.3.1/pyproject.toml` & `mac_voice_assistant-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mac_voice_assistant"
-version = "0.3.1"
+version = "0.3.2"
 authors = [{ name="Manish Raj", email="manishraj1.618@gmail.com" }]
 description = "A voice assistant prototype"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     'Development Status :: 1 - Planning',
     "Programming Language :: Python :: 3",
```

### Comparing `mac_voice_assistant-0.3.1/setup.py` & `mac_voice_assistant-0.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 
 setup(
     name='mac_voice_assistant',
-    version='0.3.1',
+    version='0.3.2',
     packages=find_packages(),
-    package_data={'mac_voice_assistant': ['audio_samples/beep.wav', 'IA/default_intents.json']},
+    package_data={'mac_voice_assistant': ['audio_samples/beep.wav', 'default_intents.json']},
     url='https://pypi.org/project/mac-voice-assistant/',
     author='Manish Raj',
     author_email='manishraj1.618@gmail.com',
     description='A generic voice assistant',
     long_description=read('README.md'),
     keywords="mac voice assistant",
 )
```

### Comparing `mac_voice_assistant-0.3.1/tests/example.py` & `mac_voice_assistant-0.3.2/tests/example.py`

 * *Files identical despite different names*

### Comparing `mac_voice_assistant-0.3.1/tests/test.py` & `mac_voice_assistant-0.3.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `mac_voice_assistant-0.3.1/tests/text_typing.py` & `mac_voice_assistant-0.3.2/tests/text_typing.py`

 * *Files identical despite different names*

