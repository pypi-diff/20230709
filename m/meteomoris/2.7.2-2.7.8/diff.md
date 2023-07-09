# Comparing `tmp/meteomoris-2.7.2.tar.gz` & `tmp/meteomoris-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteomoris-2.7.2.tar", last modified: Thu Mar  9 19:41:50 2023, max compression
+gzip compressed data, was "meteomoris-2.7.8.tar", last modified: Sun Jul  9 16:13:01 2023, max compression
```

## Comparing `meteomoris-2.7.2.tar` & `meteomoris-2.7.8.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-03-09 19:41:50.837872 meteomoris-2.7.2/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1081 2022-02-20 07:28:44.000000 meteomoris-2.7.2/LICENSE
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11690 2023-03-09 19:41:50.837872 meteomoris-2.7.2/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    10663 2023-01-29 20:05:03.000000 meteomoris-2.7.2/README.md
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-03-09 19:41:50.825872 meteomoris-2.7.2/meteomoris/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      644 2023-03-09 19:41:17.000000 meteomoris-2.7.2/meteomoris/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1103 2023-01-25 11:38:50.000000 meteomoris-2.7.2/meteomoris/__main__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    39503 2023-03-09 19:40:47.000000 meteomoris-2.7.2/meteomoris/meteo.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-03-09 19:41:50.825872 meteomoris-2.7.2/meteomoris.egg-info/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11690 2023-03-09 19:41:50.000000 meteomoris-2.7.2/meteomoris.egg-info/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      308 2023-03-09 19:41:50.000000 meteomoris-2.7.2/meteomoris.egg-info/SOURCES.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-03-09 19:41:50.000000 meteomoris-2.7.2/meteomoris.egg-info/dependency_links.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       56 2023-03-09 19:41:50.000000 meteomoris-2.7.2/meteomoris.egg-info/entry_points.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       65 2023-03-09 19:41:50.000000 meteomoris-2.7.2/meteomoris.egg-info/requires.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       11 2023-03-09 19:41:50.000000 meteomoris-2.7.2/meteomoris.egg-info/top_level.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       79 2023-03-09 19:41:50.837872 meteomoris-2.7.2/setup.cfg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     9624 2023-01-23 09:57:01.000000 meteomoris-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:13:01.044159 meteomoris-2.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-09 16:12:51.000000 meteomoris-2.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-09 16:13:01.044159 meteomoris-2.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-09 16:12:51.000000 meteomoris-2.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:13:01.044159 meteomoris-2.7.8/meteomoris/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-09 16:12:51.000000 meteomoris-2.7.8/meteomoris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-09 16:12:51.000000 meteomoris-2.7.8/meteomoris/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40607 2023-07-09 16:12:51.000000 meteomoris-2.7.8/meteomoris/meteo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:13:01.044159 meteomoris-2.7.8/meteomoris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-09 16:13:01.000000 meteomoris-2.7.8/meteomoris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-09 16:13:01.000000 meteomoris-2.7.8/meteomoris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 16:13:01.000000 meteomoris-2.7.8/meteomoris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-09 16:13:01.000000 meteomoris-2.7.8/meteomoris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-09 16:13:01.000000 meteomoris-2.7.8/meteomoris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 16:13:01.000000 meteomoris-2.7.8/meteomoris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-09 16:13:01.044159 meteomoris-2.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-09 16:12:51.000000 meteomoris-2.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:13:01.044159 meteomoris-2.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-09 16:12:51.000000 meteomoris-2.7.8/tests/test_main.py
```

### Comparing `meteomoris-2.7.2/LICENSE` & `meteomoris-2.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meteomoris-2.7.2/PKG-INFO` & `meteomoris-2.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteomoris
-Version: 2.7.2
+Version: 2.7.8
 Summary: Package to get weather information about Mauritius from the official meteo website.
 Home-page: https://github.com/Abdur-RahmaanJ/meteomoris
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/meteomoris/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/meteomoris/
 Keywords: weather mauritius meteo
@@ -28,14 +28,26 @@
 
 ```
 pip install meteomoris
 ```
 
 Venv explanations at footer.
 
