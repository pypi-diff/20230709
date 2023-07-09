# Comparing `tmp/matplotlib_ai-1.0.1.tar.gz` & `tmp/matplotlib_ai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_ai-1.0.1.tar", last modified: Fri Jul  7 09:19:40 2023, max compression
+gzip compressed data, was "matplotlib_ai-1.0.2.tar", last modified: Sun Jul  9 04:51:03 2023, max compression
```

## Comparing `matplotlib_ai-1.0.1.tar` & `matplotlib_ai-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-07 09:19:40.473145 matplotlib_ai-1.0.1/
--rw-r--r--   0 yorio      (501) staff       (20)     1066 2023-07-07 06:14:42.000000 matplotlib_ai-1.0.1/LICENSE
--rw-r--r--   0 yorio      (501) staff       (20)      854 2023-07-07 09:19:40.472985 matplotlib_ai-1.0.1/PKG-INFO
--rw-r--r--   0 yorio      (501) staff       (20)     2247 2023-07-07 07:06:27.000000 matplotlib_ai-1.0.1/README.md
-drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-07 09:19:40.472155 matplotlib_ai-1.0.1/matplotlib_ai/
--rw-rw-r--   0 yorio      (501) staff       (20)        0 2023-07-07 00:49:48.000000 matplotlib_ai-1.0.1/matplotlib_ai/__init__.py
--rw-rw-r--   0 yorio      (501) staff       (20)     2764 2023-07-07 06:31:14.000000 matplotlib_ai-1.0.1/matplotlib_ai/matplotlib_ai.py
-drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-07 09:19:40.472791 matplotlib_ai-1.0.1/matplotlib_ai.egg-info/
--rw-r--r--   0 yorio      (501) staff       (20)      854 2023-07-07 09:19:40.000000 matplotlib_ai-1.0.1/matplotlib_ai.egg-info/PKG-INFO
--rw-r--r--   0 yorio      (501) staff       (20)      231 2023-07-07 09:19:40.000000 matplotlib_ai-1.0.1/matplotlib_ai.egg-info/SOURCES.txt
--rw-r--r--   0 yorio      (501) staff       (20)        1 2023-07-07 09:19:40.000000 matplotlib_ai-1.0.1/matplotlib_ai.egg-info/dependency_links.txt
--rw-r--r--   0 yorio      (501) staff       (20)       14 2023-07-07 09:19:40.000000 matplotlib_ai-1.0.1/matplotlib_ai.egg-info/top_level.txt
--rw-r--r--   0 yorio      (501) staff       (20)       38 2023-07-07 09:19:40.473199 matplotlib_ai-1.0.1/setup.cfg
--rw-r--r--   0 yorio      (501) staff       (20)     1002 2023-07-07 09:19:08.000000 matplotlib_ai-1.0.1/setup.py
+drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 04:51:03.938228 matplotlib_ai-1.0.2/
+-rw-r--r--   0 yorio      (501) staff       (20)     1066 2023-07-07 06:14:42.000000 matplotlib_ai-1.0.2/LICENSE
+-rw-r--r--   0 yorio      (501) staff       (20)      854 2023-07-09 04:51:03.938070 matplotlib_ai-1.0.2/PKG-INFO
+-rw-r--r--   0 yorio      (501) staff       (20)     2353 2023-07-08 19:26:28.000000 matplotlib_ai-1.0.2/README.md
+drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 04:51:03.937238 matplotlib_ai-1.0.2/matplotlib_ai/
+-rw-rw-r--   0 yorio      (501) staff       (20)        0 2023-07-07 00:49:48.000000 matplotlib_ai-1.0.2/matplotlib_ai/__init__.py
+-rw-rw-r--   0 yorio      (501) staff       (20)     4613 2023-07-09 01:00:12.000000 matplotlib_ai-1.0.2/matplotlib_ai/matplotlib_ai.py
+drwxr-xr-x   0 yorio      (501) staff       (20)        0 2023-07-09 04:51:03.937860 matplotlib_ai-1.0.2/matplotlib_ai.egg-info/
+-rw-r--r--   0 yorio      (501) staff       (20)      854 2023-07-09 04:51:03.000000 matplotlib_ai-1.0.2/matplotlib_ai.egg-info/PKG-INFO
+-rw-r--r--   0 yorio      (501) staff       (20)      231 2023-07-09 04:51:03.000000 matplotlib_ai-1.0.2/matplotlib_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 yorio      (501) staff       (20)        1 2023-07-09 04:51:03.000000 matplotlib_ai-1.0.2/matplotlib_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 yorio      (501) staff       (20)       14 2023-07-09 04:51:03.000000 matplotlib_ai-1.0.2/matplotlib_ai.egg-info/top_level.txt
+-rw-r--r--   0 yorio      (501) staff       (20)       38 2023-07-09 04:51:03.938288 matplotlib_ai-1.0.2/setup.cfg
+-rw-r--r--   0 yorio      (501) staff       (20)     1002 2023-07-09 04:50:48.000000 matplotlib_ai-1.0.2/setup.py
```

### Comparing `matplotlib_ai-1.0.1/LICENSE` & `matplotlib_ai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_ai-1.0.1/PKG-INFO` & `matplotlib_ai-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib_ai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A GPT-powered tool to bring no-code data visualization to life!
 Home-page: https://github.com/notY0rick/mpl_ai
 Author: Yorick Chern
 Author-email: yorichek.007@gmail.com
 License: MIT
 Keywords: python,gpt,matplotlib,no code,LLM
 Platform: UNKNOWN
