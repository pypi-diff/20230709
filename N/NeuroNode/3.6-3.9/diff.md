# Comparing `tmp/NeuroNode-3.6.tar.gz` & `tmp/NeuroNode-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuroNode-3.6.tar", last modified: Sat Jul  8 13:30:46 2023, max compression
+gzip compressed data, was "NeuroNode-3.9.tar", last modified: Sat Jul  8 13:51:28 2023, max compression
```

## Comparing `NeuroNode-3.6.tar` & `NeuroNode-3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:30:46.920103 NeuroNode-3.6/
--rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NeuroNode-3.6/LICENSE.text
--rw-rw-rw-   0        0        0      748 2023-07-08 13:30:46.920103 NeuroNode-3.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NeuroNode-3.6/README.md
--rw-rw-rw-   0        0        0      877 2023-07-08 13:29:57.000000 NeuroNode-3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 13:30:46.920103 NeuroNode-3.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-08 13:30:46.841238 NeuroNode-3.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 13:30:46.904466 NeuroNode-3.6/src/NeuroNode.egg-info/
--rw-rw-rw-   0        0        0      748 2023-07-08 13:30:46.000000 NeuroNode-3.6/src/NeuroNode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-08 13:30:46.000000 NeuroNode-3.6/src/NeuroNode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:30:46.000000 NeuroNode-3.6/src/NeuroNode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-08 13:30:46.000000 NeuroNode-3.6/src/NeuroNode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-08 13:30:46.920103 NeuroNode-3.6/src/neuronode/
--rw-rw-rw-   0        0        0        0 2023-02-05 09:46:02.000000 NeuroNode-3.6/src/neuronode/Debug.py
--rw-rw-rw-   0        0        0     7798 2023-07-08 13:29:17.000000 NeuroNode-3.6/src/neuronode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.637231 NeuroNode-3.9/
+-rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NeuroNode-3.9/LICENSE.text
+-rw-rw-rw-   0        0        0      748 2023-07-08 13:51:28.630128 NeuroNode-3.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NeuroNode-3.9/README.md
+-rw-rw-rw-   0        0        0      877 2023-07-08 13:38:30.000000 NeuroNode-3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 13:51:28.637231 NeuroNode-3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.578534 NeuroNode-3.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.622682 NeuroNode-3.9/src/NeuroNode.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 13:51:28.000000 NeuroNode-3.9/src/NeuroNode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 13:51:28.630128 NeuroNode-3.9/src/neuronode/
+-rw-rw-rw-   0        0        0        0 2023-02-05 09:46:02.000000 NeuroNode-3.9/src/neuronode/Debug.py
+-rw-rw-rw-   0        0        0     7201 2023-07-08 13:50:44.000000 NeuroNode-3.9/src/neuronode/__init__.py
```

### Comparing `NeuroNode-3.6/LICENSE.text` & `NeuroNode-3.9/LICENSE.text`

 * *Files identical despite different names*

### Comparing `NeuroNode-3.6/PKG-INFO` & `NeuroNode-3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroNode
-Version: 3.6
+Version: 3.9
 Summary: The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <jaysinghdulrasar@gmail.com>
 Project-URL: WebApp, https://neuro-node.web.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NeuroNode-3.6/pyproject.toml` & `NeuroNode-3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeuroNode"
-version = "3.6"
+version = "3.9"
 authors = [
   { name="Jay Singh", email="jaysinghdulrasar@gmail.com" },
 ]
 description = '''The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 WebSite : https://neuro-node.web.app'''
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `NeuroNode-3.6/src/NeuroNode.egg-info/PKG-INFO` & `NeuroNode-3.9/src/NeuroNode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroNode
-Version: 3.6
+Version: 3.9
 Summary: The Neuro Node is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences. Utilizing a vast neural network comprising more than 1 trillion parameters, the Neuro Node has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <jaysinghdulrasar@gmail.com>
 Project-URL: WebApp, https://neuro-node.web.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `NeuroNode-3.6/src/neuronode/__init__.py` & `NeuroNode-3.9/src/neuronode/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,203 +7,205 @@
 import shutil
 import torch
 os.system("pip install scenedetect")
 from scenedetect import detect, ContentDetector, split_video_ffmpeg
 os.system("pip install mega.py")
 import mega
 
-def Sync(urls, device_id):
+class DataOptimizer():
 
