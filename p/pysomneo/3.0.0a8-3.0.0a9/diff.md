# Comparing `tmp/pysomneo-3.0.0a8.tar.gz` & `tmp/pysomneo-3.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysomneo-3.0.0a8.tar", last modified: Sat Jul  8 13:51:48 2023, max compression
+gzip compressed data, was "pysomneo-3.0.0a9.tar", last modified: Sat Jul  8 14:01:46 2023, max compression
```

## Comparing `pysomneo-3.0.0a8.tar` & `pysomneo-3.0.0a9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:51:48.789000 pysomneo-3.0.0a8/
--rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a8/LICENSE
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:51:48.788052 pysomneo-3.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a8/README.md
--rw-rw-rw-   0        0        0      775 2023-07-08 13:51:20.000000 pysomneo-3.0.0a8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-08 13:51:48.769262 pysomneo-3.0.0a8/pysomneo/
--rw-rw-rw-   0        0        0    23487 2023-07-08 13:51:15.000000 pysomneo-3.0.0a8/pysomneo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:51:48.786830 pysomneo-3.0.0a8/pysomneo.egg-info/
--rw-rw-rw-   0        0        0    41813 2023-07-08 13:51:48.000000 pysomneo-3.0.0a8/pysomneo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-08 13:51:48.000000 pysomneo-3.0.0a8/pysomneo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:51:48.000000 pysomneo-3.0.0a8/pysomneo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 13:51:48.000000 pysomneo-3.0.0a8/pysomneo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 13:51:48.789000 pysomneo-3.0.0a8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 14:01:46.319236 pysomneo-3.0.0a9/
+-rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-3.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0    41813 2023-07-08 14:01:46.318169 pysomneo-3.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-3.0.0a9/README.md
+-rw-rw-rw-   0        0        0      775 2023-07-08 14:01:21.000000 pysomneo-3.0.0a9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-08 14:01:46.303912 pysomneo-3.0.0a9/pysomneo/
+-rw-rw-rw-   0        0        0    23773 2023-07-08 14:01:13.000000 pysomneo-3.0.0a9/pysomneo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 14:01:46.317173 pysomneo-3.0.0a9/pysomneo.egg-info/
+-rw-rw-rw-   0        0        0    41813 2023-07-08 14:01:46.000000 pysomneo-3.0.0a9/pysomneo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-08 14:01:46.000000 pysomneo-3.0.0a9/pysomneo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 14:01:46.000000 pysomneo-3.0.0a9/pysomneo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 14:01:46.000000 pysomneo-3.0.0a9/pysomneo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 14:01:46.319236 pysomneo-3.0.0a9/setup.cfg
```

### Comparing `pysomneo-3.0.0a8/LICENSE` & `pysomneo-3.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysomneo-3.0.0a8/PKG-INFO` & `pysomneo-3.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a8
+Version: 3.0.0a9
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysomneo-3.0.0a8/pyproject.toml` & `pysomneo-3.0.0a9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "requests>=2.24.0",
     "urllib3>=1.26.5"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysomneo"
-version = "3.0.0alpha8"
+version = "3.0.0alpha9"
 authors = [
   { name="Ruud van der Horst", email="pypi@mail.ruudvdhorst.nl" },
 ]
 description = "A library to communicate with the API of Philips Somneo."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pysomneo-3.0.0a8/pysomneo/__init__.py` & `pysomneo-3.0.0a9/pysomneo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,22 +565,30 @@
         if volume > 1:
             volume = 1
 
         self._put('wuply', payload={'sdvol': int(volume * 24 + 1)})
 
     def set_source_player(self, source: str | int):
         """Set the source of the player, either 'aux' or preset 1..5"""
+        previous_state = self.player['onoff']
         if source == 'aux' or source == 'AUX':
             print('aux source')
             self._put('wuply', payload=
                       {'snddv': 'aux', 
                        'sndss': 0,
-                       'onoff': self.player['onoff'],
+                       'onoff': previous_state,
                        'tempy': False
-                       }
+                    }
+                )
+            self._put('wuply', payload=
+                      {'snddv': 'aux', 
+                       'sndss': 0,
+                       'onoff': previous_state,
+                       'tempy': False
+                    }
                 )
 
         elif source in range(1,6):
             print('radio source')
             self._put('wuply', payload=
                       {'snddv': 'fmr', 
                        'sndch': str(source),
```

### Comparing `pysomneo-3.0.0a8/pysomneo.egg-info/PKG-INFO` & `pysomneo-3.0.0a9/pysomneo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 3.0.0a8
+Version: 3.0.0a9
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

