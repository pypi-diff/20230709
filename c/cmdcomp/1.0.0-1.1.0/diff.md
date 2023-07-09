# Comparing `tmp/cmdcomp-1.0.0.tar.gz` & `tmp/cmdcomp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.0.0.tar", max compression
+gzip compressed data, was "cmdcomp-1.1.0.tar", max compression
```

## Comparing `cmdcomp-1.0.0.tar` & `cmdcomp-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      501 2023-07-09 07:27:06.298379 cmdcomp-1.0.0/README.md
--rw-r--r--   0        0        0       79 2023-07-05 12:41:19.219375 cmdcomp-1.0.0/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2117 2023-07-06 12:23:19.304229 cmdcomp-1.0.0/cmdcomp/app.py
--rw-r--r--   0        0        0     1962 2023-07-09 07:09:24.304223 cmdcomp-1.0.0/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-04 14:18:59.358598 cmdcomp-1.0.0/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      211 2023-07-06 12:23:19.304229 cmdcomp-1.0.0/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-06 12:23:19.304229 cmdcomp-1.0.0/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-04 14:18:59.358598 cmdcomp-1.0.0/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-09 07:09:24.304223 cmdcomp-1.0.0/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-06 12:23:19.304229 cmdcomp-1.0.0/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-06 12:23:19.304229 cmdcomp-1.0.0/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-06 12:23:19.304229 cmdcomp-1.0.0/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-09 07:09:24.304223 cmdcomp-1.0.0/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-06 12:23:19.304229 cmdcomp-1.0.0/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-05 13:57:54.899379 cmdcomp-1.0.0/cmdcomp/exception.py
--rw-r--r--   0        0        0       64 2023-07-05 12:51:39.839380 cmdcomp-1.0.0/cmdcomp/main.py
--rw-r--r--   0        0        0       81 2023-07-04 14:20:18.957418 cmdcomp-1.0.0/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1623 2023-07-09 07:09:24.304223 cmdcomp-1.0.0/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1169 2023-07-09 07:09:24.304223 cmdcomp-1.0.0/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1202 2023-07-09 07:30:32.832323 cmdcomp-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 cmdcomp-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/README.md
+-rw-r--r--   0        0        0       79 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2117 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/app.py
+-rw-r--r--   0        0        0     1983 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3193 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/exception.py
+-rw-r--r--   0        0        0       64 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/main.py
+-rw-r--r--   0        0        0       81 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/shell_type.py
+-rw-r--r--   0        0        0     1623 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1169 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1687 2023-07-09 20:50:38.598378 cmdcomp-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 cmdcomp-1.1.0/PKG-INFO
```

### Comparing `cmdcomp-1.0.0/cmdcomp/app.py` & `cmdcomp-1.1.0/cmdcomp/app.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.0.0/cmdcomp/completion.py` & `cmdcomp-1.1.0/cmdcomp/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     env = Environment(
         loader=FileSystemLoader(Path(__file__).parent / "templates"),
     )
     template = env.get_template(f"{shell.value}.sh.jinja")
 
     return template.render(
         app_name=config.app.name,
-        app_aliases=config.root.aliases,
+        app_aliases=config.app.aliases + config.root.aliases,
         completions_list=generate_completions_list(config),
     )
 
 
 def generate_completions_list(config: Config):
     completions_list = [get_candidates(config.root)]
```

### Comparing `cmdcomp-1.0.0/cmdcomp/config/command/command.py` & `cmdcomp-1.1.0/cmdcomp/config/command/command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.0.0/cmdcomp/config/config.py` & `cmdcomp-1.1.0/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.0.0/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.1.0/cmdcomp/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.0.0/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.1.0/cmdcomp/templates/zsh.sh.jinja`

 * *Files identical despite different names*

