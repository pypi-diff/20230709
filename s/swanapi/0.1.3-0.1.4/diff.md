# Comparing `tmp/swanapi-0.1.3-py3-none-any.whl.zip` & `tmp/swanapi-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 7406 bytes, number of entries: 12
+Zip file size: 9011 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       62 b- defN 23-Jul-08 12:12 swanapi/__init__.py
--rw-r--r--  2.0 unx     6378 b- defN 23-Jul-08 08:54 swanapi/base_inference.py
+-rw-r--r--  2.0 unx     7611 b- defN 23-Jul-09 11:38 swanapi/base_inference.py
 -rw-r--r--  2.0 unx      833 b- defN 23-Jul-08 11:33 swanapi/make_build.py
--rw-r--r--  2.0 unx     1897 b- defN 23-Jul-08 09:00 swanapi/server.py
--rw-r--r--  2.0 unx      572 b- defN 23-Jul-08 07:57 swanapi/utils.py
+-rw-r--r--  2.0 unx     1790 b- defN 23-Jul-09 11:44 swanapi/server.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 07:52 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
--rw-r--r--  2.0 unx     4869 b- defN 23-Jul-08 12:12 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      347 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      947 b- defN 23-Jul-08 12:13 swanapi-0.1.3.dist-info/RECORD
-12 files, 16058 bytes uncompressed, 5808 bytes compressed:  63.8%
+-rw-r--r--  2.0 unx     3656 b- defN 23-Jul-09 12:44 swanapi/docker_builder/config.py
+-rw-r--r--  2.0 unx     2309 b- defN 23-Jul-09 12:44 swanapi/docker_builder/generate_dockerfile.py
+-rw-r--r--  2.0 unx     1406 b- defN 23-Jul-09 12:44 swanapi/docker_builder/runner.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/RECORD
+14 files, 20371 bytes uncompressed, 7107 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -12,26 +12,32 @@
 
 Filename: swanapi/utils.py
 Comment: 
 
 Filename: swanapi/docker_builder/__init__.py
 Comment: 
 
+Filename: swanapi/docker_builder/config.py
+Comment: 
+
+Filename: swanapi/docker_builder/generate_dockerfile.py
+Comment: 
+
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.3.dist-info/METADATA
+Filename: swanapi-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.3.dist-info/WHEEL
+Filename: swanapi-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.3.dist-info/entry_points.txt
+Filename: swanapi-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.3.dist-info/top_level.txt
+Filename: swanapi-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.3.dist-info/RECORD
+Filename: swanapi-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/base_inference.py

