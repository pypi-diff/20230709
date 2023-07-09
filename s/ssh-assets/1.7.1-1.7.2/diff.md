# Comparing `tmp/ssh_assets-1.7.1.tar.gz` & `tmp/ssh_assets-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_assets-1.7.1.tar", max compression
+gzip compressed data, was "ssh_assets-1.7.2.tar", max compression
```

## Comparing `ssh_assets-1.7.1.tar` & `ssh_assets-1.7.2.tar`

### file list

```diff
@@ -1,52 +1,51 @@
--rw-r--r--   0        0        0     1497 2023-03-10 16:09:07.188928 ssh_assets-1.7.1/LICENSE
--rw-r--r--   0        0        0     2809 2022-10-02 11:53:32.860750 ssh_assets-1.7.1/README.md
--rw-r--r--   0        0        0     1040 2023-03-10 16:10:56.492050 ssh_assets-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      171 2023-03-10 16:13:57.273018 ssh_assets-1.7.1/ssh_assets/__init__.py
--rw-r--r--   0        0        0      209 2023-03-10 16:13:47.114248 ssh_assets-1.7.1/ssh_assets/authorized_keys/__init__.py
--rw-r--r--   0        0        0     1264 2023-03-10 16:13:45.529669 ssh_assets-1.7.1/ssh_assets/authorized_keys/constants.py
--rw-r--r--   0        0        0     1428 2023-03-10 16:13:49.836308 ssh_assets-1.7.1/ssh_assets/authorized_keys/loader.py
--rw-r--r--   0        0        0     3765 2023-03-10 16:13:44.262707 ssh_assets-1.7.1/ssh_assets/authorized_keys/options.py
--rw-r--r--   0        0        0     2935 2023-03-10 16:13:51.098308 ssh_assets-1.7.1/ssh_assets/authorized_keys/public_key.py
--rw-r--r--   0        0        0     1807 2023-03-10 16:14:15.319191 ssh_assets-1.7.1/ssh_assets/base.py
--rw-r--r--   0        0        0      161 2023-03-10 16:13:03.555223 ssh_assets-1.7.1/ssh_assets/bin/__init__.py
--rw-r--r--   0        0        0     3302 2023-03-10 16:13:42.828749 ssh_assets-1.7.1/ssh_assets/bin/base.py
--rw-r--r--   0        0        0      168 2023-03-10 16:13:04.931567 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/__init__.py
--rw-r--r--   0        0        0      154 2023-03-10 16:13:16.090682 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/__init__.py
--rw-r--r--   0        0        0      907 2023-03-10 16:13:14.389312 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/add.py
--rw-r--r--   0        0        0     2784 2023-03-10 16:13:19.123086 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/base.py
--rw-r--r--   0        0        0      770 2023-03-10 16:13:09.939571 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/command.py
--rw-r--r--   0        0        0      807 2023-03-10 16:13:07.571525 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/delete.py
--rw-r--r--   0        0        0      828 2023-03-10 16:13:17.449474 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/edit.py
--rw-r--r--   0        0        0      693 2023-03-10 16:13:12.001754 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/list.py
--rw-r--r--   0        0        0      160 2023-03-10 16:13:30.542227 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/__init__.py
--rw-r--r--   0        0        0      816 2023-03-10 16:13:26.977258 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/add.py
--rw-r--r--   0        0        0     3277 2023-03-10 16:13:37.228645 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/base.py
--rw-r--r--   0        0        0      968 2023-03-10 16:13:23.929387 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/command.py
--rw-r--r--   0        0        0      844 2023-03-10 16:13:20.972716 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/delete.py
--rw-r--r--   0        0        0      819 2023-03-10 16:13:32.534298 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/edit.py
--rw-r--r--   0        0        0     2998 2023-03-10 16:13:25.401076 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/list.py
--rw-r--r--   0        0        0     1719 2023-03-10 16:13:35.651237 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/load.py
--rw-r--r--   0        0        0     1634 2023-03-10 16:13:28.280940 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/unload.py
--rw-r--r--   0        0        0      810 2023-03-10 16:13:40.987959 ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/main.py
--rw-r--r--   0        0        0      214 2023-03-10 16:12:55.772469 ssh_assets-1.7.1/ssh_assets/configuration/__init__.py
--rw-r--r--   0        0        0     4819 2023-03-10 16:12:59.167339 ssh_assets-1.7.1/ssh_assets/configuration/groups.py
--rw-r--r--   0        0        0     9546 2023-03-10 16:12:57.459247 ssh_assets-1.7.1/ssh_assets/configuration/keys.py
--rw-r--r--   0        0        0     2591 2023-03-10 16:13:02.098254 ssh_assets-1.7.1/ssh_assets/configuration/loader.py
--rw-r--r--   0        0        0      385 2023-03-10 16:13:52.390895 ssh_assets-1.7.1/ssh_assets/constants.py
--rw-r--r--   0        0        0       53 2023-02-07 06:11:05.344538 ssh_assets-1.7.1/ssh_assets/data/bash/ssh-assets.sh
--rwxr-xr-x   0        0        0      348 2023-02-18 03:46:07.390466 ssh_assets-1.7.1/ssh_assets/data/zsh/ssh_assets
--rw-r--r--   0        0        0     3615 2023-03-10 16:13:54.700340 ssh_assets-1.7.1/ssh_assets/duration.py
--rw-r--r--   0        0        0      334 2023-03-10 16:13:58.862011 ssh_assets-1.7.1/ssh_assets/exceptions.py
--rw-r--r--   0        0        0      151 2023-03-10 16:14:03.977174 ssh_assets-1.7.1/ssh_assets/keys/__init__.py
--rw-r--r--   0        0        0     4864 2023-03-10 16:14:09.848567 ssh_assets-1.7.1/ssh_assets/keys/agent.py
--rw-r--r--   0        0        0     4275 2023-03-10 16:14:12.078924 ssh_assets-1.7.1/ssh_assets/keys/base.py
--rw-r--r--   0        0        0      663 2023-03-10 16:14:02.440659 ssh_assets-1.7.1/ssh_assets/keys/constants.py
--rw-r--r--   0        0        0     4879 2023-03-10 16:14:06.501535 ssh_assets-1.7.1/ssh_assets/keys/file.py
--rw-r--r--   0        0        0     3876 2023-03-10 16:14:05.299417 ssh_assets-1.7.1/ssh_assets/keys/filter_set.py
--rw-r--r--   0        0        0     1738 2023-03-10 16:13:55.834893 ssh_assets-1.7.1/ssh_assets/session.py
--rw-r--r--   0        0        0      165 2023-03-10 16:12:50.881303 ssh_assets-1.7.1/ssh_assets/token/__init__.py
--rw-r--r--   0        0        0     1670 2023-03-10 16:12:53.533415 ssh_assets-1.7.1/ssh_assets/token/base.py
--rw-r--r--   0        0        0     6058 2023-03-10 16:12:44.557144 ssh_assets-1.7.1/ssh_assets/token/client.py
--rw-r--r--   0        0        0     2988 2023-03-10 16:12:41.832463 ssh_assets-1.7.1/ssh_assets/token/server.py
--rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 ssh_assets-1.7.1/setup.py
--rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 ssh_assets-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-03-10 16:09:07.188928 ssh_assets-1.7.2/LICENSE
+-rw-r--r--   0        0        0     2809 2022-10-02 11:53:32.860750 ssh_assets-1.7.2/README.md
+-rw-r--r--   0        0        0     1089 2023-07-09 02:56:26.048858 ssh_assets-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-03-10 16:13:57.273018 ssh_assets-1.7.2/ssh_assets/__init__.py
+-rw-r--r--   0        0        0      209 2023-03-10 16:13:47.114248 ssh_assets-1.7.2/ssh_assets/authorized_keys/__init__.py
+-rw-r--r--   0        0        0     1264 2023-03-10 16:13:45.529669 ssh_assets-1.7.2/ssh_assets/authorized_keys/constants.py
+-rw-r--r--   0        0        0     1428 2023-03-10 16:13:49.836308 ssh_assets-1.7.2/ssh_assets/authorized_keys/loader.py
+-rw-r--r--   0        0        0     3765 2023-03-10 16:13:44.262707 ssh_assets-1.7.2/ssh_assets/authorized_keys/options.py
+-rw-r--r--   0        0        0     2935 2023-03-10 16:13:51.098308 ssh_assets-1.7.2/ssh_assets/authorized_keys/public_key.py
+-rw-r--r--   0        0        0     1807 2023-03-10 16:14:15.319191 ssh_assets-1.7.2/ssh_assets/base.py
+-rw-r--r--   0        0        0      161 2023-03-10 16:13:03.555223 ssh_assets-1.7.2/ssh_assets/bin/__init__.py
+-rw-r--r--   0        0        0     3302 2023-03-10 16:13:42.828749 ssh_assets-1.7.2/ssh_assets/bin/base.py
+-rw-r--r--   0        0        0      168 2023-03-10 16:13:04.931567 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/__init__.py
+-rw-r--r--   0        0        0      154 2023-03-10 16:13:16.090682 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/__init__.py
+-rw-r--r--   0        0        0      907 2023-03-10 16:13:14.389312 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/add.py
+-rw-r--r--   0        0        0     2784 2023-03-10 16:13:19.123086 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/base.py
+-rw-r--r--   0        0        0      770 2023-03-10 16:13:09.939571 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/command.py
+-rw-r--r--   0        0        0      807 2023-03-10 16:13:07.571525 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/delete.py
+-rw-r--r--   0        0        0      828 2023-03-10 16:13:17.449474 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/edit.py
+-rw-r--r--   0        0        0      693 2023-03-10 16:13:12.001754 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/list.py
+-rw-r--r--   0        0        0      160 2023-03-10 16:13:30.542227 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/__init__.py
+-rw-r--r--   0        0        0      816 2023-03-10 16:13:26.977258 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/add.py
+-rw-r--r--   0        0        0     3277 2023-03-10 16:13:37.228645 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/base.py
+-rw-r--r--   0        0        0      968 2023-03-10 16:13:23.929387 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/command.py
+-rw-r--r--   0        0        0      844 2023-03-10 16:13:20.972716 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/delete.py
+-rw-r--r--   0        0        0      819 2023-03-10 16:13:32.534298 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/edit.py
+-rw-r--r--   0        0        0     2998 2023-06-10 11:26:01.537727 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/list.py
+-rw-r--r--   0        0        0     1719 2023-03-10 16:13:35.651237 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/load.py
+-rw-r--r--   0        0        0     1634 2023-03-10 16:13:28.280940 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/unload.py
+-rw-r--r--   0        0        0      810 2023-03-10 16:13:40.987959 ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/main.py
+-rw-r--r--   0        0        0      214 2023-03-10 16:12:55.772469 ssh_assets-1.7.2/ssh_assets/configuration/__init__.py
+-rw-r--r--   0        0        0     4819 2023-03-10 16:12:59.167339 ssh_assets-1.7.2/ssh_assets/configuration/groups.py
+-rw-r--r--   0        0        0     9546 2023-03-10 16:12:57.459247 ssh_assets-1.7.2/ssh_assets/configuration/keys.py
+-rw-r--r--   0        0        0     2591 2023-03-10 16:13:02.098254 ssh_assets-1.7.2/ssh_assets/configuration/loader.py
+-rw-r--r--   0        0        0      385 2023-03-10 16:13:52.390895 ssh_assets-1.7.2/ssh_assets/constants.py
+-rw-r--r--   0        0        0       53 2023-02-07 06:11:05.344538 ssh_assets-1.7.2/ssh_assets/data/bash/ssh-assets.sh
+-rwxr-xr-x   0        0        0      348 2023-02-18 03:46:07.390466 ssh_assets-1.7.2/ssh_assets/data/zsh/ssh_assets
+-rw-r--r--   0        0        0     3615 2023-03-10 16:13:54.700340 ssh_assets-1.7.2/ssh_assets/duration.py
+-rw-r--r--   0        0        0      334 2023-03-10 16:13:58.862011 ssh_assets-1.7.2/ssh_assets/exceptions.py
+-rw-r--r--   0        0        0      151 2023-03-10 16:14:03.977174 ssh_assets-1.7.2/ssh_assets/keys/__init__.py
+-rw-r--r--   0        0        0     4872 2023-06-10 11:24:13.629109 ssh_assets-1.7.2/ssh_assets/keys/agent.py
+-rw-r--r--   0        0        0     4275 2023-03-10 16:14:12.078924 ssh_assets-1.7.2/ssh_assets/keys/base.py
+-rw-r--r--   0        0        0      663 2023-03-10 16:14:02.440659 ssh_assets-1.7.2/ssh_assets/keys/constants.py
+-rw-r--r--   0        0        0     4879 2023-03-10 16:14:06.501535 ssh_assets-1.7.2/ssh_assets/keys/file.py
+-rw-r--r--   0        0        0     3876 2023-03-10 16:14:05.299417 ssh_assets-1.7.2/ssh_assets/keys/filter_set.py
+-rw-r--r--   0        0        0     1738 2023-03-10 16:13:55.834893 ssh_assets-1.7.2/ssh_assets/session.py
+-rw-r--r--   0        0        0      165 2023-03-10 16:12:50.881303 ssh_assets-1.7.2/ssh_assets/token/__init__.py
+-rw-r--r--   0        0        0     1670 2023-03-10 16:12:53.533415 ssh_assets-1.7.2/ssh_assets/token/base.py
+-rw-r--r--   0        0        0     6058 2023-03-10 16:12:44.557144 ssh_assets-1.7.2/ssh_assets/token/client.py
+-rw-r--r--   0        0        0     2988 2023-03-10 16:12:41.832463 ssh_assets-1.7.2/ssh_assets/token/server.py
+-rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 ssh_assets-1.7.2/PKG-INFO
```

### Comparing `ssh_assets-1.7.1/LICENSE` & `ssh_assets-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/README.md` & `ssh_assets-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/pyproject.toml` & `ssh_assets-1.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssh_assets"
-version = "1.7.1"
+version = "1.7.2"
 description = "SSH asset and key management tools"
 authors = ["Ilkka Tuohela <hile@iki.fi>"]
 homepage = "https://github.com/hile/ssh-assets"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
