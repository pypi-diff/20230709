# Comparing `tmp/swanapi-0.1.4-py3-none-any.whl.zip` & `tmp/swanapi-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9011 bytes, number of entries: 14
+Zip file size: 9008 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       62 b- defN 23-Jul-08 12:12 swanapi/__init__.py
 -rw-r--r--  2.0 unx     7611 b- defN 23-Jul-09 11:38 swanapi/base_inference.py
--rw-r--r--  2.0 unx      833 b- defN 23-Jul-08 11:33 swanapi/make_build.py
+-rw-r--r--  2.0 unx      754 b- defN 23-Jul-09 13:31 swanapi/make_build.py
 -rw-r--r--  2.0 unx     1790 b- defN 23-Jul-09 11:44 swanapi/server.py
 -rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 07:52 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
--rw-r--r--  2.0 unx     3656 b- defN 23-Jul-09 12:44 swanapi/docker_builder/config.py
--rw-r--r--  2.0 unx     2309 b- defN 23-Jul-09 12:44 swanapi/docker_builder/generate_dockerfile.py
--rw-r--r--  2.0 unx     1406 b- defN 23-Jul-09 12:44 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 12:45 swanapi-0.1.4.dist-info/RECORD
-14 files, 20371 bytes uncompressed, 7107 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx     3668 b- defN 23-Jul-09 12:55 swanapi/docker_builder/config.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-Jul-09 12:50 swanapi/docker_builder/generate_dockerfile.py
+-rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 13:22 swanapi/docker_builder/runner.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/RECORD
+14 files, 20318 bytes uncompressed, 7104 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.4.dist-info/METADATA
+Filename: swanapi-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.4.dist-info/WHEEL
+Filename: swanapi-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.4.dist-info/entry_points.txt
+Filename: swanapi-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.4.dist-info/top_level.txt
+Filename: swanapi-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.4.dist-info/RECORD
+Filename: swanapi-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/make_build.py

```diff
@@ -1,27 +1,26 @@
 from .docker_builder.runner import Runner
 import argparse
 
 
 def build():
-    if args.build:
-        if args.config:
-            runner = Runner(config_filename=args.config)
-        else:
-            raise ValueError("config[-c] value is empty")
-        if args.tag:
-            runner.build(image_name=args.tag)
-        else:
-            raise ValueError("tag[-t] value is empty")
-    else:
+    try:
+        _ = args.build
+    except ValueError:
         raise ValueError("You need to 'build' parameters liked 'swanapi build -t image_name'")
+    else:
+        runner = Runner()
+        if args.run:
+            runner.build(image_name=args.tag, running=True)
+        else:
+            runner.build(image_name=args.tag, running=False)
 
 
 parser = argparse.ArgumentParser(description='Welcome to SwanAPI Help')
 parser.add_argument('build', help='build docker image')
-parser.add_argument('-c', '--config', default="swan.yaml", help='filepath of swan.yaml')
+parser.add_argument('-r', '--run', action="store_true", help='run docker image')
 parser.add_argument('-t', '--tag', help='docker image tag')
 
 args = parser.parse_args()
 
 if __name__ == "__main__":
     build()
```

## swanapi/docker_builder/config.py

```diff
@@ -53,53 +53,53 @@
         self.predict_cli = "predict.py"
         self.predict_host = "0.0.0.0"
         self.predict_port_typecheck()
 
     def build_gpu_typecheck(self) -> None:
         GPU_LIST = ['false', 'true']
         GPU_DEFAULT = "false"
-        if self.config_buid["gpu"]:
+        if 'gpu' in self.config_buid:
             if str(self.config_buid["gpu"]).lower() not in GPU_LIST:
                 raise TypeError("[Error] 'gpu' in swan.yaml is not bool")
             else:
                 self.gpu = self.config_buid["gpu"]
         else:
             self.gpu = GPU_DEFAULT
 
     def build_system_packages_typecheck(self) -> None:
-        if self.config_buid["system_packages"]:
+        if 'system_packages' in self.config_buid:
             self.system_packages = self.config_buid["system_packages"]
         else:
             self.system_packages = None
 
     def build_python_version_typecheck(self) -> None:
-        if self.config_buid["python_version"]:
+        if 'python_version' in self.config_buid:
             self.python_version = self.config_buid["python_version"]
         else:
             self.python_version = "3.10"
 
     def build_python_packages_typecheck(self) -> None:
-        if self.config_buid["python_packages"]:
+        if 'python_packages' in self.config_buid:
             value = self.config_buid["python_packages"]
             if not isinstance(value, list):
                 raise TypeError("[Error] 'python_packages' in swan.yaml is not list")
             self.python_packages = value
         else:
             self.python_packages = None
 
     def build_python_sourece_typecheck(self) -> None:
         PYTHON_SOURCE_LIST = ["cn", "us"]
         PYTHON_SOURCE_DEFAULT = 'us'
-        if self.config_buid["python_sourece"]:
+        if 'python_sourece' in self.config_buid:
             self.python_sourece = self.config_buid["python_sourece"]
             if self.python_sourece not in PYTHON_SOURCE_LIST:
                 raise ValueError("[Error] 'python_sourece' in swan.yaml is not in {}".format(PYTHON_SOURCE_LIST))
         else:
             self.python_sourece = PYTHON_SOURCE_DEFAULT
 
     def predict_port_typecheck(self) -> None:
-        if self.config_predict["port"]:
+        if 'port' in self.config_predict:
             if not isinstance(self.config_predict["port"], int):
                 raise TypeError("[Error] 'port' in swan.yaml is not int")
             self.predict_port = self.config_predict["port"]
         else:
             self.predict_port = 8000
```

