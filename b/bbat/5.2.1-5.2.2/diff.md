# Comparing `tmp/bbat-5.2.1.tar.gz` & `tmp/bbat-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-5.2.1.tar", last modified: Sun Jul  9 07:19:15 2023, max compression
+gzip compressed data, was "bbat-5.2.2.tar", last modified: Sun Jul  9 16:22:55 2023, max compression
```

## Comparing `bbat-5.2.1.tar` & `bbat-5.2.2.tar`

### file list

```diff
@@ -1,14 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 07:19:15.987538 bbat-5.2.1/
--rw-rw-rw-   0        0        0      289 2023-07-09 07:19:15.986539 bbat-5.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-09 07:13:47.000000 bbat-5.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 07:19:15.979539 bbat-5.2.1/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-09 07:19:15.000000 bbat-5.2.1/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-07-09 07:19:15.000000 bbat-5.2.1/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 07:19:15.000000 bbat-5.2.1/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 07:19:15.000000 bbat-5.2.1/bbat.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-09 07:19:15.984543 bbat-5.2.1/letsgo/
--rw-rw-rw-   0        0        0        0 2023-07-09 07:00:10.000000 bbat-5.2.1/letsgo/__init__.py
--rw-rw-rw-   0        0        0       44 2023-07-09 07:00:10.000000 bbat-5.2.1/letsgo/hi.py
--rw-rw-rw-   0        0        0      197 2023-07-09 07:00:10.000000 bbat-5.2.1/letsgo/time.py
--rw-rw-rw-   0        0        0       42 2023-07-09 07:19:15.987538 bbat-5.2.1/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-07-09 07:18:57.000000 bbat-5.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.103239 bbat-5.2.2/
+-rw-rw-rw-   0        0        0      289 2023-07-09 16:22:55.102242 bbat-5.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-09 07:13:47.000000 bbat-5.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.054648 bbat-5.2.2/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:29:16.000000 bbat-5.2.2/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1525 2023-07-09 15:58:34.000000 bbat-5.2.2/bbat/config.py
+-rw-rw-rw-   0        0        0      587 2023-07-09 13:24:38.000000 bbat-5.2.2/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.077221 bbat-5.2.2/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:50:01.000000 bbat-5.2.2/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5357 2023-07-09 16:15:32.000000 bbat-5.2.2/bbat/db/a_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-05 12:04:50.000000 bbat-5.2.2/bbat/db/a_sqlite.py
+-rw-rw-rw-   0        0        0     2321 2023-07-09 14:43:07.000000 bbat-5.2.2/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0       30 2023-07-09 12:57:03.000000 bbat-5.2.2/bbat/hi.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.084335 bbat-5.2.2/bbat/http/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:29:16.000000 bbat-5.2.2/bbat/http/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-05 12:04:50.000000 bbat-5.2.2/bbat/http/cors.py
+-rw-rw-rw-   0        0        0     4442 2023-07-09 16:17:08.000000 bbat-5.2.2/bbat/http/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-09 15:23:45.000000 bbat-5.2.2/bbat/http/flask.py
+-rw-rw-rw-   0        0        0     1279 2023-07-09 15:06:59.000000 bbat-5.2.2/bbat/http/sanic.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.094159 bbat-5.2.2/bbat/http/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-09 14:55:40.000000 bbat-5.2.2/bbat/http/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-07-09 15:37:00.000000 bbat-5.2.2/bbat/http/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7556 2023-07-09 15:36:55.000000 bbat-5.2.2/bbat/http/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2258 2023-07-09 15:37:13.000000 bbat-5.2.2/bbat/http/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      723 2023-07-09 15:37:17.000000 bbat-5.2.2/bbat/http/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-05 12:04:50.000000 bbat-5.2.2/bbat/http/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1474 2023-07-09 15:37:22.000000 bbat-5.2.2/bbat/http/url_to_sql/where.py
+-rw-rw-rw-   0        0        0      142 2023-07-09 14:27:43.000000 bbat-5.2.2/bbat/uuid.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.072037 bbat-5.2.2/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 16:22:54.000000 bbat-5.2.2/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 16:22:55.104239 bbat-5.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-07-09 16:22:23.000000 bbat-5.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 16:22:55.101207 bbat-5.2.2/test/
+-rw-rw-rw-   0        0        0      191 2023-07-09 14:21:27.000000 bbat-5.2.2/test/test_config.py
+-rw-rw-rw-   0        0        0      178 2023-07-09 14:38:03.000000 bbat-5.2.2/test/test_db_mysql.py
+-rw-rw-rw-   0        0        0     2560 2023-07-09 15:27:40.000000 bbat-5.2.2/test/test_http_flask.py
+-rw-rw-rw-   0        0        0      815 2023-07-09 16:18:43.000000 bbat-5.2.2/test/test_http_sanic.py
+-rw-rw-rw-   0        0        0       69 2023-07-09 15:37:38.000000 bbat-5.2.2/test/test_http_server_db.py
```

