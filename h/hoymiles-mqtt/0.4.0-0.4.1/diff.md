# Comparing `tmp/hoymiles_mqtt-0.4.0.tar.gz` & `tmp/hoymiles_mqtt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoymiles_mqtt-0.4.0.tar", max compression
+gzip compressed data, was "hoymiles_mqtt-0.4.1.tar", max compression
```

## Comparing `hoymiles_mqtt-0.4.0.tar` & `hoymiles_mqtt-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-02-07 22:42:12.721820 hoymiles_mqtt-0.4.0/LICENSE
--rw-r--r--   0        0        0     8784 2023-02-07 22:42:12.721820 hoymiles_mqtt-0.4.0/README.md
--rw-r--r--   0        0        0      119 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/hoymiles_mqtt/__init__.py
--rw-r--r--   0        0        0     6584 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/hoymiles_mqtt/__main__.py
--rw-r--r--   0        0        0    10667 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/hoymiles_mqtt/ha.py
--rw-r--r--   0        0        0     1218 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/hoymiles_mqtt/mqtt.py
--rw-r--r--   0        0        0     2069 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/hoymiles_mqtt/runners.py
--rw-r--r--   0        0        0     2902 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      545 2023-02-07 22:42:12.725820 hoymiles_mqtt-0.4.0/tests/test_hoymiles_mqtt.py
--rw-r--r--   0        0        0    10432 1970-01-01 00:00:00.000000 hoymiles_mqtt-0.4.0/setup.py
--rw-r--r--   0        0        0    11120 1970-01-01 00:00:00.000000 hoymiles_mqtt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-09 20:41:44.202034 hoymiles_mqtt-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8784 2023-07-09 20:41:44.202034 hoymiles_mqtt-0.4.1/README.md
+-rw-r--r--   0        0        0      119 2023-07-09 20:41:44.202034 hoymiles_mqtt-0.4.1/hoymiles_mqtt/__init__.py
+-rw-r--r--   0        0        0     6534 2023-07-09 20:41:44.202034 hoymiles_mqtt-0.4.1/hoymiles_mqtt/__main__.py
+-rw-r--r--   0        0        0    10667 2023-07-09 20:41:44.202034 hoymiles_mqtt-0.4.1/hoymiles_mqtt/ha.py
+-rw-r--r--   0        0        0     1218 2023-07-09 20:41:44.206034 hoymiles_mqtt-0.4.1/hoymiles_mqtt/mqtt.py
+-rw-r--r--   0        0        0     2069 2023-07-09 20:41:44.206034 hoymiles_mqtt-0.4.1/hoymiles_mqtt/runners.py
+-rw-r--r--   0        0        0     2902 2023-07-09 20:41:44.206034 hoymiles_mqtt-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-09 20:41:44.206034 hoymiles_mqtt-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      545 2023-07-09 20:41:44.206034 hoymiles_mqtt-0.4.1/tests/test_hoymiles_mqtt.py
+-rw-r--r--   0        0        0    10870 1970-01-01 00:00:00.000000 hoymiles_mqtt-0.4.1/PKG-INFO
```

### Comparing `hoymiles_mqtt-0.4.0/LICENSE` & `hoymiles_mqtt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoymiles_mqtt-0.4.0/README.md` & `hoymiles_mqtt-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hoymiles_mqtt-0.4.0/hoymiles_mqtt/__main__.py` & `hoymiles_mqtt-0.4.1/hoymiles_mqtt/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,24 +72,22 @@
         env_var='MICROINVERTER_TYPE',
         help='Type od microinverters in the installation. Mixed types are not supported.',
     )
     cfg_parser.add(
         '--mi-entities',
         required=False,
         nargs="+",
-        action='append',
         default=MI_ENTITIES,
         env_var='MI_ENTITIES',
         help='Microinverter entities that will be sent to MQTT. By default all entities are presented.',
     )
     cfg_parser.add(
         '--port-entities',
         required=False,
         nargs="+",
-        action='append',
         default=PORT_ENTITIES,
         env_var='PORT_ENTITIES',
         help="Microinverters' port entities (in fact PV panel entities) that will be sent to MQTT. By default all "
         "entities are presented.",
     )
     cfg_parser.add(
         '--expire-after',
```

### Comparing `hoymiles_mqtt-0.4.0/hoymiles_mqtt/ha.py` & `hoymiles_mqtt-0.4.1/hoymiles_mqtt/ha.py`

 * *Files identical despite different names*

### Comparing `hoymiles_mqtt-0.4.0/hoymiles_mqtt/mqtt.py` & `hoymiles_mqtt-0.4.1/hoymiles_mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `hoymiles_mqtt-0.4.0/hoymiles_mqtt/runners.py` & `hoymiles_mqtt-0.4.1/hoymiles_mqtt/runners.py`

 * *Files identical despite different names*

### Comparing `hoymiles_mqtt-0.4.0/pyproject.toml` & `hoymiles_mqtt-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "hoymiles-mqtt"
-version = "0.4.0"
+version = "0.4.1"
 homepage = "https://github.com/wasilukm/hoymiles-mqtt"
 description = "Send data from Hoymiles photovoltaic installation to MQTT server."
 authors = ["Foo Bar <foo@bar.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `hoymiles_mqtt-0.4.0/tests/test_hoymiles_mqtt.py` & `hoymiles_mqtt-0.4.1/tests/test_hoymiles_mqtt.py`

 * *Files identical despite different names*

### Comparing `hoymiles_mqtt-0.4.0/PKG-INFO` & `hoymiles_mqtt-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoymiles-mqtt
-Version: 0.4.0
+Version: 0.4.1
 Summary: Send data from Hoymiles photovoltaic installation to MQTT server.
 Home-page: https://github.com/wasilukm/hoymiles-mqtt
 License: MIT
 Author: Foo Bar
 Author-email: foo@bar.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,19 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: ConfigArgParse (>=1.5.3,<2.0.0)
 Requires-Dist: black (==22.3.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
```

