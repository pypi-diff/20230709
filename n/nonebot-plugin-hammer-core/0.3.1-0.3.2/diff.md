# Comparing `tmp/nonebot-plugin-hammer-core-0.3.1.tar.gz` & `tmp/nonebot_plugin_hammer_core-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hammer-core-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_hammer_core-0.3.2.tar", max compression
```

## Comparing `nonebot-plugin-hammer-core-0.3.1.tar` & `nonebot_plugin_hammer_core-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11558 2022-07-31 13:29:05.685625 nonebot-plugin-hammer-core-0.3.1/LICENSE
--rw-r--r--   0        0        0        0 2022-07-31 13:18:58.894461 nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/__init__.py
--rw-r--r--   0        0        0        0 2022-07-30 11:42:07.474000 nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/util/__init__.py
--rw-r--r--   0        0        0      670 2022-08-20 13:52:12.941000 nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/util/constant.py
--rw-r--r--   0        0        0      694 2022-08-21 09:18:17.013000 nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/util/message_factory.py
--rw-r--r--   0        0        0     1648 2022-08-22 03:33:06.200560 nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/util/onebot_utils.py
--rw-r--r--   0        0        0      805 2022-08-22 03:30:15.115314 nonebot-plugin-hammer-core-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1546 2022-08-21 14:35:29.925159 nonebot-plugin-hammer-core-0.3.1/README.md
--rw-r--r--   0        0        0     2284 2022-08-22 03:33:22.109931 nonebot-plugin-hammer-core-0.3.1/setup.py
--rw-r--r--   0        0        0     2167 2022-08-22 03:33:22.109931 nonebot-plugin-hammer-core-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2022-07-31 13:29:05.685625 nonebot_plugin_hammer_core-0.3.2/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-31 13:18:58.894461 nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-30 11:42:07.474000 nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/util/__init__.py
+-rw-r--r--   0        0        0      670 2022-08-20 13:52:12.941000 nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/util/constant.py
+-rw-r--r--   0        0        0      694 2022-08-21 09:18:17.013000 nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/util/message_factory.py
+-rw-r--r--   0        0        0     1648 2022-08-22 03:33:06.200560 nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/util/onebot_utils.py
+-rw-r--r--   0        0        0      805 2023-07-09 08:44:37.913127 nonebot_plugin_hammer_core-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1546 2022-08-21 14:35:29.925159 nonebot_plugin_hammer_core-0.3.2/README.md
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 nonebot_plugin_hammer_core-0.3.2/PKG-INFO
```

### Comparing `nonebot-plugin-hammer-core-0.3.1/LICENSE` & `nonebot_plugin_hammer_core-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/util/constant.py` & `nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/util/constant.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/util/message_factory.py` & `nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/util/message_factory.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hammer-core-0.3.1/nonebot_plugin_hammer_core/util/onebot_utils.py` & `nonebot_plugin_hammer_core-0.3.2/nonebot_plugin_hammer_core/util/onebot_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hammer-core-0.3.1/pyproject.toml` & `nonebot_plugin_hammer_core-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-hammer-core"
-version = "0.3.1"
+version = "0.3.2"
 description = "core dependency of nonebot-plugin-hammer-xxx"
 authors = ["ArgonarioD <739062975@qq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://docs.hammer-hfut.tk:233"
 repository = "https://github.com/ArgonarioD/nonebot-plugin-hammer-core"
 classifiers = [
@@ -15,15 +15,15 @@
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-nonebot-adapter-onebot = "^2.1.1"
+nonebot-adapter-onebot = "^2.2.3"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-hammer-core-0.3.1/README.md` & `nonebot_plugin_hammer_core-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hammer-core-0.3.1/setup.py` & `nonebot_plugin_hammer_core-0.3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,54 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-hammer-core
+Version: 0.3.2
+Summary: core dependency of nonebot-plugin-hammer-xxx
+Home-page: https://docs.hammer-hfut.tk:233
+License: Apache-2.0
+Author: ArgonarioD
+Author-email: 739062975@qq.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Project-URL: Repository, https://github.com/ArgonarioD/nonebot-plugin-hammer-core
+Description-Content-Type: text/markdown
+
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
+
+<div align="center">
+
+# Nonebot Plugin Hammer Core
+
+</div>
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/ArgonarioD/nonebot-plugin-hammer-core/main/LICENSE">
+    <img src="https://img.shields.io/github/license/ArgonarioD/nonebot-plugin-hammer-core" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-hammer-core">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-hammer-core.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.9-blue.svg" alt="python">
+  <img src="https://img.shields.io/badge/nonebot-2.0.0b4-orange" alt="nonebot2">
+</p>
+
+
+## 介绍
+本仓库为nonebot-plugin-hammer-xxx等插件的核心依赖，其中主要内容为我本人（ArgonarioD）在开发nonebot2插件与bot时常用的轮子，本仓库在一般情况下不作为nonebot的插件而是作为插件的依赖库安装到nonebot的运行环境中
+
+## 已经实现的轮子
+ - `util/constant.py` 常量
+ - `util/message_factory.py` 快速构建消息（回复消息）
+ - `util/onebot_utils.get_qq_nickname_with_group` 查找QQ群员昵称字符串格式化生成（对不在本群的群员查找昵称与对应群名并格式化生成）
+
+## 鸣谢
+ - [onebot](https://github.com/botuniverse/onebot)
+ - [nonebot2](https://github.com/nonebot/nonebot2)
 
-packages = \
-['nonebot_plugin_hammer_core', 'nonebot_plugin_hammer_core.util']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['nonebot-adapter-onebot>=2.1.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-hammer-core',
-    'version': '0.3.1',
-    'description': 'core dependency of nonebot-plugin-hammer-xxx',
-    'long_description': '<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# Nonebot Plugin Hammer Core\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/ArgonarioD/nonebot-plugin-hammer-core/main/LICENSE">\n    <img src="https://img.shields.io/github/license/ArgonarioD/nonebot-plugin-hammer-core" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot-plugin-hammer-core">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-hammer-core.svg" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.9-blue.svg" alt="python">\n  <img src="https://img.shields.io/badge/nonebot-2.0.0b4-orange" alt="nonebot2">\n</p>\n\n\n## 介绍\n本仓库为nonebot-plugin-hammer-xxx等插件的核心依赖，其中主要内容为我本人（ArgonarioD）在开发nonebot2插件与bot时常用的轮子，本仓库在一般情况下不作为nonebot的插件而是作为插件的依赖库安装到nonebot的运行环境中\n\n## 已经实现的轮子\n - `util/constant.py` 常量\n - `util/message_factory.py` 快速构建消息（回复消息）\n - `util/onebot_utils.get_qq_nickname_with_group` 查找QQ群员昵称字符串格式化生成（对不在本群的群员查找昵称与对应群名并格式化生成）\n\n## 鸣谢\n - [onebot](https://github.com/botuniverse/onebot)\n - [nonebot2](https://github.com/nonebot/nonebot2)\n\n---\n~~*如果觉得有用的话求点个Star啵QwQ*~~',
-    'author': 'ArgonarioD',
-    'author_email': '739062975@qq.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://docs.hammer-hfut.tk:233',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
+---
+~~*如果觉得有用的话求点个Star啵QwQ*~~
```

#### html2text {}

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_hammer_core', 'nonebot_plugin_hammer_core.util'] package_data
-= \ {'': ['*']} install_requires = \ ['nonebot-adapter-onebot>=2.1.1,<3.0.0']
-setup_kwargs = { 'name': 'nonebot-plugin-hammer-core', 'version': '0.3.1',
-'description': 'core dependency of nonebot-plugin-hammer-xxx',
-'long_description': '
-                                \n [nonebot]\n
-\n\n
-                     \n\n# Nonebot Plugin Hammer Core\n\n
-\n\n
-           \n \n_[license]\n\n \n_[pypi]\n\n [python]\n [nonebot2]\n
-\n\n\n## ä»ç»\næ¬ä»åºä¸ºnonebot-plugin-hammer-
-xxxç­æä»¶çæ ¸å¿ä¾èµï¼å¶ä¸­ä¸»è¦åå®¹ä¸ºææ¬äººï¼ArgonarioDï¼å¨å¼ånonebot2æä»¶ä¸botæ¶å¸¸ç¨çè½®å­ï¼æ¬ä»åºå¨ä¸è¬æåµä¸ä¸ä½ä¸ºnonebotçæä»¶èæ¯ä½ä¸ºæä»¶çä¾èµåºå®è£å°nonebotçè¿è¡ç¯å¢ä¸­\n\n##
-å·²ç»å®ç°çè½®å­\n - `util/constant.py` å¸¸é\n - `util/
-message_factory.py` å¿«éæå»ºæ¶æ¯ï¼åå¤æ¶æ¯ï¼\n - `util/
+Metadata-Version: 2.1 Name: nonebot-plugin-hammer-core Version: 0.3.2 Summary:
+core dependency of nonebot-plugin-hammer-xxx Home-page: https://docs.hammer-
+hfut.tk:233 License: Apache-2.0 Author: ArgonarioD Author-email:
+739062975@qq.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0) Project-URL: Repository,
+https://github.com/ArgonarioD/nonebot-plugin-hammer-core Description-Content-
+Type: text/markdown
+                                   [nonebot]
+                         # Nonebot Plugin Hammer Core
+                     [license] [pypi] [python] [nonebot2]
+## ä»ç» æ¬ä»åºä¸ºnonebot-plugin-hammer-
+xxxç­æä»¶çæ ¸å¿ä¾èµï¼å¶ä¸­ä¸»è¦åå®¹ä¸ºææ¬äººï¼ArgonarioDï¼å¨å¼ånonebot2æä»¶ä¸botæ¶å¸¸ç¨çè½®å­ï¼æ¬ä»åºå¨ä¸è¬æåµä¸ä¸ä½ä¸ºnonebotçæä»¶èæ¯ä½ä¸ºæä»¶çä¾èµåºå®è£å°nonebotçè¿è¡ç¯å¢ä¸­
+## å·²ç»å®ç°çè½®å­ - `util/constant.py` å¸¸é - `util/
+message_factory.py` å¿«éæå»ºæ¶æ¯ï¼åå¤æ¶æ¯ï¼ - `util/
 onebot_utils.get_qq_nickname_with_group`
-æ¥æ¾QQç¾¤åæµç§°å­ç¬¦ä¸²æ ¼å¼åçæï¼å¯¹ä¸å¨æ¬ç¾¤çç¾¤åæ¥æ¾æµç§°ä¸å¯¹åºç¾¤åå¹¶æ ¼å¼åçæï¼\n\n##
-é¸£è°¢\n - [onebot](https://github.com/botuniverse/onebot)\n - [nonebot2]
-(https://github.com/nonebot/nonebot2)\n\n---
-\n~~*å¦æè§å¾æç¨çè¯æ±ç¹ä¸ªStaråµQwQ*~~', 'author': 'ArgonarioD',
-'author_email': '739062975@qq.com', 'maintainer': None, 'maintainer_email':
-None, 'url': 'https://docs.hammer-hfut.tk:233', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+æ¥æ¾QQç¾¤åæµç§°å­ç¬¦ä¸²æ ¼å¼åçæï¼å¯¹ä¸å¨æ¬ç¾¤çç¾¤åæ¥æ¾æµç§°ä¸å¯¹åºç¾¤åå¹¶æ ¼å¼åçæï¼
+## é¸£è°¢ - [onebot](https://github.com/botuniverse/onebot) - [nonebot2](https:
+//github.com/nonebot/nonebot2) --
+- ~~*å¦æè§å¾æç¨çè¯æ±ç¹ä¸ªStaråµQwQ*~~
```

