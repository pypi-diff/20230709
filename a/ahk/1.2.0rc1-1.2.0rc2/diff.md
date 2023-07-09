# Comparing `tmp/ahk-1.2.0rc1.tar.gz` & `tmp/ahk-1.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.2.0rc1.tar", last modified: Sat Jul  8 06:57:43 2023, max compression
+gzip compressed data, was "ahk-1.2.0rc2.tar", last modified: Sun Jul  9 19:18:37 2023, max compression
```

## Comparing `ahk-1.2.0rc1.tar` & `ahk-1.2.0rc2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   180681 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    44668 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    83686 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174928 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    40339 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-08 06:57:43.000000 ahk-1.2.0rc1/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-08 06:57:43.213669 ahk-1.2.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 06:57:30.000000 ahk-1.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.629729 ahk-1.2.0rc2/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180681 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44691 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83807 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174928 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    79035 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.629729 ahk-1.2.0rc2/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 19:18:37.000000 ahk-1.2.0rc2/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-09 19:18:37.633729 ahk-1.2.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 19:18:25.000000 ahk-1.2.0rc2/setup.py
```

### Comparing `ahk-1.2.0rc1/PKG-INFO` & `ahk-1.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.2.0rc1
+Version: 1.2.0rc2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -130,15 +130,15 @@
 ahk.add_hotstring('btw', 'by the way')  # string replacements
 ahk.add_hotstring('btw', my_callback) # call python function in response to the hotstring
 ```
 
 You can also remove hotstrings:
 
 ```python
-ahk.remove_hotstring('btw')  # remove hotkey by the trigger sequence
+ahk.remove_hotstring('btw')  # remove a hotstring by its trigger sequence
 ahk.clear_hotstrings()  # remove all registered hotstrings
 ```
 
 ## Mouse
 
 ```python
 from ahk import AHK
```

### Comparing `ahk-1.2.0rc1/ahk/__init__.py` & `ahk-1.2.0rc2/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/_async/engine.py` & `ahk-1.2.0rc2/ahk/_async/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/_async/transport.py` & `ahk-1.2.0rc2/ahk/_async/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,15 +333,15 @@
         self,
         /,
         executable_path: str = '',
         directives: Optional[list[Union[Directive, Type[Directive]]]] = None,
         **kwargs: Any,
     ):
         self._executable_path: str = _resolve_executable_path(executable_path=executable_path)
-        self._hotkey_transport = ThreadedHotkeyTransport(executable_path=self._executable_path)
+        self._hotkey_transport = ThreadedHotkeyTransport(executable_path=self._executable_path, directives=directives)
         self._directives: list[Union[Directive, Type[Directive]]] = directives or []
 
     def on_clipboard_change(
         self, callback: Callable[[int], Any], ex_handler: Optional[Callable[[int, Exception], Any]] = None
     ) -> None:
         self._hotkey_transport.on_clipboard_change(callback, ex_handler)
         return None
```

### Comparing `ahk-1.2.0rc1/ahk/_async/window.py` & `ahk-1.2.0rc2/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/_constants.py` & `ahk-1.2.0rc2/ahk/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -2773,14 +2773,21 @@
 }
 {% endblock autoexecute %}
 {% endblock daemon_script %}
 
 """
 
 HOTKEYS_SCRIPT_TEMPLATE = r"""#Persistent
+{% for directive in directives %}
+{% if directive.apply_to_hotkeys_process %}
+
+{{ directive }}
+{% endif %}
+{% endfor %}
+
 {% if on_clipboard %}
 OnClipboardChange("ClipChanged")
 {% endif %}
 KEEPALIVE := Chr(57344)
 SetTimer, keepalive, 1000
```

### Comparing `ahk-1.2.0rc1/ahk/_hotkey.py` & `ahk-1.2.0rc2/ahk/_hotkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from typing import runtime_checkable
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import jinja2
 
+from .directives import Directive
+
 if sys.version_info >= (3, 10):
     from typing import ParamSpec
 else:
     from typing_extensions import ParamSpec
 
 
 import logging
@@ -53,23 +55,31 @@
         logging.error(f'Failure in clipboard callback {failure!r}', exc_info=True)
     else:
         logging.fatal(f'Ex handler called with bad value {failure!r}', exc_info=False)
         raise TypeError(f'bad value for ex handler {failure!r}') from ex
 
 
 class HotkeyTransportBase(ABC):
