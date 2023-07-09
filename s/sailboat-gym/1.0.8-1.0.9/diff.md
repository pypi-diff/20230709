# Comparing `tmp/sailboat-gym-1.0.8.tar.gz` & `tmp/sailboat-gym-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sailboat-gym-1.0.8.tar", last modified: Wed May 31 14:31:44 2023, max compression
+gzip compressed data, was "sailboat-gym-1.0.9.tar", last modified: Wed May 31 15:00:50 2023, max compression
```

## Comparing `sailboat-gym-1.0.8.tar` & `sailboat-gym-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 14:31:44.942918 sailboat-gym-1.0.8/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.8/LICENSE
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1403 2023-05-31 14:31:44.942780 sailboat-gym-1.0.8/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.8/README.md
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 14:31:44.939603 sailboat-gym-1.0.8/sailboat_gym/
--rw-------   0 lucasmrdt   (501) staff       (20)      445 2023-05-31 14:31:37.000000 sailboat-gym-1.0.8/sailboat_gym/__init__.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 14:31:44.940975 sailboat-gym-1.0.8/sailboat_gym/envs/
--rw-------   0 lucasmrdt   (501) staff       (20)       41 2023-05-11 14:46:14.000000 sailboat-gym-1.0.8/sailboat_gym/envs/__init__.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      599 2023-05-11 15:47:26.000000 sailboat-gym-1.0.8/sailboat_gym/envs/env.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 14:31:44.941813 sailboat-gym-1.0.8/sailboat_gym/envs/sailboat_lsa/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       35 2023-05-11 14:43:54.000000 sailboat-gym-1.0.8/sailboat_gym/envs/sailboat_lsa/__init__.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     4054 2023-05-23 08:29:42.000000 sailboat-gym-1.0.8/sailboat_gym/envs/sailboat_lsa/lsa_env.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     6855 2023-05-31 14:30:21.000000 sailboat-gym-1.0.8/sailboat_gym/envs/sailboat_lsa/lsa_sim.py
--rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.8/sailboat_gym/interfaces.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 14:31:44.942412 sailboat-gym-1.0.8/sailboat_gym/renderers/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       41 2023-05-05 10:46:33.000000 sailboat-gym-1.0.8/sailboat_gym/renderers/__init__.py
--rw-------   0 lucasmrdt   (501) staff       (20)    12313 2023-05-23 08:55:36.000000 sailboat-gym-1.0.8/sailboat_gym/renderers/cv_2d_renderer.py
--rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.8/sailboat_gym/types.py
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     2410 2023-05-23 13:57:59.000000 sailboat-gym-1.0.8/sailboat_gym/utils.py
-drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 14:31:44.940586 sailboat-gym-1.0.8/sailboat_gym.egg-info/
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     1403 2023-05-31 14:31:44.000000 sailboat-gym-1.0.8/sailboat_gym.egg-info/PKG-INFO
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      559 2023-05-31 14:31:44.000000 sailboat-gym-1.0.8/sailboat_gym.egg-info/SOURCES.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 14:31:44.000000 sailboat-gym-1.0.8/sailboat_gym.egg-info/dependency_links.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)      173 2023-05-31 14:31:44.000000 sailboat-gym-1.0.8/sailboat_gym.egg-info/requires.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 14:31:44.000000 sailboat-gym-1.0.8/sailboat_gym.egg-info/top_level.txt
--rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 14:31:44.942970 sailboat-gym-1.0.8/setup.cfg
--rw-r--r--   0 lucasmrdt   (501) staff       (20)     2726 2023-05-31 07:43:54.000000 sailboat-gym-1.0.8/setup.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 15:00:49.998652 sailboat-gym-1.0.9/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1074 2023-05-23 13:44:12.000000 sailboat-gym-1.0.9/LICENSE
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1403 2023-05-31 15:00:49.998494 sailboat-gym-1.0.9/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     5949 2023-05-31 06:34:03.000000 sailboat-gym-1.0.9/README.md
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 15:00:49.994715 sailboat-gym-1.0.9/sailboat_gym/
+-rw-------   0 lucasmrdt   (501) staff       (20)      445 2023-05-31 15:00:30.000000 sailboat-gym-1.0.9/sailboat_gym/__init__.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 15:00:49.996353 sailboat-gym-1.0.9/sailboat_gym/envs/
+-rw-------   0 lucasmrdt   (501) staff       (20)       41 2023-05-11 14:46:14.000000 sailboat-gym-1.0.9/sailboat_gym/envs/__init__.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      599 2023-05-11 15:47:26.000000 sailboat-gym-1.0.9/sailboat_gym/envs/env.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 15:00:49.997513 sailboat-gym-1.0.9/sailboat_gym/envs/sailboat_lsa/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       35 2023-05-11 14:43:54.000000 sailboat-gym-1.0.9/sailboat_gym/envs/sailboat_lsa/__init__.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     4054 2023-05-23 08:29:42.000000 sailboat-gym-1.0.9/sailboat_gym/envs/sailboat_lsa/lsa_env.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     6916 2023-05-31 15:00:02.000000 sailboat-gym-1.0.9/sailboat_gym/envs/sailboat_lsa/lsa_sim.py
+-rw-------   0 lucasmrdt   (501) staff       (20)      699 2023-05-11 15:38:32.000000 sailboat-gym-1.0.9/sailboat_gym/interfaces.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 15:00:49.998101 sailboat-gym-1.0.9/sailboat_gym/renderers/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       41 2023-05-05 10:46:33.000000 sailboat-gym-1.0.9/sailboat_gym/renderers/__init__.py
+-rw-------   0 lucasmrdt   (501) staff       (20)    12313 2023-05-23 08:55:36.000000 sailboat-gym-1.0.9/sailboat_gym/renderers/cv_2d_renderer.py
+-rw-------   0 lucasmrdt   (501) staff       (20)     1475 2023-05-23 13:57:54.000000 sailboat-gym-1.0.9/sailboat_gym/types.py
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2411 2023-05-31 15:00:18.000000 sailboat-gym-1.0.9/sailboat_gym/utils.py
+drwxr-xr-x   0 lucasmrdt   (501) staff       (20)        0 2023-05-31 15:00:49.995914 sailboat-gym-1.0.9/sailboat_gym.egg-info/
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     1403 2023-05-31 15:00:49.000000 sailboat-gym-1.0.9/sailboat_gym.egg-info/PKG-INFO
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      559 2023-05-31 15:00:49.000000 sailboat-gym-1.0.9/sailboat_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)        1 2023-05-31 15:00:49.000000 sailboat-gym-1.0.9/sailboat_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)      173 2023-05-31 15:00:49.000000 sailboat-gym-1.0.9/sailboat_gym.egg-info/requires.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       13 2023-05-31 15:00:49.000000 sailboat-gym-1.0.9/sailboat_gym.egg-info/top_level.txt
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)       38 2023-05-31 15:00:49.998744 sailboat-gym-1.0.9/setup.cfg
+-rw-r--r--   0 lucasmrdt   (501) staff       (20)     2726 2023-05-31 07:43:54.000000 sailboat-gym-1.0.9/setup.py
```

### Comparing `sailboat-gym-1.0.8/LICENSE` & `sailboat-gym-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/PKG-INFO` & `sailboat-gym-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sailboat-gym
-Version: 1.0.8
+Version: 1.0.9
 Summary: A dynamic gym simulation environment specifically designed for sailboats.
 Home-page: https://github.com/lucasmrdt/sailboat-gym
 Author: Lucas Marandat
 Author-email: lucas.mrdt+sailboat@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/lucasmrdt/sailboat-gym
 Project-URL: Repository, https://github.com/lucasmrdt/sailboat-gym