```diff
@@ -1,31 +1,32 @@
-from .utils import check_elements_in_list, is_float
+from .utils import check_elements_in_list, is_float, is_list, is_dict
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 import inspect
 import numpy as np
 import cv2
 import base64
 
 
 class BaseInference:
     def __init__(self):
-        # self.model's options - ["both", "input_only", "output_only"]
+        # self.mode's options - ["both", "input_only", "output_only"]
         self.mode = "both"
-        self.io_types = ["text", "image", "number"]
         self.fn = None
         self.inputs = None
         self.outputs = None
         self.signature = None
         self.fn_param_names = None
         self.TYPES = {
             "text": str,
-            "image": Union[bytes],
+            "image": Union[bytes, str],
             "number": Union[int, float],
+            "list": list,
+            "dict": dict,
         }
-        self.inputs_typing = None
+        self.types_list = list(self.TYPES.keys())
         self.outputs_typing = None
         self.prediction_inputs = None
         self.prediction_inputs_keys = None
         self.prediction_output_num_variables = None
 
     def inference_type_checker(self) -> None:
         # 如果fn是列表，报错
@@ -53,22 +54,20 @@
         if not isinstance(self.inputs, list):
             self.inputs = [self.inputs]
         if not isinstance(self.outputs, list):
             self.outputs = [self.outputs]
 
         # 类型检查: 输入的类型是否在io_types中
         if self.mode == "both":
-            assert check_elements_in_list(self.inputs, self.io_types)
-            assert check_elements_in_list(self.outputs, self.io_types)
+            assert check_elements_in_list(self.inputs, self.types_list)
+            assert check_elements_in_list(self.outputs, self.types_list)
         elif self.mode == "input_only":
-            assert check_elements_in_list(self.inputs, self.io_types)
+            assert check_elements_in_list(self.inputs, self.types_list)
         else:
-            assert check_elements_in_list(self.outputs, self.io_types)
-
-        self.inputs_typing = [self.TYPES[input] for input in self.inputs]
+            assert check_elements_in_list(self.outputs, self.types_list)
 
     def get_fn_information(self) -> None:
         # 得到fn函数的签名信息
         self.signature = inspect.signature(self.fn)
 
         # 得到fn函数的参数名
         self.fn_param_names = [param for param in self.signature.parameters]
@@ -81,26 +80,40 @@
 
         self.prediction_inputs_keys = list(self.prediction_inputs.keys())
         assert check_elements_in_list(self.prediction_inputs_keys, self.fn_param_names)  # 判断请求输入的参数名是否与定义的一致
 
     def prediction_input_converter(self) -> None:
         # 根据post输入类型，做相应的转换
         for iter, (keys, values) in enumerate(self.prediction_inputs.items()):
+            # 对于输入的类型为image的情况
+            if self.inputs[iter] == "image":
+                if isinstance(values, bytes):
+                    self.prediction_inputs[keys] = cv2.imdecode(np.frombuffer(values, np.uint8), cv2.IMREAD_UNCHANGED)
+                # 如果输入的是字符串，则作为图像路径处理
+                elif isinstance(values, str):
+                    self.prediction_inputs[keys] = cv2.imread(values, cv2.IMREAD_UNCHANGED)
+                else:
+                    raise TypeError("输入的类型与定义的image类型不一致")
+
             # 对于输入的类型为number的情况
-            if self.inputs[iter] == self.TYPES["number"]:
+            elif self.inputs[iter] == "number":
                 assert is_float(values), "输入的类型与定义的number类型不一致"
                 self.prediction_inputs[keys] = float(values)
-            # 对于输入的类型为image的情况
-            elif type(values) == self.TYPES["image"]:
-                self.prediction_inputs[keys] = cv2.imdecode(np.frombuffer(values, np.uint8), cv2.IMREAD_UNCHANGED)
             # 对于输入的类型为text的情况
-            elif type(values) == self.TYPES["text"]:
+            elif self.inputs[iter] == "text":
+                assert isinstance(values, str), "输入的类型与定义的text类型不一致"
                 self.prediction_inputs[keys] = values
+            # 对于输入的类型为list的情况
+            elif self.inputs[iter] == "list":
+                self.prediction_inputs[keys] = is_list(values)
+            # 对于输入的类型为dict的情况
+            elif self.inputs[iter] == self.TYPES["dict"]:
+                self.prediction_inputs[keys] = is_dict(values)
             else:
-                assert isinstance(values, self.inputs[iter]), "输入的类型与定义的不一致"
+                raise TypeError("输入的类型与定义的不一致")
 
     def prediction_output_type_checker(self, result: Any) -> None:
         # 判断返回值类型是否为元组
         if isinstance(result, tuple):
             self.prediction_output_num_variables = len(result)
         elif result is None:
             self.prediction_output_num_variables = 0
@@ -116,14 +129,18 @@
                 assert isinstance(result, np.ndarray)
                 result = cv2.imencode(".jpg", result)[1].tostring()
                 result = base64.b64encode(result)
             elif self.outputs == ["text"]:
                 assert isinstance(result, str)
             elif self.outputs == ["number"]:
                 assert isinstance(result, (int, float))
+            elif self.outputs == ["dict"]:
+                assert isinstance(result, dict)
+            elif self.outputs == ["list"]:
+                assert isinstance(result, list)
             result_json = {"content": result}
         # 如果输出的变量数量>=2
         elif self.prediction_output_num_variables >= 2:
             result = list(result)
             result_json = {}
             for iter, output in enumerate(self.outputs):
                 if output == "image":
@@ -132,11 +149,17 @@
                     result_json[iter] = {"content": base64.b64encode(result[iter])}
                 elif output == "text":
                     assert isinstance(result[iter], str)
                     result_json[iter] = {"content": result[iter]}
                 elif output == "number":
                     assert isinstance(result[iter], (int, float))
                     result_json[iter] = {"content": result[iter]}
+                elif self.outputs == ["dict"]:
+                    assert isinstance(result, dict)
+                    result_json[iter] = {"content": result[iter]}
+                elif self.outputs == ["list"]:
+                    assert isinstance(result, list)
+                    result_json[iter] = {"content": result[iter]}
         else:
             result_json = {"content": None}
 
         return result_json
```