+# Ubuntu
+
+```
+sudo add-apt-repository ppa:abdur-rahmaanj/meteomoris-ppa
+sudo apt update
+sudo apt-get install meteomoris
+```
+
+# Important changes
+
+- year output removed from tides, added a meta label for year and month
+
 # Examples
 
 NOTE: Add `print=True` to get a tabular representation
 
 ```python
 >>> from meteomoris import *
 
@@ -194,27 +206,27 @@
             ...
         },
         'february': {
             1: ['00:36', '63', '10:49', '58', '06:12', '49', '18:21', '28'],
             ...
         }
     },
-    'year': 2023,
     'month_format': {
         'date': [
             '1st High Tide (Time (Local))',
             '1st High Tide (Height (cm))',
             '2nd High Tide (Time (Local))',
             '2nd High Tide (Height (cm))',
             '1st Low Tide (Time (Local))',
             '1st Low Tide (Height (cm))',
             '2nd Low Tide (Time (Local))',
             '2nd Low Tide (Height (cm))'
         ]
-    }
+    },
+    'meta': {'months': [['january', '2023'], ['feruary', '2023']]}
 }
 >>> get_latest()
 {
     'rainfall24h': {
         'info': 'Rainfall in (mm) from 28 January 2023 10 PM  to 29 January 2023 10 PM',
         'data': {
             'Albion': '',
@@ -338,14 +350,19 @@
 
 Run
 
 `python -m pytest tests/`
 
 # Changelog
 
+## 2.7.8
+
+- Fixes
+- Debian package published
+
 ## 2.7.0
 
 - Add latest data in API + today
 
 ## 2.6.0
 
 - Add tide
```

### Comparing `meteomoris-2.7.2/README.md` & `meteomoris-2.7.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 
 ```
 pip install meteomoris
 ```
 
 Venv explanations at footer.
 
+# Ubuntu
+
+```
+sudo add-apt-repository ppa:abdur-rahmaanj/meteomoris-ppa
+sudo apt update
+sudo apt-get install meteomoris
+```
+
+# Important changes
+
+- year output removed from tides, added a meta label for year and month
+
 # Examples
 
 NOTE: Add `print=True` to get a tabular representation
 
 ```python
 >>> from meteomoris import *
 
@@ -170,27 +182,27 @@
             ...
         },
         'february': {
             1: ['00:36', '63', '10:49', '58', '06:12', '49', '18:21', '28'],
             ...
         }
     },
-    'year': 2023,
     'month_format': {
         'date': [
             '1st High Tide (Time (Local))',
             '1st High Tide (Height (cm))',
             '2nd High Tide (Time (Local))',
             '2nd High Tide (Height (cm))',
             '1st Low Tide (Time (Local))',
             '1st Low Tide (Height (cm))',
             '2nd Low Tide (Time (Local))',
             '2nd Low Tide (Height (cm))'
         ]
-    }
+    },
+    'meta': {'months': [['january', '2023'], ['feruary', '2023']]}
 }
 >>> get_latest()
 {
     'rainfall24h': {
         'info': 'Rainfall in (mm) from 28 January 2023 10 PM  to 29 January 2023 10 PM',
         'data': {
             'Albion': '',
@@ -314,14 +326,19 @@
 
 Run
 
 `python -m pytest tests/`
 
 # Changelog
 
+## 2.7.8
+
+- Fixes
+- Debian package published
+
 ## 2.7.0
 
 - Add latest data in API + today
 
 ## 2.6.0
 
 - Add tide
```

### Comparing `meteomoris-2.7.2/meteomoris/__init__.py` & `meteomoris-2.7.8/meteomoris/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 get_eclipses_raw = Meteo.get_eclipses_raw
 get_eclipses = Meteo.get_eclipses
 get_equinoxes = Meteo.get_equinoxes
 get_solstices = Meteo.get_solstices
 get_tides = Meteo.get_tides
 get_latest = Meteo.get_latest
 
-__version__ = "2.7.2"
+__version__ = "2.7.8"
```

### Comparing `meteomoris-2.7.2/meteomoris/__main__.py` & `meteomoris-2.7.8/meteomoris/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from meteomoris import *
 
 @click.group()
 def cli():
     pass
 
 
