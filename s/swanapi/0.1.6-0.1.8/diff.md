# Comparing `tmp/swanapi-0.1.6-py3-none-any.whl.zip` & `tmp/swanapi-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9123 bytes, number of entries: 14
+Zip file size: 9341 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       62 b- defN 23-Jul-08 12:12 swanapi/__init__.py
 -rw-r--r--  2.0 unx     7611 b- defN 23-Jul-09 11:38 swanapi/base_inference.py
--rw-r--r--  2.0 unx      754 b- defN 23-Jul-09 13:31 swanapi/make_build.py
+-rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
 -rw-r--r--  2.0 unx     1850 b- defN 23-Jul-09 16:44 swanapi/server.py
 -rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 07:52 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
--rw-r--r--  2.0 unx     3897 b- defN 23-Jul-09 17:16 swanapi/docker_builder/config.py
--rw-r--r--  2.0 unx     2623 b- defN 23-Jul-09 17:11 swanapi/docker_builder/generate_dockerfile.py
--rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 13:22 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 17:18 swanapi-0.1.6.dist-info/RECORD
-14 files, 20917 bytes uncompressed, 7219 bytes compressed:  65.5%
+-rw-r--r--  2.0 unx     3889 b- defN 23-Jul-09 18:35 swanapi/docker_builder/config.py
+-rw-r--r--  2.0 unx     3338 b- defN 23-Jul-09 18:35 swanapi/docker_builder/generate_dockerfile.py
+-rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 18:39 swanapi/docker_builder/runner.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-09 18:39 swanapi-0.1.8.dist-info/RECORD
+14 files, 21733 bytes uncompressed, 7437 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.6.dist-info/METADATA
+Filename: swanapi-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.6.dist-info/WHEEL
+Filename: swanapi-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.6.dist-info/entry_points.txt
+Filename: swanapi-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.6.dist-info/top_level.txt
+Filename: swanapi-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.6.dist-info/RECORD
+Filename: swanapi-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/make_build.py

```diff
@@ -6,21 +6,22 @@
     try:
         _ = args.build
     except ValueError:
         raise ValueError("You need to 'build' parameters liked 'swanapi build -t image_name'")
     else:
         runner = Runner()
         if args.run:
-            runner.build(image_name=args.tag, running=True)
+            runner.build(image_name=args.tag, running=True, save=args.save)
         else:
-            runner.build(image_name=args.tag, running=False)
+            runner.build(image_name=args.tag, running=False, save=False)
 
 
 parser = argparse.ArgumentParser(description='Welcome to SwanAPI Help')
 parser.add_argument('build', help='build docker image')
 parser.add_argument('-r', '--run', action="store_true", help='run docker image')
 parser.add_argument('-t', '--tag', help='docker image tag')
+parser.add_argument('-s', '--save', action="store_true", help='save Dockerfile')
 
 args = parser.parse_args()
 
 if __name__ == "__main__":
     build()
```

## swanapi/docker_builder/config.py

```diff
@@ -83,25 +83,25 @@
     def build_python_packages_typecheck(self) -> None:
         if 'python_packages' in self.config_buid:
             value = self.config_buid["python_packages"]
             if not isinstance(value, list):
                 raise TypeError("[Error] 'python_packages' in swan.yaml is not list")
             self.python_packages = value
         else:
-            self.python_packages = None
+            self.python_packages = []
 
     def build_python_sourece_typecheck(self) -> None:
         PYTHON_SOURCE_LIST = ["cn", "us"]
         PYTHON_SOURCE_DEFAULT = 'us'
-        if 'python_sourece' in self.config_buid:
-            self.python_sourece = self.config_buid["python_sourece"]
-            if self.python_sourece not in PYTHON_SOURCE_LIST:
-                raise ValueError("[Error] 'python_sourece' in swan.yaml is not in {}".format(PYTHON_SOURCE_LIST))
+        if 'python_source' in self.config_buid:
+            self.python_source = self.config_buid["python_source"]
+            if self.python_source not in PYTHON_SOURCE_LIST:
+                raise ValueError("[Error] 'python_source' in swan.yaml is not in {}".format(PYTHON_SOURCE_LIST))
         else:
-            self.python_sourece = PYTHON_SOURCE_DEFAULT
+            self.python_source = PYTHON_SOURCE_DEFAULT
 
     def predict_port_typecheck(self) -> None:
         if 'port' in self.config_predict:
             if not isinstance(self.config_predict["port"], int):
                 raise TypeError("[Error] 'port' in swan.yaml is not int")
             self.predict_port = self.config_predict["port"]
         else:
```

## swanapi/docker_builder/generate_dockerfile.py