-    class DataOptimizer():
-        def __init__(self, directory):
-            self.directory = directory
-
-        def DownloadData(self, urls):
-            for i, url in enumerate(urls):
-                r = requests.get(url, allow_redirects=True)
-                open('Video' + str(i + 1) + '.mp4', 'wb').write(r.content)
-
-        def PrepareData(self):
-            if os.path.exists(self.directory + "/Scenes"):
-                shutil.rmtree(self.directory + "/Scenes")
-            os.mkdir(self.directory + "/Scenes")
-
-            video_files = [f for f in os.listdir(self.directory) if
-                           f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(
-                               ".mov") or f.endswith(".webm")]
-
-            for video_file in video_files:
-                video_path = os.path.join(self.directory, video_file)
-                scene_list = detect(video_path, ContentDetector())
-                os.chdir(self.directory + "/Scenes")
-                split_video_ffmpeg(video_path, scene_list, show_progress=True)
-                # os.remove(video_path)
-            self.directory = self.directory + "/Scenes"
-
-            video_files = [f for f in os.listdir(self.directory) if
-                           f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(".mov")]
-            Train_X = list()
-            FirstFrames = list()
-            i = 1
-            for video_file in video_files:
-                FirstFrames.append(i)
-                video_path = os.path.join(self.directory, video_file)
-                video = cv2.VideoCapture(video_path)
-
-                while video.isOpened():
-                    ret, frame = video.read()
-                    if not ret or i == 10000:
-                        break
+    def __init__(self, directory):
+        self.directory = directory
 
-                    frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-
-                    Train_X.append(frame.reshape(36864, ))
+    def DownloadData(self, urls):
+        for i, url in enumerate(urls):
+            r = requests.get(url, allow_redirects=True)
+            open('Video' + str(i + 1) + '.mp4', 'wb').write(r.content)
+
+    def PrepareData(self):
+        if os.path.exists(self.directory + "/Scenes"):
+            shutil.rmtree(self.directory + "/Scenes")
+        os.mkdir(self.directory + "/Scenes")
+
+        video_files = [f for f in os.listdir(self.directory) if
+                       f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(
+                           ".mov") or f.endswith(".webm")]
+
+        for video_file in video_files:
+            video_path = os.path.join(self.directory, video_file)
+            scene_list = detect(video_path, ContentDetector())
+            os.chdir(self.directory + "/Scenes")
+            split_video_ffmpeg(video_path, scene_list, show_progress=True)
+            # os.remove(video_path)
+        self.directory = self.directory + "/Scenes"
+
+        video_files = [f for f in os.listdir(self.directory) if
+                       f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(".mov")]
+        Train_X = list()
+        FirstFrames = list()
+        i = 1
+        for video_file in video_files:
+            FirstFrames.append(i)
+            video_path = os.path.join(self.directory, video_file)
+            video = cv2.VideoCapture(video_path)
+
+            while video.isOpened():
+                ret, frame = video.read()
+                if not ret or i == 10000:
+                    break
+
+                frame = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
+
+                Train_X.append(frame.reshape(36864, ))
+
+                i += 1
+
+            video.release()
+        Train_X = np.array(Train_X).T  # 144x256
+
+        return Train_X, FirstFrames
+
+
+class Convection3D():
+    def __init__(self):
+        pass
+
+    def Generate(self, directory=os.getcwd() + "/Scenes"):
+        model_type = "DPT_Large"
+        midas = torch.hub.load("intel-isl/MiDas", model_type, force_reload=False)
+        device = torch.device("cuba") if torch.cuda.is_available() else torch.device("cpu")
+        midas.to(device)
+        midas.eval()
+        midas_transforms = torch.hub.load("intel-isl/MiDas", "transforms")
+
+        if model_type == "DPT_Large" or model_type == "DPT_Hybrid":
+            transform = midas_transforms.dpt_transform
+        else:
+            transform = midas_transforms.small_transform
+
+        video_files = [f for f in os.listdir(directory) if
+                       f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(".mov")]
+        Conv3D = list()
+        i = 1
+        for video_file in video_files:
+            video_path = os.path.join(directory, video_file)
+            video = cv2.VideoCapture(video_path)
+            while video.isOpened():
+                ret, frame = video.read()
+                if ret == False or i == 10000:
+                    break
+
+                img = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                input_batch = transform(img).to(device)
+
+                with torch.no_grad():
+                    prediction = midas(input_batch)
+                    prediction = torch.nn.functional.interpolate(
+                        prediction.unsqueeze(1),
+                        size=img.shape[:2],
+                        mode="bicubic",
+                        align_corners=False,
+                    ).squeeze()
+
+                    depth_map = prediction.cpu().numpy()
+                    depth_map = cv2.normalize(depth_map, None, 0, 1, norm_type=cv2.NORM_MINMAX, dtype=cv2.CV_64F)
+                    depth_map = (depth_map * 255).astype(np.uint8)
+                    Conv3D.append(depth_map.reshape(36864, ))
+                    print(i)
 
                     i += 1
 