@@ -31,14 +31,18 @@
 flake8-bugbear = "^22"
 flake8-quotes = "^3"
 pycodestyle = "^2"
 pyflakes = "^3"
 pylint = "^2"
 pytest = "^7"
 tox = "^4"
+ruff = "^0.0.261"
 
 [tool.poetry.scripts]
 ssh-assets = "ssh_assets.bin.ssh_assets.main:main"
 
+[tool.ruff]
+line-length = 120
+
 [build-system]
-requires = ["poetry-core>=1.3.2"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ssh_assets-1.7.1/ssh_assets/authorized_keys/constants.py` & `ssh_assets-1.7.2/ssh_assets/authorized_keys/constants.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/authorized_keys/loader.py` & `ssh_assets-1.7.2/ssh_assets/authorized_keys/loader.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/authorized_keys/options.py` & `ssh_assets-1.7.2/ssh_assets/authorized_keys/options.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/authorized_keys/public_key.py` & `ssh_assets-1.7.2/ssh_assets/authorized_keys/public_key.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/base.py` & `ssh_assets-1.7.2/ssh_assets/base.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/base.py` & `ssh_assets-1.7.2/ssh_assets/bin/base.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/add.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/add.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/base.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/base.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/command.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/command.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/delete.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/delete.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/edit.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/edit.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/groups/list.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/groups/list.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/add.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/add.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/base.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/base.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/command.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/command.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/delete.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/delete.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/edit.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/edit.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/list.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/list.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/load.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/load.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/keys/unload.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/keys/unload.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/bin/ssh_assets/main.py` & `ssh_assets-1.7.2/ssh_assets/bin/ssh_assets/main.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/configuration/groups.py` & `ssh_assets-1.7.2/ssh_assets/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/configuration/keys.py` & `ssh_assets-1.7.2/ssh_assets/configuration/keys.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/configuration/loader.py` & `ssh_assets-1.7.2/ssh_assets/configuration/loader.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/duration.py` & `ssh_assets-1.7.2/ssh_assets/duration.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/keys/agent.py` & `ssh_assets-1.7.2/ssh_assets/keys/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class AgentKey(SSHKeyLoader):
     """
     SSH key details from SSH agent key listing
     """
     line: str
     __identity_attributes__ = AGENT_KEY_IDENTITY_ATTRIBUTES
 
-    def __init__(self, line: str, hash_algorithm: str):
+    def __init__(self, line: str, hash_algorithm: str) -> None:
         super().__init__(hash_algorithm)
         self.line = line
         self.__parse_key_info_line__(line)
 
     def __repr__(self) -> str:
         return self.line
```

### Comparing `ssh_assets-1.7.1/ssh_assets/keys/base.py` & `ssh_assets-1.7.2/ssh_assets/keys/base.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/keys/constants.py` & `ssh_assets-1.7.2/ssh_assets/keys/constants.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/keys/file.py` & `ssh_assets-1.7.2/ssh_assets/keys/file.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/keys/filter_set.py` & `ssh_assets-1.7.2/ssh_assets/keys/filter_set.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/session.py` & `ssh_assets-1.7.2/ssh_assets/session.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/token/base.py` & `ssh_assets-1.7.2/ssh_assets/token/base.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/token/client.py` & `ssh_assets-1.7.2/ssh_assets/token/client.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/ssh_assets/token/server.py` & `ssh_assets-1.7.2/ssh_assets/token/server.py`

 * *Files identical despite different names*

### Comparing `ssh_assets-1.7.1/setup.py` & `ssh_assets-1.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,119 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ssh-assets
+Version: 1.7.2
+Summary: SSH asset and key management tools
+Home-page: https://github.com/hile/ssh-assets
+License: BSD-3-Clause
+Author: Ilkka Tuohela
+Author-email: hile@iki.fi
+Requires-Python: >=3.9,<4.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: cli-toolkit (>=2.2,<3.0)
+Description-Content-Type: text/markdown
+
+![Unit Tests](https://github.com/hile/ssh-assets/actions/workflows/unittest.yml/badge.svg)
+![Style Checks](https://github.com/hile/ssh-assets/actions/workflows/lint.yml/badge.svg)
+
+# SSH assets python library
+
+This little utility allows configuring SSH keys to be loaded automatically to
+the SSH agent based on asset configuration files, and can detect loaded keys
+based on the key hash to avoid reloading existing keys.
+
+This library can:
+
+- load SSH key details from various key formats to get key hashes, comments and other key details
+- detect keys loaded to the SSH agent by key hash instead of filename
+- define known SSH keys from multiple locations (project specific folders, shared team folders) with
+  options to name and autoload the key with the module
+- load and unload keys to the agent based on custom configuration file, without asking key password
+  if the key was already loaded
+
+# Installing
+
+This tool can be installed from PyPI.
+
+```bash
+pip install ssh-assets
+```
+
+## Using the CLI tool
+
+This package installs command line utility `ssh-assets`. The tool currently has
+only one command `load-keys` that can be used to load the keys configured in
+the assets configuration file as shown below.
+
+Following command loads any keys not yet loaded to the agent, but limits this
+to the keys with `autoload` property set to `true`:
+
+```bash
+ssh-assets keys load
+ssh-assets keys load --group personal
+ssh-assets keys edit personal --no-autoload
+ssh-assets keys edit personal --autoload
+ssh-assets keys add demo --path ~/.ssh/id_rsa.demo --autoload --expire=8h
+ssh-assets keys delete demo
+```
+
+## SSH assets configuration file
+
+This module uses configuration file `~/.ssh/assets.yml` to define paths to the
+SSH keys.
+
+Example configuration file:
+
+```yaml
+---
+groups:
+  - name: personal
+    expire: 5d
+    keys:
+      - personal
+      - missing-demo-key
+  - name: work
+    expire: 1d
+    keys:
+      - aws
+      - master
+      - myproject
+keys:
+  - name: personal
+    path: ~/.ssh/id_rsa
+    autoload: true
+  - name: aws
+    path: ~/.ssh/id_rsa-aws
+  - name: myproject
+    path: ~/Work/Keys/ssh_project_id
+    autoload: true
+  - name: master
+    expire: 1d
+    path: ~/Work/Keys/master_ssh_key
+```
+
+- `autoload` defaults to False in configuration if not specified.
+- `expore` defines a valid value for key expiration in SSH agent, for example `8h` or `5d`
+
+## Example python code
+
+With such configuration file, you can load the keys marked as `autoload` to the SSH
+agent with following example code. Calling the load method again does not try loading
+the keys again (key is detected in agent loaded keys by hash).
+
+```python
+from ssh_assets.session import SshAssetSession
+SshAssetSession().load_pending_keys()
+```
 
-packages = \
-['ssh_assets',
- 'ssh_assets.authorized_keys',
- 'ssh_assets.bin',
- 'ssh_assets.bin.ssh_assets',
- 'ssh_assets.bin.ssh_assets.groups',
- 'ssh_assets.bin.ssh_assets.keys',
- 'ssh_assets.configuration',
- 'ssh_assets.keys',
- 'ssh_assets.token']
-
-package_data = \
-{'': ['*'], 'ssh_assets': ['data/bash/*', 'data/zsh/*']}
-
-install_requires = \
-['cli-toolkit>=2.2,<3.0']
-
-entry_points = \
-{'console_scripts': ['ssh-assets = ssh_assets.bin.ssh_assets.main:main']}
-
-setup_kwargs = {
-    'name': 'ssh-assets',
-    'version': '1.7.1',
-    'description': 'SSH asset and key management tools',
-    'long_description': '![Unit Tests](https://github.com/hile/ssh-assets/actions/workflows/unittest.yml/badge.svg)\n![Style Checks](https://github.com/hile/ssh-assets/actions/workflows/lint.yml/badge.svg)\n\n# SSH assets python library\n\nThis little utility allows configuring SSH keys to be loaded automatically to\nthe SSH agent based on asset configuration files, and can detect loaded keys\nbased on the key hash to avoid reloading existing keys.\n\nThis library can:\n\n- load SSH key details from various key formats to get key hashes, comments and other key details\n- detect keys loaded to the SSH agent by key hash instead of filename\n- define known SSH keys from multiple locations (project specific folders, shared team folders) with\n  options to name and autoload the key with the module\n- load and unload keys to the agent based on custom configuration file, without asking key password\n  if the key was already loaded\n\n# Installing\n\nThis tool can be installed from PyPI.\n\n```bash\npip install ssh-assets\n```\n\n## Using the CLI tool\n\nThis package installs command line utility `ssh-assets`. The tool currently has\nonly one command `load-keys` that can be used to load the keys configured in\nthe assets configuration file as shown below.\n\nFollowing command loads any keys not yet loaded to the agent, but limits this\nto the keys with `autoload` property set to `true`:\n\n```bash\nssh-assets keys load\nssh-assets keys load --group personal\nssh-assets keys edit personal --no-autoload\nssh-assets keys edit personal --autoload\nssh-assets keys add demo --path ~/.ssh/id_rsa.demo --autoload --expire=8h\nssh-assets keys delete demo\n```\n\n## SSH assets configuration file\n\nThis module uses configuration file `~/.ssh/assets.yml` to define paths to the\nSSH keys.\n\nExample configuration file:\n\n```yaml\n---\ngroups:\n  - name: personal\n    expire: 5d\n    keys:\n      - personal\n      - missing-demo-key\n  - name: work\n    expire: 1d\n    keys:\n      - aws\n      - master\n      - myproject\nkeys:\n  - name: personal\n    path: ~/.ssh/id_rsa\n    autoload: true\n  - name: aws\n    path: ~/.ssh/id_rsa-aws\n  - name: myproject\n    path: ~/Work/Keys/ssh_project_id\n    autoload: true\n  - name: master\n    expire: 1d\n    path: ~/Work/Keys/master_ssh_key\n```\n\n- `autoload` defaults to False in configuration if not specified.\n- `expore` defines a valid value for key expiration in SSH agent, for example `8h` or `5d`\n\n## Example python code\n\nWith such configuration file, you can load the keys marked as `autoload` to the SSH\nagent with following example code. Calling the load method again does not try loading\nthe keys again (key is detected in agent loaded keys by hash).\n\n```python\nfrom ssh_assets.session import SshAssetSession\nSshAssetSession().load_pending_keys()\n```\n\n## History\n\nThis module replaces previous module `systematic-ssh-config` when ready.\n',
-    'author': 'Ilkka Tuohela',
-    'author_email': 'hile@iki.fi',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/hile/ssh-assets',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+## History
 
+This module replaces previous module `systematic-ssh-config` when ready.
 
-setup(**setup_kwargs)
```

