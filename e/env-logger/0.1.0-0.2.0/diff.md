# Comparing `tmp/env_logger-0.1.0.tar.gz` & `tmp/env_logger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_logger-0.1.0.tar", max compression
+gzip compressed data, was "env_logger-0.2.0.tar", max compression
```

## Comparing `env_logger-0.1.0.tar` & `env_logger-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-09 14:20:55.837601 env_logger-0.1.0/LICENSE
--rw-r--r--   0        0        0      927 2023-07-09 14:20:55.837601 env_logger-0.1.0/README.md
--rw-r--r--   0        0        0      526 2023-07-09 14:20:55.837601 env_logger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3838 2023-07-09 14:20:55.837601 env_logger-0.1.0/src/env_logger/__init__.py
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 env_logger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-09 14:41:17.266011 env_logger-0.2.0/LICENSE
+-rw-r--r--   0        0        0      927 2023-07-09 14:41:17.266011 env_logger-0.2.0/README.md
+-rw-r--r--   0        0        0      526 2023-07-09 14:41:17.270011 env_logger-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4344 2023-07-09 14:41:17.270011 env_logger-0.2.0/src/env_logger/__init__.py
+-rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 env_logger-0.2.0/PKG-INFO
```

### Comparing `env_logger-0.1.0/LICENSE` & `env_logger-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `env_logger-0.1.0/README.md` & `env_logger-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `env_logger-0.1.0/pyproject.toml` & `env_logger-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "env_logger"
-version = "0.1.0"
+version = "0.2.0"
 description = "The easy way to configure logging"
 license = "MIT"
 authors = ["AP Ljungquist <ap@ljungquist.eu>"]
 readme = "README.md"
 homepage = "https://github.com/apljungquist/env_logger_py"
```

### Comparing `env_logger-0.1.0/src/env_logger/__init__.py` & `env_logger-0.2.0/src/env_logger/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,20 +69,35 @@
             logging.LogRecord("name", logging.INFO, "pathname", 0, "msg", (), None)
         )
     except Exception as e:
         raise ValueError(f"Invalid log format: {text}") from e
     return text
 
 
+def _valid_handlers(text: Optional[str]) -> Optional[List[logging.Handler]]:
+    if text is None:
+        return None
+    if text == "rich":
+        try:
+            import rich.logging
+
+            return [rich.logging.RichHandler()]
+        except ImportError as e:
+            raise ValueError(
+                f"Invalid log handler: {text} (install rich to enable this handler)"
+            ) from e
+    raise ValueError(f"Invalid log handler: {text}")
+
+
 def _style_output() -> bool:
     # Inspired by https://clig.dev/#output
     # But I disagree with the authors on using stderr for logging.
     if not sys.stderr.isatty():
         return False
-    if os.environ.get("NO_COLOR") != "0":
+    if os.environ.get("NO_COLOR", "0") != "0":
         return False
     if os.environ.get("TERM") == "dumb":
         return False
     return True
 
 
 def configure(**kwargs) -> None:
@@ -97,15 +112,15 @@
         "level",
         lambda: _valid_level(os.environ.get("LOG_LEVEL")),
         lambda: "INFO",
     )
     _resolve(
         kwargs,
         "handlers",
-        lambda: None,
+        lambda: _valid_handlers(os.environ.get("LOG_HANDLER")),
         lambda: [Handler(style_output=_style_output())],
     )
     logging.basicConfig(**kwargs)
 
 
 def _demo() -> None:
     logger.debug("A debug message")
```

### Comparing `env_logger-0.1.0/PKG-INFO` & `env_logger-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-logger
-Version: 0.1.0
+Version: 0.2.0
 Summary: The easy way to configure logging
 Home-page: https://github.com/apljungquist/env_logger_py
 License: MIT
 Author: AP Ljungquist
 Author-email: ap@ljungquist.eu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