## swanapi/server.py

```diff
@@ -1,29 +1,26 @@
 from flask import Flask, request
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 from .utils import bytes_encoder
 from .base_inference import BaseInference
 import json
 
-app = Flask("app")
+app = Flask("SwanAPI Server")
 
 
 class SwanInference(BaseInference):
     def __init__(self):
         super().__init__()
 
     def inference(self,
-                   fn: Callable,
-                   inputs: Union[list, str, None] = None,
-                   outputs: Union[list, str, None] = None,
-                   description: str = None
-                   ) -> None:
-        """
-        输入推理函数、输入类型、输出类型，设定推理模式
-        """
+                  fn: Callable,
+                  inputs: Union[list[str], str, None],
+                  outputs: Union[list[str], str, None],
+                  description: str
+                  ) -> None:
         self.fn = fn
         self.inputs = inputs
         self.outputs = outputs
 
         # 检查fn、inputs和outputs的类型是否符合规范
         self.inference_type_checker()
         # 得到fn的形参名称
```

## swanapi/utils.py

```diff
@@ -20,7 +20,26 @@
     判断是否为浮点数
     """
     try:
         float(value)
         return True
     except ValueError:
         return False
+
+
+def is_list(value):
+    """
+    判断是否为列表，并返回转为后的字典
+    """
+    list_obj = eval(value)
+    assert isinstance(list_obj, list), "输入的类型与定义的list类型不一致"
+    return list_obj
+
+
+def is_dict(value):
+    """
+    判断是否为字典，并返回转为后的字典
+    """
+    dict_obj = eval(value)
+    print(dict_obj, type(dict_obj))
+    assert isinstance(dict_obj, dict), "输入的类型与定义的dict类型不一致"
+    return dict_obj
```

## swanapi/docker_builder/runner.py

