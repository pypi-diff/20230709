# Comparing `tmp/gpterm-tool-0.0.1.tar.gz` & `tmp/gpterm-tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpterm-tool-0.0.1.tar", last modified: Sun Jul  9 19:52:34 2023, max compression
+gzip compressed data, was "gpterm-tool-0.0.2.tar", last modified: Sun Jul  9 20:14:07 2023, max compression
```

## Comparing `gpterm-tool-0.0.1.tar` & `gpterm-tool-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 19:52:34.251526 gpterm-tool-0.0.1/
--rw-rw-r--   0 adem       (501) staff       (20)     1049 2023-07-09 18:45:08.000000 gpterm-tool-0.0.1/LICENCE.txt
--rw-rw-r--   0 adem       (501) staff       (20)       26 2020-04-20 13:20:58.000000 gpterm-tool-0.0.1/MANIFEST.in
--rw-r--r--   0 adem       (501) staff       (20)     6898 2023-07-09 19:52:34.251407 gpterm-tool-0.0.1/PKG-INFO
--rw-rw-r--   0 adem       (501) staff       (20)     6203 2023-07-09 19:42:14.000000 gpterm-tool-0.0.1/README.md
-drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 19:52:34.249828 gpterm-tool-0.0.1/gpterm.egg-info/
--rw-r--r--   0 adem       (501) staff       (20)      333 2023-07-09 19:43:47.000000 gpterm-tool-0.0.1/gpterm.egg-info/SOURCES.txt
--rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 19:43:47.000000 gpterm-tool-0.0.1/gpterm.egg-info/dependency_links.txt
--rw-r--r--   0 adem       (501) staff       (20)       39 2023-07-09 19:43:47.000000 gpterm-tool-0.0.1/gpterm.egg-info/entry_points.txt
--rw-r--r--   0 adem       (501) staff       (20)      109 2023-07-09 19:43:47.000000 gpterm-tool-0.0.1/gpterm.egg-info/requires.txt
--rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 19:43:47.000000 gpterm-tool-0.0.1/gpterm.egg-info/top_level.txt
-drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 19:52:34.250518 gpterm-tool-0.0.1/gpterm_tool.egg-info/
--rw-r--r--   0 adem       (501) staff       (20)     6898 2023-07-09 19:52:34.000000 gpterm-tool-0.0.1/gpterm_tool.egg-info/PKG-INFO
--rw-r--r--   0 adem       (501) staff       (20)      520 2023-07-09 19:52:34.000000 gpterm-tool-0.0.1/gpterm_tool.egg-info/SOURCES.txt
--rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 19:52:34.000000 gpterm-tool-0.0.1/gpterm_tool.egg-info/dependency_links.txt
--rw-r--r--   0 adem       (501) staff       (20)       39 2023-07-09 19:52:34.000000 gpterm-tool-0.0.1/gpterm_tool.egg-info/entry_points.txt
--rw-r--r--   0 adem       (501) staff       (20)      109 2023-07-09 19:52:34.000000 gpterm-tool-0.0.1/gpterm_tool.egg-info/requires.txt
--rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 19:52:34.000000 gpterm-tool-0.0.1/gpterm_tool.egg-info/top_level.txt
--rw-rw-r--   0 adem       (501) staff       (20)      110 2023-07-06 17:58:30.000000 gpterm-tool-0.0.1/requirements.txt
--rw-r--r--   0 adem       (501) staff       (20)       38 2023-07-09 19:52:34.251563 gpterm-tool-0.0.1/setup.cfg
--rw-r--r--   0 adem       (501) staff       (20)     1617 2023-07-09 19:51:06.000000 gpterm-tool-0.0.1/setup.py
-drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 19:52:34.251239 gpterm-tool-0.0.1/src/
--rw-r--r--   0 adem       (501) staff       (20)       13 2023-07-09 19:02:30.000000 gpterm-tool-0.0.1/src/__init__.py
--rw-r--r--   0 adem       (501) staff       (20)     1851 2023-07-06 13:47:19.000000 gpterm-tool-0.0.1/src/alpaca.py
--rw-r--r--   0 adem       (501) staff       (20)     3771 2023-07-06 14:09:07.000000 gpterm-tool-0.0.1/src/gpterm.py
--rw-r--r--   0 adem       (501) staff       (20)      867 2023-07-06 13:47:24.000000 gpterm-tool-0.0.1/src/llm_writer.py
--rw-r--r--   0 adem       (501) staff       (20)     4536 2023-07-08 21:16:20.000000 gpterm-tool-0.0.1/src/responser.py
--rw-r--r--   0 adem       (501) staff       (20)      632 2023-07-06 10:57:19.000000 gpterm-tool-0.0.1/src/utils.py
+drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 20:14:07.021471 gpterm-tool-0.0.2/
+-rw-rw-r--   0 adem       (501) staff       (20)     1049 2023-07-09 18:45:08.000000 gpterm-tool-0.0.2/LICENCE.txt
+-rw-rw-r--   0 adem       (501) staff       (20)       32 2023-07-09 20:06:30.000000 gpterm-tool-0.0.2/MANIFEST.in
+-rw-r--r--   0 adem       (501) staff       (20)     7002 2023-07-09 20:14:07.021359 gpterm-tool-0.0.2/PKG-INFO
+-rw-rw-r--   0 adem       (501) staff       (20)     6307 2023-07-09 20:03:43.000000 gpterm-tool-0.0.2/README.md
+drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 20:14:07.019602 gpterm-tool-0.0.2/gpterm.egg-info/
+-rw-r--r--   0 adem       (501) staff       (20)      333 2023-07-09 19:43:47.000000 gpterm-tool-0.0.2/gpterm.egg-info/SOURCES.txt
+-rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 19:43:47.000000 gpterm-tool-0.0.2/gpterm.egg-info/dependency_links.txt
+-rw-r--r--   0 adem       (501) staff       (20)       39 2023-07-09 19:43:47.000000 gpterm-tool-0.0.2/gpterm.egg-info/entry_points.txt
+-rw-r--r--   0 adem       (501) staff       (20)      109 2023-07-09 19:43:47.000000 gpterm-tool-0.0.2/gpterm.egg-info/requires.txt
+-rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 19:43:47.000000 gpterm-tool-0.0.2/gpterm.egg-info/top_level.txt
+drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 20:14:07.020286 gpterm-tool-0.0.2/gpterm_tool.egg-info/
+-rw-r--r--   0 adem       (501) staff       (20)     7002 2023-07-09 20:14:06.000000 gpterm-tool-0.0.2/gpterm_tool.egg-info/PKG-INFO
+-rw-r--r--   0 adem       (501) staff       (20)      536 2023-07-09 20:14:07.000000 gpterm-tool-0.0.2/gpterm_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 20:14:06.000000 gpterm-tool-0.0.2/gpterm_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 adem       (501) staff       (20)       39 2023-07-09 20:14:06.000000 gpterm-tool-0.0.2/gpterm_tool.egg-info/entry_points.txt
+-rw-r--r--   0 adem       (501) staff       (20)      109 2023-07-09 20:14:06.000000 gpterm-tool-0.0.2/gpterm_tool.egg-info/requires.txt
+-rw-r--r--   0 adem       (501) staff       (20)        1 2023-07-09 20:14:06.000000 gpterm-tool-0.0.2/gpterm_tool.egg-info/top_level.txt
+drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 20:14:07.020413 gpterm-tool-0.0.2/images/
+-rw-r--r--   0 adem       (501) staff       (20)    69552 2023-07-08 17:57:25.000000 gpterm-tool-0.0.2/images/logo.png
+-rw-rw-r--   0 adem       (501) staff       (20)      110 2023-07-06 17:58:30.000000 gpterm-tool-0.0.2/requirements.txt
+-rw-r--r--   0 adem       (501) staff       (20)       38 2023-07-09 20:14:07.021514 gpterm-tool-0.0.2/setup.cfg
+-rw-r--r--   0 adem       (501) staff       (20)     1617 2023-07-09 20:13:04.000000 gpterm-tool-0.0.2/setup.py
+drwxr-xr-x   0 adem       (501) staff       (20)        0 2023-07-09 20:14:07.021196 gpterm-tool-0.0.2/src/
+-rw-r--r--   0 adem       (501) staff       (20)       13 2023-07-09 19:02:30.000000 gpterm-tool-0.0.2/src/__init__.py
+-rw-r--r--   0 adem       (501) staff       (20)     1851 2023-07-06 13:47:19.000000 gpterm-tool-0.0.2/src/alpaca.py
+-rw-r--r--   0 adem       (501) staff       (20)     3771 2023-07-06 14:09:07.000000 gpterm-tool-0.0.2/src/gpterm.py
+-rw-r--r--   0 adem       (501) staff       (20)      867 2023-07-06 13:47:24.000000 gpterm-tool-0.0.2/src/llm_writer.py
+-rw-r--r--   0 adem       (501) staff       (20)     4536 2023-07-08 21:16:20.000000 gpterm-tool-0.0.2/src/responser.py
+-rw-r--r--   0 adem       (501) staff       (20)      632 2023-07-06 10:57:19.000000 gpterm-tool-0.0.2/src/utils.py
```

### Comparing `gpterm-tool-0.0.1/LICENCE.txt` & `gpterm-tool-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gpterm-tool-0.0.1/PKG-INFO` & `gpterm-tool-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterm-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Creating Intelligent Terminal Apps with ChatGPT and LLM Models
 Home-page: https://github.com/ademakdogan/GPTerm
 Author: A.Akdogan
 Author-email: adem.akdogan92@gmail.com
 License: MIT
 Keywords: CHATGPT,NLP,LLM,TERMINAL
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 
 <p align="center">
