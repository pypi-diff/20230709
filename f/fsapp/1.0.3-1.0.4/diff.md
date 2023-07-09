# Comparing `tmp/fsapp-1.0.3.tar.gz` & `tmp/fsapp-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsapp-1.0.3.tar", last modified: Thu Jun 22 13:57:51 2023, max compression
+gzip compressed data, was "fsapp-1.0.4.tar", last modified: Sun Jul  9 12:59:35 2023, max compression
```

## Comparing `fsapp-1.0.3.tar` & `fsapp-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.390213 fsapp-1.0.3/
--rw-rw-rw-   0        0        0     1091 2023-03-29 11:26:53.000000 fsapp-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      329 2023-06-22 13:57:51.390213 fsapp-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12282 2023-05-11 13:29:45.000000 fsapp-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.338297 fsapp-1.0.3/fsapp/
--rw-rw-rw-   0        0        0      234 2023-03-29 08:18:14.000000 fsapp-1.0.3/fsapp/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-05-11 12:33:20.000000 fsapp-1.0.3/fsapp/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.353922 fsapp-1.0.3/fsapp/api/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:02:46.000000 fsapp-1.0.3/fsapp/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.369569 fsapp-1.0.3/fsapp/api/endpoints/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:20:14.000000 fsapp-1.0.3/fsapp/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-03-29 07:55:56.000000 fsapp-1.0.3/fsapp/api/endpoints/auth.py
--rw-rw-rw-   0        0        0     1875 2023-06-22 13:30:32.000000 fsapp-1.0.3/fsapp/api/endpoints/search.py
--rw-rw-rw-   0        0        0      442 2023-04-01 07:48:00.000000 fsapp-1.0.3/fsapp/api/endpoints/utils.py
--rw-rw-rw-   0        0        0      310 2023-03-29 07:55:56.000000 fsapp-1.0.3/fsapp/api/routers.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.374578 fsapp-1.0.3/fsapp/api/schemas/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:03:17.000000 fsapp-1.0.3/fsapp/api/schemas/__init__.py
--rw-rw-rw-   0        0        0      253 2023-06-22 13:06:35.000000 fsapp-1.0.3/fsapp/api/schemas/requests.py
--rw-rw-rw-   0        0        0      628 2023-03-15 13:12:47.000000 fsapp-1.0.3/fsapp/api/schemas/responses.py
--rw-rw-rw-   0        0        0      615 2023-06-22 13:55:05.000000 fsapp-1.0.3/fsapp/base.py
--rw-rw-rw-   0        0        0      929 2023-05-03 14:22:38.000000 fsapp-1.0.3/fsapp/classes.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.374578 fsapp-1.0.3/fsapp/core/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:19:31.000000 fsapp-1.0.3/fsapp/core/__init__.py
--rw-rw-rw-   0        0        0     1173 2023-06-22 13:55:05.000000 fsapp-1.0.3/fsapp/core/config.py
--rw-rw-rw-   0        0        0      418 2023-05-03 14:11:55.000000 fsapp-1.0.3/fsapp/core/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.353922 fsapp-1.0.3/fsapp.egg-info/
--rw-rw-rw-   0        0        0      329 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      360 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1057 2023-06-22 13:06:55.000000 fsapp-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 13:57:51.390213 fsapp-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.374578 fsapp-1.0.3/tests/
--rw-rw-rw-   0        0        0      340 2023-06-22 13:56:28.000000 fsapp-1.0.3/tests/test_endpoints.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.780512 fsapp-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-03-29 11:26:53.000000 fsapp-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      329 2023-07-09 12:59:35.780512 fsapp-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12282 2023-05-11 13:29:45.000000 fsapp-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.595519 fsapp-1.0.4/fsapp/
+-rw-rw-rw-   0        0        0      234 2023-03-29 08:18:14.000000 fsapp-1.0.4/fsapp/__init__.py
+-rw-rw-rw-   0        0        0     1981 2023-07-09 12:48:04.000000 fsapp-1.0.4/fsapp/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.648922 fsapp-1.0.4/fsapp/api/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:02:46.000000 fsapp-1.0.4/fsapp/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.680184 fsapp-1.0.4/fsapp/api/endpoints/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:20:14.000000 fsapp-1.0.4/fsapp/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-03-29 07:55:56.000000 fsapp-1.0.4/fsapp/api/endpoints/auth.py
+-rw-rw-rw-   0        0        0     1898 2023-07-09 12:54:03.000000 fsapp-1.0.4/fsapp/api/endpoints/search.py
+-rw-rw-rw-   0        0        0      442 2023-04-01 07:48:00.000000 fsapp-1.0.4/fsapp/api/endpoints/utils.py
+-rw-rw-rw-   0        0        0      310 2023-03-29 07:55:56.000000 fsapp-1.0.4/fsapp/api/routers.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.711433 fsapp-1.0.4/fsapp/api/schemas/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:03:17.000000 fsapp-1.0.4/fsapp/api/schemas/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-06-22 13:06:35.000000 fsapp-1.0.4/fsapp/api/schemas/requests.py
+-rw-rw-rw-   0        0        0      628 2023-03-15 13:12:47.000000 fsapp-1.0.4/fsapp/api/schemas/responses.py
+-rw-rw-rw-   0        0        0      615 2023-06-22 13:55:05.000000 fsapp-1.0.4/fsapp/base.py
+-rw-rw-rw-   0        0        0      929 2023-05-03 14:22:38.000000 fsapp-1.0.4/fsapp/classes.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.764951 fsapp-1.0.4/fsapp/core/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:19:31.000000 fsapp-1.0.4/fsapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1173 2023-06-22 13:55:05.000000 fsapp-1.0.4/fsapp/core/config.py
+-rw-rw-rw-   0        0        0      418 2023-05-03 14:11:55.000000 fsapp-1.0.4/fsapp/core/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.626723 fsapp-1.0.4/fsapp.egg-info/
+-rw-rw-rw-   0        0        0      329 2023-07-09 12:59:35.000000 fsapp-1.0.4/fsapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-07-09 12:59:35.000000 fsapp-1.0.4/fsapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:59:35.000000 fsapp-1.0.4/fsapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      360 2023-07-09 12:59:35.000000 fsapp-1.0.4/fsapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-09 12:59:35.000000 fsapp-1.0.4/fsapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-09 12:54:15.000000 fsapp-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 12:59:35.780512 fsapp-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 12:59:35.780512 fsapp-1.0.4/tests/
+-rw-rw-rw-   0        0        0      340 2023-06-22 13:56:28.000000 fsapp-1.0.4/tests/test_endpoints.py
```

### Comparing `fsapp-1.0.3/LICENSE` & `fsapp-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/README.md` & `fsapp-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/fsapp/__main__.py` & `fsapp-1.0.4/fsapp/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from hashlib import md5
 from prettytable import PrettyTable
 
 fields = {
+    "_all_": "Чтобы отбрабатывать все возможные виды",
     "phone": "Телефонный номер",
     "account.fb.id": "Id Facebook",
     "account.insta.id": "Id Instagram",
     "account.insta.username": "Ник Instagram",
     "account.linkedin.id": "Id Linkedin",
     "account.linkedin.username": "Ник Linkedin",
     "account.ok.id": "Id OK",
```

### Comparing `fsapp-1.0.3/fsapp/api/endpoints/auth.py` & `fsapp-1.0.4/fsapp/api/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/fsapp/api/endpoints/search.py` & `fsapp-1.0.4/fsapp/api/endpoints/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     if token != settings.token:
         return HTTPException(status_code=503, detail="Auth depends")
     # Получаем тип передаваемых данных
     data_type = request.data_type
     # Значения, переданные для поиска
     values: list = request.value
     # Смотрим, есть ли обработчик именно этого класса
-    if (search_class := handlers.get(data_type)) is not None:
+    if (search_class := handlers.get(data_type, handlers.get('_all_'))) is not None:
         try:
             # Создание экземляра Вашего класса и передача ему параметров
             searcher = handlers.get_instance(search_class)
             # Передаем результат в функцию подготовки ответа и возвращаем ResponseBody
             success, data = await searcher.execute_search(data_type, values)
             return make_response(success, data)
         except Exception as error:
```

### Comparing `fsapp-1.0.3/fsapp/api/schemas/responses.py` & `fsapp-1.0.4/fsapp/api/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/fsapp/base.py` & `fsapp-1.0.4/fsapp/base.py`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/fsapp/classes.py` & `fsapp-1.0.4/fsapp/classes.py`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/fsapp/core/config.py` & `fsapp-1.0.4/fsapp/core/config.py`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/fsapp.egg-info/SOURCES.txt` & `fsapp-1.0.4/fsapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsapp-1.0.3/pyproject.toml` & `fsapp-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsapp"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Scrandi Coulson", email = "scrandi.coulson@ro.ru" },
 ]
 description = "Fastapi web-app"
 #readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

