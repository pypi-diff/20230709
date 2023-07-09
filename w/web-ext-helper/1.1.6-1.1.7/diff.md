# Comparing `tmp/web_ext_helper-1.1.6.tar.gz` & `tmp/web_ext_helper-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.1.6.tar", max compression
+gzip compressed data, was "web_ext_helper-1.1.7.tar", max compression
```

## Comparing `web_ext_helper-1.1.6.tar` & `web_ext_helper-1.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.6/LICENSE
--rw-r--r--   0        0        0      654 2023-06-19 17:41:14.311771 web_ext_helper-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.6/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.6/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.6/web_ext_helper/functions.py
--rw-r--r--   0        0        0    18518 2023-06-19 17:40:52.404327 web_ext_helper-1.1.6/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 web_ext_helper-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.1.7/LICENSE
+-rw-r--r--   0        0        0      654 2023-07-09 20:23:41.176913 web_ext_helper-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.1.7/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.1.7/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.1.7/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    20341 2023-07-09 20:23:21.044790 web_ext_helper-1.1.7/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 web_ext_helper-1.1.7/PKG-INFO
```

### Comparing `web_ext_helper-1.1.6/LICENSE` & `web_ext_helper-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.6/pyproject.toml` & `web_ext_helper-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.1.6"
+version = "1.1.7"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.1.6/README.md` & `web_ext_helper-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.6/web_ext_helper/functions.py` & `web_ext_helper-1.1.7/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.1.6/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.1.7/web_ext_helper/web_ext_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.1.6"
+__ext_version__ = "1.1.7"
 
 import os
 import json
 import shutil
 import typer
 import zipfile
 import rich.progress
@@ -26,15 +26,14 @@
 cached_app_dir = os.path.dirname(os.path.dirname(cached_app_build_dir))
 os.makedirs(cached_app_build_dir, exist_ok=True)
 os.makedirs(os.path.dirname(cached_app_data_env_dir), exist_ok=True)
 
 load_dotenv(cached_app_data_env_dir)
 
 app = typer.Typer()
-typer.clear()
 
 try:
     with open("src/manifest.json", "r") as manifest_file:
         manifest_data = json.load(manifest_file)
 
     manifest_name = manifest_data["name"]
     manifest_name_lower = manifest_data["name"].lower()
@@ -402,39 +401,54 @@
         description,
         permissions,
         logo,
         browser_action_title,
         strict_min_version,
         app_id,
     ):
-        typer.clear()
-        name = typer.prompt("Name of the extension (required)", default=name)
+        name = typer.prompt(
+            f"Name of the extension ({bcolors.FAIL}required{bcolors.ENDC})",
+            default=f"{bcolors.OKGREEN}{name}{bcolors.ENDC}"
+            if name is not None
+            else None,
+        )
         version = typer.prompt(
             "Version of the extension",
-            default=version if is_validation else "1.0.0",
+            default=f"{bcolors.OKGREEN}{version}{bcolors.ENDC}"
+            if is_validation
+            else f"{bcolors.OKGREEN}1.0.0{bcolors.ENDC}",
         )
+        version = version.replace(bcolors.OKGREEN, "").replace(bcolors.ENDC, "")
         if len(version.split(".")) != 3:
             error("Version must follow the pattern major.minor.patch")
             raise typer.Exit(1)
         description = typer.prompt(
-            "Description of the extension (required)", default=description
+            f"Description of the extension ({bcolors.FAIL}required{bcolors.ENDC})",
+            default=f"{bcolors.OKGREEN}{description}{bcolors.ENDC}"
+            if description is not None
+            else None,
         )
         permissions = typer.prompt(
-            "Permissions of the extension (separated by ',')",
-            default=", ".join(permissions) if is_validation else "",
-            show_default=True,
+            f"Permissions of the extension ({bcolors.PURPLE}separated by ','{bcolors.ENDC})",
+            default=f"{bcolors.OKGREEN}{', '.join(permissions)}{bcolors.ENDC}"
+            if is_validation
+            else "",
         )
         permissions = (
             list(map(lambda x: x.strip(), permissions.split(",")))
             if permissions != ""
             else []
         )
         logo = typer.prompt(
-            "Path to logo of the extension (leave blank for none)",
-            default=(logo if logo is not None else "") if is_validation else "",
+            f"Path to logo of the extension ({bcolors.PURPLE}leave blank for none{bcolors.ENDC})",
+            default=(
+                f"{bcolors.OKGREEN}{logo}{bcolors.ENDC}" if logo is not None else ""
+            )
+            if is_validation
+            else "",
             show_default=False if not is_validation else True,
         )
         if logo == "":
             logo = None
         else:
             if not os.path.exists(logo):
                 error("Logo not found")