-  <img width="180" src="./images/logo.png" alt="ChatSQL">
+  <img width="180" src="./images/logo.png" alt="GPTerm">
   <h1 align="center">GPTerm</h1>
 </p>
 
 
 This project focuses on converting plain text into shell commands using different models, including ChatGPT and various open-source language models. While some models yielded good results, others did not meet the desired level of success. The project primarily utilized iTerm as the terminal application for testing, but assessments with other terminals have yet to be conducted as the emphasis is on running and comparing the models. However, it is anticipated that other terminal applications would also be suitable for this project.
 
 The project consists of two main parts. In the first part, users can manually enter and execute shell commands without closing the plugin. The second part involves translating given plain text into shell commands, which are then presented to the user. Users have the flexibility to modify or delete sections of the generated command without execution, if desired. Both sections operate in a similar manner. To indicate the intention of obtaining shell commands from plain text only, users need to prefix the plain text with dot (.). This allows the application to distinguish between manual command entry and obtaining commands from plain text.
@@ -35,15 +35,15 @@
 This part can be developed further.
 
 All packages are installed before starting.  The following command is used for this installation process (python 3.8 is used in this project):
 
 
 ## Usage
 
-To begin with, it is recommended to work within an environment. In this project, the conda environment "py1" (sample conda env name) is utilized for development. Then;
+To begin with, **it is recommended to work within an environment.** In this project, the conda environment "py1" (sample conda env name) is utilized for development. Then;
 
 ```
   pip3 install gpterm-tool
 ```
 You can run the provided above command for installation purposes.  Once installed, it can be utilized by using the 'gpterm' keyword on iTerm or any other terminal application.
 - Run with ChatGPT model (Highly Recommended)
 ```
@@ -96,15 +96,15 @@
 >>> mkdir sample_1 && cd sample_1 \\ Wrong one here !
 
 name_ai ---> . Create a file named nw_1 with .txt extension and add all the numbers from 1 to 10 in it
 
 >>> touch nw_1.txt && echo '1 2 3 4 5 6 7 8 9 10' >> nw_1.txt
 ```
 