-    def __init__(self, executable_path: str, default_ex_handler: Optional[Callable[[str, Exception], Any]] = None):
+    def __init__(
+        self,
+        executable_path: str,
+        default_ex_handler: Optional[Callable[[str, Exception], Any]] = None,
+        directives: Optional[list[Directive | Type[Directive]]] = None,
+    ):
         self._executable_path = executable_path
         self._hotkeys: Dict[str, Hotkey] = {}
         self._default_ex_handler: Callable[[str, Exception], Any] = default_ex_handler or _default_ex_handler
         self._hotstrings: Dict[str, Hotstring] = {}
         self._running: bool = False
         self._get_callback_registry = functools.lru_cache(maxsize=None)(self._callback_registry_uncached)
         self._clipboard_callback: Optional[Callable[[int], Any]] = None
         self._clipboard_ex_handler: Optional[Callable[[int, Exception], Any]] = None
+        if directives is None:
+            directives = []
+        self._directives: list[Directive | Type[Directive]] = directives
 
     @property
     def _callback_registry(self) -> Dict[str, Union[Hotkey, Hotstring]]:
         return self._get_callback_registry()
 
     def _callback_registry_uncached(self) -> Dict[str, Union[Hotkey, Hotstring]]:
         registry: Dict[str, Union[Hotkey, Hotstring]] = dict(self._hotkeys)
@@ -146,16 +156,21 @@
 
 
 class STOP:
     ...
 
 
 class ThreadedHotkeyTransport(HotkeyTransportBase):
-    def __init__(self, executable_path: str, default_ex_handler: Optional[Callable[[str, Exception], Any]] = None):
-        super().__init__(executable_path=executable_path, default_ex_handler=default_ex_handler)
+    def __init__(
+        self,
+        executable_path: str,
+        default_ex_handler: Optional[Callable[[str, Exception], Any]] = None,
+        directives: Optional[list[Directive | Type[Directive]]] = None,
+    ):
+        super().__init__(executable_path=executable_path, default_ex_handler=default_ex_handler, directives=directives)
         self._callback_threads: List[threading.Thread] = []
         self._proc: Optional[subprocess.Popen[bytes]] = None
         self._callback_queue: Queue[Union[str, Type[STOP]]] = Queue()
         self._listener_thread: Optional[threading.Thread] = None
         self._dispatcher_thread: Optional[threading.Thread] = None
         loader: jinja2.BaseLoader
         try:
@@ -201,19 +216,19 @@
         dispatcher_thread = threading.Thread(target=self.dispatcher, daemon=True)
         self._dispatcher_thread = dispatcher_thread
         dispatcher_thread.start()
 
     def stop(self) -> None:
         assert self._running is True, 'Not running! Must be started first!'
         assert self._dispatcher_thread is not None
-        for i in range(1, 6):
+        for i in range(1, 11):
             if self._proc is not None:
                 break
-            logging.debug(f'stop called before dispatched has started proc. Waiting for proc ({i}/5)')
-            time.sleep(0.2)
+            logging.debug(f'stop called before dispatched has started proc. Waiting for proc ({i}/10)')
+            time.sleep(0.1)
         assert self._proc is not None
         self._running = False
 
         self._callback_queue.empty()
         self._callback_queue.put_nowait(STOP)
         logging.debug('Waiting for stop...')
         if self._dispatcher_thread is not None:
@@ -277,15 +292,18 @@
 
     def _render_hotkey_tempate(self) -> str:
         if self._clipboard_callback is not None:
             on_clipboard = True
         else:
             on_clipboard = False
         ret = self._template.render(
-            hotkeys=list(self._hotkeys.values()), hotstrings=self._hotstrings.values(), on_clipboard=on_clipboard
+            hotkeys=list(self._hotkeys.values()),
+            hotstrings=self._hotstrings.values(),
+            on_clipboard=on_clipboard,
+            directives=self._directives,
         )
         return ret
 
     def listener(self) -> None:
         hotkey_script_contents = self._render_hotkey_tempate()
         logging.debug('hotkey script contents:\n%s', hotkey_script_contents)
         with tempfile.TemporaryDirectory(prefix='python-ahk') as tmpdirname:
```

### Comparing `ahk-1.2.0rc1/ahk/_sync/engine.py` & `ahk-1.2.0rc2/ahk/_sync/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/_sync/transport.py` & `ahk-1.2.0rc2/ahk/_sync/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
         self,
         /,
         executable_path: str = '',
         directives: Optional[list[Union[Directive, Type[Directive]]]] = None,
         **kwargs: Any,
     ):
         self._executable_path: str = _resolve_executable_path(executable_path=executable_path)
