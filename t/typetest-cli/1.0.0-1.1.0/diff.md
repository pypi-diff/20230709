# Comparing `tmp/typetest-cli-1.0.0.tar.gz` & `tmp/typetest-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetest-cli-1.0.0.tar", last modified: Fri Jul  7 23:58:50 2023, max compression
+gzip compressed data, was "typetest-cli-1.1.0.tar", last modified: Sat Jul  8 22:23:24 2023, max compression
```

## Comparing `typetest-cli-1.0.0.tar` & `typetest-cli-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-07 23:58:50.813273 typetest-cli-1.0.0/
--rw-r--r--   0 senyc     (1000) senyc     (1000)     1062 2023-07-07 01:09:21.000000 typetest-cli-1.0.0/LICENSE
--rw-r--r--   0 senyc     (1000) senyc     (1000)       29 2023-07-07 19:35:03.000000 typetest-cli-1.0.0/MANIFEST.in
--rw-r--r--   0 senyc     (1000) senyc     (1000)      220 2023-07-07 23:58:50.813273 typetest-cli-1.0.0/PKG-INFO
--rw-r--r--   0 senyc     (1000) senyc     (1000)       64 2023-07-07 01:09:21.000000 typetest-cli-1.0.0/README.md
--rw-r--r--   0 senyc     (1000) senyc     (1000)      607 2023-07-07 23:33:10.000000 typetest-cli-1.0.0/pyproject.toml
--rw-r--r--   0 senyc     (1000) senyc     (1000)       38 2023-07-07 23:58:50.813273 typetest-cli-1.0.0/setup.cfg
--rw-r--r--   0 senyc     (1000) senyc     (1000)      276 2023-07-07 23:55:26.000000 typetest-cli-1.0.0/setup.py
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-07 23:58:50.813273 typetest-cli-1.0.0/src/
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-07 23:58:50.813273 typetest-cli-1.0.0/src/typetest_cli/
--rw-r--r--   0 senyc     (1000) senyc     (1000)        0 2023-07-07 21:44:48.000000 typetest-cli-1.0.0/src/typetest_cli/__init__.py
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-07 23:58:50.813273 typetest-cli-1.0.0/src/typetest_cli/text/
--rw-r--r--   0 senyc     (1000) senyc     (1000)       81 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/eight.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       57 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/five.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       83 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/four.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      117 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/nine.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      114 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/one.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       97 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/seven.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       88 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/six.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      169 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/ten.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       93 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/three.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      115 2023-07-07 21:35:59.000000 typetest-cli-1.0.0/src/typetest_cli/text/two.txt
--rwxr-xr-x   0 senyc     (1000) senyc     (1000)     4178 2023-07-07 23:52:39.000000 typetest-cli-1.0.0/src/typetest_cli/typetest.py
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-07 23:58:50.813273 typetest-cli-1.0.0/src/typetest_cli.egg-info/
--rw-r--r--   0 senyc     (1000) senyc     (1000)      220 2023-07-07 23:58:50.000000 typetest-cli-1.0.0/src/typetest_cli.egg-info/PKG-INFO
--rw-r--r--   0 senyc     (1000) senyc     (1000)      662 2023-07-07 23:58:50.000000 typetest-cli-1.0.0/src/typetest_cli.egg-info/SOURCES.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)        1 2023-07-07 23:58:50.000000 typetest-cli-1.0.0/src/typetest_cli.egg-info/dependency_links.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       56 2023-07-07 23:58:50.000000 typetest-cli-1.0.0/src/typetest_cli.egg-info/entry_points.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)        5 2023-07-07 23:58:50.000000 typetest-cli-1.0.0/src/typetest_cli.egg-info/requires.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       13 2023-07-07 23:58:50.000000 typetest-cli-1.0.0/src/typetest_cli.egg-info/top_level.txt
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-08 22:23:23.996909 typetest-cli-1.1.0/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)     1062 2023-07-07 01:09:21.000000 typetest-cli-1.1.0/LICENSE
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       29 2023-07-07 19:35:03.000000 typetest-cli-1.1.0/MANIFEST.in
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      220 2023-07-08 22:23:23.996909 typetest-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       64 2023-07-07 01:09:21.000000 typetest-cli-1.1.0/README.md
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      607 2023-07-08 22:23:04.000000 typetest-cli-1.1.0/pyproject.toml
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       38 2023-07-08 22:23:23.996909 typetest-cli-1.1.0/setup.cfg
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      328 2023-07-08 22:22:54.000000 typetest-cli-1.1.0/setup.py
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-08 22:23:23.996909 typetest-cli-1.1.0/src/
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-08 22:23:23.996909 typetest-cli-1.1.0/src/typetest_cli/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)        0 2023-07-07 21:44:48.000000 typetest-cli-1.1.0/src/typetest_cli/__init__.py
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-08 22:23:23.996909 typetest-cli-1.1.0/src/typetest_cli/text/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       81 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/eight.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       57 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/five.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       83 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/four.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      117 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/nine.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      114 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/one.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       97 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/seven.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       88 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/six.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      169 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/ten.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       93 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/three.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      115 2023-07-07 21:35:59.000000 typetest-cli-1.1.0/src/typetest_cli/text/two.txt
+-rwxr-xr-x   0 senyc     (1000) senyc     (1000)     4298 2023-07-08 22:22:54.000000 typetest-cli-1.1.0/src/typetest_cli/typetest.py
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-08 22:23:23.996909 typetest-cli-1.1.0/src/typetest_cli.egg-info/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      220 2023-07-08 22:23:23.000000 typetest-cli-1.1.0/src/typetest_cli.egg-info/PKG-INFO
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      662 2023-07-08 22:23:23.000000 typetest-cli-1.1.0/src/typetest_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)        1 2023-07-08 22:23:23.000000 typetest-cli-1.1.0/src/typetest_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       56 2023-07-08 22:23:23.000000 typetest-cli-1.1.0/src/typetest_cli.egg-info/entry_points.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)        5 2023-07-08 22:23:23.000000 typetest-cli-1.1.0/src/typetest_cli.egg-info/requires.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       13 2023-07-08 22:23:23.000000 typetest-cli-1.1.0/src/typetest_cli.egg-info/top_level.txt
```

### Comparing `typetest-cli-1.0.0/LICENSE` & `typetest-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typetest-cli-1.0.0/pyproject.toml` & `typetest-cli-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
     requires = ["setuptools"]
 
 [project]
     name = "typetest-cli"