```diff
@@ -1,151 +1,44 @@
-"""
-将用户定义的swan.yaml转换为Dockerfile
-"""
-import yaml
+import os
 import subprocess
+from config import SwanYaml
+from generate_dockerfile import DockerfileBuild
 
 
 class Runner:
+    """
+    SwanAPI深度学习镜像构建的入口类
+    """
     def __init__(self, config_filename: str):
-        self.config = SwanConfig(config_filename)
+        self.config = SwanYaml(config_filename)
         self.dockerfile = DockerfileBuild(self.config).get_dockerfile()
 
-    def build(self, image_name: str):
+    def build(self, image_name: str, running=False, save=False) -> None:
+        """
+        构建镜像并运行服务。
+        :param image_name: 构建的镜像Tag名
+        :param running: 构建完成后是否运行容器
+        :param save: 构建完成后是否保留Dockerfile
+        """
         print("--> Building Docker Image...")
-        # print(self.dockerfile)
+
+        # 将生成的Dockerfile写入当前目录
         with open("Dockerfile", "w") as f:
             f.write(self.dockerfile)
-        # 构建镜像
+
+        # 命令：镜像构建
         cmd = ["docker", "build", "-t", "{}".format(image_name), "."]
         subprocess.run(cmd)
-        # subprocess.run(cmd, input=self.dockerfile, text=True)
-        # 运行容器，获得FastAPI的localhost链接
-        subprocess.run(["docker", "run", "-p", f"{self.config.predict_port}:{self.config.predict_port}",
-                        "{}".format(image_name)])
-        print("--> Building Docker Finish.")
-
 
-class SwanConfig:
-    def __init__(self, filename):
-        self.config = self.yaml2dict(filename)
-
-        #  build部分
-        self.config_buid = self.config["build"]
-        # 获取build中的信息
-        self.gpu = self.bool_typecheck(self.config_buid["gpu"])
-        if "system_packages" in self.config_buid:
-            self.system_packages = self.config_buid["system_packages"]
-        else:
-            self.system_packages = None
-
-        self.python_version = self.config_buid["python_version"]
-        self.python_packages = self.config_buid["python_packages"]
-
-        if "python_sourece" in self.config_buid:
-            self.python_sourece = self.config_buid["python_sourece"]
-        else:
-            self.python_sourece = None
-
-        # 获得predict重的信息
-        self.config_predict = self.config["predict"]
-        # self.cli = self.config_predict["cli"]
-        self.cli = "predict.py"
-        self.predict_host = "0.0.0.0"
-        self.predict_port = self.config_predict["port"]
-
-    def bool_typecheck(self, input):
-        # 如果yaml中的gpu项不为bool值，则报错
-        if isinstance(input, bool):
-            return input
-        else:
-            raise TypeError("[Error] 'gpu' in swan.yaml is not bool")
+        # 如果不保存，在本地目录删除Dockerfile文件
+        if not save:
+            os.remove("Dockerfile")
 
-    def yaml2dict(self, filename: str):
-        """
-        Read the YAML file to dict.
-        :param filename: yaml file path
-        :return: dict
-        """
-        with open(filename, 'r') as file:
-            data = yaml.load(file, Loader=yaml.FullLoader)
-        return data
-
-
-class DockerfileBuild:
-    def __init__(self, configs: SwanConfig):
-        self.config = configs
-        self.python_prepackage = ["swanapi"]
-
-    def get_dockerfile(self):
-        # 根据build中的信息，构建一个Dockerfile
-        dockerfile_text = """"""
-        dockerfile_text += self.get_FORM()
-        prefile_apt, prefile_python = self.get_prefile()
-        dockerfile_text += prefile_apt
-        dockerfile_text += prefile_python
-        dockerfile_text += self.get_apt_packages()
-        dockerfile_text += self.get_python_packages(self.python_prepackage)
-        dockerfile_text += self.get_clean()
-        dockerfile_text += self.get_runtime()
-        return dockerfile_text
-
-    def get_FORM(self):
-        if self.config.python_version == "3.10":
-            return "FROM ubuntu:22.04\n"
-        else:
-            return "FROM ubuntu:20.04\n"
-
-    def get_prefile(self):
-        prefile_apt = """
-RUN apt-get clean  && \ 
-    apt-get update
-"""
-        prefile_python = """
-RUN apt-get install -y python3 curl && \ 
-    curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py  && \ 
-    python3 get-pip.py && \ 
-    pip3 install -U pip
-"""
-        return prefile_apt, prefile_python
-
-    def get_apt_packages(self):
-        if self.config.system_packages is None:
-            return ""
-        else:
-            apt_packages = ""
-            for package in self.config.system_packages:
-                apt_packages += package + " "
-            return """
-RUN apt-get install -y --no-install-recommends {}
-    """.format(apt_packages)
-
-    def get_python_packages(self, prepackages):
-        pip_packages = ""
-        for prepackage in prepackages:
-            pip_packages += prepackage + " "
-        for package in self.config.python_packages:
-            pip_packages += package + " "
-
-        if self.config.python_sourece == "cn":
-            pip_packages += " -i " + "https://pypi.tuna.tsinghua.edu.cn/simple"
-
-        return """
-RUN pip3 install --no-cache-dir {}
-""".format(pip_packages)
-
-    def get_clean(self):
-        return """
-RUN echo "==> Clean up..."  && \ 
-    rm -rf ~/.cache/pip
-    """
+        print("--> Building Docker Finish.")
+        # 命令：如果running is True, 容器运行, 开启API服务与端口映射
+        if running:
+            subprocess.run(["docker", "run", "-p", f"{self.config.predict_port}:{self.config.predict_port}",
+                            "{}".format(image_name)])
 
-    def get_runtime(self):
-        return """
-COPY . /app
 
-WORKDIR /app
 
-CMD [\"python3\", \"{}\"]""".format(self.config.cli)
 
-# CMD [\"python\", \"{}\", \"--host\", \"{}\",  \"--port\", \"{}\"]""".format(
-#             self.config.cli, self.config.predict_host, self.config.predict_port)
```

