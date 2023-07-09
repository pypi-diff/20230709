# Comparing `tmp/swanapi-0.1.5-py3-none-any.whl.zip` & `tmp/swanapi-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9008 bytes, number of entries: 14
+Zip file size: 9123 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       62 b- defN 23-Jul-08 12:12 swanapi/__init__.py
 -rw-r--r--  2.0 unx     7611 b- defN 23-Jul-09 11:38 swanapi/base_inference.py
 -rw-r--r--  2.0 unx      754 b- defN 23-Jul-09 13:31 swanapi/make_build.py
--rw-r--r--  2.0 unx     1790 b- defN 23-Jul-09 11:44 swanapi/server.py
+-rw-r--r--  2.0 unx     1850 b- defN 23-Jul-09 16:44 swanapi/server.py
 -rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 07:52 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
--rw-r--r--  2.0 unx     3668 b- defN 23-Jul-09 12:55 swanapi/docker_builder/config.py
--rw-r--r--  2.0 unx     2310 b- defN 23-Jul-09 12:50 swanapi/docker_builder/generate_dockerfile.py
+-rw-r--r--  2.0 unx     3897 b- defN 23-Jul-09 17:16 swanapi/docker_builder/config.py
+-rw-r--r--  2.0 unx     2623 b- defN 23-Jul-09 17:11 swanapi/docker_builder/generate_dockerfile.py
 -rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 13:22 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 13:32 swanapi-0.1.5.dist-info/RECORD
-14 files, 20318 bytes uncompressed, 7104 bytes compressed:  65.0%
+-rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/RECORD
+14 files, 20917 bytes uncompressed, 7219 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.5.dist-info/METADATA
+Filename: swanapi-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.5.dist-info/WHEEL
+Filename: swanapi-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.5.dist-info/entry_points.txt
+Filename: swanapi-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.5.dist-info/top_level.txt
+Filename: swanapi-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.5.dist-info/RECORD
+Filename: swanapi-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/server.py

```diff
@@ -9,21 +9,22 @@
 
 class SwanInference(BaseInference):
     def __init__(self):
         super().__init__()
 
     def inference(self,
                   fn: Callable,
-                  inputs: Union[list[str], str, None],
-                  outputs: Union[list[str], str, None],
-                  description: str
+                  inputs: Union[list[str], str, None] = None,
+                  outputs: Union[list[str], str, None] = None,
+                  description: str = None
                   ) -> None:
         self.fn = fn
         self.inputs = inputs
         self.outputs = outputs
+        self.description = description
 
         # 检查fn、inputs和outputs的类型是否符合规范
         self.inference_type_checker()
         # 得到fn的形参名称
         self.get_fn_information()
 
     def prediction(self, **inputs):
```

## swanapi/docker_builder/config.py

```diff
@@ -68,15 +68,18 @@
     def build_system_packages_typecheck(self) -> None:
         if 'system_packages' in self.config_buid:
             self.system_packages = self.config_buid["system_packages"]
         else:
             self.system_packages = None
 
     def build_python_version_typecheck(self) -> None:
+        PYTHON_VERSION_LIST = ["3.8", "3.9", "3.10"]
         if 'python_version' in self.config_buid:
+            assert self.config_buid["python_version"] in PYTHON_VERSION_LIST,\
+                "[Error] 'python_version' in swan.yaml is not in {}".format(PYTHON_VERSION_LIST)
             self.python_version = self.config_buid["python_version"]
         else:
             self.python_version = "3.10"
 
     def build_python_packages_typecheck(self) -> None:
         if 'python_packages' in self.config_buid:
             value = self.config_buid["python_packages"]
```

## swanapi/docker_builder/generate_dockerfile.py

```diff
@@ -15,29 +15,37 @@
         dockerfile_text += self.get_clean()
         dockerfile_text += self.get_runtime()
         return dockerfile_text
 
     def get_FORM(self):
         if self.config.python_version == "3.10":
             return "FROM ubuntu:22.04\n"
+        elif self.config.python_version == "3.8" or self.config.python_version == "3.9":
+            return "FROM ubuntu:20.04\n"
         else:
-            # return "FROM ubuntu:20.04\n"
             raise TypeError("[Error] The current version of swanapi only supports 3.10")
 
     def get_preoperation(self):
         apt_preoperation = """
 RUN apt-get clean  && \ 
     apt-get update
 """
-        python_packages_preoperation = """
+        if self.config.python_version == "3.10":
+            python_packages_preoperation = """
 RUN apt-get install -y python3 curl && \ 
     curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py  && \ 
     python3 get-pip.py && \ 
     pip3 install -U pip
 """
+        else:
+            python_packages_preoperation = f"""
+RUN apt-get update && \
+    apt-get install -y python{self.config.python_version} python3-pip
+            """
+
         return apt_preoperation + python_packages_preoperation
 
     def get_apt_packages(self):
         if self.config.system_packages is not None:
             apt_packages = ""
             for package in self.config.system_packages:
                 apt_packages += package + " "
```