-    version = "1.0.0"
+    version = "1.1.0"
     authors = [
         {name = "senyc"},
     ]
     description = "Prints an interactable line of text that records speed and accuracy of matching upon completion"
     requires-python = ">=3.8"
     dependencies = [
         "rich",
```

### Comparing `typetest-cli-1.0.0/src/typetest_cli/typetest.py` & `typetest-cli-1.1.0/src/typetest_cli/typetest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,116 +15,121 @@
 from rich.console import Console
 from rich.live import Live
 
 user_dir = os.path.expanduser('~')
 here = os.path.abspath(os.path.dirname(__file__))
 
 SOURCE_DIR: Final[str] = f'{here}/text'
-EXTERN_DIR: Final[str] = f'{user_dir}.local/share/typetest-cli/text'
+EXTERN_DIR: Final[str] = f'{user_dir}/.local/share/typetest-cli/text'
 
 @contextmanager
 def raw_mode(file):
     """Puts the terminal into raw mode, allowing for full reading of user's input.
-    On exit, restores the terminal to the previous settings."""
+    On exit, restores the terminal to previous settings."""
     old_settings = termios.tcgetattr(file.fileno())
     try:
         tty.setraw(file.fileno())
         yield
     finally:
         termios.tcsetattr(file.fileno(), termios.TCSADRAIN, old_settings)
 
 def get_char() -> str:
+    """Gets the next character input from the user"""
     with raw_mode(sys.stdin):
         char = sys.stdin.read(1)
     return char
 
-def displayed_text(source: str, user_input: str) -> str:
+def format_text(source: str, user_input: str) -> str:
     final_text = ''
     for source_char, input_char in zip(source, user_input):
         if source_char == input_char:
-            final_text += f'[green]{source_char}'
+            final_text += f'[green]{source_char}[/]'
         else:
-            final_text += (f'[red]{source_char}' if source_char != ' ' else '[red]_')
-    return final_text + '[blue]' + (source[len(user_input)] if source[len(user_input)] != ' ' else '_') + '[white]' + source[len(user_input) + 1: len(source):]
-
-def is_backspace(char: str) -> bool:
-    return char == '\x7f'
+            final_text += f"[red]{source_char if source_char != ' ' else '_'}[/]"
+    if len(user_input) < len(source):
+        return final_text + f"[blue]{source[len(user_input)]}[/]{source[len(user_input) + 1:]}"
+    return final_text
 
 def calc_wpm(time_seconds: float, letters: int) -> int:
     words = letters / 5
     minutes = time_seconds / 60
     return math.floor(words / minutes)
 
-def is_quit(char: str) -> bool:
-    return (char != '' and ord(char) == 3) or (char == '\n' or char == '\r')
-
-def calc_correctness_percent(failures: int, letters: int) -> int:
-    return round(((letters - failures) / letters) * 100)
+def get_accuracy(failures: int, letters: int) -> int:
+    return math.floor(((letters - failures) / letters) * 100)
 
 def count_failures(source: str, user_input: str) -> int:
     failures = 0
     for source_letter, user_input_letter in zip(source, user_input):
         if user_input_letter != source_letter:
             failures += 1
     return failures
 
-def get_random_file(*args):
+def get_random_file(*args) -> str:
     options = []
     for directory in args:
         files = glob.glob(f'{directory}/*')
         options.extend(files)
     return random.choice(options)
 
+def not_quit(char: str) -> bool:
+    """Checks for SIGINT or return"""
+    return not (char != '' and ord(char) == 3) or (char == '\n' or char == '\r')
+
+def add_to(current_input: str, new_char: str) -> str:
+    def is_backspace(char: str) -> bool:
+        return char == '\x7f'
+
+    if is_backspace(new_char):
+        if len(current_input) > 0:
+            return current_input[:-1]
+        else:
+            return current_input
+    return current_input + new_char
+
+
 def main() -> None:
     parser = argparse.ArgumentParser(
         prog='typetest',
         description='Prints an interactable line of text for matching',
         epilog='Only prints out stats if the entire line is written out'
     )
 
     parser.add_argument('--hide-acc', '-a', action='store_true', help='hides the accuracy statistic')
     parser.add_argument('--hide-wpm', '-w', action='store_true', help='hides the word per minute statistic')
     parser.add_argument('--only-base', '-b', action='store_false', help='Only uses the base text')
 
     args = parser.parse_args()
-    if not args.only_base:
-        file = get_random_file(SOURCE_DIR, EXTERN_DIR)
-    else:
+    if args.only_base:
         file = get_random_file(SOURCE_DIR)
-
+    else:
+        file = get_random_file(SOURCE_DIR, EXTERN_DIR)
 
     with open(file, encoding='utf-8', mode='r') as file:
         DATA = file.read().strip('\n').strip(' ')
 
-    total_character_count = len(DATA)
-    user_input = ''
-    console = Console(soft_wrap=True, no_color=False)
+    console = Console(soft_wrap=False, no_color=False)
     start = end = None
+    user_input = ''
 
-    with Live(console=console, refresh_per_second=30) as display:
-        while True:
-            display.update(displayed_text(DATA, user_input))
-            char = get_char()
-            # Starts only after first character entered
+    with Live(console=console, auto_refresh=False) as display:
+        display.update(DATA, refresh=True)
+        while not_quit(char := get_char()) and len(user_input := add_to(user_input, char)) < len(DATA):
             if start is None:
                 start = time.time()
-            if is_quit(char):
-                return
-            user_input = user_input[:-1] if is_backspace(char) else user_input + char
-            if len(user_input) >= total_character_count:
-                end = time.time()
-                break
+            display.update(format_text(DATA, user_input), refresh=True)
+        end = time.time()
+        display.update(format_text(DATA, user_input), refresh=True)
 
-    # Validates the there is an endtime to display
-    if not end:
+    if len(user_input) != len(DATA):
         return
 
     if not args.hide_acc:
-        print(calc_correctness_percent(count_failures(DATA, user_input), total_character_count), "percent correct")
+        print(get_accuracy(count_failures(DATA, user_input), len(DATA)), "percent correct")
 
     if not args.hide_wpm:
-        print(calc_wpm(end - start, total_character_count), "words per minute")
+        print(calc_wpm(end - start, len(DATA)), "words per minute")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `typetest-cli-1.0.0/src/typetest_cli.egg-info/SOURCES.txt` & `typetest-cli-1.1.0/src/typetest_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

