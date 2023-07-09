# Comparing `tmp/EDEMDSPTFEB23-0.0.1.tar.gz` & `tmp/EDEMDSPTFEB23-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EDEMDSPTFEB23-0.0.1.tar", last modified: Sun Jul  9 18:58:56 2023, max compression
+gzip compressed data, was "EDEMDSPTFEB23-0.0.3.tar", last modified: Sun Jul  9 20:17:15 2023, max compression
```

## Comparing `EDEMDSPTFEB23-0.0.1.tar` & `EDEMDSPTFEB23-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 18:58:56.623033 EDEMDSPTFEB23-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-09 18:58:56.603026 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23/
--rw-rw-rw-   0        0        0       42 2023-07-09 18:53:44.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:58:56.622032 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23/procesamiento/
--rw-rw-rw-   0        0        0       42 2023-07-09 18:53:54.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23/procesamiento/__init__.py
--rw-rw-rw-   0        0        0     4275 2023-07-09 18:53:54.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23/procesamiento/preprocesado.py
-drwxrwxrwx   0        0        0        0 2023-07-09 18:58:56.618033 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23.egg-info/
--rw-rw-rw-   0        0        0      180 2023-07-09 18:58:56.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-09 18:58:56.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 18:58:56.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-07-09 18:58:56.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-09 18:58:56.000000 EDEMDSPTFEB23-0.0.1/EDEMDSPTFEB23.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       49 2023-07-05 09:28:28.000000 EDEMDSPTFEB23-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      180 2023-07-09 18:58:56.624032 EDEMDSPTFEB23-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-07-05 09:26:56.000000 EDEMDSPTFEB23-0.0.1/README.md
--rw-rw-rw-   0        0        0       85 2023-07-09 18:58:56.626035 EDEMDSPTFEB23-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      371 2023-07-09 18:58:42.000000 EDEMDSPTFEB23-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:17:15.515583 EDEMDSPTFEB23-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:17:15.480574 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:17:15.514582 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23/clasificador/
+-rw-rw-rw-   0        0        0       33 2023-07-09 19:32:08.000000 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23/clasificador/__init__.py
+-rw-rw-rw-   0        0        0      883 2023-07-09 20:16:43.000000 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23/clasificador/clasificador.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:17:15.511581 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23.egg-info/
+-rw-rw-rw-   0        0        0      180 2023-07-09 20:17:15.000000 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-09 20:17:15.000000 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 20:17:15.000000 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 20:17:15.000000 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-09 20:17:15.000000 EDEMDSPTFEB23-0.0.3/EDEMDSPTFEB23.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       49 2023-07-05 09:28:28.000000 EDEMDSPTFEB23-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      180 2023-07-09 20:17:15.515583 EDEMDSPTFEB23-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2023-07-05 09:26:56.000000 EDEMDSPTFEB23-0.0.3/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-09 20:17:15.521583 EDEMDSPTFEB23-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-07-09 20:15:22.000000 EDEMDSPTFEB23-0.0.3/setup.py
```