```diff
@@ -18,15 +18,15 @@
 
     def get_FORM(self):
         if self.config.python_version == "3.10":
             return "FROM ubuntu:22.04\n"
         elif self.config.python_version == "3.8" or self.config.python_version == "3.9":
             return "FROM ubuntu:20.04\n"
         else:
-            raise TypeError("[Error] The current version of swanapi only supports 3.10")
+            raise TypeError("[Error] The current version of swanapi only supports [3.8, 3.9, 3.10]")
 
     def get_preoperation(self):
         apt_preoperation = """
 RUN apt-get clean  && \ 
     apt-get update
 """
         if self.config.python_version == "3.10":
@@ -34,44 +34,58 @@
 RUN apt-get install -y python3 curl && \ 
     curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py  && \ 
     python3 get-pip.py && \ 
     pip3 install -U pip
 """
         else:
             python_packages_preoperation = f"""
-RUN apt-get update && \
+RUN apt-get update && \  
     apt-get install -y python{self.config.python_version} python3-pip
-            """
+"""
+
+        # 如果是国内源，需要设置pip清华源
+        if self.config.python_source == "cn":
+            python_packages_preoperation += """
+RUN pip3 config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
+"""
 
         return apt_preoperation + python_packages_preoperation
 
     def get_apt_packages(self):
         if self.config.system_packages is not None:
             apt_packages = ""
             for package in self.config.system_packages:
                 apt_packages += package + " "
             return """
 RUN apt-get install -y --no-install-recommends {}
-    """.format(apt_packages)
+""".format(apt_packages)
         else:
-            """"""
+            return ""
 
     def get_python_packages(self, prepackages):
-        pip_packages = ""
-        for prepackage in prepackages:
-            pip_packages += prepackage + " "
-        for package in self.config.python_packages:
-            pip_packages += package + " "
+        prepackages_text = ""
+        package_text = ""
 
-        if self.config.python_sourece == "cn":
-            pip_packages += " -i " + "https://pypi.tuna.tsinghua.edu.cn/simple"
+        if len(prepackages) == 0 and len(self.config.python_packages) == 0:
+            return ""
+        if len(prepackages) != 0:
+            for prepackage in prepackages:
+                prepackages_text += " pip3 install --no-cache-dir {} ".format(prepackage)
+                if prepackage != prepackages[-1]:
+                    prepackages_text += "&& \ \n   "
+            prepackages_text = "RUN" + prepackages_text
+
+        if len(self.config.python_packages) != 0:
+            for package in self.config.python_packages:
+                package_text += " pip3 install --no-cache-dir {} ".format(package)
+                if package != self.config.python_packages[-1]:
+                    package_text += "&& \ \n   "
+            package_text = "RUN" + package_text
 
-        return """
-RUN pip3 install --no-cache-dir {}
-""".format(pip_packages)
+        return prepackages_text + "\n" + package_text + "\n"
 
     def get_clean(self):
         return """
 RUN echo "==> Clean up..."  && \ 
     rm -rf ~/.cache/pip
     """
```

## Comparing `swanapi-0.1.6.dist-info/RECORD` & `swanapi-0.1.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swanapi/__init__.py,sha256=T69A5YM84uwabbMeLbIZuDpk6R7ZcA51IrNFJOfRyq8,62
 swanapi/base_inference.py,sha256=rx-hZRfL4fK91zkqt2O134gZS7_hmG893gWUWXGatkE,7611
-swanapi/make_build.py,sha256=SX9eOGmQM0Lt7PiMj3ygMZtRyIIwlU2kqBdn12UHyaQ,754
+swanapi/make_build.py,sha256=P4WsA52pftJyNLrU986UKkYPY88VLzRMgQJ6s_UUTY0,863
 swanapi/server.py,sha256=VYblGUvpBEYKb4NN5cXWFvybXqU5o9qsMNpdf01bp2o,1850
 swanapi/utils.py,sha256=VE09kmCHcSnPzCgCRdumEu5vnKjMwFAzWl29FoU6vs0,1065
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swanapi/docker_builder/config.py,sha256=w7PWbyYX7UNdmGYFmGZA-HB-ml_yb12WTvAvfMdk0I0,3897
-swanapi/docker_builder/generate_dockerfile.py,sha256=QiqCd0qGdwaUG7Ye4nxKJ_1gbGx6vrENYPg6HjDh0VM,2623
+swanapi/docker_builder/config.py,sha256=CspWGMAyxZz_rd2JecCrsC4nL75Zh3o7XGAXMVHa32o,3889
+swanapi/docker_builder/generate_dockerfile.py,sha256=o9WDfAlemjxP17gy0inWU1mF3HJG05PQtsyOeEzk51c,3338
 swanapi/docker_builder/runner.py,sha256=uDToZ5UfgshahcnKbu8Eb7enLLry2pVHn7e2bJB56vk,1419
-swanapi-0.1.6.dist-info/METADATA,sha256=sD5WMMglD2xJC7gwLH-Fb5T6wKrRRmGQu3uI0ok2n-E,347
-swanapi-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.1.6.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.1.6.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.1.6.dist-info/RECORD,,
+swanapi-0.1.8.dist-info/METADATA,sha256=xATSodZjDMUR8t23ytcvzDbrLbOD5l_lRYyZr9VapRA,347
+swanapi-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.1.8.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.1.8.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.1.8.dist-info/RECORD,,
```

