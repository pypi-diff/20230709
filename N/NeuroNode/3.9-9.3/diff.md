# Comparing `tmp/NeuroNode-3.9.tar.gz` & `tmp/NeuroNode-9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroNode-3.9.tar", last modified: Sat Jul  8 13:51:28 2023, max compression
+gzip compressed data, was "NeuroNode-9.3.tar", last modified: Sun Jul  9 02:52:58 2023, max compression
```

## Comparing `NeuroNode-3.9.tar` & `NeuroNode-9.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.637231 NeuroNode-3.9/
--rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NeuroNode-3.9/LICENSE.text
--rw-rw-rw-   0        0        0      748 2023-07-08 13:51:28.630128 NeuroNode-3.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NeuroNode-3.9/README.md
--rw-rw-rw-   0        0        0      877 2023-07-08 13:38:30.000000 NeuroNode-3.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 13:51:28.637231 NeuroNode-3.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.578534 NeuroNode-3.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.622682 NeuroNode-3.9/src/NeuroNode.egg-info/
--rw-rw-rw-   0        0        0      748 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.630128 NeuroNode-3.9/src/neuronode/
--rw-rw-rw-   0        0        0        0 2023-02-05 09:46:02.000000 NeuroNode-3.9/src/neuronode/Debug.py
--rw-rw-rw-   0        0        0     7201 2023-07-08 13:50:44.000000 NeuroNode-3.9/src/neuronode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 02:52:58.642941 NeuroNode-9.3/
+-rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NeuroNode-9.3/LICENSE.text
+-rw-rw-rw-   0        0        0      748 2023-07-09 02:52:58.642941 NeuroNode-9.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NeuroNode-9.3/README.md
+-rw-rw-rw-   0        0        0      877 2023-07-09 02:52:01.000000 NeuroNode-9.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 02:52:58.642941 NeuroNode-9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 02:52:58.596063 NeuroNode-9.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 02:52:58.627315 NeuroNode-9.3/src/NeuroNode.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-07-09 02:52:58.000000 NeuroNode-9.3/src/NeuroNode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-09 02:52:58.000000 NeuroNode-9.3/src/NeuroNode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 02:52:58.000000 NeuroNode-9.3/src/NeuroNode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-09 02:52:58.000000 NeuroNode-9.3/src/NeuroNode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 02:52:58.642941 NeuroNode-9.3/src/neuronode/
+-rw-rw-rw-   0        0        0        0 2023-07-09 02:42:34.000000 NeuroNode-9.3/src/neuronode/Debug.py
+-rw-rw-rw-   0        0        0     7388 2023-07-09 02:51:01.000000 NeuroNode-9.3/src/neuronode/__init__.py
```

### Comparing `NeuroNode-3.9/LICENSE.text` & `NeuroNode-9.3/LICENSE.text`

 * *Files identical despite different names*

### Comparing `NeuroNode-3.9/PKG-INFO` & `NeuroNode-9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroNode
-Version: 3.9
+Version: 9.3
 Summary: The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <jaysinghdulrasar@gmail.com>
 Project-URL: WebApp, https://neuro-node.web.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NeuroNode-3.9/pyproject.toml` & `NeuroNode-9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeuroNode"
-version = "3.9"
+version = "9.3"
 authors = [
   { name="Jay Singh", email="jaysinghdulrasar@gmail.com" },
 ]
 description = '''The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 WebSite : https://neuro-node.web.app'''
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `NeuroNode-3.9/src/NeuroNode.egg-info/PKG-INFO` & `NeuroNode-9.3/src/NeuroNode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroNode
-Version: 3.9
+Version: 9.3
 Summary: The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <jaysinghdulrasar@gmail.com>
 Project-URL: WebApp, https://neuro-node.web.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NeuroNode-3.9/src/neuronode/__init__.py` & `NeuroNode-9.3/src/neuronode/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import numpy as np
 import pickle
 import time
 import requests
 import shutil
 import torch
 os.system("pip install scenedetect")
-from scenedetect import detect, ContentDetector, split_video_ffmpeg
 os.system("pip install mega.py")
-import mega
+os.system("pip install timm")
+from scenedetect import detect, ContentDetector, split_video_ffmpeg
+from mega import Mega
 
 class DataOptimizer():
 
     def __init__(self, directory):
         self.directory = directory
 
     def DownloadData(self, urls):
@@ -113,15 +114,15 @@
                     print(i)
 
                     i += 1
 
         return np.array(Conv3D).T
 
 
-class NextFrameGenerator:
+class NextFrameGenerator():
     def __init__(self):
         pass
 
     def Train(self, X, Y, num_iterations=1000, learning_rate=0.01):
         W1 = np.random.randn(40000, 16) * 0.01
         b1 = np.zeros((40000, 1))
         W2 = np.random.randn(1000, 40000) * 0.01
@@ -177,35 +178,39 @@
             print(i, " iteration finished at - ", time.strftime("%H:%M:%S"))
 
         file = open("Discriminator.bin", 'wb')
         pickle.dump(parameters, file)
 
         return parameters
 
+def Sync(urls, device_id):
 
-device_id="1"
-DataOptimizer=DataOptimizer(os.getcwd())
-DataOptimizer.DownloadData(urls=["https://checker.in/go/13987"])
-Train_X,FirstFrames=DataOptimizer.PrepareData()
-Conv3D=Convection3D().Generate()
-
-file=open(".\\"+device_id+"Train_X.bin",'wb')
-pickle.dump(Train_X,file)
-file.close()
-file=open(".\\"+device_id+"FirstFrames.bin",'wb')
-pickle.dump(FirstFrames,file)
-file.close()
-file=open(".\\"+device_id+"Conv3D.bin",'wb')
-pickle.dump(Conv3D,file)
-file.close()
-print("done")
-mega=Mega()
-log=mega.login("neuronode.bin@gmail.com","getAccessAtNeuroNodeDataStorage")
-log.upload("Train_X.bin")
-log.upload("FirstFrames.bin")
-log.upload("Conv3D.bin")
+    global DataOptimizer
+    global Convection3D
+    global NextFrameGenerator
+
+    Data_Optimizer=DataOptimizer(os.getcwd())
+    Data_Optimizer.DownloadData(urls)
+    Train_X,FirstFrames=Data_Optimizer.PrepareData()
+    Conv3D=Convection3D().Generate()
+
+    file=open(".\\"+device_id+"Train_X.bin",'wb')
+    pickle.dump(Train_X,file)
+    file.close()
+    file=open(".\\"+device_id+"FirstFrames.bin",'wb')
+    pickle.dump(FirstFrames,file)
+    file.close()
+    file=open(".\\"+device_id+"Conv3D.bin",'wb')
+    pickle.dump(Conv3D,file)
+    file.close()
+    print("done")
+    mega=Mega()
+    log=mega.login("neuronode.bin@gmail.com","getAccessAtNeuroNodeDataStorage")
+    log.upload("Train_X.bin")
+    log.upload("FirstFrames.bin")
+    log.upload("Conv3D.bin")
 
     # Generator = NextFrameGenerator()
     # Train_D = np.random.randint(0, 255, (241, 10000))
     # Train_D_Y = np.random.randint(0, 1, (240, 10000))
     # print("data loaded...")
     # NextFrameGenerator.Train(Train_D, Train_D_Y)
```