-                video.release()
-            Train_X = np.array(Train_X).T  # 144x256
+        return np.array(Conv3D).T
+
+
+class NextFrameGenerator:
+    def __init__(self):
+        pass
+
+    def Train(self, X, Y, num_iterations=1000, learning_rate=0.01):
+        W1 = np.random.randn(40000, 16) * 0.01
+        b1 = np.zeros((40000, 1))
+        W2 = np.random.randn(1000, 40000) * 0.01
+        b2 = np.zeros((1000, 1))
+        W3 = np.random.randn(2400, 1000) * 0.01
+        b3 = np.zeros((2400, 1))
+        W4 = np.random.randn(240, 2400) * 0.01
+        b4 = np.zeros((16, 1))
+        print("weights init...")
+
+        for i in range(num_iterations):
+            # forward prop
+            Z1 = np.dot(W1, X) + b1
+            A1 = np.maximum(0, Z1)
+
+            Z2 = np.dot(W2, A1) + b2
+            A2 = np.maximum(0, Z2)
+
+            Z3 = np.dot(W3, A2) + b3
+            A3 = np.maximum(0, Z3)
+
+            Z4 = np.dot(W4, A3) + b4
+            A4 = 1 / (1 + np.exp(-Z4))
+
+            # backward prop
+
+            m = X.shape[1]
+
+            dZ4 = A4 - Y
+
+            dW4 = (1 / m) * np.dot(dZ4, A3.T)
+            db4 = (1 / m) * np.sum(dZ4, axis=1, keepdims=True)
 
-            return Train_X, FirstFrames
+            dA3 = np.dot(W4.T, dZ4)
+            dZ3 = np.multiply(dA3, np.int64(A3 > 0))
 