```

### Comparing `sailboat-gym-1.0.8/README.md` & `sailboat-gym-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/sailboat_gym/envs/env.py` & `sailboat-gym-1.0.9/sailboat_gym/envs/env.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/sailboat_gym/envs/sailboat_lsa/lsa_env.py` & `sailboat-gym-1.0.9/sailboat_gym/envs/sailboat_lsa/lsa_env.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/sailboat_gym/envs/sailboat_lsa/lsa_sim.py` & `sailboat-gym-1.0.9/sailboat_gym/envs/sailboat_lsa/lsa_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
                 raise Exception(
                     f'Image not found: {str(e)}. '
                     'Please check that the image exists on the Docker registry and try again.'
                 )
 
             if is_debugging():
                 print('[LSASim] Launched new docker container')
+                print(self.container.logs().decode('utf-8'))
 
         return container
 
     def __wait_until_ready(self):
         with DurationProgress(total=17, desc='Waiting for docker container to be ready'):
             while True:
                 logs = self.container.logs().decode('utf-8')
```

### Comparing `sailboat-gym-1.0.8/sailboat_gym/interfaces.py` & `sailboat-gym-1.0.9/sailboat_gym/interfaces.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/sailboat_gym/renderers/cv_2d_renderer.py` & `sailboat-gym-1.0.9/sailboat_gym/renderers/cv_2d_renderer.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/sailboat_gym/types.py` & `sailboat-gym-1.0.9/sailboat_gym/types.py`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/sailboat_gym/utils.py` & `sailboat-gym-1.0.9/sailboat_gym/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             self.thread.join()
         if self.pbar is not None:
             self.pbar.close()
 
     def __update_progress(self):
         while not self.has_finished:
             self.pbar.update()
-            time.sleep(1)
+            time.sleep(.1)
 
 
 def profiling(func, prefix=''):
     stats = {'count': 0, 'first_call_time': None, 'duration': 0}
 
     def flush():
         freq = stats['count'] / (time.time() - stats['first_call_time'])
```

### Comparing `sailboat-gym-1.0.8/sailboat_gym.egg-info/PKG-INFO` & `sailboat-gym-1.0.9/sailboat_gym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sailboat-gym
-Version: 1.0.8
+Version: 1.0.9
 Summary: A dynamic gym simulation environment specifically designed for sailboats.
 Home-page: https://github.com/lucasmrdt/sailboat-gym
 Author: Lucas Marandat
 Author-email: lucas.mrdt+sailboat@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/lucasmrdt/sailboat-gym
 Project-URL: Repository, https://github.com/lucasmrdt/sailboat-gym
```

### Comparing `sailboat-gym-1.0.8/sailboat_gym.egg-info/SOURCES.txt` & `sailboat-gym-1.0.9/sailboat_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sailboat-gym-1.0.8/setup.py` & `sailboat-gym-1.0.9/setup.py`

 * *Files identical despite different names*

