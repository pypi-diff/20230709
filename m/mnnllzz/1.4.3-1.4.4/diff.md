# Comparing `tmp/mnnllzz-1.4.3.tar.gz` & `tmp/mnnllzz-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnnllzz-1.4.3.tar", last modified: Thu Jul  6 10:04:07 2023, max compression
+gzip compressed data, was "mnnllzz-1.4.4.tar", last modified: Sun Jul  9 09:17:36 2023, max compression
```

## Comparing `mnnllzz-1.4.3.tar` & `mnnllzz-1.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:04:07.138214 mnnllzz-1.4.3/
--rw-rw-rw-   0        0        0      405 2023-07-06 10:04:07.138214 mnnllzz-1.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 10:04:07.138214 mnnllzz-1.4.3/mnnllzz/
--rw-rw-rw-   0        0        0        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.3/mnnllzz/__init__.py
--rw-rw-rw-   0        0        0      537 2023-02-20 17:34:38.000000 mnnllzz-1.4.3/mnnllzz/__main__.py
--rw-rw-rw-   0        0        0    25012 2023-06-19 06:36:33.000000 mnnllzz-1.4.3/mnnllzz/mnnllzz.py
--rw-rw-rw-   0        0        0       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      450 2023-07-06 10:03:19.288242 mnnllzz-1.4.3/setup.py
+drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2023-07-09 09:17:36.026002 mnnllzz-1.4.4/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      391 2023-07-09 09:17:36.026002 mnnllzz-1.4.4/PKG-INFO
+drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2023-07-09 09:17:36.025002 mnnllzz-1.4.4/mnnllzz/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.4/mnnllzz/__init__.py
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      864 2023-07-09 08:27:11.455779 mnnllzz-1.4.4/mnnllzz/__main__.py
+-rw-r--r--   0 andrea    (1000) andrea    (1000)    25012 2023-06-19 06:36:33.000000 mnnllzz-1.4.4/mnnllzz/mnnllzz.py
+-rw-r--r--   0 andrea    (1000) andrea    (1000)       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.4/setup.cfg
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      450 2023-07-09 09:17:06.463652 mnnllzz-1.4.4/setup.py
```

### Comparing `mnnllzz-1.4.3/mnnllzz/mnnllzz.py` & `mnnllzz-1.4.4/mnnllzz/mnnllzz.py`

 * *Files identical despite different names*