```

### Comparing `matplotlib_ai-1.0.1/README.md` & `matplotlib_ai-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# matplotlib_ai
+# `matplotlib_ai`
 Do you also have a love-hate relationship with [matplotlib](https://matplotlib.org/)? So do I! That's why I created this mini-project that can help you graph your data using natural language. The package dependencies require `openai` and `matplotlib`, and it is unbelievably easy to use. Calling OpenAI's GPT API, prompt engineering, and using few-shot learning, `matplotlib_ai` is capable of generating graphs without requiring you to write a single line of `matplotlib` code!
 
+Import `matplotlib_ai` via pip:
+```
+pip install matplotlib_ai
+```
+
 Say we have a dictionary `data` with 4 curves labeled `'a'`, `'b'`, `'c'`, and `'d'`:
 ```python
 import numpy as np
-data = {'a': np.arange(50),
-		'c': np.random.randint(0, 50, 50),
-		'd': np.random.randn(50)}
-data['b'] = data['a'] + 10 * np.random.randn(50)
-data['d'] = np.abs(data['d']) * 100
+data = {'a': [...], # some curve
+        'b': [...], # some curve
+	'c': [...], # some curve
+	'd': [...], # some curve}
 ```
 If we wanted to graph each curve and make curve `'a'` dashed and call this graph "my ekg when i see you :)", the most sensible thing would be to write `matplotlib` code as such:
 ```python
 import matplotlib.pyplot as plt
 plt.plot(data['a'], linestyle='dashed', label='a')
 plt.plot(data['b'], label='b')
 plt.plot(data['c'], label='c')
@@ -22,30 +26,32 @@
 plt.show()
 ```
 However, with `matplotlib_ai` it is as easy as:
 ```python
 from matplotlib_ai.matplotlib_ai import matplotlib_ai
 mpl_ai = matplotlib_ai("YOUR-OPENAI-API-KEY")
 prompt = "graph a curve for each item in data and title the graph 'my ekg when i see you :)'. " + 
-		 "Make curve 'a' in data a dashed line.""
+	 "Make curve 'a' in data a dashed line."
 code = mpl_ai(prompt)
 ```
 Then, `mpl_ai` would generate:
 
 
 ![yuhhhh](https://scontent.xx.fbcdn.net/v/t1.15752-9/358351553_1042559263392780_1124760776888830793_n.png?stp=dst-png_p403x403&_nc_cat=108&cb=99be929b-3346023f&ccb=1-7&_nc_sid=aee45a&_nc_ohc=w_K4__DK_HMAX89R78B&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AdS4drpaM2oqdda3Xpu_gWoU3Lv0wmRGzSGGPBBaF9hE9g&oe=64CF178D)
 
 
 
 To see the code generated by GPT, simply print it like so:
 ```
 >>> print(code)		# the code generated by GPT
 import matplotlib.pyplot as plt
 for key, value in data.items():
-  if key == 'a':
-    plt.plot(value, linestyle='dashed', label=key)
-  else:
-    plt.plot(value, label=key)
+    if key == 'a':
+        plt.plot(value, linestyle='dashed', label=key)
+    else:
+        plt.plot(value, label=key)
 plt.title('my ekg when i see you :)')
 plt.legend()
 plt.show()
 ```
+
+This project is at its early stages, I hope to make it more comprehensive in time :)
```

### Comparing `matplotlib_ai-1.0.1/matplotlib_ai/matplotlib_ai.py` & `matplotlib_ai-1.0.2/matplotlib_ai/matplotlib_ai.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,89 @@
 import openai
 import inspect
-import matplotlib.pyplot as plt
+
 
 class matplotlib_ai:
 
-    def __init__(self, openai_api_key):
-        assert isinstance(openai_api_key, str), "openen_api_key needs to be provided as a string!"
-        self.api_key = openai_api_key
-        openai.api_key = self.api_key
+    def __init__(self, api_key, engine='gpt', model_name='gpt-3.5-turbo'):
+        """
+        Initializer for matplotlib_ai.
+
+        :param api_key: the api key needed to access the models - str
+        :param engine: the type of engine to be used - str
+        :param model_name: the specified model to be used - str or None
+        """
+
+        assert isinstance(api_key, str), "api_key needs to be provided as a string!"
+        assert engine in ['gpt'], f"engine needs to be one of ['gpt']"
+
+        self.api_key = api_key
+        if engine == 'gpt':
+            self.engine = 'gpt'
+            if model_name is not None:
+                self.model_name = model_name
+            else:
+                self.model_name = 'gpt-3.5-turbo'
+            openai.api_key = self.api_key
 
     @staticmethod
     def create_prompt(message):
         if message[-1] == '.':
             message = message[:-1]
         message = message[0].lower() + message[1:]
         training_prompt = \
-        f"""
+            f"""
         Prompt: Using matplotlib, create a box and whisker plot for x, y, and z. Assume the variables already exist. Return the code only.
         Response: import matplotlib.pyplot as plt\n\nplt.boxplot([x, y, z])\n\nplt.show()
         Prompt: Using matplotlib, plot three histograms, one for x, y, and z each. Assume variables already exist. Return the code only.
         Response: import matplotlib.pyplot as plt\n\nplt.hist(x, bins=10)\nplt.xlabel('x')\nplt.ylabel('Frequency')\nplt.title('Histogram of x')\nplt.show()\n\nplt.hist(y, bins=10)\nplt.xlabel('y')\nplt.ylabel('Frequency')\nplt.title('Histogram of y')\nplt.show()\n\nplt.hist(z, bins=10)\nplt.xlabel('z')\nplt.ylabel('Frequency')\nplt.title('Histogram of z')\nplt.show()
         Prompt: Using matplotlib, generate a scatter plot using data where data is a dictionary. Title it 'damn wtf'. Assume variables already exist. Return the code only.
         Response: import matplotlib.pyplot as plt\n\nplt.scatter('a', 'b', c='c', s='d', data=data)\n\nplt.xlabel('entry a')\n\nplt.ylabel('entry b')\n\nplt.show()
         Prompt: Using matplotlib, plot three different graphs for the data names and values. Assume variables already exist. Return the code only.
         Response: import matplotlib.pyplot as plt\n\nplt.subplot(131)\n\nplt.bar(names, values)\n\nplt.subplot(132)\n\nplt.scatter(names, values)\n\nplt.subplot(133)\n\nplt.plot(names, values)\n\nplt.suptitle('Categorical Plotting')\n\nplt.show()
         Prompt: Using matplotlib, {message}. Assume variables already exist. Return the code only.
         Response: 
         """
 
         return training_prompt
 
-    @staticmethod
-    def call_gpt(message):
+    def call_gpt(self, message):
         prompt = matplotlib_ai.create_prompt(message)
-        response = openai.ChatCompletion.create(model="gpt-3.5-turbo", messages=[{"role": "system", "content": prompt}])
+        response = openai.ChatCompletion.create(model=self.model_name, messages=[{"role": "system", "content": prompt}])
         response = response['choices'][0]['message']['content']
         return response
-    
-    def __call__(self, prompt, print_code=False):
-        frame = inspect.currentframe().f_back
-        prompt = matplotlib_ai.create_prompt(prompt)
-        code = matplotlib_ai.call_gpt(prompt)
-        if print_code:
-            print(code)
-        exec(code, frame.f_globals, frame.f_locals)
-        return code
+
+    def __call__(self, prompt, print_code=False, auto_rerun=True, n_candidates=1):
+        """
+        Main function that takes a user prompt to produce the desired graph.
+        :param prompt: the input prompt describing the graph(s) the user wants - str
+        :param print_code: whether to print out the AI-generated code - bool
+        :param auto_rerun: automatically reruns the AI if the generated code fails - bool
+        :param n_candidates: how many candidate graphs it should generate - int
+        :return: codes: a list of AI-generated code - list
+        """
+        assert isinstance(prompt, str), "prompt needs to be a string"
+        assert isinstance(print_code, str), "print_code needs to be a string"
+        assert isinstance(auto_rerun, bool), "auto_rerun needs to be a boolean"
+        assert isinstance(n_candidates, int), "n_candidates need to be an integer"
+        assert n_candidates >= 1, "n_candidates need to be >= 1"
+
+        count = 0
+        codes = []
+        if self.engine == 'gpt':
+            frame = inspect.currentframe().f_back
+            prompt = matplotlib_ai.create_prompt(prompt)
+            keep_trying = auto_rerun
+            while keep_trying:
+                try:
+                    code = self.call_gpt(prompt)
+                    if print_code:
+                        print(code)
+                    exec(code, frame.f_globals, frame.f_locals)
+                    count += 1
+                    codes.append(code)
+                    if count == n_candidates:
+                        keep_trying = False
+                except:
+                    pass
+
+            return codes
```

### Comparing `matplotlib_ai-1.0.1/matplotlib_ai.egg-info/PKG-INFO` & `matplotlib_ai-1.0.2/matplotlib_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib-ai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A GPT-powered tool to bring no-code data visualization to life!
 Home-page: https://github.com/notY0rick/mpl_ai
 Author: Yorick Chern
 Author-email: yorichek.007@gmail.com
 License: MIT
 Keywords: python,gpt,matplotlib,no code,LLM
 Platform: UNKNOWN
```

### Comparing `matplotlib_ai-1.0.1/setup.py` & `matplotlib_ai-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 The package dependencies require openai and matplotlib, and it is unbelievably easy to use. 
 Calling OpenAI's GPT API, prompt engineering, and using few-shot learning, matplotlib_ai is capable 
 of generating graphs without requiring you to write a single line of matplotlib code! Check out this GitHub link:
 https://github.com/notY0rick/matplotlib_ai
 """
 
 setup(name='matplotlib_ai',
-      version='1.0.1',
+      version='1.0.2',
       description='A GPT-powered tool to bring no-code data visualization to life!',
       long_description=LONG_DESC,
       author='Yorick Chern',
       author_email='yorichek.007@gmail.com',
       url='https://github.com/notY0rick/mpl_ai',
       packages=find_packages(),
       keywords=['python', 'gpt', 'matplotlib', 'no code', 'LLM'],
```

