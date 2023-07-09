# Comparing `tmp/punch_clock-0.1.0.tar.gz` & `tmp/punch_clock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punch_clock-0.1.0.tar", max compression
+gzip compressed data, was "punch_clock-0.1.1.tar", max compression
```

## Comparing `punch_clock-0.1.0.tar` & `punch_clock-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      937 2023-07-09 11:48:54.216029 punch_clock-0.1.0/README.md
--rw-r--r--   0        0        0      142 2023-07-09 12:01:53.888026 punch_clock-0.1.0/punch_clock/__init__.py
--rw-r--r--   0        0        0     1566 2023-07-09 11:58:42.490026 punch_clock-0.1.0/punch_clock/punch_clock.py
--rw-r--r--   0        0        0      991 2023-07-09 12:03:39.044025 punch_clock-0.1.0/punch_clock/utils.py
--rw-r--r--   0        0        0      888 2023-07-09 11:48:54.217028 punch_clock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 punch_clock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      417 2023-07-09 13:39:18.048071 punch_clock-0.1.1/README.md
+-rw-r--r--   0        0        0      143 2023-07-09 13:36:57.967071 punch_clock-0.1.1/punch_clock/__init__.py
+-rw-r--r--   0        0        0     1563 2023-07-09 13:36:57.967071 punch_clock-0.1.1/punch_clock/punch_clock.py
+-rw-r--r--   0        0        0      916 2023-07-09 13:36:57.967071 punch_clock-0.1.1/punch_clock/utils.py
+-rw-r--r--   0        0        0      901 2023-07-09 13:36:57.967071 punch_clock-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 punch_clock-0.1.1/PKG-INFO
```

### Comparing `punch_clock-0.1.0/punch_clock/punch_clock.py` & `punch_clock-0.1.1/punch_clock/punch_clock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import git
 import os
 from . import utils
 import click
 
+
 def get_repo() -> git.Repo:
     return git.Repo(".")
 
+
 def get_name(git_config: git.GitConfigParser) -> str:
     name = git_config.get_value("user", "name")
     name = name.replace(" ", "-")
     name = "".join([c if c.isalnum() else "-" for c in name])
     name = "_".join(name.split("-"))
     name = name.lower()
     return name
 
+
 def get_email(git_config: git.GitConfigParser) -> str:
     return git_config.get_value("user", "email")
 
+
 def push_repo(repo: git.Repo, m: str, dir: str, name: str) -> None:
     filename = f"{dir}/{name}.md"
     repo.index.add(filename)
     repo.index.commit(m)
     repo.remotes.origin.push()
     pass
 
+
 def entry_in(name: str, dir: str) -> None:
     try:
         with open(f"{dir}/{name}.md", "r+") as f:
             f.seek(0, os.SEEK_END)
             f.seek(f.tell() - 1, os.SEEK_SET)
             if f.read(1) == "\n":
                 f.write(f"| {utils.get_time()} |")
@@ -45,8 +50,7 @@
             if f.read(1) != "\n":
                 content = click.prompt(">> what did you do?", type=str)
                 f.write(f" {utils.get_time()} | {content} |\n")
             else:
                 raise Exception("!!! already punched out !!!")
     except Exception as e:
         raise e
-
```

### Comparing `punch_clock-0.1.0/punch_clock/utils.py` & `punch_clock-0.1.1/punch_clock/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from datetime import datetime
 
+
 def create_folder(dir: str) -> None:
-    print(os.path.exists(dir))
     if not os.path.exists(dir):
         try:
             os.mkdir(dir)
         except:
             raise Exception("ERROR - cannot create the folder")
 
+
 def create_user(name: str, email: str, dir: str) -> None:
-    print(os.path.exists(f"{dir}/{name}.md"))
     if not os.path.exists(f"{dir}/{name}.md"):
         try:
             create_folder(dir)
             with open(f"{dir}/{name}.md", "w") as f:
                 f.write(f"| Name | Email |\n")
                 f.write(f"| ---- | ----- |\n")
                 f.write(f"| {name} | {email} |\n\n\n")
```

### Comparing `punch_clock-0.1.0/pyproject.toml` & `punch_clock-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "punch-clock"
-version = "0.1.0"
-description = "to track R and D students"
+version = "0.1.1"
+description = "to track working hours directly in git"
 authors = ["Debora Oliveira <deb.olibeira@protonmail.com>"]
 readme = "README.md"
 packages = [{include = "punch_clock"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 gitpython = "^3.1.31"
```