-    class Convection3D():
-        def __init__(self):
-            pass
-
-        def Generate(self, directory=os.getcwd() + "/Scenes"):
-            model_type = "DPT_Large"
-            midas = torch.hub.load("intel-isl/MiDas", model_type, force_reload=False)
-            device = torch.device("cuba") if torch.cuda.is_available() else torch.device("cpu")
-            midas.to(device)
-            midas.eval()
-            midas_transforms = torch.hub.load("intel-isl/MiDas", "transforms")
-
-            if model_type == "DPT_Large" or model_type == "DPT_Hybrid":
-                transform = midas_transforms.dpt_transform
-            else:
-                transform = midas_transforms.small_transform
-
-            video_files = [f for f in os.listdir(directory) if
-                           f.endswith(".mp4") or f.endswith(".mkv") or f.endswith(".avi") or f.endswith(".mov")]
-            Conv3D = list()
-            i = 1
-            for video_file in video_files:
-                video_path = os.path.join(directory, video_file)
-                video = cv2.VideoCapture(video_path)
-                while video.isOpened():
-                    ret, frame = video.read()
-                    if ret == False or i == 10000:
-                        break
-
-                    img = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-                    input_batch = transform(img).to(device)
-
-                    with torch.no_grad():
-                        prediction = midas(input_batch)
-                        prediction = torch.nn.functional.interpolate(
-                            prediction.unsqueeze(1),
-                            size=img.shape[:2],
-                            mode="bicubic",
-                            align_corners=False,
-                        ).squeeze()
-
-                        depth_map = prediction.cpu().numpy()
-                        depth_map = cv2.normalize(depth_map, None, 0, 1, norm_type=cv2.NORM_MINMAX, dtype=cv2.CV_64F)
-                        depth_map = (depth_map * 255).astype(np.uint8)
-                        Conv3D.append(depth_map.reshape(36864, ))
-                        print(i)
-
-                        i += 1
-
-            return np.array(Conv3D).T
-
-    class NextFrameGenerator:
-        def __init__(self):
-            pass
-
-        def Train(self, X, Y, num_iterations=1000, learning_rate=0.01):
-            W1 = np.random.randn(40000, 16) * 0.01
-            b1 = np.zeros((40000, 1))
-            W2 = np.random.randn(1000, 40000) * 0.01
-            b2 = np.zeros((1000, 1))
-            W3 = np.random.randn(2400, 1000) * 0.01
-            b3 = np.zeros((2400, 1))
-            W4 = np.random.randn(240, 2400) * 0.01
-            b4 = np.zeros((16, 1))
-            print("weights init...")
-
-            for i in range(num_iterations):
-                # forward prop
-                Z1 = np.dot(W1, X) + b1
-                A1 = np.maximum(0, Z1)
-
-                Z2 = np.dot(W2, A1) + b2
-                A2 = np.maximum(0, Z2)
-
-                Z3 = np.dot(W3, A2) + b3
-                A3 = np.maximum(0, Z3)
-
-                Z4 = np.dot(W4, A3) + b4
-                A4 = 1 / (1 + np.exp(-Z4))
-
-                # backward prop
-
-                m = X.shape[1]
-
-                dZ4 = A4 - Y
-
-                dW4 = (1 / m) * np.dot(dZ4, A3.T)
-                db4 = (1 / m) * np.sum(dZ4, axis=1, keepdims=True)
-
-                dA3 = np.dot(W4.T, dZ4)
-                dZ3 = np.multiply(dA3, np.int64(A3 > 0))
-
-                dW3 = (1 / m) * np.dot(dZ3, A2.T)
-                db3 = (1 / m) * np.sum(dZ3, axis=1, keepdims=True)
-
-                dA2 = np.dot(W3.T, dZ3)
-                dZ2 = np.multiply(dA2, np.int64(A2 > 0))
-
-                dW2 = (1 / m) * np.dot(dZ2, A1.T)
-                db2 = (1 / m) * np.sum(dZ2, axis=1, keepdims=True)
-
-                dA1 = np.dot(W2.T, dZ2)
-                dZ1 = np.multiply(dA1, np.int64(A1 > 0))
-
-                dW1 = (1 / m) * np.dot(dZ1, X.T)
-                db1 = (1 / m) * np.sum(dZ1, axis=1, keepdims=True)
-
-                parameters = (dW1, db1, dW2, db2, dW3, db3, dW4, db4)
-                print(i, " iteration finished at - ", time.strftime("%H:%M:%S"))
-
-            file = open("Discriminator.bin", 'wb')
-            pickle.dump(parameters, file)
-
-            return parameters
-
-    DataOptimizer = DataOptimizer(os.getcwd())
-    DataOptimizer.DownloadData(urls)
-    Train_X, FirstFrames = DataOptimizer.PrepareData()
-    Conv3D = Convection3D().Generate()
-
-    file = open(".\\" + device_id + "Train_X.bin", 'wb')
-    pickle.dump(Train_X, file)
-    file.close()
-    file = open(".\\" + device_id + "FirstFrames.bin", 'wb')
-    pickle.dump(FirstFrames, file)
-    file.close()
-    file = open(".\\" + device_id + "Conv3D.bin", 'wb')
-    pickle.dump(Conv3D, file)
-    file.close()
-    print("done")
-    mega = Mega()
-    log = mega.login("neuronode.bin@gmail.com", "getAccessAtNeuroNodeDataStorage")
-    log.upload("Train_X.bin")
-    log.upload("FirstFrames.bin")
-    log.upload("Conv3D.bin")
+            dW3 = (1 / m) * np.dot(dZ3, A2.T)
+            db3 = (1 / m) * np.sum(dZ3, axis=1, keepdims=True)
+
+            dA2 = np.dot(W3.T, dZ3)
+            dZ2 = np.multiply(dA2, np.int64(A2 > 0))
+
+            dW2 = (1 / m) * np.dot(dZ2, A1.T)
+            db2 = (1 / m) * np.sum(dZ2, axis=1, keepdims=True)
+
+            dA1 = np.dot(W2.T, dZ2)
+            dZ1 = np.multiply(dA1, np.int64(A1 > 0))
+
+            dW1 = (1 / m) * np.dot(dZ1, X.T)
+            db1 = (1 / m) * np.sum(dZ1, axis=1, keepdims=True)
+
+            parameters = (dW1, db1, dW2, db2, dW3, db3, dW4, db4)
+            print(i, " iteration finished at - ", time.strftime("%H:%M:%S"))
+
+        file = open("Discriminator.bin", 'wb')
+        pickle.dump(parameters, file)
+
+        return parameters
+
+
+device_id="1"
+DataOptimizer=DataOptimizer(os.getcwd())
+DataOptimizer.DownloadData(urls=["https://checker.in/go/13987"])
+Train_X,FirstFrames=DataOptimizer.PrepareData()
+Conv3D=Convection3D().Generate()
+
+file=open(".\\"+device_id+"Train_X.bin",'wb')
+pickle.dump(Train_X,file)
+file.close()
+file=open(".\\"+device_id+"FirstFrames.bin",'wb')
+pickle.dump(FirstFrames,file)
+file.close()
+file=open(".\\"+device_id+"Conv3D.bin",'wb')
+pickle.dump(Conv3D,file)
+file.close()
+print("done")
+mega=Mega()
+log=mega.login("neuronode.bin@gmail.com","getAccessAtNeuroNodeDataStorage")
+log.upload("Train_X.bin")
+log.upload("FirstFrames.bin")
+log.upload("Conv3D.bin")
 
     # Generator = NextFrameGenerator()
     # Train_D = np.random.randint(0, 255, (241, 10000))
     # Train_D_Y = np.random.randint(0, 1, (240, 10000))
     # print("data loaded...")
     # NextFrameGenerator.Train(Train_D, Train_D_Y)
-
```