-        self._hotkey_transport = ThreadedHotkeyTransport(executable_path=self._executable_path)
+        self._hotkey_transport = ThreadedHotkeyTransport(executable_path=self._executable_path, directives=directives)
         self._directives: list[Union[Directive, Type[Directive]]] = directives or []
 
     def on_clipboard_change(
         self, callback: Callable[[int], Any], ex_handler: Optional[Callable[[int, Exception], Any]] = None
     ) -> None:
         self._hotkey_transport.on_clipboard_change(callback, ex_handler)
         return None
@@ -355,17 +355,14 @@
         self._hotkey_transport.remove_hotstring(hotstring)
         return None
 
     def clear_hotstrings(self) -> None:
         self._hotkey_transport.clear_hotstrings()
         return None
 
-
-
-
     def start_hotkeys(self) -> None:
         return self._hotkey_transport.start()
 
     def stop_hotkeys(self) -> None:
         return self._hotkey_transport.stop()
 
     def init(self) -> None:
```

### Comparing `ahk-1.2.0rc1/ahk/_sync/window.py` & `ahk-1.2.0rc2/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/_utils.py` & `ahk-1.2.0rc2/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/directives.py` & `ahk-1.2.0rc2/ahk/directives.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     """
     Simple directive class
     They are designed to be hashable and comparable with string equivalent of AHK directive.
     Directives that don't require arguments do not need to be instantiated.
     """
 
     def __init__(self, **kwargs: Any):
-        super().__init__(name=self.name, **kwargs)
+        apply_to_hotkeys = kwargs.pop('apply_to_hotkeys_process', False)
+        super().__init__(name=self.name, apply_to_hotkeys_process=apply_to_hotkeys, **kwargs)
         self._kwargs = kwargs
 
     @property
     def name(self) -> str:
         return self.__class__.__name__
 
     def __str__(self) -> str:
```

### Comparing `ahk-1.2.0rc1/ahk/keys.py` & `ahk-1.2.0rc2/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/message.py` & `ahk-1.2.0rc2/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/templates/daemon.ahk` & `ahk-1.2.0rc2/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/ahk/templates/hotkeys.ahk` & `ahk-1.2.0rc2/ahk/templates/hotkeys.ahk`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 #Persistent
+{% for directive in directives %}
+{% if directive.apply_to_hotkeys_process %}
+
+{{ directive }}
+{% endif %}
+{% endfor %}
+
 {% if on_clipboard %}
 OnClipboardChange("ClipChanged")
 {% endif %}
 KEEPALIVE := Chr(57344)
 SetTimer, keepalive, 1000
```

### Comparing `ahk-1.2.0rc1/ahk.egg-info/PKG-INFO` & `ahk-1.2.0rc2/ahk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.2.0rc1
+Version: 1.2.0rc2
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
@@ -130,15 +130,15 @@
 ahk.add_hotstring('btw', 'by the way')  # string replacements
 ahk.add_hotstring('btw', my_callback) # call python function in response to the hotstring
 ```
 
 You can also remove hotstrings:
 
 ```python
-ahk.remove_hotstring('btw')  # remove hotkey by the trigger sequence
+ahk.remove_hotstring('btw')  # remove a hotstring by its trigger sequence
 ahk.clear_hotstrings()  # remove all registered hotstrings
 ```
 
 ## Mouse
 
 ```python
 from ahk import AHK
```

### Comparing `ahk-1.2.0rc1/ahk.egg-info/SOURCES.txt` & `ahk-1.2.0rc2/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/buildunasync.py` & `ahk-1.2.0rc2/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.2.0rc1/docs/README.md` & `ahk-1.2.0rc2/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 ahk.add_hotstring('btw', 'by the way')  # string replacements
 ahk.add_hotstring('btw', my_callback) # call python function in response to the hotstring
 ```
 
 You can also remove hotstrings:
 
 ```python
-ahk.remove_hotstring('btw')  # remove hotkey by the trigger sequence
+ahk.remove_hotstring('btw')  # remove a hotstring by its trigger sequence
 ahk.clear_hotstrings()  # remove all registered hotstrings
 ```
 
 ## Mouse
 
 ```python
 from ahk import AHK
```

### Comparing `ahk-1.2.0rc1/setup.cfg` & `ahk-1.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.2.0rc1
+version = 1.2.0rc2
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords =
```

