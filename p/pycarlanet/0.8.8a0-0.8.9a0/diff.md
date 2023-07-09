# Comparing `tmp/pycarlanet-0.8.8a0.tar.gz` & `tmp/pycarlanet-0.8.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycarlanet-0.8.8a0.tar", last modified: Fri Mar 10 10:56:15 2023, max compression
+gzip compressed data, was "pycarlanet-0.8.9a0.tar", last modified: Fri Mar 10 11:01:38 2023, max compression
```

## Comparing `pycarlanet-0.8.8a0.tar` & `pycarlanet-0.8.9a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 10:56:15.023714 pycarlanet-0.8.8a0/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-10 10:56:15.023714 pycarlanet-0.8.8a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 10:56:15.023714 pycarlanet-0.8.8a0/pycarlanet/
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/pycarlanet/CarlanetActor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/pycarlanet/CarlanetManager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/pycarlanet/OMNeTWorldListener.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/pycarlanet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 10:56:15.023714 pycarlanet-0.8.8a0/pycarlanet/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/pycarlanet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/pycarlanet/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 10:56:15.023714 pycarlanet-0.8.8a0/pycarlanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-10 10:56:15.000000 pycarlanet-0.8.8a0/pycarlanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-03-10 10:56:15.000000 pycarlanet-0.8.8a0/pycarlanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-10 10:56:15.000000 pycarlanet-0.8.8a0/pycarlanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-03-10 10:56:15.000000 pycarlanet-0.8.8a0/pycarlanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-10 10:56:15.000000 pycarlanet-0.8.8a0/pycarlanet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-10 10:56:15.023714 pycarlanet-0.8.8a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 10:56:15.023714 pycarlanet-0.8.8a0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     5759 2023-03-10 10:56:04.000000 pycarlanet-0.8.8a0/tests/test_communication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/pycarlanet/
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/CarlanetActor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7053 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/CarlanetManager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/EventListener.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/pycarlanet/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/pycarlanet/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/pycarlanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-10 11:01:38.000000 pycarlanet-0.8.9a0/pycarlanet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 11:01:38.216633 pycarlanet-0.8.9a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     5759 2023-03-10 11:01:28.000000 pycarlanet-0.8.9a0/tests/test_communication.py
```

### Comparing `pycarlanet-0.8.8a0/LICENSE` & `pycarlanet-0.8.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycarlanet-0.8.8a0/pycarlanet/CarlanetActor.py` & `pycarlanet-0.8.9a0/pycarlanet/CarlanetActor.py`

 * *Files identical despite different names*

### Comparing `pycarlanet-0.8.8a0/pycarlanet/CarlanetManager.py` & `pycarlanet-0.8.9a0/pycarlanet/CarlanetManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import abc
 import json
 import os
 import carla
 import zmq
 
-from pycarlanet import OMNeTWorldListener, SimulatorStatus
+from pycarlanet import EventListener, SimulatorStatus
 from pycarlanet import CarlanetActor
 from pycarlanet.utils import preconditions
 
 
 class UnknownMessageCarlanetError(RuntimeError):
     def __init__(self, unknown_msg):
         self.unknown_msg = unknown_msg
 
     def __repr__(self) -> str:
         return "I don't know how to handle the following msg: " + self.unknown_msg['message_type']
 
 
 class CarlanetManager:
-    def __init__(self, listening_port, omnet_world_listener: OMNeTWorldListener, save_config_path=None):
+    def __init__(self, listening_port, omnet_world_listener: EventListener, save_config_path=None):
         self._listening_port = listening_port
         self._omnet_world_listener = omnet_world_listener
         self._message_handler: MessageHandlerState = None
         self._carlanet_actors = dict()
         self._save_config_path = save_config_path
 
     def _start_server(self):
@@ -32,15 +32,14 @@
         self.socket.setsockopt(zmq.LINGER, 100)
         self.socket.bind(f"tcp://*:{self._listening_port}")
         print("server running")
 
     def _receive_data_from_omnet(self):
         message = self.socket.recv()
         json_data = json.loads(message.decode("utf-8"))
-        print(json_data)
         self.timestamp = json_data['timestamp']
         return json_data
 
     def start_simulation(self):
         self._start_server()
         self.set_message_handler_state(InitMessageHandlerState)
         try:
@@ -52,16 +51,14 @@
 
         except Exception as e:
             self._omnet_world_listener.on_simulation_error(e)
         finally:
             self.socket.close()
 
     def _send_data_to_omnet(self, answer):
-        print(answer)
-
         self.socket.send(json.dumps(answer).encode('utf-8'))
 
     def set_message_handler_state(self, msg_handler_cls):
         self._message_handler = msg_handler_cls(self)
 
     def add_dynamic_actor(self, actor_id: str, carlanet_actor: CarlanetActor):
         """
@@ -80,15 +77,15 @@
         """
         del self._carlanet_actors[actor_id]
 
 
 class MessageHandlerState(abc.ABC):
     def __init__(self, carlanet_manager: CarlanetManager):
         self._manager = carlanet_manager
-        self.omnet_world_listener: OMNeTWorldListener = self._manager._omnet_world_listener
+        self.omnet_world_listener: EventListener = self._manager._omnet_world_listener
         self._carlanet_actors = self._manager._carlanet_actors
 
     def handle_message(self, message):
         message_type = message['message_type']
         if hasattr(self, message_type):
             meth = getattr(self, message_type)
             return meth(message)
```

### Comparing `pycarlanet-0.8.8a0/pycarlanet/OMNeTWorldListener.py` & `pycarlanet-0.8.9a0/pycarlanet/EventListener.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class SimulatorStatus(enum.Enum):
     RUNNING = 0
     FINISHED_OK = 1
     FINISHED_ERROR = -1
 
 
-class OMNeTWorldListener(abc.ABC):
+class EventListener(abc.ABC):
 
     def on_static_actor_created(self, actor_id: str, actor_type: str, actor_config) -> (float, CarlanetActor):
         """
         Callback called at the beginning of the simulation, OMNeT says which actors it has and communicate
         with carla to create those actors in the world
         :param actor_id:
         :param actor_type:
```

### Comparing `pycarlanet-0.8.8a0/pycarlanet/utils/decorators.py` & `pycarlanet-0.8.9a0/pycarlanet/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pycarlanet-0.8.8a0/setup.py` & `pycarlanet-0.8.9a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 import sys
 from pathlib import Path
 
 setup(
     name="pycarlanet",
     packages=find_packages(include=['pycarlanet', 'pycarlanet.utils']),
-    version="0.8.8-alpha",
+    version="0.8.9-alpha",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type='text/markdown',
     author="Valerio Cislaghi, Christian Quadri",
     license='MIT',
     python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.9',
     install_requires=[
         'pyzmq==23.2.1',
```

### Comparing `pycarlanet-0.8.8a0/tests/test_communication.py` & `pycarlanet-0.8.9a0/tests/test_communication.py`

 * *Files identical despite different names*

