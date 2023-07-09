# Comparing `tmp/keyflow-0.1.1.tar.gz` & `tmp/keyflow-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyflow-0.1.1.tar", last modified: Sat Jul  1 15:14:27 2023, max compression
+gzip compressed data, was "keyflow-1.1.1.tar", last modified: Sun Jul  9 12:02:13 2023, max compression
```

## Comparing `keyflow-0.1.1.tar` & `keyflow-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 15:14:27.253548 keyflow-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-07-01 14:44:31.000000 keyflow-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4791 2023-07-01 15:14:27.250568 keyflow-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4224 2023-07-01 15:09:40.000000 keyflow-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 15:14:27.187548 keyflow-0.1.1/keyflow/
--rw-rw-rw-   0        0        0     8184 2023-07-01 14:45:29.000000 keyflow-0.1.1/keyflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:14:27.245546 keyflow-0.1.1/keyflow.egg-info/
--rw-rw-rw-   0        0        0     4791 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 15:14:27.000000 keyflow-0.1.1/keyflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      675 2023-07-01 15:11:09.000000 keyflow-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 15:14:27.253548 keyflow-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 12:02:13.054457 keyflow-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-09 10:28:08.000000 keyflow-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5098 2023-07-09 12:02:13.052458 keyflow-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4531 2023-07-09 11:58:27.000000 keyflow-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 12:02:12.915455 keyflow-1.1.1/keyflow/
+-rw-rw-rw-   0        0        0     9037 2023-07-09 11:39:42.000000 keyflow-1.1.1/keyflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:02:13.048460 keyflow-1.1.1/keyflow.egg-info/
+-rw-rw-rw-   0        0        0     5098 2023-07-09 12:02:12.000000 keyflow-1.1.1/keyflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-07-09 12:02:12.000000 keyflow-1.1.1/keyflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:02:12.000000 keyflow-1.1.1/keyflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 12:02:12.000000 keyflow-1.1.1/keyflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      675 2023-07-09 11:59:08.000000 keyflow-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 12:02:13.055458 keyflow-1.1.1/setup.cfg
```

### Comparing `keyflow-0.1.1/LICENSE` & `keyflow-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keyflow-0.1.1/PKG-INFO` & `keyflow-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyflow
-Version: 0.1.1
+Version: 1.1.1
 Summary: A small python library to simulate typing in the console and custom text formatting.
 Author-email: Aneousion <sanusirry@gmail.com>
 Project-URL: Homepage, https://github.com/aneousion/keyflow
 Project-URL: Bug Tracker, https://github.com/aneousion/keyflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,14 +48,15 @@
 #### Parameters
 
 - `text` (str): The text to be printed.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