-@cli.command()
-def dashboard():
-    print("---")
+# @cli.command()
+# def dashboard():
+#     print("---")
 
 @cli.command(help="Week forecast")
 def forecast():
     get_weekforecast(print=True)
 
 @cli.command(help="Sunrise (Mauritius)")
 def sunrisemu():
```

### Comparing `meteomoris-2.7.2/meteomoris/meteo.py` & `meteomoris-2.7.8/meteomoris/meteo.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from pprint import pprint
     from rich.console import Console
     from rich.columns import Columns
     from rich.table import Table
     from rich.panel import Panel
     import datetime
     import calendar
+    import re
 except Exception as e:
     pass
 
 import sys
 
 
 # def __download_file(url, path):
@@ -435,16 +436,16 @@
         data = dict()
         for i, row in enumerate(rows):
             cols = row.find_all("td")
 
             cols = [ele.text.strip() for ele in cols]
 
             if i == 0:
-                month1 = cols[1].lower()
-                month2 = cols[2].lower()
+                month1 = re.sub('\d+', '', cols[1].lower()).strip()
+                month2 = re.sub('\d+', '', cols[2].lower()).strip()
                 data = {month1: {}, month2: {}}
 
             elif i > 1:
                 date = int(cols[0])
                 m1_rise = cols[1]
                 m1_set = cols[2]
                 m2_rise = cols[3]
@@ -1000,67 +1001,93 @@
     @classmethod
     def get_tides(cls, print=False):
         print_ = print
 
         URL = "http://metservice.intnet.mu/sun-moon-and-tides-tides-mauritius.php"
         r = requests.get(URL, headers=cls.headers)
         soup = BeautifulSoup(r.content, "html.parser")
-        h2s = soup.find_all("h2")
         tables = soup.find_all("table")
-
-        tide_info = None
-
-        month1 = tables[0]
-        month2 = tables[1]
-        
-        month1 = [e.strip() for e in month1.text.strip().split('\n') if e.strip()]
-        month1 = month1[14:]
-
-        month2 = [e.strip() for e in month2.text.strip().split('\n') if e.strip()]
-        month2 = month2[14:]
-
-        h2txts = [h2.text for h2 in h2s]
-        h2txt = ' '.join(h2txts)
-
-        month1_name = h2txt.casefold().split(' for ')[1].split()[0]
-        month2_name = h2txt.casefold().split(' for ')[1].split()[2]
-        year = int(h2txt.casefold().split(' for ')[1].split()[3])
-
+        #cls.print(len(tables))
+        if len(tables) == 1:
+            text_arr = tables[0].text.split()
+            text_arr_cleaned = []
+            months = []
+            years = []
+            month_names = [m.casefold() for m in calendar.month_name if m]
+            for t in text_arr:
+                if t.casefold() in month_names:
+                    months.append(t.casefold())
+                    text_arr_cleaned.append(t.casefold())
+                elif re.findall('\d\d\d\d', t):
+                    text_arr_cleaned.append(t.casefold())
+                    years.append(t)
+                elif ((t.casefold() not in ['date', '1st', '2nd', '(local)', '(height)',
+                                        'tide', 'low', 'high', 'time', 'height',
+                                        '(cm)']) 
+                    ):
+                    text_arr_cleaned.append(t)
+
+        # cls.print(text_arr_cleaned)
+        #     [
+        # 'july',
+        # '2023',
+        # '1',
+        # '12:02',
+        # '54',
+        # '23:11',
+        # '57',
+        # '05:29',
+        # '6',
+        # '17:28',
+        # '28',
+        # '2',
+        # cls.print(months)
+        # cls.print(years)
         tide_info = {
             'months': {
-                month1_name: {},
-                month2_name: {}
+
             },
-            'year': year,
             'month_format': {
                 'date': [
                 '1st High Tide (Time (Local))', 
                 '1st High Tide (Height (cm))',
                 '2nd High Tide (Time (Local))', 
                 '2nd High Tide (Height (cm))',
                 '1st Low Tide (Time (Local))', 
                 '1st Low Tide (Height (cm))',
                 '2nd Low Tide (Time (Local))', 
                 '2nd Low Tide (Height (cm))',
                 ]
+            },
+            'meta':{
+                'months':[]
             }
         }