## swanapi/docker_builder/generate_dockerfile.py

```diff
@@ -1,8 +1,8 @@
-from config import SwanYaml
+from .config import SwanYaml
 
 
 class DockerfileBuild:
     def __init__(self, configs: SwanYaml):
         self.config = configs
 
     def get_dockerfile(self):
```

## swanapi/docker_builder/runner.py

```diff
@@ -1,18 +1,19 @@
 import os
 import subprocess
-from config import SwanYaml
-from generate_dockerfile import DockerfileBuild
+from .config import SwanYaml
+from .generate_dockerfile import DockerfileBuild
 
 
 class Runner:
     """
     SwanAPI深度学习镜像构建的入口类
     """
-    def __init__(self, config_filename: str):
+
+    def __init__(self, config_filename: str = "swan.yaml"):
         self.config = SwanYaml(config_filename)
         self.dockerfile = DockerfileBuild(self.config).get_dockerfile()
 
     def build(self, image_name: str, running=False, save=False) -> None:
         """
         构建镜像并运行服务。
         :param image_name: 构建的镜像Tag名
@@ -34,11 +35,7 @@
             os.remove("Dockerfile")
 
         print("--> Building Docker Finish.")
         # 命令：如果running is True, 容器运行, 开启API服务与端口映射
         if running:
             subprocess.run(["docker", "run", "-p", f"{self.config.predict_port}:{self.config.predict_port}",
                             "{}".format(image_name)])
-
-
-
-
```

## Comparing `swanapi-0.1.4.dist-info/RECORD` & `swanapi-0.1.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swanapi/__init__.py,sha256=T69A5YM84uwabbMeLbIZuDpk6R7ZcA51IrNFJOfRyq8,62
 swanapi/base_inference.py,sha256=rx-hZRfL4fK91zkqt2O134gZS7_hmG893gWUWXGatkE,7611
-swanapi/make_build.py,sha256=eetDgQdCyQzsCVCniHPTee29bo0j4rfENxsVQMzeSys,833
+swanapi/make_build.py,sha256=SX9eOGmQM0Lt7PiMj3ygMZtRyIIwlU2kqBdn12UHyaQ,754
 swanapi/server.py,sha256=8hQCa2OX3-1_9l4U8vmMlv4aKKOn3z1YB0nNkhNc93s,1790
 swanapi/utils.py,sha256=VE09kmCHcSnPzCgCRdumEu5vnKjMwFAzWl29FoU6vs0,1065
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swanapi/docker_builder/config.py,sha256=LTC8azLLmMQQ5SPR8C37Gyzvs2VbI0FZosTVEBqO_HY,3656
-swanapi/docker_builder/generate_dockerfile.py,sha256=4teTBd0Hun_WbHS7UAB-AEHsHI6B51fTe6_ZWWaHung,2309
-swanapi/docker_builder/runner.py,sha256=TTY153DnEGedGu5h1iLSCpKeJARcZSy41GyN-1grwN8,1406
-swanapi-0.1.4.dist-info/METADATA,sha256=JqzrUmw1OZMQPa5vvSvvNKexC_fjQM-ms2BjciVE7sA,347
-swanapi-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.1.4.dist-info/entry_points.txt,sha256=fgN0mUcvpscd5X6ZbWlK1FYJPU2l89EDR5qkKLNg1b4,53
-swanapi-0.1.4.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.1.4.dist-info/RECORD,,
+swanapi/docker_builder/config.py,sha256=N1M3GtMFrmIsKrFQb2bj-Igp6wGW8wKwWczPNJ1xXzs,3668
+swanapi/docker_builder/generate_dockerfile.py,sha256=HZfA1AAnL2FtiSnGxzSysM1ryZ7LYLOgcD-lL1IW5J0,2310
+swanapi/docker_builder/runner.py,sha256=uDToZ5UfgshahcnKbu8Eb7enLLry2pVHn7e2bJB56vk,1419
+swanapi-0.1.5.dist-info/METADATA,sha256=8WzwSAO77YYL-sAfmWZuxwOgChy6Oded8lPNxeLaqPU,347
+swanapi-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.1.5.dist-info/entry_points.txt,sha256=fgN0mUcvpscd5X6ZbWlK1FYJPU2l89EDR5qkKLNg1b4,53
+swanapi-0.1.5.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.1.5.dist-info/RECORD,,
```