+- `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
 
 ### kfinput
@@ -71,16 +72,17 @@
 #### Parameters
 
 - `text` (str): The text to be displayed as a prompt.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
+- `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
-- `use_pyip` (callable, optional): A [pyinputplus](https://pypi.org/project/PyInputPlus/) function to use for input. Default is None.
+- `use_pyip` (callable, optional): A [pyinputplus](https://github.com/asweigart/pyinputplus) function to use for input. Default is None.
 - `pyip_params` (dict, optional): Additional parameters to pass to the `use_pyip` function. Default is an empty dictionary.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
```

### Comparing `keyflow-0.1.1/README.md` & `keyflow-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 #### Parameters
 
 - `text` (str): The text to be printed.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
+- `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
 
 ### kfinput
@@ -57,16 +58,17 @@
 #### Parameters
 
 - `text` (str): The text to be displayed as a prompt.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
+- `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
-- `use_pyip` (callable, optional): A [pyinputplus](https://pypi.org/project/PyInputPlus/) function to use for input. Default is None.
+- `use_pyip` (callable, optional): A [pyinputplus](https://github.com/asweigart/pyinputplus) function to use for input. Default is None.
 - `pyip_params` (dict, optional): Additional parameters to pass to the `use_pyip` function. Default is an empty dictionary.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
```

### Comparing `keyflow-0.1.1/keyflow/__init__.py` & `keyflow-1.1.1/keyflow/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,29 +8,31 @@
     """
     Custom exception class for KeyFlow-related errors.
     """
 
     pass
 
 
-def _print_formatted_text(underline=False, bold=False, italics=False, fore_color: str = None, back_color: str = None):
+def _print_formatted_text(underline=False, bold=False, italics=False, fore_color: str = None, back_color: str = None, highlight: str = None):
+    if highlight:
+        return
     if underline:
         print('\033[4m', end='', flush=True)
     if bold:
         print('\033[1m', end='', flush=True)
     if italics:
         print('\033[3m', end='', flush=True)
     if fore_color:
         print(Fore.__dict__.get(fore_color.upper(), Fore.RESET), end='', flush=True)
     if back_color:
         print(Back.__dict__.get(back_color.upper(), Back.RESET), end='', flush=True)
 
 
 
-def kfprint(text: str, speed: float = 0.2, retype: str = None, fore_color: str = None, back_color: str = None, typing: bool = True, error: float = 0.2, underline: bool = False, bold: bool = False, italics: bool = False):
+def kfprint(text: str, speed: float = 0.2, retype: str = None, fore_color: str = None, back_color: str = None, highlight: str = None, typing: bool = True, error: float = 0.2, underline: bool = False, bold: bool = False, italics: bool = False):
     """
     Prints the text with a simulated typing effect and supports custom foreground and background colors.
 
     Args:
     -
         `text` (str): The text to be printed.
 
@@ -38,14 +40,16 @@
 
         `retype` (str, optional): Text to be retyped after printing. Default is None.
 
         `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 
         `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
 
+        `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
+        
         `typing` (bool, optional): Whether to simulate typing effect. Default is True.
 
         `error` (float, optional): The probability of making an error while typing. Default is 0.2, that is, a 20% chance of making a mistake.
 
         `underline` (bool, optional): Whether to underline the text. Default is False.
 
         `italics` (bool, optional): Whether to italicize the text. Default is False.
@@ -62,30 +66,36 @@
         raise KeyFlowException("The 'retype' parameter must be a string")
     if not isinstance(speed, float):
         raise KeyFlowException("The 'speed' parameter must be a float")
     if not isinstance(fore_color, (str, type(None))):
         raise KeyFlowException("The 'fore_color' parameter must be a string")
     if not isinstance(back_color, (str, type(None))):
         raise KeyFlowException("The 'back_color' parameter must be a string")
+    if not isinstance(highlight, (str, type(None))):
+        raise KeyFlowException("The 'highlight' parameter must be a string")
     if not isinstance(typing, bool):
         raise KeyFlowException("The 'typing' parameter must be a boolean")
     if not isinstance(error, float):
         raise KeyFlowException("The 'error' parameter must be a float")
     if not isinstance(underline, bool):
         raise KeyFlowException("The 'underline' parameter must be a boolean")
     if not isinstance(italics, bool):
         raise KeyFlowException("The 'italics' parameter must be a boolean")
     if not isinstance(bold, bool):
         raise KeyFlowException("The 'bold' parameter must be a boolean")
 
     if not typing:
-        _print_formatted_text(underline=underline, bold=bold, italics=italics, fore_color=fore_color, back_color=back_color)
-        print(text, end='', flush=True)
+        _print_formatted_text(underline=underline, bold=bold, italics=italics, fore_color=fore_color, back_color=back_color, highlight=highlight)
+        if highlight:
+            print(text.replace(highlight, f'{Fore.__dict__.get(fore_color.upper(), Fore.RESET)}{Back.__dict__.get(back_color.upper(), Back.RESET)}{highlight}{Style.RESET_ALL}'), end='', flush=True)
+        else:
+            print(text, end='', flush=True)
         print(Style.RESET_ALL, end='', flush=True)
         return
+    
     stop_typing = False
 
     def pause_resume_typing(event):
         nonlocal stop_typing
         stop_typing = not stop_typing
 
     keyboard.on_press_key(key='Space', callback=pause_resume_typing)
@@ -140,15 +150,15 @@
         print('_', end='', flush=True)
         time.sleep(1)
         print('\b', end='', flush=True)
         time.sleep(1)
     keyboard.unhook_all()
 
 
-def kfinput(text: str, speed: float = 0.2, retype: str = None, fore_color: str = None, back_color: str = None, typing: bool = True, use_pyip = None, pyip_params: dict = {}, error: float = 0.2, underline: bool = False, bold: bool = False, italics: bool = False):
+def kfinput(text: str, speed: float = 0.2, retype: str = None, fore_color: str = None, back_color: str = None, highlight: str = None, typing: bool = True, use_pyip = None, pyip_params: dict = {}, error: float = 0.2, underline: bool = False, bold: bool = False, italics: bool = False):
     """
     Displays text with a simulated typing effect and supports custom foreground and background colors.
     Waits for user input and returns the entered value.
 
     Args:
     -
         `text` (str): The text to be displayed as a prompt.
@@ -157,14 +167,16 @@
 
         `retype` (str, optional): Text to be retyped after printing. Default is None.
 
         `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 
         `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
 
+        `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
+
         `typing` (bool, optional): Whether to simulate typing effect. Default is True.
 
         `use_pyip` (callable, optional): A pyinputplus function to use for input. Default is None.
 
         `pyip_params` (dict, optional): Additional parameters to pass to `use_pyip` function. Default is an empty dictionary.
 
         `error` (float, optional): The probability of making an error while typing. Default is 0.2, that is, a 20% chance of making a mistake.
@@ -189,15 +201,15 @@
     if not isinstance(pyip_params, dict):
         raise KeyFlowException(
             "The 'pyip_params' parameter must be a dictionary of parameters")
     if 'prompt' in pyip_params.keys():
         del pyip_params['prompt']
 
     kfprint(text, speed=speed, retype=retype, fore_color=fore_color,
-            back_color=back_color, typing=typing, error=error, underline=underline, italics=italics, bold=bold)
+            back_color=back_color, typing=typing, error=error, underline=underline, italics=italics, bold=bold, highlight=highlight)
     _blinking_cursor_animation()
     try:
         if use_pyip != None:
             var = use_pyip(**pyip_params)
             return var
         var = input()
         return var
```

### Comparing `keyflow-0.1.1/keyflow.egg-info/PKG-INFO` & `keyflow-1.1.1/keyflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyflow
-Version: 0.1.1
+Version: 1.1.1
 Summary: A small python library to simulate typing in the console and custom text formatting.
 Author-email: Aneousion <sanusirry@gmail.com>
 Project-URL: Homepage, https://github.com/aneousion/keyflow
 Project-URL: Bug Tracker, https://github.com/aneousion/keyflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,14 +48,15 @@
 #### Parameters
 
 - `text` (str): The text to be printed.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
+- `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
 
 ### kfinput
@@ -71,16 +72,17 @@
 #### Parameters
 
 - `text` (str): The text to be displayed as a prompt.
 - `speed` (float, optional): The typing speed in seconds per character. Default is 0.2.
 - `retype` (str, optional): Text to be retyped after printing. Default is None.
 - `fore_color` (str, optional): The foreground color code or name to apply to the text. Default is None.
 - `back_color` (str, optional): The background color code or name to apply to the text. Default is None.
+- `highlight` (str, optional): Text to be highlighted with the `fore_color` and `back_color`, works only when typing is set to false. Default is None.
 - `typing` (bool, optional): Whether to simulate typing effect. Default is True.
-- `use_pyip` (callable, optional): A [pyinputplus](https://pypi.org/project/PyInputPlus/) function to use for input. Default is None.
+- `use_pyip` (callable, optional): A [pyinputplus](https://github.com/asweigart/pyinputplus) function to use for input. Default is None.
 - `pyip_params` (dict, optional): Additional parameters to pass to the `use_pyip` function. Default is an empty dictionary.
 - `error` (float, optional): The probability of making an error while typing. Default is 0.2.
 - `underline` (bool, optional): Whether to underline the text. Default is False.
 - `bold` (bool, optional): Whether to bold the text. Default is False.
 - `italics` (bool, optional): Whether to italicize the text. Default is False.
```

### Comparing `keyflow-0.1.1/pyproject.toml` & `keyflow-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'keyboard', 'colorama']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keyflow"
-version = "0.1.1"
+version = "1.1.1"
 authors = [
   { name="Aneousion", email="sanusirry@gmail.com" },
 ]
 description = 'A small python library to simulate typing in the console and custom text formatting.'
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