-As observed earlier, ChatGPT provides highly accurate responses. In the WizardCoder model, it successfully generated the correct command in two out of the three requests, although it did produce an incorrect command in one request. **Remember! The ChatGPT model is highly suitable for implementation, while the others are still in the experimental phase.**
+As observed earlier, ChatGPT provides highly accurate responses. In the WizardCoder model, it successfully generated the correct command in two out of the three requests, although it did produce an incorrect command in one request. Sometimes MPT and WizardCoder models return our prompt as result. **Remember! The ChatGPT model is highly suitable for implementation, while the others are still in the experimental phase. They are not suitable for use yet.**
 
 _**Note:** As previously explained, it is important to note that open-source models may sometimes produce noisy results. To solve this issue, the [json_extractor](/src/responser.py) function is utilized to filter out any unwanted noise and obtain the desired outcome. This function can be adjusted to handle JSONDecodeError exceptions, ensuring smooth execution. In future iterations, the regex pattern will be refined to encompass all possible error cases. However, for the current implementation, the pattern has been tailored to address the most prevalent sources of noise, considering the constraints of time. However, in the current implementation, the pattern has been adjusted to effectively handle the main sources of noise, taking into account the time limitations._
 
 
 ## TODOS
 
 - [X] Test of ChatGPT
```

### Comparing `gpterm-tool-0.0.1/README.md` & `gpterm-tool-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 <p align="center">
-  <img width="180" src="./images/logo.png" alt="ChatSQL">
+  <img width="180" src="./images/logo.png" alt="GPTerm">
   <h1 align="center">GPTerm</h1>
 </p>
 
 
 This project focuses on converting plain text into shell commands using different models, including ChatGPT and various open-source language models. While some models yielded good results, others did not meet the desired level of success. The project primarily utilized iTerm as the terminal application for testing, but assessments with other terminals have yet to be conducted as the emphasis is on running and comparing the models. However, it is anticipated that other terminal applications would also be suitable for this project.
 
 The project consists of two main parts. In the first part, users can manually enter and execute shell commands without closing the plugin. The second part involves translating given plain text into shell commands, which are then presented to the user. Users have the flexibility to modify or delete sections of the generated command without execution, if desired. Both sections operate in a similar manner. To indicate the intention of obtaining shell commands from plain text only, users need to prefix the plain text with dot (.). This allows the application to distinguish between manual command entry and obtaining commands from plain text.