-
+        for i, month in enumerate(months):
+            tide_info['meta']['months'].append([months[i], years[i]])
+        
+        tc_i = 0
+        current_month = None
+        month_pad = 0
+        while tc_i < len(text_arr_cleaned):
+            text = text_arr_cleaned[tc_i]
+            if text in month_names:
+                # current_month = f'{text_arr_cleaned[tc_i]}_{text_arr_cleaned[tc_i+1]}'
+                current_month = f'{text_arr_cleaned[tc_i]}'
+                tide_info['months'][current_month] = {}
+                month_pad += 1
+                tc_i += 2
+                continue 
+            else:
+                if (tc_i - (2 * month_pad)) % 9 == 0:
+                    date = int(text_arr_cleaned[tc_i])
+                    tide_info['months'][current_month][date] = text_arr_cleaned[tc_i+1:tc_i+9]
+                    tc_i += 8
+            tc_i += 1
         # cls.print(tide_info)
-        # cls.print(month1)
-        # cls.print(month2)
-        for i, e in enumerate(month1):
-            # cls.print(i, e)
-            if ((i) % 9) == 0:
-                tide_info['months'][month1_name][int(e)] = month1[i+1:i+9]
-
-        for i, e in enumerate(month2):
-            if ((i) % 9) == 0:
-                tide_info['months'][month2_name][int(e)] = month2[i+1:i+9]
-
         return tide_info
 
 
     @classmethod
     def get_rainfall(cls, print=False):
         print_ = print
```

### Comparing `meteomoris-2.7.2/meteomoris.egg-info/PKG-INFO` & `meteomoris-2.7.8/meteomoris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteomoris
-Version: 2.7.2
+Version: 2.7.8
 Summary: Package to get weather information about Mauritius from the official meteo website.
 Home-page: https://github.com/Abdur-RahmaanJ/meteomoris
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 Project-URL: Bug Reports, https://github.com/Abdur-RahmaanJ/meteomoris/issues
 Project-URL: Source, https://github.com/Abdur-RahmaanJ/meteomoris/
 Keywords: weather mauritius meteo
@@ -28,14 +28,26 @@
 
 ```
 pip install meteomoris
 ```
 
 Venv explanations at footer.
 
+# Ubuntu
+
+```
+sudo add-apt-repository ppa:abdur-rahmaanj/meteomoris-ppa
+sudo apt update
+sudo apt-get install meteomoris
+```
+
+# Important changes
+
+- year output removed from tides, added a meta label for year and month
+
 # Examples
 
 NOTE: Add `print=True` to get a tabular representation
 
 ```python
 >>> from meteomoris import *
 
@@ -194,27 +206,27 @@
             ...
         },
         'february': {
             1: ['00:36', '63', '10:49', '58', '06:12', '49', '18:21', '28'],
             ...
         }
     },
-    'year': 2023,
     'month_format': {
         'date': [
             '1st High Tide (Time (Local))',
             '1st High Tide (Height (cm))',
             '2nd High Tide (Time (Local))',
             '2nd High Tide (Height (cm))',
             '1st Low Tide (Time (Local))',
             '1st Low Tide (Height (cm))',
             '2nd Low Tide (Time (Local))',
             '2nd Low Tide (Height (cm))'
         ]
-    }
+    },
+    'meta': {'months': [['january', '2023'], ['feruary', '2023']]}
 }
 >>> get_latest()
 {
     'rainfall24h': {
         'info': 'Rainfall in (mm) from 28 January 2023 10 PM  to 29 January 2023 10 PM',
         'data': {
             'Albion': '',
@@ -338,14 +350,19 @@
 
 Run
 
 `python -m pytest tests/`
 
 # Changelog
 
+## 2.7.8
+
+- Fixes
+- Debian package published
+
 ## 2.7.0
 
 - Add latest data in API + today
 
 ## 2.6.0
 
 - Add tide
```

### Comparing `meteomoris-2.7.2/setup.py` & `meteomoris-2.7.8/setup.py`

 * *Files identical despite different names*

