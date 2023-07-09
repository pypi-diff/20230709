# Comparing `tmp/tclab-sdk-1.3.3.tar.gz` & `tmp/tclab-sdk-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclab-sdk-1.3.3.tar", last modified: Sun Jul  9 02:14:55 2023, max compression
+gzip compressed data, was "tclab-sdk-1.3.4.tar", last modified: Sun Jul  9 02:42:45 2023, max compression
```

## Comparing `tclab-sdk-1.3.3.tar` & `tclab-sdk-1.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 02:14:55.550975 tclab-sdk-1.3.3/
--rw-rw-rw-   0        0        0      888 2023-07-09 02:14:55.549975 tclab-sdk-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 02:14:55.551976 tclab-sdk-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-07-09 02:14:53.000000 tclab-sdk-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:14:55.512278 tclab-sdk-1.3.3/tclab/
--rw-rw-rw-   0        0        0    16594 2023-07-09 02:14:08.000000 tclab-sdk-1.3.3/tclab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 02:14:55.547983 tclab-sdk-1.3.3/tclab_sdk.egg-info/
--rw-rw-rw-   0        0        0      888 2023-07-09 02:14:55.000000 tclab-sdk-1.3.3/tclab_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-09 02:14:55.000000 tclab-sdk-1.3.3/tclab_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 02:14:55.000000 tclab-sdk-1.3.3/tclab_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-09 02:14:55.000000 tclab-sdk-1.3.3/tclab_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-09 02:14:55.000000 tclab-sdk-1.3.3/tclab_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 02:42:45.906373 tclab-sdk-1.3.4/
+-rw-rw-rw-   0        0        0      888 2023-07-09 02:42:45.904361 tclab-sdk-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 02:42:45.906373 tclab-sdk-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-07-09 02:42:35.000000 tclab-sdk-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:42:45.865360 tclab-sdk-1.3.4/tclab/
+-rw-rw-rw-   0        0        0    16809 2023-07-09 02:41:41.000000 tclab-sdk-1.3.4/tclab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:42:45.901358 tclab-sdk-1.3.4/tclab_sdk.egg-info/
+-rw-rw-rw-   0        0        0      888 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-09 02:42:45.000000 tclab-sdk-1.3.4/tclab_sdk.egg-info/top_level.txt
```

### Comparing `tclab-sdk-1.3.3/PKG-INFO` & `tclab-sdk-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tclab-sdk-1.3.3/setup.py` & `tclab-sdk-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tclab-sdk",  # 模块名称
-    version="1.3.3",  # 当前版本
+    version="1.3.4",  # 当前版本
     author="Haotian Yang",  # 作者
     author_email="yht1592754117@126.com",  # 作者邮箱
     description="TC Laboratory Central_Management_System Client Module",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
```

### Comparing `tclab-sdk-1.3.3/tclab/__init__.py` & `tclab-sdk-1.3.4/tclab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,20 @@
         self.lab_server_address = lab_server_address
         self.lab_server_port = port
         self.lab_server = f'{self.lab_server_address}:{port}'
         self.key = key
         # 密钥管理
         self.keys=self._keys()
         self.keys._request=self.request
+        # 检查是否能连接
+        try:
+            self.request('/status')
+        except Exception as e:
+            if str(e)=='failed to connect':
+                raise Exception('failed to connect')
 
     def encrypt_data(self,data: str, key: str):
         """加密函数
 
         Args:
             data (str): 待加密的数据
             key (str): 加密密钥
```

### Comparing `tclab-sdk-1.3.3/tclab_sdk.egg-info/PKG-INFO` & `tclab-sdk-1.3.4/tclab_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