@@ -16,15 +16,15 @@
 This part can be developed further.
 
 All packages are installed before starting.  The following command is used for this installation process (python 3.8 is used in this project):
 
 
 ## Usage
 
-To begin with, it is recommended to work within an environment. In this project, the conda environment "py1" (sample conda env name) is utilized for development. Then;
+To begin with, **it is recommended to work within an environment.** In this project, the conda environment "py1" (sample conda env name) is utilized for development. Then;
 
 ```
   pip3 install gpterm-tool
 ```
 You can run the provided above command for installation purposes.  Once installed, it can be utilized by using the 'gpterm' keyword on iTerm or any other terminal application.
 - Run with ChatGPT model (Highly Recommended)
 ```
@@ -77,15 +77,15 @@
 >>> mkdir sample_1 && cd sample_1 \\ Wrong one here !
 
 name_ai ---> . Create a file named nw_1 with .txt extension and add all the numbers from 1 to 10 in it
 
 >>> touch nw_1.txt && echo '1 2 3 4 5 6 7 8 9 10' >> nw_1.txt
 ```
 
-As observed earlier, ChatGPT provides highly accurate responses. In the WizardCoder model, it successfully generated the correct command in two out of the three requests, although it did produce an incorrect command in one request. **Remember! The ChatGPT model is highly suitable for implementation, while the others are still in the experimental phase.**
+As observed earlier, ChatGPT provides highly accurate responses. In the WizardCoder model, it successfully generated the correct command in two out of the three requests, although it did produce an incorrect command in one request. Sometimes MPT and WizardCoder models return our prompt as result. **Remember! The ChatGPT model is highly suitable for implementation, while the others are still in the experimental phase. They are not suitable for use yet.**
 
 _**Note:** As previously explained, it is important to note that open-source models may sometimes produce noisy results. To solve this issue, the [json_extractor](/src/responser.py) function is utilized to filter out any unwanted noise and obtain the desired outcome. This function can be adjusted to handle JSONDecodeError exceptions, ensuring smooth execution. In future iterations, the regex pattern will be refined to encompass all possible error cases. However, for the current implementation, the pattern has been tailored to address the most prevalent sources of noise, considering the constraints of time. However, in the current implementation, the pattern has been adjusted to effectively handle the main sources of noise, taking into account the time limitations._
 
 
 ## TODOS
 
 - [X] Test of ChatGPT
```

### Comparing `gpterm-tool-0.0.1/gpterm_tool.egg-info/PKG-INFO` & `gpterm-tool-0.0.2/gpterm_tool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterm-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Creating Intelligent Terminal Apps with ChatGPT and LLM Models
 Home-page: https://github.com/ademakdogan/GPTerm
 Author: A.Akdogan
 Author-email: adem.akdogan92@gmail.com
 License: MIT
 Keywords: CHATGPT,NLP,LLM,TERMINAL
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 
 <p align="center">
-  <img width="180" src="./images/logo.png" alt="ChatSQL">
+  <img width="180" src="./images/logo.png" alt="GPTerm">
   <h1 align="center">GPTerm</h1>
 </p>
 
 
 This project focuses on converting plain text into shell commands using different models, including ChatGPT and various open-source language models. While some models yielded good results, others did not meet the desired level of success. The project primarily utilized iTerm as the terminal application for testing, but assessments with other terminals have yet to be conducted as the emphasis is on running and comparing the models. However, it is anticipated that other terminal applications would also be suitable for this project.
 
 The project consists of two main parts. In the first part, users can manually enter and execute shell commands without closing the plugin. The second part involves translating given plain text into shell commands, which are then presented to the user. Users have the flexibility to modify or delete sections of the generated command without execution, if desired. Both sections operate in a similar manner. To indicate the intention of obtaining shell commands from plain text only, users need to prefix the plain text with dot (.). This allows the application to distinguish between manual command entry and obtaining commands from plain text.