## Comparing `swanapi-0.1.3.dist-info/RECORD` & `swanapi-0.1.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 swanapi/__init__.py,sha256=T69A5YM84uwabbMeLbIZuDpk6R7ZcA51IrNFJOfRyq8,62
-swanapi/base_inference.py,sha256=Wp2jIC2SeAgS5TDjj0u1QG8S_ZKlOYi81LryF1PdltU,6378
+swanapi/base_inference.py,sha256=rx-hZRfL4fK91zkqt2O134gZS7_hmG893gWUWXGatkE,7611
 swanapi/make_build.py,sha256=eetDgQdCyQzsCVCniHPTee29bo0j4rfENxsVQMzeSys,833
-swanapi/server.py,sha256=ewk3Wt3GMOXJLNzAi_6C86LoDgiqWlZP9TPr8T5IdPA,1897
-swanapi/utils.py,sha256=YlXVC6k_5yeZ1EuUR-LpF5DOEpcLG00Uks4LEYPLwRo,572
+swanapi/server.py,sha256=8hQCa2OX3-1_9l4U8vmMlv4aKKOn3z1YB0nNkhNc93s,1790
+swanapi/utils.py,sha256=VE09kmCHcSnPzCgCRdumEu5vnKjMwFAzWl29FoU6vs0,1065
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swanapi/docker_builder/runner.py,sha256=uknif9LNfCgAnVgb_kNpTvk_GMu4wdkkYV6jK0vG1Lc,4869
-swanapi-0.1.3.dist-info/METADATA,sha256=VUMI8xncyU-usn-rfwa0d097nXknnV_K02-ZLljsk-E,347
-swanapi-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.1.3.dist-info/entry_points.txt,sha256=fgN0mUcvpscd5X6ZbWlK1FYJPU2l89EDR5qkKLNg1b4,53
-swanapi-0.1.3.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.1.3.dist-info/RECORD,,
+swanapi/docker_builder/config.py,sha256=LTC8azLLmMQQ5SPR8C37Gyzvs2VbI0FZosTVEBqO_HY,3656
+swanapi/docker_builder/generate_dockerfile.py,sha256=4teTBd0Hun_WbHS7UAB-AEHsHI6B51fTe6_ZWWaHung,2309
+swanapi/docker_builder/runner.py,sha256=TTY153DnEGedGu5h1iLSCpKeJARcZSy41GyN-1grwN8,1406
+swanapi-0.1.4.dist-info/METADATA,sha256=JqzrUmw1OZMQPa5vvSvvNKexC_fjQM-ms2BjciVE7sA,347
+swanapi-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.1.4.dist-info/entry_points.txt,sha256=fgN0mUcvpscd5X6ZbWlK1FYJPU2l89EDR5qkKLNg1b4,53
+swanapi-0.1.4.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.1.4.dist-info/RECORD,,
```