@@ -443,47 +457,69 @@
             try:
                 Image.open(logo)
             except:
                 error("Invalid image")
                 raise typer.Exit(1)
         browser_action_title = typer.prompt(
             "Title of the browser action",
-            default=browser_action_title if is_validation else name,
-        )
+            default=f"{bcolors.OKGREEN}{browser_action_title}{bcolors.ENDC}"
+            if is_validation
+            else f"{bcolors.OKGREEN}{name}{bcolors.ENDC}",
+        )
+        browser_action_title = browser_action_title.replace(
+            bcolors.OKGREEN, ""
+        ).replace(bcolors.ENDC, "")
         strict_min_version = typer.prompt(
             "Strict minimum version of Firefox",
-            default=strict_min_version if is_validation else 48.0,
-            type=float,
-        )
-        app_id = typer.prompt("App ID of the extension (required)", default=app_id)
+            default=f"{bcolors.OKGREEN}{strict_min_version}{bcolors.ENDC}"
+            if is_validation
+            else f"{bcolors.OKGREEN}48.0{bcolors.ENDC}",
+        )
+        if strict_min_version == "\x1b[92m48.0\x1b[0m":
+            strict_min_version = "48.0"
+        assert float(strict_min_version) >= 48.0
+        app_id = typer.prompt(
+            f"App ID of the extension ({bcolors.FAIL}required{bcolors.ENDC})",
+            default=f"{bcolors.OKGREEN}{app_id}{bcolors.ENDC}"
+            if app_id is not None
+            else None,
+        )
+
+        def validate_input():
+            prompt = typer.prompt(
+                f"""
+Name: {bcolors.PURPLE}{name}{bcolors.ENDC}
+Version: {bcolors.PURPLE}{version}{bcolors.ENDC}
+Description: {bcolors.PURPLE}{description}{bcolors.ENDC}
+Permissions: {bcolors.PURPLE}{permissions}{bcolors.ENDC}
+Logo: {bcolors.PURPLE}{logo}{bcolors.ENDC}
+Browser action title: {bcolors.PURPLE}{browser_action_title}{bcolors.ENDC}
+Strict minimum version: {bcolors.PURPLE}{strict_min_version}{bcolors.ENDC}
+App ID: {bcolors.PURPLE}{app_id}{bcolors.ENDC}
+
+    """,
+                prompt_suffix=f"{bcolors.OKCYAN}Continue? [Y/n]:{bcolors.ENDC}",
+            ).lower()
+            if prompt in ["n", "no"]:
+                typer.echo("\n")
+                return ask_for_input(
+                    True,
+                    name,
+                    version,
+                    description,
+                    permissions,
+                    logo,
+                    browser_action_title,
+                    strict_min_version,
+                    app_id,
+                )
+            elif prompt not in ["y", "yes", ""]:
+                return validate_input()
 
-        if not typer.confirm(
-            f"""
-Name: {name}
-Version: {version}
-Description: {description}
-Permissions: {permissions}
-Logo: {logo}
-Browser action title: {browser_action_title}
-Strict minimum version: {strict_min_version}
-App ID: {app_id}
-""",
-            default=True,
-        ):
-            return ask_for_input(
-                True,
-                name,
-                version,
-                description,
-                permissions,
-                logo,
-                browser_action_title,
-                strict_min_version,
-                app_id,
-            )
+        validate_input()
 
         if name == "" or description == "" or app_id == "":
             error("Name, description and app ID are required")
             raise typer.Exit(1)
 
         if logo != None and not os.path.exists(logo):
             error("Logo not found")
```

### Comparing `web_ext_helper-1.1.6/PKG-INFO` & `web_ext_helper-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.1.6
+Version: 1.1.7
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