@@ -35,15 +35,15 @@
 This part can be developed further.
 
 All packages are installed before starting.  The following command is used for this installation process (python 3.8 is used in this project):
 
 
 ## Usage
 
-To begin with, it is recommended to work within an environment. In this project, the conda environment "py1" (sample conda env name) is utilized for development. Then;
+To begin with, **it is recommended to work within an environment.** In this project, the conda environment "py1" (sample conda env name) is utilized for development. Then;
 
 ```
   pip3 install gpterm-tool
 ```
 You can run the provided above command for installation purposes.  Once installed, it can be utilized by using the 'gpterm' keyword on iTerm or any other terminal application.
 - Run with ChatGPT model (Highly Recommended)
 ```
@@ -96,15 +96,15 @@
 >>> mkdir sample_1 && cd sample_1 \\ Wrong one here !
 
 name_ai ---> . Create a file named nw_1 with .txt extension and add all the numbers from 1 to 10 in it
 
 >>> touch nw_1.txt && echo '1 2 3 4 5 6 7 8 9 10' >> nw_1.txt
 ```
 
-As observed earlier, ChatGPT provides highly accurate responses. In the WizardCoder model, it successfully generated the correct command in two out of the three requests, although it did produce an incorrect command in one request. **Remember! The ChatGPT model is highly suitable for implementation, while the others are still in the experimental phase.**
+As observed earlier, ChatGPT provides highly accurate responses. In the WizardCoder model, it successfully generated the correct command in two out of the three requests, although it did produce an incorrect command in one request. Sometimes MPT and WizardCoder models return our prompt as result. **Remember! The ChatGPT model is highly suitable for implementation, while the others are still in the experimental phase. They are not suitable for use yet.**
 
 _**Note:** As previously explained, it is important to note that open-source models may sometimes produce noisy results. To solve this issue, the [json_extractor](/src/responser.py) function is utilized to filter out any unwanted noise and obtain the desired outcome. This function can be adjusted to handle JSONDecodeError exceptions, ensuring smooth execution. In future iterations, the regex pattern will be refined to encompass all possible error cases. However, for the current implementation, the pattern has been tailored to address the most prevalent sources of noise, considering the constraints of time. However, in the current implementation, the pattern has been adjusted to effectively handle the main sources of noise, taking into account the time limitations._
 
 
 ## TODOS
 
 - [X] Test of ChatGPT
```

### Comparing `gpterm-tool-0.0.1/gpterm_tool.egg-info/SOURCES.txt` & `gpterm-tool-0.0.2/gpterm_tool.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 gpterm.egg-info/top_level.txt
 gpterm_tool.egg-info/PKG-INFO
 gpterm_tool.egg-info/SOURCES.txt
 gpterm_tool.egg-info/dependency_links.txt
 gpterm_tool.egg-info/entry_points.txt
 gpterm_tool.egg-info/requires.txt
 gpterm_tool.egg-info/top_level.txt
+images/logo.png
 src/__init__.py
 src/alpaca.py
 src/gpterm.py
 src/llm_writer.py
 src/responser.py
 src/utils.py
```

### Comparing `gpterm-tool-0.0.1/setup.py` & `gpterm-tool-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #script_files = glob.glob('')
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='gpterm-tool',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages('src'),
     license='MIT',
     description = 'Creating Intelligent Terminal Apps with ChatGPT and LLM Models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'A.Akdogan',                   
     author_email = 'adem.akdogan92@gmail.com',
```

### Comparing `gpterm-tool-0.0.1/src/alpaca.py` & `gpterm-tool-0.0.2/src/alpaca.py`

 * *Files identical despite different names*

### Comparing `gpterm-tool-0.0.1/src/gpterm.py` & `gpterm-tool-0.0.2/src/gpterm.py`

 * *Files identical despite different names*

### Comparing `gpterm-tool-0.0.1/src/llm_writer.py` & `gpterm-tool-0.0.2/src/llm_writer.py`

 * *Files identical despite different names*

### Comparing `gpterm-tool-0.0.1/src/responser.py` & `gpterm-tool-0.0.2/src/responser.py`

 * *Files identical despite different names*

### Comparing `gpterm-tool-0.0.1/src/utils.py` & `gpterm-tool-0.0.2/src/utils.py`

 * *Files identical despite different names*

