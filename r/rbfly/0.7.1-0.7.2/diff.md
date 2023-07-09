# Comparing `tmp/rbfly-0.7.1.tar.gz` & `tmp/rbfly-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfly-0.7.1.tar", last modified: Sun Jun 25 18:55:01 2023, max compression
+gzip compressed data, was "rbfly-0.7.2.tar", last modified: Sun Jul  9 10:05:52 2023, max compression
```

## Comparing `rbfly-0.7.1.tar` & `rbfly-0.7.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2023-01-11 23:13:37.000000 rbfly-0.7.1/COPYING
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-06-25 18:55:01.419360 rbfly-0.7.1/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-06-19 18:52:56.000000 rbfly-0.7.1/README
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      183 2023-06-09 14:43:29.000000 rbfly-0.7.1/pyproject.toml
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.406026 rbfly-0.7.1/rbfly/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      935 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   171073 2023-06-25 08:30:58.000000 rbfly-0.7.1/rbfly/_buffer.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1435 2023-01-16 12:48:43.000000 rbfly-0.7.1/rbfly/_buffer.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/_buffer.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   160017 2023-06-25 08:30:58.000000 rbfly-0.7.1/rbfly/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/_codec.h
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2023-05-29 23:14:21.000000 rbfly-0.7.1/rbfly/_codec.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/_codec.pyx
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.409360 rbfly-0.7.1/rbfly/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   677200 2023-06-25 08:30:59.000000 rbfly-0.7.1/rbfly/amqp/_message.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1617 2023-06-14 21:25:05.000000 rbfly-0.7.1/rbfly/amqp/_message.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1538 2023-06-15 21:01:28.000000 rbfly-0.7.1/rbfly/amqp/_message.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20434 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/amqp/_message.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3894 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/cm.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2023-01-30 14:42:53.000000 rbfly-0.7.1/rbfly/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/py.typed
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1685 2023-06-15 16:46:02.000000 rbfly-0.7.1/rbfly/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1168133 2023-06-25 08:30:59.000000 rbfly-0.7.1/rbfly/streams/_client.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2350 2023-06-25 07:47:11.000000 rbfly-0.7.1/rbfly/streams/_client.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    15997 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/streams/_client.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   672712 2023-06-25 08:31:00.000000 rbfly-0.7.1/rbfly/streams/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1563 2023-06-10 19:30:42.000000 rbfly-0.7.1/rbfly/streams/_codec.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12460 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/streams/_codec.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   463176 2023-06-25 08:31:00.000000 rbfly-0.7.1/rbfly/streams/_mqueue.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2023-02-01 18:34:41.000000 rbfly-0.7.1/rbfly/streams/_mqueue.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3933 2023-06-25 08:30:55.000000 rbfly-0.7.1/rbfly/streams/_mqueue.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18064 2023-06-25 07:49:01.000000 rbfly-0.7.1/rbfly/streams/client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8690 2023-06-10 20:40:38.000000 rbfly-0.7.1/rbfly/streams/codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2023-02-01 15:06:50.000000 rbfly-0.7.1/rbfly/streams/const.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1103 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5229 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    29111 2023-06-13 20:22:14.000000 rbfly-0.7.1/rbfly/streams/protocol.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1075 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4004 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/streams/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/tests/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/__init__.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/tests/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10104 2023-06-16 12:13:33.000000 rbfly-0.7.1/rbfly/tests/amqp/test_message.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.419360 rbfly-0.7.1/rbfly/tests/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    13944 2023-06-19 07:59:59.000000 rbfly-0.7.1/rbfly/tests/streams/test_client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    14725 2023-06-10 22:58:17.000000 rbfly-0.7.1/rbfly/tests/streams/test_codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2271 2023-02-01 15:02:22.000000 rbfly-0.7.1/rbfly/tests/streams/test_mqueue.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1344 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/streams/test_offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/tests/test_util.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2287 2023-06-15 16:54:08.000000 rbfly-0.7.1/rbfly/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2023-01-11 23:13:37.000000 rbfly-0.7.1/rbfly/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-06-25 18:55:01.406026 rbfly-0.7.1/rbfly.egg-info/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1235 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/SOURCES.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/dependency_links.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      216 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/requires.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2023-06-25 18:55:01.000000 rbfly-0.7.1/rbfly.egg-info/top_level.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1422 2023-06-25 18:55:01.422693 rbfly-0.7.1/setup.cfg
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1705 2023-06-15 10:13:31.000000 rbfly-0.7.1/setup.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.767012 rbfly-0.7.2/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2023-01-11 23:13:37.000000 rbfly-0.7.2/COPYING
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-07-09 10:05:52.767012 rbfly-0.7.2/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-06-19 18:52:56.000000 rbfly-0.7.2/README
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      183 2023-06-09 14:43:29.000000 rbfly-0.7.2/pyproject.toml
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.753679 rbfly-0.7.2/rbfly/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      935 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   171073 2023-06-25 08:30:58.000000 rbfly-0.7.2/rbfly/_buffer.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1435 2023-01-16 12:48:43.000000 rbfly-0.7.2/rbfly/_buffer.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2023-06-25 08:30:55.000000 rbfly-0.7.2/rbfly/_buffer.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   160017 2023-06-25 08:30:58.000000 rbfly-0.7.2/rbfly/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/_codec.h
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2023-05-29 23:14:21.000000 rbfly-0.7.2/rbfly/_codec.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2023-06-25 08:30:55.000000 rbfly-0.7.2/rbfly/_codec.pyx
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.757012 rbfly-0.7.2/rbfly/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   678127 2023-06-28 11:13:44.000000 rbfly-0.7.2/rbfly/amqp/_message.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1629 2023-06-28 11:12:37.000000 rbfly-0.7.2/rbfly/amqp/_message.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1538 2023-06-15 21:01:28.000000 rbfly-0.7.2/rbfly/amqp/_message.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20482 2023-06-28 11:13:39.000000 rbfly-0.7.2/rbfly/amqp/_message.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3894 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/cm.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2023-01-30 14:42:53.000000 rbfly-0.7.2/rbfly/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/py.typed
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.763679 rbfly-0.7.2/rbfly/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1685 2023-06-15 16:46:02.000000 rbfly-0.7.2/rbfly/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1223766 2023-07-08 19:10:52.000000 rbfly-0.7.2/rbfly/streams/_client.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2475 2023-07-07 00:45:55.000000 rbfly-0.7.2/rbfly/streams/_client.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    17212 2023-07-07 00:54:11.000000 rbfly-0.7.2/rbfly/streams/_client.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   673716 2023-07-08 19:27:12.000000 rbfly-0.7.2/rbfly/streams/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1563 2023-06-10 19:30:42.000000 rbfly-0.7.2/rbfly/streams/_codec.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12510 2023-07-08 19:27:07.000000 rbfly-0.7.2/rbfly/streams/_codec.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   463176 2023-06-25 08:31:00.000000 rbfly-0.7.2/rbfly/streams/_mqueue.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2023-02-01 18:34:41.000000 rbfly-0.7.2/rbfly/streams/_mqueue.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3933 2023-06-25 08:30:55.000000 rbfly-0.7.2/rbfly/streams/_mqueue.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18064 2023-07-07 00:27:08.000000 rbfly-0.7.2/rbfly/streams/client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8690 2023-06-10 20:40:38.000000 rbfly-0.7.2/rbfly/streams/codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2023-07-06 09:59:27.000000 rbfly-0.7.2/rbfly/streams/const.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1103 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/streams/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5229 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/streams/offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    29999 2023-07-06 23:35:17.000000 rbfly-0.7.2/rbfly/streams/protocol.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1075 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/streams/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4004 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/streams/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.767012 rbfly-0.7.2/rbfly/tests/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/tests/__init__.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.767012 rbfly-0.7.2/rbfly/tests/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/tests/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10104 2023-06-16 12:13:33.000000 rbfly-0.7.2/rbfly/tests/amqp/test_message.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.767012 rbfly-0.7.2/rbfly/tests/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/tests/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    15245 2023-07-07 00:42:01.000000 rbfly-0.7.2/rbfly/tests/streams/test_client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    16803 2023-06-28 11:26:15.000000 rbfly-0.7.2/rbfly/tests/streams/test_codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2271 2023-02-01 15:02:22.000000 rbfly-0.7.2/rbfly/tests/streams/test_mqueue.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1344 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/tests/streams/test_offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/tests/test_util.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2287 2023-06-15 16:54:08.000000 rbfly-0.7.2/rbfly/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2023-01-11 23:13:37.000000 rbfly-0.7.2/rbfly/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2023-07-09 10:05:52.753679 rbfly-0.7.2/rbfly.egg-info/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1826 2023-07-09 10:05:52.000000 rbfly-0.7.2/rbfly.egg-info/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1235 2023-07-09 10:05:52.000000 rbfly-0.7.2/rbfly.egg-info/SOURCES.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2023-07-09 10:05:52.000000 rbfly-0.7.2/rbfly.egg-info/dependency_links.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      217 2023-07-09 10:05:52.000000 rbfly-0.7.2/rbfly.egg-info/requires.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2023-07-09 10:05:52.000000 rbfly-0.7.2/rbfly.egg-info/top_level.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1423 2023-07-09 10:05:52.767012 rbfly-0.7.2/setup.cfg
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1705 2023-06-15 10:13:31.000000 rbfly-0.7.2/setup.py
```

### Comparing `rbfly-0.7.1/COPYING` & `rbfly-0.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/PKG-INFO` & `rbfly-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.7.1
+Version: 0.7.2
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
```

### Comparing `rbfly-0.7.1/README` & `rbfly-0.7.2/README`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/__init__.py` & `rbfly-0.7.2/rbfly/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/_buffer.c` & `rbfly-0.7.2/rbfly/_buffer.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/_buffer.pxd` & `rbfly-0.7.2/rbfly/_buffer.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/_buffer.pyx` & `rbfly-0.7.2/rbfly/_buffer.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/_codec.c` & `rbfly-0.7.2/rbfly/_codec.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/_codec.h` & `rbfly-0.7.2/rbfly/_codec.h`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/_codec.pxd` & `rbfly-0.7.2/rbfly/_codec.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/_codec.pyx` & `rbfly-0.7.2/rbfly/_codec.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/amqp/__init__.py` & `rbfly-0.7.2/rbfly/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/amqp/_message.c` & `rbfly-0.7.2/rbfly/amqp/_message.c`

 * *Files 0% similar despite different names*

```diff
@@ -2239,15 +2239,15 @@
 static double (*__pyx_f_5rbfly_6_codec_unpack_double)(char const *); /*proto*/
 static void (*__pyx_f_5rbfly_6_codec_pack_uint32)(char *, uint32_t); /*proto*/
 static void (*__pyx_f_5rbfly_6_codec_pack_uint64)(char *, uint64_t); /*proto*/
 static void (*__pyx_f_5rbfly_6_codec_pack_double)(char *, double); /*proto*/
 
 /* Module declarations from "rbfly.amqp._message" */
 static Py_ssize_t __pyx_f_5rbfly_4amqp_8_message_c_encode_amqp(struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *); /*proto*/
-static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp(struct __pyx_t_5rbfly_7_buffer_Buffer *); /*proto*/
+static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t); /*proto*/
 static CYTHON_INLINE void __pyx_f_5rbfly_4amqp_8_message__next_code(struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t *, uint8_t *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5rbfly_4amqp_8_message__decode_value(struct __pyx_t_5rbfly_7_buffer_Buffer *, uint8_t); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_t_5rbfly_4amqp_8_message_t_func_decode_compound, __pyx_t_5rbfly_4amqp_8_message_t_func_compound_size, struct __pyx_t_5rbfly_7_buffer_Buffer *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5rbfly_4amqp_8_message__decode_list(struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t, uint32_t); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5rbfly_4amqp_8_message__decode_map(struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t, uint32_t); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_t_5rbfly_4amqp_8_message_t_func_strb_size, struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t); /*proto*/
 static CYTHON_INLINE void __pyx_f_5rbfly_4amqp_8_message__decode_size8(struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t *); /*proto*/
@@ -5184,90 +5184,106 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_pf_5rbfly_4amqp_8_message_2decode_amqp(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_buffer) {
+  PyObject *__pyx_v_size = 0;
   struct __pyx_t_5rbfly_7_buffer_Buffer __pyx_v_buff;
   struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  struct __pyx_t_5rbfly_7_buffer_Buffer __pyx_t_1;
-  char *__pyx_t_2;
-  Py_ssize_t __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  struct __pyx_t_5rbfly_7_buffer_Buffer __pyx_t_3;
+  char *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_amqp", 0);
 
   /* "rbfly/amqp/_message.pyx":204
  *     """
  *     cdef:
- *         Buffer buff = Buffer(buffer, len(buffer), 0)             # <<<<<<<<<<<<<<
- *     return c_decode_amqp(&buff)
- * 
+ *         cdef size = len(buffer)             # <<<<<<<<<<<<<<
+ *         Buffer buff = Buffer(buffer, size, 0)
+ *     return c_decode_amqp(&buff, size)
  */
   if (unlikely(__pyx_v_buffer == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(1, 204, __pyx_L1_error)
-  }
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_buffer); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 204, __pyx_L1_error)
-  __pyx_t_1.buffer = __pyx_t_2;
-  if (unlikely(__pyx_v_buffer == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 204, __pyx_L1_error)
   }
-  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_buffer); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 204, __pyx_L1_error)
-  __pyx_t_1.size = __pyx_t_3;
-  __pyx_t_1.offset = 0;
-  __pyx_v_buff = __pyx_t_1;
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_buffer); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 204, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_size = __pyx_t_2;
+  __pyx_t_2 = 0;
 
   /* "rbfly/amqp/_message.pyx":205
  *     cdef:
- *         Buffer buff = Buffer(buffer, len(buffer), 0)
- *     return c_decode_amqp(&buff)             # <<<<<<<<<<<<<<
+ *         cdef size = len(buffer)
+ *         Buffer buff = Buffer(buffer, size, 0)             # <<<<<<<<<<<<<<
+ *     return c_decode_amqp(&buff, size)
+ * 
+ */
+  if (unlikely(__pyx_v_buffer == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+    __PYX_ERR(1, 205, __pyx_L1_error)
+  }
+  __pyx_t_4 = __Pyx_PyBytes_AsWritableString(__pyx_v_buffer); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 205, __pyx_L1_error)
+  __pyx_t_3.buffer = __pyx_t_4;
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_size); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 205, __pyx_L1_error)
+  __pyx_t_3.size = __pyx_t_1;
+  __pyx_t_3.offset = 0;
+  __pyx_v_buff = __pyx_t_3;
+
+  /* "rbfly/amqp/_message.pyx":206
+ *         cdef size = len(buffer)
+ *         Buffer buff = Buffer(buffer, size, 0)
+ *     return c_decode_amqp(&buff, size)             # <<<<<<<<<<<<<<
  * 
  * #
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_4 = ((PyObject *)__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp((&__pyx_v_buff))); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_r = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_4);
-  __pyx_t_4 = 0;
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_size); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 206, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp((&__pyx_v_buff), __pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 206, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_2);
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "rbfly/amqp/_message.pyx":197
  *     return c_encode_amqp(&buff, message)
  * 
  * def decode_amqp(bytes buffer) -> MessageCtx:             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP message.
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("rbfly.amqp._message.decode_amqp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_size);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":211
+/* "rbfly/amqp/_message.pyx":212
  * #
  * 
- * cdef MessageCtx c_decode_amqp(Buffer *buffer):             # <<<<<<<<<<<<<<
+ * cdef MessageCtx c_decode_amqp(Buffer *buffer, Py_ssize_t size):             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP message.
  */
 
-static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp(struct __pyx_t_5rbfly_7_buffer_Buffer *__pyx_v_buffer) {
+static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp(struct __pyx_t_5rbfly_7_buffer_Buffer *__pyx_v_buffer, CYTHON_UNUSED Py_ssize_t __pyx_v_size) {
   uint32_t __pyx_v_desc_code;
   uint8_t __pyx_v_type_code;
   PyObject *__pyx_v_msg_annotations = 0;
   PyObject *__pyx_v_app_properties = 0;
   PyObject *__pyx_v_body = 0;
   struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -5281,213 +5297,213 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("c_decode_amqp", 0);
 
-  /* "rbfly/amqp/_message.pyx":220
+  /* "rbfly/amqp/_message.pyx":221
  *         uint32_t desc_code
  *         uint8_t type_code
  *         object msg_annotations = {}             # <<<<<<<<<<<<<<
  *         object app_properties = {}
  *         object body
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_msg_annotations = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "rbfly/amqp/_message.pyx":221
+  /* "rbfly/amqp/_message.pyx":222
  *         uint8_t type_code
  *         object msg_annotations = {}
  *         object app_properties = {}             # <<<<<<<<<<<<<<
  *         object body
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 221, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_app_properties = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "rbfly/amqp/_message.pyx":224
+  /* "rbfly/amqp/_message.pyx":225
  *         object body
  * 
  *     _next_code(buffer, &desc_code, &type_code)             # <<<<<<<<<<<<<<
  *     if desc_code == MESSAGE_ANNOTATIONS:
  *         msg_annotations = _decode_value(buffer, type_code)
  */
-  __pyx_f_5rbfly_4amqp_8_message__next_code(__pyx_v_buffer, (&__pyx_v_desc_code), (&__pyx_v_type_code)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 224, __pyx_L1_error)
+  __pyx_f_5rbfly_4amqp_8_message__next_code(__pyx_v_buffer, (&__pyx_v_desc_code), (&__pyx_v_type_code)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":225
+  /* "rbfly/amqp/_message.pyx":226
  * 
  *     _next_code(buffer, &desc_code, &type_code)
  *     if desc_code == MESSAGE_ANNOTATIONS:             # <<<<<<<<<<<<<<
  *         msg_annotations = _decode_value(buffer, type_code)
  *         _next_code(buffer, &desc_code, &type_code)
  */
   __pyx_t_2 = (__pyx_v_desc_code == 0x5372);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":226
+    /* "rbfly/amqp/_message.pyx":227
  *     _next_code(buffer, &desc_code, &type_code)
  *     if desc_code == MESSAGE_ANNOTATIONS:
  *         msg_annotations = _decode_value(buffer, type_code)             # <<<<<<<<<<<<<<
  *         _next_code(buffer, &desc_code, &type_code)
  * 
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 226, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_msg_annotations, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":227
+    /* "rbfly/amqp/_message.pyx":228
  *     if desc_code == MESSAGE_ANNOTATIONS:
  *         msg_annotations = _decode_value(buffer, type_code)
  *         _next_code(buffer, &desc_code, &type_code)             # <<<<<<<<<<<<<<
  * 
  *     # _next_code used in previous block, so `if` not `elif` here
  */
-    __pyx_f_5rbfly_4amqp_8_message__next_code(__pyx_v_buffer, (&__pyx_v_desc_code), (&__pyx_v_type_code)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 227, __pyx_L1_error)
+    __pyx_f_5rbfly_4amqp_8_message__next_code(__pyx_v_buffer, (&__pyx_v_desc_code), (&__pyx_v_type_code)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 228, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":225
+    /* "rbfly/amqp/_message.pyx":226
  * 
  *     _next_code(buffer, &desc_code, &type_code)
  *     if desc_code == MESSAGE_ANNOTATIONS:             # <<<<<<<<<<<<<<
  *         msg_annotations = _decode_value(buffer, type_code)
  *         _next_code(buffer, &desc_code, &type_code)
  */
   }
 
-  /* "rbfly/amqp/_message.pyx":230
+  /* "rbfly/amqp/_message.pyx":231
  * 
  *     # _next_code used in previous block, so `if` not `elif` here
  *     if desc_code == MESSAGE_APP_PROPERTIES:             # <<<<<<<<<<<<<<
  *         app_properties = _decode_value(buffer, type_code)
  *         _next_code(buffer, &desc_code, &type_code)
  */
   __pyx_t_2 = (__pyx_v_desc_code == 0x5374);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":231
+    /* "rbfly/amqp/_message.pyx":232
  *     # _next_code used in previous block, so `if` not `elif` here
  *     if desc_code == MESSAGE_APP_PROPERTIES:
  *         app_properties = _decode_value(buffer, type_code)             # <<<<<<<<<<<<<<
  *         _next_code(buffer, &desc_code, &type_code)
  * 
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 231, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_app_properties, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":232
+    /* "rbfly/amqp/_message.pyx":233
  *     if desc_code == MESSAGE_APP_PROPERTIES:
  *         app_properties = _decode_value(buffer, type_code)
  *         _next_code(buffer, &desc_code, &type_code)             # <<<<<<<<<<<<<<
  * 
  *     # _next_code used in previous block, so `if` not `elif` here
  */
-    __pyx_f_5rbfly_4amqp_8_message__next_code(__pyx_v_buffer, (&__pyx_v_desc_code), (&__pyx_v_type_code)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 232, __pyx_L1_error)
+    __pyx_f_5rbfly_4amqp_8_message__next_code(__pyx_v_buffer, (&__pyx_v_desc_code), (&__pyx_v_type_code)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 233, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":230
+    /* "rbfly/amqp/_message.pyx":231
  * 
  *     # _next_code used in previous block, so `if` not `elif` here
  *     if desc_code == MESSAGE_APP_PROPERTIES:             # <<<<<<<<<<<<<<
  *         app_properties = _decode_value(buffer, type_code)
  *         _next_code(buffer, &desc_code, &type_code)
  */
   }
 
-  /* "rbfly/amqp/_message.pyx":235
+  /* "rbfly/amqp/_message.pyx":236
  * 
  *     # _next_code used in previous block, so `if` not `elif` here
  *     if desc_code == MESSAGE_OPAQUE_BINARY:             # <<<<<<<<<<<<<<
  *         if type_code == TYPE_BINARY_SHORT:
  *             body = _decode_strb(_decode_size8, buffer, type_code)
  */
   switch (__pyx_v_desc_code) {
     case 0x5375:
 
-    /* "rbfly/amqp/_message.pyx":236
+    /* "rbfly/amqp/_message.pyx":237
  *     # _next_code used in previous block, so `if` not `elif` here
  *     if desc_code == MESSAGE_OPAQUE_BINARY:
  *         if type_code == TYPE_BINARY_SHORT:             # <<<<<<<<<<<<<<
  *             body = _decode_strb(_decode_size8, buffer, type_code)
  *         elif type_code == TYPE_BINARY_LONG:
  */
     switch (__pyx_v_type_code) {
       case 0xA0:
 
-      /* "rbfly/amqp/_message.pyx":237
+      /* "rbfly/amqp/_message.pyx":238
  *     if desc_code == MESSAGE_OPAQUE_BINARY:
  *         if type_code == TYPE_BINARY_SHORT:
  *             body = _decode_strb(_decode_size8, buffer, type_code)             # <<<<<<<<<<<<<<
  *         elif type_code == TYPE_BINARY_LONG:
  *             body = _decode_strb(_decode_size32, buffer, type_code)
  */
-      __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 237, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 238, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_body = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "rbfly/amqp/_message.pyx":236
+      /* "rbfly/amqp/_message.pyx":237
  *     # _next_code used in previous block, so `if` not `elif` here
  *     if desc_code == MESSAGE_OPAQUE_BINARY:
  *         if type_code == TYPE_BINARY_SHORT:             # <<<<<<<<<<<<<<
  *             body = _decode_strb(_decode_size8, buffer, type_code)
  *         elif type_code == TYPE_BINARY_LONG:
  */
       break;
       case 0xB0:
 
-      /* "rbfly/amqp/_message.pyx":239
+      /* "rbfly/amqp/_message.pyx":240
  *             body = _decode_strb(_decode_size8, buffer, type_code)
  *         elif type_code == TYPE_BINARY_LONG:
  *             body = _decode_strb(_decode_size32, buffer, type_code)             # <<<<<<<<<<<<<<
  *         else:
  *             raise AMQPDecoderError(
  */
-      __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 239, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_body = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "rbfly/amqp/_message.pyx":238
+      /* "rbfly/amqp/_message.pyx":239
  *         if type_code == TYPE_BINARY_SHORT:
  *             body = _decode_strb(_decode_size8, buffer, type_code)
  *         elif type_code == TYPE_BINARY_LONG:             # <<<<<<<<<<<<<<
  *             body = _decode_strb(_decode_size32, buffer, type_code)
  *         else:
  */
       break;
       default:
 
-      /* "rbfly/amqp/_message.pyx":241
+      /* "rbfly/amqp/_message.pyx":242
  *             body = _decode_strb(_decode_size32, buffer, type_code)
  *         else:
  *             raise AMQPDecoderError(             # <<<<<<<<<<<<<<
  *                 'Cannot decode message, descriptor=0x{:06x}, type code=0x{:02x}'
  *                 .format(desc_code, type_code)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 241, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 242, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
 
-      /* "rbfly/amqp/_message.pyx":243
+      /* "rbfly/amqp/_message.pyx":244
  *             raise AMQPDecoderError(
  *                 'Cannot decode message, descriptor=0x{:06x}, type code=0x{:02x}'
  *                 .format(desc_code, type_code)             # <<<<<<<<<<<<<<
  *             )
  *     elif desc_code == MESSAGE_VALUE:
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_descriptor, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 243, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_descriptor, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 244, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_desc_code); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 243, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_desc_code); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 244, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_v_type_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 243, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_v_type_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 244, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -5499,15 +5515,15 @@
       }
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_8, __pyx_t_6, __pyx_t_7};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_9, 2+__pyx_t_9);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 243, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
       __pyx_t_5 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5520,76 +5536,76 @@
         }
       }
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 241, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 242, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(1, 241, __pyx_L1_error)
+      __PYX_ERR(1, 242, __pyx_L1_error)
       break;
     }
 
-    /* "rbfly/amqp/_message.pyx":235
+    /* "rbfly/amqp/_message.pyx":236
  * 
  *     # _next_code used in previous block, so `if` not `elif` here
  *     if desc_code == MESSAGE_OPAQUE_BINARY:             # <<<<<<<<<<<<<<
  *         if type_code == TYPE_BINARY_SHORT:
  *             body = _decode_strb(_decode_size8, buffer, type_code)
  */
     break;
     case 0x5377:
 
-    /* "rbfly/amqp/_message.pyx":246
+    /* "rbfly/amqp/_message.pyx":247
  *             )
  *     elif desc_code == MESSAGE_VALUE:
  *         body = _decode_value(buffer, type_code)             # <<<<<<<<<<<<<<
  *     else:
  *         raise AMQPDecoderError(
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 246, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":245
+    /* "rbfly/amqp/_message.pyx":246
  *                 .format(desc_code, type_code)
  *             )
  *     elif desc_code == MESSAGE_VALUE:             # <<<<<<<<<<<<<<
  *         body = _decode_value(buffer, type_code)
  *     else:
  */
     break;
     default:
 
-    /* "rbfly/amqp/_message.pyx":248
+    /* "rbfly/amqp/_message.pyx":249
  *         body = _decode_value(buffer, type_code)
  *     else:
  *         raise AMQPDecoderError(             # <<<<<<<<<<<<<<
  *             'Cannot decode message, descriptor 0x{:06x}'.format(desc_code)
  *         )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 248, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "rbfly/amqp/_message.pyx":249
+    /* "rbfly/amqp/_message.pyx":250
  *     else:
  *         raise AMQPDecoderError(
  *             'Cannot decode message, descriptor 0x{:06x}'.format(desc_code)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_descriptor_2, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_descriptor_2, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_desc_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_desc_code); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -5600,15 +5616,15 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_7};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 249, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 250, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_t_5 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
@@ -5621,85 +5637,85 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 248, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 249, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(1, 248, __pyx_L1_error)
+    __PYX_ERR(1, 249, __pyx_L1_error)
     break;
   }
 
-  /* "rbfly/amqp/_message.pyx":252
+  /* "rbfly/amqp/_message.pyx":253
  *         )
  * 
  *     return MessageCtx(             # <<<<<<<<<<<<<<
  *         body,
  *         annotations=msg_annotations,
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
 
-  /* "rbfly/amqp/_message.pyx":253
+  /* "rbfly/amqp/_message.pyx":254
  * 
  *     return MessageCtx(
  *         body,             # <<<<<<<<<<<<<<
  *         annotations=msg_annotations,
  *         app_properties=app_properties,
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 252, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_body);
   __Pyx_GIVEREF(__pyx_v_body);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_body);
 
-  /* "rbfly/amqp/_message.pyx":254
+  /* "rbfly/amqp/_message.pyx":255
  *     return MessageCtx(
  *         body,
  *         annotations=msg_annotations,             # <<<<<<<<<<<<<<
  *         app_properties=app_properties,
  *     )
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 254, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotations, __pyx_v_msg_annotations) < 0) __PYX_ERR(1, 254, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotations, __pyx_v_msg_annotations) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":255
+  /* "rbfly/amqp/_message.pyx":256
  *         body,
  *         annotations=msg_annotations,
  *         app_properties=app_properties,             # <<<<<<<<<<<<<<
  *     )
  * 
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_app_properties, __pyx_v_app_properties) < 0) __PYX_ERR(1, 254, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_app_properties, __pyx_v_app_properties) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":252
+  /* "rbfly/amqp/_message.pyx":253
  *         )
  * 
  *     return MessageCtx(             # <<<<<<<<<<<<<<
  *         body,
  *         annotations=msg_annotations,
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx), __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 252, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx), __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_4);
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":211
+  /* "rbfly/amqp/_message.pyx":212
  * #
  * 
- * cdef MessageCtx c_decode_amqp(Buffer *buffer):             # <<<<<<<<<<<<<<
+ * cdef MessageCtx c_decode_amqp(Buffer *buffer, Py_ssize_t size):             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP message.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -5716,15 +5732,15 @@
   __Pyx_XDECREF(__pyx_v_app_properties);
   __Pyx_XDECREF(__pyx_v_body);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":258
+/* "rbfly/amqp/_message.pyx":259
  *     )
  * 
  * cdef inline void _next_code(             # <<<<<<<<<<<<<<
  *     Buffer *buffer,
  *     uint32_t *desc_code,
  */
 
@@ -5734,44 +5750,44 @@
   char *__pyx_t_1;
   uint32_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_next_code", 0);
 
-  /* "rbfly/amqp/_message.pyx":266
+  /* "rbfly/amqp/_message.pyx":267
  *         uint32_t dc
  * 
  *     dc = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))             # <<<<<<<<<<<<<<
  *     type_code[0] = dc & 0xff
  *     desc_code[0] = dc >> 8
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 266, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 266, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 267, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 267, __pyx_L1_error)
   __pyx_v_dc = __pyx_t_2;
 
-  /* "rbfly/amqp/_message.pyx":267
+  /* "rbfly/amqp/_message.pyx":268
  * 
  *     dc = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     type_code[0] = dc & 0xff             # <<<<<<<<<<<<<<
  *     desc_code[0] = dc >> 8
  * 
  */
   (__pyx_v_type_code[0]) = (__pyx_v_dc & 0xff);
 
-  /* "rbfly/amqp/_message.pyx":268
+  /* "rbfly/amqp/_message.pyx":269
  *     dc = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     type_code[0] = dc & 0xff
  *     desc_code[0] = dc >> 8             # <<<<<<<<<<<<<<
  * 
  * cdef inline object _decode_value(Buffer *buffer, uint8_t type_code):
  */
   (__pyx_v_desc_code[0]) = (__pyx_v_dc >> 8);
 
-  /* "rbfly/amqp/_message.pyx":258
+  /* "rbfly/amqp/_message.pyx":259
  *     )
  * 
  * cdef inline void _next_code(             # <<<<<<<<<<<<<<
  *     Buffer *buffer,
  *     uint32_t *desc_code,
  */
 
@@ -5779,15 +5795,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.amqp._message._next_code", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbfly/amqp/_message.pyx":270
+/* "rbfly/amqp/_message.pyx":271
  *     desc_code[0] = dc >> 8
  * 
  * cdef inline object _decode_value(Buffer *buffer, uint8_t type_code):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object body
  */
 
@@ -5811,132 +5827,132 @@
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_value", 0);
 
-  /* "rbfly/amqp/_message.pyx":275
+  /* "rbfly/amqp/_message.pyx":276
  *         uint64_t ts
  * 
  *     if type_code == TYPE_BINARY_SHORT:             # <<<<<<<<<<<<<<
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *     elif type_code == TYPE_BINARY_LONG:
  */
   switch (__pyx_v_type_code) {
     case 0xA0:
 
-    /* "rbfly/amqp/_message.pyx":276
+    /* "rbfly/amqp/_message.pyx":277
  * 
  *     if type_code == TYPE_BINARY_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_BINARY_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 276, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":275
+    /* "rbfly/amqp/_message.pyx":276
  *         uint64_t ts
  * 
  *     if type_code == TYPE_BINARY_SHORT:             # <<<<<<<<<<<<<<
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *     elif type_code == TYPE_BINARY_LONG:
  */
     break;
     case 0xB0:
 
-    /* "rbfly/amqp/_message.pyx":278
+    /* "rbfly/amqp/_message.pyx":279
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *     elif type_code == TYPE_BINARY_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_STRING_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 278, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 279, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":277
+    /* "rbfly/amqp/_message.pyx":278
  *     if type_code == TYPE_BINARY_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *     elif type_code == TYPE_BINARY_LONG:             # <<<<<<<<<<<<<<
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *     elif type_code == TYPE_STRING_SHORT:
  */
     break;
     case 0xA1:
 
-    /* "rbfly/amqp/_message.pyx":280
+    /* "rbfly/amqp/_message.pyx":281
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *     elif type_code == TYPE_STRING_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_STRING_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 280, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":279
+    /* "rbfly/amqp/_message.pyx":280
  *     elif type_code == TYPE_BINARY_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *     elif type_code == TYPE_STRING_SHORT:             # <<<<<<<<<<<<<<
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *     elif type_code == TYPE_STRING_LONG:
  */
     break;
     case 0xB1:
 
-    /* "rbfly/amqp/_message.pyx":282
+    /* "rbfly/amqp/_message.pyx":283
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *     elif type_code == TYPE_STRING_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_SYMBOL_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 282, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 283, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":281
+    /* "rbfly/amqp/_message.pyx":282
  *     elif type_code == TYPE_STRING_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *     elif type_code == TYPE_STRING_LONG:             # <<<<<<<<<<<<<<
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *     elif type_code == TYPE_SYMBOL_SHORT:
  */
     break;
     case 0xA3:
 
-    /* "rbfly/amqp/_message.pyx":284
+    /* "rbfly/amqp/_message.pyx":285
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *     elif type_code == TYPE_SYMBOL_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)             # <<<<<<<<<<<<<<
  *         body = Symbol(body)
  *     elif type_code == TYPE_SYMBOL_LONG:
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 284, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size8, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 285, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":285
+    /* "rbfly/amqp/_message.pyx":286
  *     elif type_code == TYPE_SYMBOL_SHORT:
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *         body = Symbol(body)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_SYMBOL_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Symbol); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 285, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Symbol); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -5946,51 +5962,51 @@
         __pyx_t_4 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_body};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 285, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 286, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_body, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":283
+    /* "rbfly/amqp/_message.pyx":284
  *     elif type_code == TYPE_STRING_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *     elif type_code == TYPE_SYMBOL_SHORT:             # <<<<<<<<<<<<<<
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *         body = Symbol(body)
  */
     break;
     case 0xB3:
 
-    /* "rbfly/amqp/_message.pyx":287
+    /* "rbfly/amqp/_message.pyx":288
  *         body = Symbol(body)
  *     elif type_code == TYPE_SYMBOL_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)             # <<<<<<<<<<<<<<
  *         body = Symbol(body)
  *     elif type_code in (BOOL_TRUE, BOOL_FALSE):
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_strb(__pyx_f_5rbfly_4amqp_8_message__decode_size32, __pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":288
+    /* "rbfly/amqp/_message.pyx":289
  *     elif type_code == TYPE_SYMBOL_LONG:
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *         body = Symbol(body)             # <<<<<<<<<<<<<<
  *     elif type_code in (BOOL_TRUE, BOOL_FALSE):
  *         body = type_code == BOOL_TRUE
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Symbol); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 288, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Symbol); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 289, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -6000,509 +6016,509 @@
         __pyx_t_4 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_body};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 289, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_body, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":286
+    /* "rbfly/amqp/_message.pyx":287
  *         body = _decode_strb(_decode_size8, buffer, type_code)
  *         body = Symbol(body)
  *     elif type_code == TYPE_SYMBOL_LONG:             # <<<<<<<<<<<<<<
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *         body = Symbol(body)
  */
     break;
     case 65:
 
-    /* "rbfly/amqp/_message.pyx":289
+    /* "rbfly/amqp/_message.pyx":290
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *         body = Symbol(body)
  *     elif type_code in (BOOL_TRUE, BOOL_FALSE):             # <<<<<<<<<<<<<<
  *         body = type_code == BOOL_TRUE
  *     elif type_code == TYPE_BOOL:
  */
     case 66:
 
-    /* "rbfly/amqp/_message.pyx":290
+    /* "rbfly/amqp/_message.pyx":291
  *         body = Symbol(body)
  *     elif type_code in (BOOL_TRUE, BOOL_FALSE):
  *         body = type_code == BOOL_TRUE             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_BOOL:
  *         body = buffer_get_uint8(buffer) == 0x01
  */
-    __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_type_code == 65)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 290, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_v_type_code == 65)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 291, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":289
+    /* "rbfly/amqp/_message.pyx":290
  *         body = _decode_strb(_decode_size32, buffer, type_code)
  *         body = Symbol(body)
  *     elif type_code in (BOOL_TRUE, BOOL_FALSE):             # <<<<<<<<<<<<<<
  *         body = type_code == BOOL_TRUE
  *     elif type_code == TYPE_BOOL:
  */
     break;
     case 86:
 
-    /* "rbfly/amqp/_message.pyx":292
+    /* "rbfly/amqp/_message.pyx":293
  *         body = type_code == BOOL_TRUE
  *     elif type_code == TYPE_BOOL:
  *         body = buffer_get_uint8(buffer) == 0x01             # <<<<<<<<<<<<<<
  *     elif type_code in (TYPE_UINT0, TYPE_ULONG0):
  *         body = 0
  */
-    __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 292, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_t_5 == 0x01)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 293, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBool_FromLong((__pyx_t_5 == 0x01)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 293, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":291
+    /* "rbfly/amqp/_message.pyx":292
  *     elif type_code in (BOOL_TRUE, BOOL_FALSE):
  *         body = type_code == BOOL_TRUE
  *     elif type_code == TYPE_BOOL:             # <<<<<<<<<<<<<<
  *         body = buffer_get_uint8(buffer) == 0x01
  *     elif type_code in (TYPE_UINT0, TYPE_ULONG0):
  */
     break;
     case 67:
 
-    /* "rbfly/amqp/_message.pyx":293
+    /* "rbfly/amqp/_message.pyx":294
  *     elif type_code == TYPE_BOOL:
  *         body = buffer_get_uint8(buffer) == 0x01
  *     elif type_code in (TYPE_UINT0, TYPE_ULONG0):             # <<<<<<<<<<<<<<
  *         body = 0
  *     elif type_code in (TYPE_UBYTE, TYPE_SMALLUINT, TYPE_SMALLULONG):
  */
     case 68:
 
-    /* "rbfly/amqp/_message.pyx":294
+    /* "rbfly/amqp/_message.pyx":295
  *         body = buffer_get_uint8(buffer) == 0x01
  *     elif type_code in (TYPE_UINT0, TYPE_ULONG0):
  *         body = 0             # <<<<<<<<<<<<<<
  *     elif type_code in (TYPE_UBYTE, TYPE_SMALLUINT, TYPE_SMALLULONG):
  *         body = buffer_get_uint8(buffer)
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_v_body = __pyx_int_0;
 
-    /* "rbfly/amqp/_message.pyx":293
+    /* "rbfly/amqp/_message.pyx":294
  *     elif type_code == TYPE_BOOL:
  *         body = buffer_get_uint8(buffer) == 0x01
  *     elif type_code in (TYPE_UINT0, TYPE_ULONG0):             # <<<<<<<<<<<<<<
  *         body = 0
  *     elif type_code in (TYPE_UBYTE, TYPE_SMALLUINT, TYPE_SMALLULONG):
  */
     break;
     case 80:
 
-    /* "rbfly/amqp/_message.pyx":295
+    /* "rbfly/amqp/_message.pyx":296
  *     elif type_code in (TYPE_UINT0, TYPE_ULONG0):
  *         body = 0
  *     elif type_code in (TYPE_UBYTE, TYPE_SMALLUINT, TYPE_SMALLULONG):             # <<<<<<<<<<<<<<
  *         body = buffer_get_uint8(buffer)
  *     elif type_code == TYPE_USHORT:
  */
     case 82:
     case 83:
 
-    /* "rbfly/amqp/_message.pyx":296
+    /* "rbfly/amqp/_message.pyx":297
  *         body = 0
  *     elif type_code in (TYPE_UBYTE, TYPE_SMALLUINT, TYPE_SMALLULONG):
  *         body = buffer_get_uint8(buffer)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_USHORT:
  *         body = unpack_uint16(buffer_claim(buffer, sizeof(uint16_t)))
  */
-    __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 296, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 296, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 297, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":295
+    /* "rbfly/amqp/_message.pyx":296
  *     elif type_code in (TYPE_UINT0, TYPE_ULONG0):
  *         body = 0
  *     elif type_code in (TYPE_UBYTE, TYPE_SMALLUINT, TYPE_SMALLULONG):             # <<<<<<<<<<<<<<
  *         body = buffer_get_uint8(buffer)
  *     elif type_code == TYPE_USHORT:
  */
     break;
     case 96:
 
-    /* "rbfly/amqp/_message.pyx":298
+    /* "rbfly/amqp/_message.pyx":299
  *         body = buffer_get_uint8(buffer)
  *     elif type_code == TYPE_USHORT:
  *         body = unpack_uint16(buffer_claim(buffer, sizeof(uint16_t)))             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_UINT:
  *         body = <uint32_t> unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint16_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 298, __pyx_L1_error)
-    __pyx_t_7 = __pyx_f_5rbfly_6_codec_unpack_uint16(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 298, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 298, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint16_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 299, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_5rbfly_6_codec_unpack_uint16(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 299, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":297
+    /* "rbfly/amqp/_message.pyx":298
  *     elif type_code in (TYPE_UBYTE, TYPE_SMALLUINT, TYPE_SMALLULONG):
  *         body = buffer_get_uint8(buffer)
  *     elif type_code == TYPE_USHORT:             # <<<<<<<<<<<<<<
  *         body = unpack_uint16(buffer_claim(buffer, sizeof(uint16_t)))
  *     elif type_code == TYPE_UINT:
  */
     break;
     case 0x70:
 
-    /* "rbfly/amqp/_message.pyx":300
+    /* "rbfly/amqp/_message.pyx":301
  *         body = unpack_uint16(buffer_claim(buffer, sizeof(uint16_t)))
  *     elif type_code == TYPE_UINT:
  *         body = <uint32_t> unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_ULONG:
  *         body = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 300, __pyx_L1_error)
-    __pyx_t_8 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 300, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(((uint32_t)__pyx_t_8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 300, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 301, __pyx_L1_error)
+    __pyx_t_8 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 301, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(((uint32_t)__pyx_t_8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 301, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":299
+    /* "rbfly/amqp/_message.pyx":300
  *     elif type_code == TYPE_USHORT:
  *         body = unpack_uint16(buffer_claim(buffer, sizeof(uint16_t)))
  *     elif type_code == TYPE_UINT:             # <<<<<<<<<<<<<<
  *         body = <uint32_t> unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     elif type_code == TYPE_ULONG:
  */
     break;
     case 0x80:
 
-    /* "rbfly/amqp/_message.pyx":302
+    /* "rbfly/amqp/_message.pyx":303
  *         body = <uint32_t> unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     elif type_code == TYPE_ULONG:
  *         body = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))             # <<<<<<<<<<<<<<
  *     elif type_code in (TYPE_BYTE, TYPE_SMALLINT, TYPE_SMALLLONG):
  *         body = <signed char> buffer_claim(buffer, 1)[0]
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 302, __pyx_L1_error)
-    __pyx_t_9 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 302, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_uint64_t(((uint64_t)__pyx_t_9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 302, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 303, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 303, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint64_t(((uint64_t)__pyx_t_9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":301
+    /* "rbfly/amqp/_message.pyx":302
  *     elif type_code == TYPE_UINT:
  *         body = <uint32_t> unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     elif type_code == TYPE_ULONG:             # <<<<<<<<<<<<<<
  *         body = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  *     elif type_code in (TYPE_BYTE, TYPE_SMALLINT, TYPE_SMALLLONG):
  */
     break;
     case 81:
 
-    /* "rbfly/amqp/_message.pyx":303
+    /* "rbfly/amqp/_message.pyx":304
  *     elif type_code == TYPE_ULONG:
  *         body = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  *     elif type_code in (TYPE_BYTE, TYPE_SMALLINT, TYPE_SMALLLONG):             # <<<<<<<<<<<<<<
  *         body = <signed char> buffer_claim(buffer, 1)[0]
  *     elif type_code == TYPE_SHORT:
  */
     case 84:
     case 85:
 
-    /* "rbfly/amqp/_message.pyx":304
+    /* "rbfly/amqp/_message.pyx":305
  *         body = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  *     elif type_code in (TYPE_BYTE, TYPE_SMALLINT, TYPE_SMALLLONG):
  *         body = <signed char> buffer_claim(buffer, 1)[0]             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_SHORT:
  *         body = <int16_t> unpack_uint16(buffer_claim(buffer, sizeof(int16_t)))
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 304, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_signed__char(((signed char)(__pyx_t_6[0]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 304, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 305, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_signed__char(((signed char)(__pyx_t_6[0]))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 305, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":303
+    /* "rbfly/amqp/_message.pyx":304
  *     elif type_code == TYPE_ULONG:
  *         body = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  *     elif type_code in (TYPE_BYTE, TYPE_SMALLINT, TYPE_SMALLLONG):             # <<<<<<<<<<<<<<
  *         body = <signed char> buffer_claim(buffer, 1)[0]
  *     elif type_code == TYPE_SHORT:
  */
     break;
     case 97:
 
-    /* "rbfly/amqp/_message.pyx":306
+    /* "rbfly/amqp/_message.pyx":307
  *         body = <signed char> buffer_claim(buffer, 1)[0]
  *     elif type_code == TYPE_SHORT:
  *         body = <int16_t> unpack_uint16(buffer_claim(buffer, sizeof(int16_t)))             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_INT:
  *         body = <int32_t> unpack_uint32(buffer_claim(buffer, sizeof(int32_t)))
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(int16_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 306, __pyx_L1_error)
-    __pyx_t_7 = __pyx_f_5rbfly_6_codec_unpack_uint16(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 306, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_int16_t(((int16_t)__pyx_t_7)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 306, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(int16_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 307, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_5rbfly_6_codec_unpack_uint16(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 307, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int16_t(((int16_t)__pyx_t_7)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":305
+    /* "rbfly/amqp/_message.pyx":306
  *     elif type_code in (TYPE_BYTE, TYPE_SMALLINT, TYPE_SMALLLONG):
  *         body = <signed char> buffer_claim(buffer, 1)[0]
  *     elif type_code == TYPE_SHORT:             # <<<<<<<<<<<<<<
  *         body = <int16_t> unpack_uint16(buffer_claim(buffer, sizeof(int16_t)))
  *     elif type_code == TYPE_INT:
  */
     break;
     case 0x71:
 
-    /* "rbfly/amqp/_message.pyx":308
+    /* "rbfly/amqp/_message.pyx":309
  *         body = <int16_t> unpack_uint16(buffer_claim(buffer, sizeof(int16_t)))
  *     elif type_code == TYPE_INT:
  *         body = <int32_t> unpack_uint32(buffer_claim(buffer, sizeof(int32_t)))             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_LONG:
  *         body = <int64_t> unpack_uint64(buffer_claim(buffer, sizeof(int64_t)))
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(int32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L1_error)
-    __pyx_t_8 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_int32_t(((int32_t)__pyx_t_8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 308, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(int32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 309, __pyx_L1_error)
+    __pyx_t_8 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 309, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int32_t(((int32_t)__pyx_t_8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 309, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":307
+    /* "rbfly/amqp/_message.pyx":308
  *     elif type_code == TYPE_SHORT:
  *         body = <int16_t> unpack_uint16(buffer_claim(buffer, sizeof(int16_t)))
  *     elif type_code == TYPE_INT:             # <<<<<<<<<<<<<<
  *         body = <int32_t> unpack_uint32(buffer_claim(buffer, sizeof(int32_t)))
  *     elif type_code == TYPE_LONG:
  */
     break;
     case 0x81:
 
-    /* "rbfly/amqp/_message.pyx":310
+    /* "rbfly/amqp/_message.pyx":311
  *         body = <int32_t> unpack_uint32(buffer_claim(buffer, sizeof(int32_t)))
  *     elif type_code == TYPE_LONG:
  *         body = <int64_t> unpack_uint64(buffer_claim(buffer, sizeof(int64_t)))             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_FLOAT:
  *         body = unpack_float(buffer_claim(buffer, sizeof(float)))
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(int64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 310, __pyx_L1_error)
-    __pyx_t_9 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 310, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyInt_From_int64_t(((int64_t)__pyx_t_9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 310, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(int64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 311, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 311, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int64_t(((int64_t)__pyx_t_9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 311, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":309
+    /* "rbfly/amqp/_message.pyx":310
  *     elif type_code == TYPE_INT:
  *         body = <int32_t> unpack_uint32(buffer_claim(buffer, sizeof(int32_t)))
  *     elif type_code == TYPE_LONG:             # <<<<<<<<<<<<<<
  *         body = <int64_t> unpack_uint64(buffer_claim(buffer, sizeof(int64_t)))
  *     elif type_code == TYPE_FLOAT:
  */
     break;
     case 0x72:
 
-    /* "rbfly/amqp/_message.pyx":312
+    /* "rbfly/amqp/_message.pyx":313
  *         body = <int64_t> unpack_uint64(buffer_claim(buffer, sizeof(int64_t)))
  *     elif type_code == TYPE_FLOAT:
  *         body = unpack_float(buffer_claim(buffer, sizeof(float)))             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_DOUBLE:
  *         body = unpack_double(buffer_claim(buffer, sizeof(double)))
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(float))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 312, __pyx_L1_error)
-    __pyx_t_10 = __pyx_f_5rbfly_6_codec_unpack_float(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 312, __pyx_L1_error)
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 312, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(float))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 313, __pyx_L1_error)
+    __pyx_t_10 = __pyx_f_5rbfly_6_codec_unpack_float(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 313, __pyx_L1_error)
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 313, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":311
+    /* "rbfly/amqp/_message.pyx":312
  *     elif type_code == TYPE_LONG:
  *         body = <int64_t> unpack_uint64(buffer_claim(buffer, sizeof(int64_t)))
  *     elif type_code == TYPE_FLOAT:             # <<<<<<<<<<<<<<
  *         body = unpack_float(buffer_claim(buffer, sizeof(float)))
  *     elif type_code == TYPE_DOUBLE:
  */
     break;
     case 0x82:
 
-    /* "rbfly/amqp/_message.pyx":314
+    /* "rbfly/amqp/_message.pyx":315
  *         body = unpack_float(buffer_claim(buffer, sizeof(float)))
  *     elif type_code == TYPE_DOUBLE:
  *         body = unpack_double(buffer_claim(buffer, sizeof(double)))             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_LIST0:
  *         body = []
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(double))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 314, __pyx_L1_error)
-    __pyx_t_11 = __pyx_f_5rbfly_6_codec_unpack_double(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 314, __pyx_L1_error)
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 314, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(double))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 315, __pyx_L1_error)
+    __pyx_t_11 = __pyx_f_5rbfly_6_codec_unpack_double(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 315, __pyx_L1_error)
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":313
+    /* "rbfly/amqp/_message.pyx":314
  *     elif type_code == TYPE_FLOAT:
  *         body = unpack_float(buffer_claim(buffer, sizeof(float)))
  *     elif type_code == TYPE_DOUBLE:             # <<<<<<<<<<<<<<
  *         body = unpack_double(buffer_claim(buffer, sizeof(double)))
  *     elif type_code == TYPE_LIST0:
  */
     break;
     case 69:
 
-    /* "rbfly/amqp/_message.pyx":316
+    /* "rbfly/amqp/_message.pyx":317
  *         body = unpack_double(buffer_claim(buffer, sizeof(double)))
  *     elif type_code == TYPE_LIST0:
  *         body = []             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_LIST8:
  *         body = _decode_compound(_decode_list, _decode_compound_size8, buffer)
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 316, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 317, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":315
+    /* "rbfly/amqp/_message.pyx":316
  *     elif type_code == TYPE_DOUBLE:
  *         body = unpack_double(buffer_claim(buffer, sizeof(double)))
  *     elif type_code == TYPE_LIST0:             # <<<<<<<<<<<<<<
  *         body = []
  *     elif type_code == TYPE_LIST8:
  */
     break;
     case 0xC0:
 
-    /* "rbfly/amqp/_message.pyx":318
+    /* "rbfly/amqp/_message.pyx":319
  *         body = []
  *     elif type_code == TYPE_LIST8:
  *         body = _decode_compound(_decode_list, _decode_compound_size8, buffer)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_LIST32:
  *         body = _decode_compound(_decode_list, _decode_compound_size32, buffer)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_list, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size8, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 318, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_list, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size8, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":317
+    /* "rbfly/amqp/_message.pyx":318
  *     elif type_code == TYPE_LIST0:
  *         body = []
  *     elif type_code == TYPE_LIST8:             # <<<<<<<<<<<<<<
  *         body = _decode_compound(_decode_list, _decode_compound_size8, buffer)
  *     elif type_code == TYPE_LIST32:
  */
     break;
     case 0xD0:
 
-    /* "rbfly/amqp/_message.pyx":320
+    /* "rbfly/amqp/_message.pyx":321
  *         body = _decode_compound(_decode_list, _decode_compound_size8, buffer)
  *     elif type_code == TYPE_LIST32:
  *         body = _decode_compound(_decode_list, _decode_compound_size32, buffer)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_MAP8:
  *         body = _decode_compound(_decode_map, _decode_compound_size8, buffer)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_list, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size32, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 320, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_list, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size32, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":319
+    /* "rbfly/amqp/_message.pyx":320
  *     elif type_code == TYPE_LIST8:
  *         body = _decode_compound(_decode_list, _decode_compound_size8, buffer)
  *     elif type_code == TYPE_LIST32:             # <<<<<<<<<<<<<<
  *         body = _decode_compound(_decode_list, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_MAP8:
  */
     break;
     case 0xC1:
 
-    /* "rbfly/amqp/_message.pyx":322
+    /* "rbfly/amqp/_message.pyx":323
  *         body = _decode_compound(_decode_list, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_MAP8:
  *         body = _decode_compound(_decode_map, _decode_compound_size8, buffer)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_MAP32:
  *         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_map, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size8, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 322, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_map, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size8, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 323, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":321
+    /* "rbfly/amqp/_message.pyx":322
  *     elif type_code == TYPE_LIST32:
  *         body = _decode_compound(_decode_list, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_MAP8:             # <<<<<<<<<<<<<<
  *         body = _decode_compound(_decode_map, _decode_compound_size8, buffer)
  *     elif type_code == TYPE_MAP32:
  */
     break;
     case 0xD1:
 
-    /* "rbfly/amqp/_message.pyx":324
+    /* "rbfly/amqp/_message.pyx":325
  *         body = _decode_compound(_decode_map, _decode_compound_size8, buffer)
  *     elif type_code == TYPE_MAP32:
  *         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_TIMESTAMP:
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_map, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size32, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 324, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_compound(__pyx_f_5rbfly_4amqp_8_message__decode_map, __pyx_f_5rbfly_4amqp_8_message__decode_compound_size32, __pyx_v_buffer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 325, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_body = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":323
+    /* "rbfly/amqp/_message.pyx":324
  *     elif type_code == TYPE_MAP8:
  *         body = _decode_compound(_decode_map, _decode_compound_size8, buffer)
  *     elif type_code == TYPE_MAP32:             # <<<<<<<<<<<<<<
  *         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_TIMESTAMP:
  */
     break;
     case 0x83:
 
-    /* "rbfly/amqp/_message.pyx":326
+    /* "rbfly/amqp/_message.pyx":327
  *         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_TIMESTAMP:
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))             # <<<<<<<<<<<<<<
  *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
  *     elif type_code == TYPE_UUID:
  */
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 326, __pyx_L1_error)
-    __pyx_t_9 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 326, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 327, __pyx_L1_error)
     __pyx_v_ts = ((uint64_t)__pyx_t_9);
 
-    /* "rbfly/amqp/_message.pyx":327
+    /* "rbfly/amqp/_message.pyx":328
  *     elif type_code == TYPE_TIMESTAMP:
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_UUID:
  *         body = uuid.UUID(bytes=buffer_claim(buffer, 16)[:16])
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_utcfromtimestamp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_utcfromtimestamp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyFloat_FromDouble((((double)__pyx_v_ts) / 1000.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble((((double)__pyx_v_ts) / 1000.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_12 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -6513,106 +6529,106 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_3};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 327, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 328, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_replace); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_replace); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_timezone); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_timezone); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_utc); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_utc); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_tzinfo, __pyx_t_3) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_tzinfo, __pyx_t_3) < 0) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_body = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "rbfly/amqp/_message.pyx":325
+    /* "rbfly/amqp/_message.pyx":326
  *     elif type_code == TYPE_MAP32:
  *         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_TIMESTAMP:             # <<<<<<<<<<<<<<
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
  */
     break;
     case 0x98:
 
-    /* "rbfly/amqp/_message.pyx":329
+    /* "rbfly/amqp/_message.pyx":330
  *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
  *     elif type_code == TYPE_UUID:
  *         body = uuid.UUID(bytes=buffer_claim(buffer, 16)[:16])             # <<<<<<<<<<<<<<
  *     else:
  *         raise AMQPDecoderError(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_uuid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 329, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_uuid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_UUID); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 329, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_UUID); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 329, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 16); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 329, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_t_6 + 0, 16 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 329, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 16); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 330, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_t_6 + 0, 16 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_bytes, __pyx_t_2) < 0) __PYX_ERR(1, 329, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_bytes, __pyx_t_2) < 0) __PYX_ERR(1, 330, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 329, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_body = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "rbfly/amqp/_message.pyx":328
+    /* "rbfly/amqp/_message.pyx":329
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
  *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
  *     elif type_code == TYPE_UUID:             # <<<<<<<<<<<<<<
  *         body = uuid.UUID(bytes=buffer_claim(buffer, 16)[:16])
  *     else:
  */
     break;
     default:
 
-    /* "rbfly/amqp/_message.pyx":331
+    /* "rbfly/amqp/_message.pyx":332
  *         body = uuid.UUID(bytes=buffer_claim(buffer, 16)[:16])
  *     else:
  *         raise AMQPDecoderError(             # <<<<<<<<<<<<<<
  *             'Cannot decode message, type code=0x{:02x}'.format(type_code)
  *         )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 331, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 332, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "rbfly/amqp/_message.pyx":332
+    /* "rbfly/amqp/_message.pyx":333
  *     else:
  *         raise AMQPDecoderError(
  *             'Cannot decode message, type code=0x{:02x}'.format(type_code)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_type_code, __pyx_n_s_format); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 332, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_type_code, __pyx_n_s_format); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_13 = __Pyx_PyInt_From_uint8_t(__pyx_v_type_code); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 332, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_From_uint8_t(__pyx_v_type_code); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_14 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_12);
       if (likely(__pyx_t_14)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
@@ -6623,15 +6639,15 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_14, __pyx_t_13};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 332, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 333, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     }
     __pyx_t_12 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6644,37 +6660,37 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_1};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 331, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 332, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 331, __pyx_L1_error)
+    __PYX_ERR(1, 332, __pyx_L1_error)
     break;
   }
 
-  /* "rbfly/amqp/_message.pyx":335
+  /* "rbfly/amqp/_message.pyx":336
  *         )
  * 
  *     return body             # <<<<<<<<<<<<<<
  * 
  * cdef inline object _decode_compound(
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_body);
   __pyx_r = __pyx_v_body;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":270
+  /* "rbfly/amqp/_message.pyx":271
  *     desc_code[0] = dc >> 8
  * 
  * cdef inline object _decode_value(Buffer *buffer, uint8_t type_code):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object body
  */
 
@@ -6691,15 +6707,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_body);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":337
+/* "rbfly/amqp/_message.pyx":338
  *     return body
  * 
  * cdef inline object _decode_compound(             # <<<<<<<<<<<<<<
  *         t_func_decode_compound decode_compound,
  *         t_func_compound_size compound_size,
  */
 
@@ -6719,54 +6735,54 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_compound", 0);
 
-  /* "rbfly/amqp/_message.pyx":349
+  /* "rbfly/amqp/_message.pyx":350
  *         object result
  * 
  *     compound_size(buffer, &size, &count)             # <<<<<<<<<<<<<<
  *     if not buffer_check_size(buffer, size):
  *         raise AMQPDecoderError(
  */
-  __pyx_v_compound_size(__pyx_v_buffer, (&__pyx_v_size), (&__pyx_v_count)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L1_error)
+  __pyx_v_compound_size(__pyx_v_buffer, (&__pyx_v_size), (&__pyx_v_count)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 350, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":350
+  /* "rbfly/amqp/_message.pyx":351
  * 
  *     compound_size(buffer, &size, &count)
  *     if not buffer_check_size(buffer, size):             # <<<<<<<<<<<<<<
  *         raise AMQPDecoderError(
  *             'Invalid buffer size for a compound, size={}'.format(size)
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 350, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 351, __pyx_L1_error)
   __pyx_t_2 = (!(__pyx_t_1 != 0));
   if (unlikely(__pyx_t_2)) {
 
-    /* "rbfly/amqp/_message.pyx":351
+    /* "rbfly/amqp/_message.pyx":352
  *     compound_size(buffer, &size, &count)
  *     if not buffer_check_size(buffer, size):
  *         raise AMQPDecoderError(             # <<<<<<<<<<<<<<
  *             'Invalid buffer size for a compound, size={}'.format(size)
  *         )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 351, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 352, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
 
-    /* "rbfly/amqp/_message.pyx":352
+    /* "rbfly/amqp/_message.pyx":353
  *     if not buffer_check_size(buffer, size):
  *         raise AMQPDecoderError(
  *             'Invalid buffer size for a compound, size={}'.format(size)             # <<<<<<<<<<<<<<
  *         )
  *     result = decode_compound(buffer, size, count)
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_buffer_size_for_a_compou, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 352, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_buffer_size_for_a_compou, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 353, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 352, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 353, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -6777,15 +6793,15 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_7};
       __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 352, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 353, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_t_6 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
@@ -6798,56 +6814,56 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 351, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 352, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 351, __pyx_L1_error)
+    __PYX_ERR(1, 352, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":350
+    /* "rbfly/amqp/_message.pyx":351
  * 
  *     compound_size(buffer, &size, &count)
  *     if not buffer_check_size(buffer, size):             # <<<<<<<<<<<<<<
  *         raise AMQPDecoderError(
  *             'Invalid buffer size for a compound, size={}'.format(size)
  */
   }
 
-  /* "rbfly/amqp/_message.pyx":354
+  /* "rbfly/amqp/_message.pyx":355
  *             'Invalid buffer size for a compound, size={}'.format(size)
  *         )
  *     result = decode_compound(buffer, size, count)             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
-  __pyx_t_3 = __pyx_v_decode_compound(__pyx_v_buffer, __pyx_v_size, __pyx_v_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 354, __pyx_L1_error)
+  __pyx_t_3 = __pyx_v_decode_compound(__pyx_v_buffer, __pyx_v_size, __pyx_v_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "rbfly/amqp/_message.pyx":355
+  /* "rbfly/amqp/_message.pyx":356
  *         )
  *     result = decode_compound(buffer, size, count)
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cdef inline object _decode_list(Buffer *buffer, uint32_t size, uint32_t count):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":337
+  /* "rbfly/amqp/_message.pyx":338
  *     return body
  * 
  * cdef inline object _decode_compound(             # <<<<<<<<<<<<<<
  *         t_func_decode_compound decode_compound,
  *         t_func_compound_size compound_size,
  */
 
@@ -6864,15 +6880,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":357
+/* "rbfly/amqp/_message.pyx":358
  *     return result
  * 
  * cdef inline object _decode_list(Buffer *buffer, uint32_t size, uint32_t count):             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP list object.
  */
 
@@ -6890,83 +6906,83 @@
   uint8_t __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_list", 0);
 
-  /* "rbfly/amqp/_message.pyx":366
+  /* "rbfly/amqp/_message.pyx":367
  *         object value
  * 
  *         list result = []             # <<<<<<<<<<<<<<
  * 
  *     for i in range(count):
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 366, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "rbfly/amqp/_message.pyx":368
+  /* "rbfly/amqp/_message.pyx":369
  *         list result = []
  * 
  *     for i in range(count):             # <<<<<<<<<<<<<<
  *         type_code = buffer_get_uint8(buffer)
  *         value = _decode_value(buffer, type_code)
  */
   __pyx_t_2 = __pyx_v_count;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "rbfly/amqp/_message.pyx":369
+    /* "rbfly/amqp/_message.pyx":370
  * 
  *     for i in range(count):
  *         type_code = buffer_get_uint8(buffer)             # <<<<<<<<<<<<<<
  *         value = _decode_value(buffer, type_code)
  *         result.append(value)
  */
-    __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 369, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 370, __pyx_L1_error)
     __pyx_v_type_code = __pyx_t_5;
 
-    /* "rbfly/amqp/_message.pyx":370
+    /* "rbfly/amqp/_message.pyx":371
  *     for i in range(count):
  *         type_code = buffer_get_uint8(buffer)
  *         value = _decode_value(buffer, type_code)             # <<<<<<<<<<<<<<
  *         result.append(value)
  * 
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 370, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 371, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":371
+    /* "rbfly/amqp/_message.pyx":372
  *         type_code = buffer_get_uint8(buffer)
  *         value = _decode_value(buffer, type_code)
  *         result.append(value)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_value); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 371, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_value); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 372, __pyx_L1_error)
   }
 
-  /* "rbfly/amqp/_message.pyx":373
+  /* "rbfly/amqp/_message.pyx":374
  *         result.append(value)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cdef inline object _decode_map(Buffer *buffer, uint32_t size, uint32_t count):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":357
+  /* "rbfly/amqp/_message.pyx":358
  *     return result
  * 
  * cdef inline object _decode_list(Buffer *buffer, uint32_t size, uint32_t count):             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP list object.
  */
 
@@ -6979,15 +6995,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":375
+/* "rbfly/amqp/_message.pyx":376
  *     return result
  * 
  * cdef inline object _decode_map(Buffer *buffer, uint32_t size, uint32_t count):             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP map object.
  */
 
@@ -7012,48 +7028,48 @@
   Py_ssize_t __pyx_t_11;
   uint8_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_map", 0);
 
-  /* "rbfly/amqp/_message.pyx":384
+  /* "rbfly/amqp/_message.pyx":385
  *         object key, value
  * 
  *         dict result = {}             # <<<<<<<<<<<<<<
  * 
  *     if count % 2 == 1:
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 384, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 385, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "rbfly/amqp/_message.pyx":386
+  /* "rbfly/amqp/_message.pyx":387
  *         dict result = {}
  * 
  *     if count % 2 == 1:             # <<<<<<<<<<<<<<
  *         raise AMQPDecoderError('AMQP map invalid count, count={}'.format(count))
  * 
  */
   __pyx_t_2 = (__Pyx_mod_long(__pyx_v_count, 2) == 1);
   if (unlikely(__pyx_t_2)) {
 
-    /* "rbfly/amqp/_message.pyx":387
+    /* "rbfly/amqp/_message.pyx":388
  * 
  *     if count % 2 == 1:
  *         raise AMQPDecoderError('AMQP map invalid count, count={}'.format(count))             # <<<<<<<<<<<<<<
  * 
  *     for i in range(0, count, 2):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 387, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_AMQP_map_invalid_count_count, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 387, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_AMQP_map_invalid_count_count, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_count); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 387, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint32_t(__pyx_v_count); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -7064,15 +7080,15 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 387, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 388, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_t_5 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
@@ -7085,110 +7101,110 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 387, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 388, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(1, 387, __pyx_L1_error)
+    __PYX_ERR(1, 388, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":386
+    /* "rbfly/amqp/_message.pyx":387
  *         dict result = {}
  * 
  *     if count % 2 == 1:             # <<<<<<<<<<<<<<
  *         raise AMQPDecoderError('AMQP map invalid count, count={}'.format(count))
  * 
  */
   }
 
-  /* "rbfly/amqp/_message.pyx":389
+  /* "rbfly/amqp/_message.pyx":390
  *         raise AMQPDecoderError('AMQP map invalid count, count={}'.format(count))
  * 
  *     for i in range(0, count, 2):             # <<<<<<<<<<<<<<
  *         type_code = buffer_get_uint8(buffer)
  *         key = _decode_value(buffer, type_code)
  */
   __pyx_t_9 = __pyx_v_count;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=2) {
     __pyx_v_i = __pyx_t_11;
 
-    /* "rbfly/amqp/_message.pyx":390
+    /* "rbfly/amqp/_message.pyx":391
  * 
  *     for i in range(0, count, 2):
  *         type_code = buffer_get_uint8(buffer)             # <<<<<<<<<<<<<<
  *         key = _decode_value(buffer, type_code)
  * 
  */
-    __pyx_t_12 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 390, __pyx_L1_error)
+    __pyx_t_12 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 391, __pyx_L1_error)
     __pyx_v_type_code = __pyx_t_12;
 
-    /* "rbfly/amqp/_message.pyx":391
+    /* "rbfly/amqp/_message.pyx":392
  *     for i in range(0, count, 2):
  *         type_code = buffer_get_uint8(buffer)
  *         key = _decode_value(buffer, type_code)             # <<<<<<<<<<<<<<
  * 
  *         type_code = buffer_get_uint8(buffer)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 391, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":393
+    /* "rbfly/amqp/_message.pyx":394
  *         key = _decode_value(buffer, type_code)
  * 
  *         type_code = buffer_get_uint8(buffer)             # <<<<<<<<<<<<<<
  *         value = _decode_value(buffer, type_code)
  * 
  */
-    __pyx_t_12 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L1_error)
+    __pyx_t_12 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 394, __pyx_L1_error)
     __pyx_v_type_code = __pyx_t_12;
 
-    /* "rbfly/amqp/_message.pyx":394
+    /* "rbfly/amqp/_message.pyx":395
  * 
  *         type_code = buffer_get_uint8(buffer)
  *         value = _decode_value(buffer, type_code)             # <<<<<<<<<<<<<<
  * 
  *         result[key] = value
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 394, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__decode_value(__pyx_v_buffer, __pyx_v_type_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 395, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "rbfly/amqp/_message.pyx":396
+    /* "rbfly/amqp/_message.pyx":397
  *         value = _decode_value(buffer, type_code)
  * 
  *         result[key] = value             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
-    if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_v_key, __pyx_v_value) < 0))) __PYX_ERR(1, 396, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_result, __pyx_v_key, __pyx_v_value) < 0))) __PYX_ERR(1, 397, __pyx_L1_error)
   }
 
-  /* "rbfly/amqp/_message.pyx":398
+  /* "rbfly/amqp/_message.pyx":399
  *         result[key] = value
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cdef inline object _decode_strb(
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":375
+  /* "rbfly/amqp/_message.pyx":376
  *     return result
  * 
  * cdef inline object _decode_map(Buffer *buffer, uint32_t size, uint32_t count):             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP map object.
  */
 
@@ -7207,15 +7223,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":400
+/* "rbfly/amqp/_message.pyx":401
  *     return result
  * 
  * cdef inline object _decode_strb(             # <<<<<<<<<<<<<<
  *         t_func_strb_size strb_size,
  *         Buffer *buffer,
  */
 
@@ -7239,93 +7255,93 @@
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_strb", 0);
 
-  /* "rbfly/amqp/_message.pyx":408
+  /* "rbfly/amqp/_message.pyx":409
  *         uint32_t size, end
  *         object result
  *         Py_ssize_t offset = buffer[0].offset             # <<<<<<<<<<<<<<
  *         char *buff = buffer[0].buffer
  * 
  */
   __pyx_t_1 = (__pyx_v_buffer[0]).offset;
   __pyx_v_offset = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":409
+  /* "rbfly/amqp/_message.pyx":410
  *         object result
  *         Py_ssize_t offset = buffer[0].offset
  *         char *buff = buffer[0].buffer             # <<<<<<<<<<<<<<
  * 
  *     strb_size(buffer, &size)
  */
   __pyx_t_2 = (__pyx_v_buffer[0]).buffer;
   __pyx_v_buff = __pyx_t_2;
 
-  /* "rbfly/amqp/_message.pyx":411
+  /* "rbfly/amqp/_message.pyx":412
  *         char *buff = buffer[0].buffer
  * 
  *     strb_size(buffer, &size)             # <<<<<<<<<<<<<<
  *     offset = buffer[0].offset
  *     end = offset + size
  */
-  __pyx_v_strb_size(__pyx_v_buffer, (&__pyx_v_size)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 411, __pyx_L1_error)
+  __pyx_v_strb_size(__pyx_v_buffer, (&__pyx_v_size)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 412, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":412
+  /* "rbfly/amqp/_message.pyx":413
  * 
  *     strb_size(buffer, &size)
  *     offset = buffer[0].offset             # <<<<<<<<<<<<<<
  *     end = offset + size
  * 
  */
   __pyx_t_1 = (__pyx_v_buffer[0]).offset;
   __pyx_v_offset = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":413
+  /* "rbfly/amqp/_message.pyx":414
  *     strb_size(buffer, &size)
  *     offset = buffer[0].offset
  *     end = offset + size             # <<<<<<<<<<<<<<
  * 
  *     if not buffer_check_size(buffer, size):
  */
   __pyx_v_end = (__pyx_v_offset + __pyx_v_size);
 
-  /* "rbfly/amqp/_message.pyx":415
+  /* "rbfly/amqp/_message.pyx":416
  *     end = offset + size
  * 
  *     if not buffer_check_size(buffer, size):             # <<<<<<<<<<<<<<
  *         raise AMQPDecoderError(
  *             'Invalid string or bytes size, size={}'.format(size)
  */
-  __pyx_t_3 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 415, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 416, __pyx_L1_error)
   __pyx_t_4 = (!(__pyx_t_3 != 0));
   if (unlikely(__pyx_t_4)) {
 
-    /* "rbfly/amqp/_message.pyx":416
+    /* "rbfly/amqp/_message.pyx":417
  * 
  *     if not buffer_check_size(buffer, size):
  *         raise AMQPDecoderError(             # <<<<<<<<<<<<<<
  *             'Invalid string or bytes size, size={}'.format(size)
  *         )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 416, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "rbfly/amqp/_message.pyx":417
+    /* "rbfly/amqp/_message.pyx":418
  *     if not buffer_check_size(buffer, size):
  *         raise AMQPDecoderError(
  *             'Invalid string or bytes size, size={}'.format(size)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_string_or_bytes_size_siz, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 417, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_string_or_bytes_size_siz, __pyx_n_s_format); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 417, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_10 = NULL;
     __pyx_t_11 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -7336,15 +7352,15 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_9};
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 417, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __pyx_t_8 = NULL;
     __pyx_t_11 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
@@ -7357,103 +7373,103 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_7};
       __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 416, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(1, 416, __pyx_L1_error)
+    __PYX_ERR(1, 417, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":415
+    /* "rbfly/amqp/_message.pyx":416
  *     end = offset + size
  * 
  *     if not buffer_check_size(buffer, size):             # <<<<<<<<<<<<<<
  *         raise AMQPDecoderError(
  *             'Invalid string or bytes size, size={}'.format(size)
  */
   }
 
-  /* "rbfly/amqp/_message.pyx":420
+  /* "rbfly/amqp/_message.pyx":421
  *         )
  * 
  *     if type_code % 2 == 1:             # <<<<<<<<<<<<<<
  *         result = buff[offset:end].decode('utf-8')
  *     else:
  */
   __pyx_t_4 = (__Pyx_mod_long(__pyx_v_type_code, 2) == 1);
   if (__pyx_t_4) {
 
-    /* "rbfly/amqp/_message.pyx":421
+    /* "rbfly/amqp/_message.pyx":422
  * 
  *     if type_code % 2 == 1:
  *         result = buff[offset:end].decode('utf-8')             # <<<<<<<<<<<<<<
  *     else:
  *         result = <bytes> buff[offset:end]
  */
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_v_buff, __pyx_v_offset, __pyx_v_end, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 421, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_v_buff, __pyx_v_offset, __pyx_v_end, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_v_result = __pyx_t_5;
     __pyx_t_5 = 0;
 
-    /* "rbfly/amqp/_message.pyx":420
+    /* "rbfly/amqp/_message.pyx":421
  *         )
  * 
  *     if type_code % 2 == 1:             # <<<<<<<<<<<<<<
  *         result = buff[offset:end].decode('utf-8')
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "rbfly/amqp/_message.pyx":423
+  /* "rbfly/amqp/_message.pyx":424
  *         result = buff[offset:end].decode('utf-8')
  *     else:
  *         result = <bytes> buff[offset:end]             # <<<<<<<<<<<<<<
  * 
  *     buffer[0].offset = end
  */
   /*else*/ {
-    __pyx_t_5 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buff + __pyx_v_offset, __pyx_v_end - __pyx_v_offset); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 423, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buff + __pyx_v_offset, __pyx_v_end - __pyx_v_offset); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = __pyx_t_5;
     __Pyx_INCREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_result = __pyx_t_6;
     __pyx_t_6 = 0;
   }
   __pyx_L4:;
 
-  /* "rbfly/amqp/_message.pyx":425
+  /* "rbfly/amqp/_message.pyx":426
  *         result = <bytes> buff[offset:end]
  * 
  *     buffer[0].offset = end             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   (__pyx_v_buffer[0]).offset = __pyx_v_end;
 
-  /* "rbfly/amqp/_message.pyx":426
+  /* "rbfly/amqp/_message.pyx":427
  * 
  *     buffer[0].offset = end
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _decode_size8(Buffer *buffer, uint32_t *size):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":400
+  /* "rbfly/amqp/_message.pyx":401
  *     return result
  * 
  * cdef inline object _decode_strb(             # <<<<<<<<<<<<<<
  *         t_func_strb_size strb_size,
  *         Buffer *buffer,
  */
 
@@ -7470,15 +7486,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":428
+/* "rbfly/amqp/_message.pyx":429
  *     return result
  * 
  * cdef inline void _decode_size8(Buffer *buffer, uint32_t *size):             # <<<<<<<<<<<<<<
  *     size[0] = buffer_get_uint8(buffer)
  * 
  */
 
@@ -7486,25 +7502,25 @@
   __Pyx_RefNannyDeclarations
   uint8_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_size8", 0);
 
-  /* "rbfly/amqp/_message.pyx":429
+  /* "rbfly/amqp/_message.pyx":430
  * 
  * cdef inline void _decode_size8(Buffer *buffer, uint32_t *size):
  *     size[0] = buffer_get_uint8(buffer)             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _decode_size32(Buffer *buffer, uint32_t *size):
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 429, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 430, __pyx_L1_error)
   (__pyx_v_size[0]) = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":428
+  /* "rbfly/amqp/_message.pyx":429
  *     return result
  * 
  * cdef inline void _decode_size8(Buffer *buffer, uint32_t *size):             # <<<<<<<<<<<<<<
  *     size[0] = buffer_get_uint8(buffer)
  * 
  */
 
@@ -7512,15 +7528,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.amqp._message._decode_size8", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbfly/amqp/_message.pyx":431
+/* "rbfly/amqp/_message.pyx":432
  *     size[0] = buffer_get_uint8(buffer)
  * 
  * cdef inline void _decode_size32(Buffer *buffer, uint32_t *size):             # <<<<<<<<<<<<<<
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  * 
  */
 
@@ -7529,26 +7545,26 @@
   char *__pyx_t_1;
   uint32_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_size32", 0);
 
-  /* "rbfly/amqp/_message.pyx":432
+  /* "rbfly/amqp/_message.pyx":433
  * 
  * cdef inline void _decode_size32(Buffer *buffer, uint32_t *size):
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _decode_compound_size8(Buffer *buffer, uint32_t *size, uint32_t *count):
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 432, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 432, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 433, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 433, __pyx_L1_error)
   (__pyx_v_size[0]) = __pyx_t_2;
 
-  /* "rbfly/amqp/_message.pyx":431
+  /* "rbfly/amqp/_message.pyx":432
  *     size[0] = buffer_get_uint8(buffer)
  * 
  * cdef inline void _decode_size32(Buffer *buffer, uint32_t *size):             # <<<<<<<<<<<<<<
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  * 
  */
 
@@ -7556,15 +7572,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.amqp._message._decode_size32", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbfly/amqp/_message.pyx":434
+/* "rbfly/amqp/_message.pyx":435
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  * 
  * cdef inline void _decode_compound_size8(Buffer *buffer, uint32_t *size, uint32_t *count):             # <<<<<<<<<<<<<<
  *     size[0] = buffer_get_uint8(buffer)
  *     count[0] = buffer_get_uint8(buffer)
  */
 
@@ -7572,35 +7588,35 @@
   __Pyx_RefNannyDeclarations
   uint8_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_compound_size8", 0);
 
-  /* "rbfly/amqp/_message.pyx":435
+  /* "rbfly/amqp/_message.pyx":436
  * 
  * cdef inline void _decode_compound_size8(Buffer *buffer, uint32_t *size, uint32_t *count):
  *     size[0] = buffer_get_uint8(buffer)             # <<<<<<<<<<<<<<
  *     count[0] = buffer_get_uint8(buffer)
  * 
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 435, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 436, __pyx_L1_error)
   (__pyx_v_size[0]) = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":436
+  /* "rbfly/amqp/_message.pyx":437
  * cdef inline void _decode_compound_size8(Buffer *buffer, uint32_t *size, uint32_t *count):
  *     size[0] = buffer_get_uint8(buffer)
  *     count[0] = buffer_get_uint8(buffer)             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _decode_compound_size32(Buffer *buffer, uint32_t *size, uint32_t *count):
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 436, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_get_uint8(__pyx_v_buffer); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 437, __pyx_L1_error)
   (__pyx_v_count[0]) = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":434
+  /* "rbfly/amqp/_message.pyx":435
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  * 
  * cdef inline void _decode_compound_size8(Buffer *buffer, uint32_t *size, uint32_t *count):             # <<<<<<<<<<<<<<
  *     size[0] = buffer_get_uint8(buffer)
  *     count[0] = buffer_get_uint8(buffer)
  */
 
@@ -7608,15 +7624,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.amqp._message._decode_compound_size8", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbfly/amqp/_message.pyx":438
+/* "rbfly/amqp/_message.pyx":439
  *     count[0] = buffer_get_uint8(buffer)
  * 
  * cdef inline void _decode_compound_size32(Buffer *buffer, uint32_t *size, uint32_t *count):             # <<<<<<<<<<<<<<
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     count[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  */
 
@@ -7625,37 +7641,37 @@
   char *__pyx_t_1;
   uint32_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_compound_size32", 0);
 
-  /* "rbfly/amqp/_message.pyx":439
+  /* "rbfly/amqp/_message.pyx":440
  * 
  * cdef inline void _decode_compound_size32(Buffer *buffer, uint32_t *size, uint32_t *count):
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))             # <<<<<<<<<<<<<<
  *     count[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  * 
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 439, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 439, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 440, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 440, __pyx_L1_error)
   (__pyx_v_size[0]) = __pyx_t_2;
 
-  /* "rbfly/amqp/_message.pyx":440
+  /* "rbfly/amqp/_message.pyx":441
  * cdef inline void _decode_compound_size32(Buffer *buffer, uint32_t *size, uint32_t *count):
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     count[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))             # <<<<<<<<<<<<<<
  * 
  * #
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 440, __pyx_L1_error)
-  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 440, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 441, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 441, __pyx_L1_error)
   (__pyx_v_count[0]) = __pyx_t_2;
 
-  /* "rbfly/amqp/_message.pyx":438
+  /* "rbfly/amqp/_message.pyx":439
  *     count[0] = buffer_get_uint8(buffer)
  * 
  * cdef inline void _decode_compound_size32(Buffer *buffer, uint32_t *size, uint32_t *count):             # <<<<<<<<<<<<<<
  *     size[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  *     count[0] = unpack_uint32(buffer_claim(buffer, sizeof(uint32_t)))
  */
 
@@ -7663,15 +7679,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.amqp._message._decode_compound_size32", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbfly/amqp/_message.pyx":446
+/* "rbfly/amqp/_message.pyx":447
  * #
  * 
  * cdef Py_ssize_t c_encode_amqp(Buffer *buffer, object message) except -1:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Py_ssize_t start = buffer.offset
  */
 
@@ -7687,180 +7703,180 @@
   int __pyx_t_3;
   char *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("c_encode_amqp", 0);
 
-  /* "rbfly/amqp/_message.pyx":448
+  /* "rbfly/amqp/_message.pyx":449
  * cdef Py_ssize_t c_encode_amqp(Buffer *buffer, object message) except -1:
  *     cdef:
  *         Py_ssize_t start = buffer.offset             # <<<<<<<<<<<<<<
  *         object body = (<MessageCtx> message).body
  * 
  */
   __pyx_t_1 = __pyx_v_buffer->offset;
   __pyx_v_start = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":449
+  /* "rbfly/amqp/_message.pyx":450
  *     cdef:
  *         Py_ssize_t start = buffer.offset
  *         object body = (<MessageCtx> message).body             # <<<<<<<<<<<<<<
  * 
  *         char *bp
  */
   __pyx_t_2 = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_v_message)->body;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_body = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "rbfly/amqp/_message.pyx":454
+  /* "rbfly/amqp/_message.pyx":455
  *         Py_ssize_t size
  * 
  *     if message.app_properties:             # <<<<<<<<<<<<<<
  *         # need 3 bytes to encode the amqp app properties descriptor
  *         bp = buffer_claim(buffer, 3)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_message, __pyx_n_s_app_properties); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 454, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_message, __pyx_n_s_app_properties); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(1, 454, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(1, 455, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
 
-    /* "rbfly/amqp/_message.pyx":456
+    /* "rbfly/amqp/_message.pyx":457
  *     if message.app_properties:
  *         # need 3 bytes to encode the amqp app properties descriptor
  *         bp = buffer_claim(buffer, 3)             # <<<<<<<<<<<<<<
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_APP_PROPERTIES)
  *         _encode_dict(buffer, message.app_properties)
  */
-    __pyx_t_4 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 456, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 457, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_4;
 
-    /* "rbfly/amqp/_message.pyx":457
+    /* "rbfly/amqp/_message.pyx":458
  *         # need 3 bytes to encode the amqp app properties descriptor
  *         bp = buffer_claim(buffer, 3)
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_APP_PROPERTIES)             # <<<<<<<<<<<<<<
  *         _encode_dict(buffer, message.app_properties)
  * 
  */
-    __pyx_f_5rbfly_4amqp_8_message__encode_descriptor(__pyx_v_bp, 0x74); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 457, __pyx_L1_error)
+    __pyx_f_5rbfly_4amqp_8_message__encode_descriptor(__pyx_v_bp, 0x74); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 458, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":458
+    /* "rbfly/amqp/_message.pyx":459
  *         bp = buffer_claim(buffer, 3)
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_APP_PROPERTIES)
  *         _encode_dict(buffer, message.app_properties)             # <<<<<<<<<<<<<<
  * 
  *     # need 3 bytes to encode the amqp message descriptor
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_message, __pyx_n_s_app_properties); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 458, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_message, __pyx_n_s_app_properties); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 459, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_dict(__pyx_v_buffer, __pyx_t_2); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 458, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_dict(__pyx_v_buffer, __pyx_t_2); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 459, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "rbfly/amqp/_message.pyx":454
+    /* "rbfly/amqp/_message.pyx":455
  *         Py_ssize_t size
  * 
  *     if message.app_properties:             # <<<<<<<<<<<<<<
  *         # need 3 bytes to encode the amqp app properties descriptor
  *         bp = buffer_claim(buffer, 3)
  */
   }
 
-  /* "rbfly/amqp/_message.pyx":461
+  /* "rbfly/amqp/_message.pyx":462
  * 
  *     # need 3 bytes to encode the amqp message descriptor
  *     bp = buffer_claim(buffer, 3)             # <<<<<<<<<<<<<<
  *     if PyBytes_CheckExact(body):
  *         size = len(body)
  */
-  __pyx_t_4 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 461, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 462, __pyx_L1_error)
   __pyx_v_bp = __pyx_t_4;
 
-  /* "rbfly/amqp/_message.pyx":462
+  /* "rbfly/amqp/_message.pyx":463
  *     # need 3 bytes to encode the amqp message descriptor
  *     bp = buffer_claim(buffer, 3)
  *     if PyBytes_CheckExact(body):             # <<<<<<<<<<<<<<
  *         size = len(body)
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_BINARY)
  */
   __pyx_t_3 = PyBytes_CheckExact(__pyx_v_body);
   if (__pyx_t_3) {
 
-    /* "rbfly/amqp/_message.pyx":463
+    /* "rbfly/amqp/_message.pyx":464
  *     bp = buffer_claim(buffer, 3)
  *     if PyBytes_CheckExact(body):
  *         size = len(body)             # <<<<<<<<<<<<<<
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_BINARY)
  *         _encode_strb(buffer, body, size, TYPE_BINARY_SHORT, TYPE_BINARY_LONG)
  */
-    __pyx_t_1 = PyObject_Length(__pyx_v_body); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 463, __pyx_L1_error)
+    __pyx_t_1 = PyObject_Length(__pyx_v_body); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 464, __pyx_L1_error)
     __pyx_v_size = __pyx_t_1;
 
-    /* "rbfly/amqp/_message.pyx":464
+    /* "rbfly/amqp/_message.pyx":465
  *     if PyBytes_CheckExact(body):
  *         size = len(body)
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_BINARY)             # <<<<<<<<<<<<<<
  *         _encode_strb(buffer, body, size, TYPE_BINARY_SHORT, TYPE_BINARY_LONG)
  *     else:
  */
-    __pyx_f_5rbfly_4amqp_8_message__encode_descriptor(__pyx_v_bp, 0x75); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 464, __pyx_L1_error)
+    __pyx_f_5rbfly_4amqp_8_message__encode_descriptor(__pyx_v_bp, 0x75); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 465, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":465
+    /* "rbfly/amqp/_message.pyx":466
  *         size = len(body)
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_BINARY)
  *         _encode_strb(buffer, body, size, TYPE_BINARY_SHORT, TYPE_BINARY_LONG)             # <<<<<<<<<<<<<<
  *     else:
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_VALUE)
  */
-    __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_v_body); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 465, __pyx_L1_error)
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_4, __pyx_v_size, 0xA0, 0xB0); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 465, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_v_body); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 466, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_4, __pyx_v_size, 0xA0, 0xB0); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 466, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":462
+    /* "rbfly/amqp/_message.pyx":463
  *     # need 3 bytes to encode the amqp message descriptor
  *     bp = buffer_claim(buffer, 3)
  *     if PyBytes_CheckExact(body):             # <<<<<<<<<<<<<<
  *         size = len(body)
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_BINARY)
  */
     goto __pyx_L4;
   }
 
-  /* "rbfly/amqp/_message.pyx":467
+  /* "rbfly/amqp/_message.pyx":468
  *         _encode_strb(buffer, body, size, TYPE_BINARY_SHORT, TYPE_BINARY_LONG)
  *     else:
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_VALUE)             # <<<<<<<<<<<<<<
  *         _encode_value(buffer, body)
  * 
  */
   /*else*/ {
-    __pyx_f_5rbfly_4amqp_8_message__encode_descriptor(__pyx_v_bp, 0x77); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 467, __pyx_L1_error)
+    __pyx_f_5rbfly_4amqp_8_message__encode_descriptor(__pyx_v_bp, 0x77); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 468, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":468
+    /* "rbfly/amqp/_message.pyx":469
  *     else:
  *         _encode_descriptor(bp, DESCRIPTOR_MESSAGE_VALUE)
  *         _encode_value(buffer, body)             # <<<<<<<<<<<<<<
  * 
  *     return buffer.offset - start
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_body); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 468, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_body); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 469, __pyx_L1_error)
   }
   __pyx_L4:;
 
-  /* "rbfly/amqp/_message.pyx":470
+  /* "rbfly/amqp/_message.pyx":471
  *         _encode_value(buffer, body)
  * 
  *     return buffer.offset - start             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _encode_descriptor(char *buffer, unsigned char code):
  */
   __pyx_r = (__pyx_v_buffer->offset - __pyx_v_start);
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":446
+  /* "rbfly/amqp/_message.pyx":447
  * #
  * 
  * cdef Py_ssize_t c_encode_amqp(Buffer *buffer, object message) except -1:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Py_ssize_t start = buffer.offset
  */
 
@@ -7871,66 +7887,66 @@
   __pyx_r = -1L;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_body);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":472
+/* "rbfly/amqp/_message.pyx":473
  *     return buffer.offset - start
  * 
  * cdef inline void _encode_descriptor(char *buffer, unsigned char code):             # <<<<<<<<<<<<<<
  *     """
  *     Encode start of AMQP descriptor.
  */
 
 static CYTHON_INLINE void __pyx_f_5rbfly_4amqp_8_message__encode_descriptor(char *__pyx_v_buffer, unsigned char __pyx_v_code) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_encode_descriptor", 0);
 
-  /* "rbfly/amqp/_message.pyx":479
+  /* "rbfly/amqp/_message.pyx":480
  *     :param code: AMQP descriptor code.
  *     """
  *     buffer[0] = DESCRIPTOR_START             # <<<<<<<<<<<<<<
  *     buffer[1] = TYPE_SMALLULONG
  *     buffer[2] = code
  */
   (__pyx_v_buffer[0]) = 0;
 
-  /* "rbfly/amqp/_message.pyx":480
+  /* "rbfly/amqp/_message.pyx":481
  *     """
  *     buffer[0] = DESCRIPTOR_START
  *     buffer[1] = TYPE_SMALLULONG             # <<<<<<<<<<<<<<
  *     buffer[2] = code
  * 
  */
   (__pyx_v_buffer[1]) = 83;
 
-  /* "rbfly/amqp/_message.pyx":481
+  /* "rbfly/amqp/_message.pyx":482
  *     buffer[0] = DESCRIPTOR_START
  *     buffer[1] = TYPE_SMALLULONG
  *     buffer[2] = code             # <<<<<<<<<<<<<<
  * 
  * cdef inline Py_ssize_t _encode_value(Buffer *buffer, object value) except -1:
  */
   (__pyx_v_buffer[2]) = __pyx_v_code;
 
-  /* "rbfly/amqp/_message.pyx":472
+  /* "rbfly/amqp/_message.pyx":473
  *     return buffer.offset - start
  * 
  * cdef inline void _encode_descriptor(char *buffer, unsigned char code):             # <<<<<<<<<<<<<<
  *     """
  *     Encode start of AMQP descriptor.
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbfly/amqp/_message.pyx":483
+/* "rbfly/amqp/_message.pyx":484
  *     buffer[2] = code
  * 
  * cdef inline Py_ssize_t _encode_value(Buffer *buffer, object value) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Encode Python object into AMQP format.
  */
 
@@ -7954,42 +7970,42 @@
   uint64_t __pyx_t_12;
   double __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_encode_value", 0);
 
-  /* "rbfly/amqp/_message.pyx":488
+  /* "rbfly/amqp/_message.pyx":489
  *     """
  *     cdef:
  *         Py_ssize_t start = buffer.offset             # <<<<<<<<<<<<<<
  *         bytes value_bin
  *         char *bp
  */
   __pyx_t_1 = __pyx_v_buffer->offset;
   __pyx_v_start = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":492
+  /* "rbfly/amqp/_message.pyx":493
  *         char *bp
  * 
  *     if PyUnicode_CheckExact(value):             # <<<<<<<<<<<<<<
  *         value_bin = value.encode('utf-8')
  *         _encode_strb(
  */
   __pyx_t_2 = PyUnicode_CheckExact(__pyx_v_value);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":493
+    /* "rbfly/amqp/_message.pyx":494
  * 
  *     if PyUnicode_CheckExact(value):
  *         value_bin = value.encode('utf-8')             # <<<<<<<<<<<<<<
  *         _encode_strb(
  *             buffer,
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 493, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7999,343 +8015,343 @@
         __pyx_t_6 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_kp_u_utf_8};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 493, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 494, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_3))) __PYX_ERR(1, 493, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_3))) __PYX_ERR(1, 494, __pyx_L1_error)
     __pyx_v_value_bin = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "rbfly/amqp/_message.pyx":496
+    /* "rbfly/amqp/_message.pyx":497
  *         _encode_strb(
  *             buffer,
  *             value_bin,             # <<<<<<<<<<<<<<
  *             len(value_bin),
  *             TYPE_STRING_SHORT,
  */
     if (unlikely(__pyx_v_value_bin == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(1, 496, __pyx_L1_error)
+      __PYX_ERR(1, 497, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_value_bin); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 496, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_value_bin); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 497, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":497
+    /* "rbfly/amqp/_message.pyx":498
  *             buffer,
  *             value_bin,
  *             len(value_bin),             # <<<<<<<<<<<<<<
  *             TYPE_STRING_SHORT,
  *             TYPE_STRING_LONG
  */
     if (unlikely(__pyx_v_value_bin == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(1, 497, __pyx_L1_error)
+      __PYX_ERR(1, 498, __pyx_L1_error)
     }
-    __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_value_bin); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 497, __pyx_L1_error)
+    __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_value_bin); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 498, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":494
+    /* "rbfly/amqp/_message.pyx":495
  *     if PyUnicode_CheckExact(value):
  *         value_bin = value.encode('utf-8')
  *         _encode_strb(             # <<<<<<<<<<<<<<
  *             buffer,
  *             value_bin,
  */
-    __pyx_t_8 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_7, __pyx_t_1, 0xA1, 0xB1); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 494, __pyx_L1_error)
+    __pyx_t_8 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_7, __pyx_t_1, 0xA1, 0xB1); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 495, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":492
+    /* "rbfly/amqp/_message.pyx":493
  *         char *bp
  * 
  *     if PyUnicode_CheckExact(value):             # <<<<<<<<<<<<<<
  *         value_bin = value.encode('utf-8')
  *         _encode_strb(
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":501
+  /* "rbfly/amqp/_message.pyx":502
  *             TYPE_STRING_LONG
  *         )
  *     elif PyBytes_CheckExact(value):             # <<<<<<<<<<<<<<
  *         _encode_strb(
  *             buffer,
  */
   __pyx_t_2 = PyBytes_CheckExact(__pyx_v_value);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":504
+    /* "rbfly/amqp/_message.pyx":505
  *         _encode_strb(
  *             buffer,
  *             value,             # <<<<<<<<<<<<<<
  *             len(value),
  *             TYPE_BINARY_SHORT,
  */
-    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 504, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 505, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":505
+    /* "rbfly/amqp/_message.pyx":506
  *             buffer,
  *             value,
  *             len(value),             # <<<<<<<<<<<<<<
  *             TYPE_BINARY_SHORT,
  *             TYPE_BINARY_LONG
  */
-    __pyx_t_8 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 505, __pyx_L1_error)
+    __pyx_t_8 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 506, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":502
+    /* "rbfly/amqp/_message.pyx":503
  *         )
  *     elif PyBytes_CheckExact(value):
  *         _encode_strb(             # <<<<<<<<<<<<<<
  *             buffer,
  *             value,
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_7, __pyx_t_8, 0xA0, 0xB0); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 502, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_7, __pyx_t_8, 0xA0, 0xB0); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 503, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":501
+    /* "rbfly/amqp/_message.pyx":502
  *             TYPE_STRING_LONG
  *         )
  *     elif PyBytes_CheckExact(value):             # <<<<<<<<<<<<<<
  *         _encode_strb(
  *             buffer,
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":509
+  /* "rbfly/amqp/_message.pyx":510
  *             TYPE_BINARY_LONG
  *         )
  *     elif PyBool_Check(value):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 1)
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE
  */
   __pyx_t_2 = PyBool_Check(__pyx_v_value);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":510
+    /* "rbfly/amqp/_message.pyx":511
  *         )
  *     elif PyBool_Check(value):
  *         bp = buffer_claim(buffer, 1)             # <<<<<<<<<<<<<<
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE
  *     elif PyLong_CheckExact(value):
  */
-    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 510, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 511, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_7;
 
-    /* "rbfly/amqp/_message.pyx":511
+    /* "rbfly/amqp/_message.pyx":512
  *     elif PyBool_Check(value):
  *         bp = buffer_claim(buffer, 1)
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE             # <<<<<<<<<<<<<<
  *     elif PyLong_CheckExact(value):
  *         if MIN_INT <= value <= MAX_INT:
  */
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 511, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     if (__pyx_t_2) {
       __pyx_t_9 = 65;
     } else {
       __pyx_t_9 = 66;
     }
     (__pyx_v_bp[0]) = __pyx_t_9;
 
-    /* "rbfly/amqp/_message.pyx":509
+    /* "rbfly/amqp/_message.pyx":510
  *             TYPE_BINARY_LONG
  *         )
  *     elif PyBool_Check(value):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 1)
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":512
+  /* "rbfly/amqp/_message.pyx":513
  *         bp = buffer_claim(buffer, 1)
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE
  *     elif PyLong_CheckExact(value):             # <<<<<<<<<<<<<<
  *         if MIN_INT <= value <= MAX_INT:
  *             bp = buffer_claim(buffer, 1 + sizeof(int32_t))
  */
   __pyx_t_2 = PyLong_CheckExact(__pyx_v_value);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":513
+    /* "rbfly/amqp/_message.pyx":514
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE
  *     elif PyLong_CheckExact(value):
  *         if MIN_INT <= value <= MAX_INT:             # <<<<<<<<<<<<<<
  *             bp = buffer_claim(buffer, 1 + sizeof(int32_t))
  *             bp[0] = TYPE_INT
  */
-    __pyx_t_3 = PyObject_RichCompare(__pyx_int_neg_2147483648, __pyx_v_value, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 513, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_int_neg_2147483648, __pyx_v_value, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 514, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_3)) {
       __Pyx_DECREF(__pyx_t_3);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_value, __pyx_int_2147483648, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 513, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_value, __pyx_int_2147483648, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 514, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 513, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_2) {
 
-      /* "rbfly/amqp/_message.pyx":514
+      /* "rbfly/amqp/_message.pyx":515
  *     elif PyLong_CheckExact(value):
  *         if MIN_INT <= value <= MAX_INT:
  *             bp = buffer_claim(buffer, 1 + sizeof(int32_t))             # <<<<<<<<<<<<<<
  *             bp[0] = TYPE_INT
  *             pack_uint32(&bp[1], <int32_t> value)
  */
-      __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(int32_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 514, __pyx_L1_error)
+      __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(int32_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 515, __pyx_L1_error)
       __pyx_v_bp = __pyx_t_7;
 
-      /* "rbfly/amqp/_message.pyx":515
+      /* "rbfly/amqp/_message.pyx":516
  *         if MIN_INT <= value <= MAX_INT:
  *             bp = buffer_claim(buffer, 1 + sizeof(int32_t))
  *             bp[0] = TYPE_INT             # <<<<<<<<<<<<<<
  *             pack_uint32(&bp[1], <int32_t> value)
  *         elif MIN_LONG <= value <= MAX_LONG:
  */
       (__pyx_v_bp[0]) = 0x71;
 
-      /* "rbfly/amqp/_message.pyx":516
+      /* "rbfly/amqp/_message.pyx":517
  *             bp = buffer_claim(buffer, 1 + sizeof(int32_t))
  *             bp[0] = TYPE_INT
  *             pack_uint32(&bp[1], <int32_t> value)             # <<<<<<<<<<<<<<
  *         elif MIN_LONG <= value <= MAX_LONG:
  *             bp = buffer_claim(buffer, 1 + sizeof(int64_t))
  */
-      __pyx_t_10 = __Pyx_PyInt_As_int32_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 516, __pyx_L1_error)
-      __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), ((int32_t)__pyx_t_10)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 516, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_As_int32_t(__pyx_v_value); if (unlikely((__pyx_t_10 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 517, __pyx_L1_error)
+      __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), ((int32_t)__pyx_t_10)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 517, __pyx_L1_error)
 
-      /* "rbfly/amqp/_message.pyx":513
+      /* "rbfly/amqp/_message.pyx":514
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE
  *     elif PyLong_CheckExact(value):
  *         if MIN_INT <= value <= MAX_INT:             # <<<<<<<<<<<<<<
  *             bp = buffer_claim(buffer, 1 + sizeof(int32_t))
  *             bp[0] = TYPE_INT
  */
       goto __pyx_L4;
     }
 
-    /* "rbfly/amqp/_message.pyx":517
+    /* "rbfly/amqp/_message.pyx":518
  *             bp[0] = TYPE_INT
  *             pack_uint32(&bp[1], <int32_t> value)
  *         elif MIN_LONG <= value <= MAX_LONG:             # <<<<<<<<<<<<<<
  *             bp = buffer_claim(buffer, 1 + sizeof(int64_t))
  *             bp[0] = TYPE_LONG
  */
-    __pyx_t_3 = PyObject_RichCompare(__pyx_int_neg_9223372036854775808, __pyx_v_value, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 517, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_int_neg_9223372036854775808, __pyx_v_value, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 518, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_3)) {
       __Pyx_DECREF(__pyx_t_3);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_value, __pyx_int_9223372036854775808, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 517, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_value, __pyx_int_9223372036854775808, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 518, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 517, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 518, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_2) {
 
-      /* "rbfly/amqp/_message.pyx":518
+      /* "rbfly/amqp/_message.pyx":519
  *             pack_uint32(&bp[1], <int32_t> value)
  *         elif MIN_LONG <= value <= MAX_LONG:
  *             bp = buffer_claim(buffer, 1 + sizeof(int64_t))             # <<<<<<<<<<<<<<
  *             bp[0] = TYPE_LONG
  *             pack_uint64(&bp[1], <int64_t> value)
  */
-      __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(int64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 518, __pyx_L1_error)
+      __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(int64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 519, __pyx_L1_error)
       __pyx_v_bp = __pyx_t_7;
 
-      /* "rbfly/amqp/_message.pyx":519
+      /* "rbfly/amqp/_message.pyx":520
  *         elif MIN_LONG <= value <= MAX_LONG:
  *             bp = buffer_claim(buffer, 1 + sizeof(int64_t))
  *             bp[0] = TYPE_LONG             # <<<<<<<<<<<<<<
  *             pack_uint64(&bp[1], <int64_t> value)
  *         elif MAX_LONG < value <= MAX_ULONG:
  */
       (__pyx_v_bp[0]) = 0x81;
 
-      /* "rbfly/amqp/_message.pyx":520
+      /* "rbfly/amqp/_message.pyx":521
  *             bp = buffer_claim(buffer, 1 + sizeof(int64_t))
  *             bp[0] = TYPE_LONG
  *             pack_uint64(&bp[1], <int64_t> value)             # <<<<<<<<<<<<<<
  *         elif MAX_LONG < value <= MAX_ULONG:
  *             bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  */
-      __pyx_t_11 = __Pyx_PyInt_As_int64_t(__pyx_v_value); if (unlikely((__pyx_t_11 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 520, __pyx_L1_error)
-      __pyx_f_5rbfly_6_codec_pack_uint64((&(__pyx_v_bp[1])), ((int64_t)__pyx_t_11)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 520, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_int64_t(__pyx_v_value); if (unlikely((__pyx_t_11 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 521, __pyx_L1_error)
+      __pyx_f_5rbfly_6_codec_pack_uint64((&(__pyx_v_bp[1])), ((int64_t)__pyx_t_11)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 521, __pyx_L1_error)
 
-      /* "rbfly/amqp/_message.pyx":517
+      /* "rbfly/amqp/_message.pyx":518
  *             bp[0] = TYPE_INT
  *             pack_uint32(&bp[1], <int32_t> value)
  *         elif MIN_LONG <= value <= MAX_LONG:             # <<<<<<<<<<<<<<
  *             bp = buffer_claim(buffer, 1 + sizeof(int64_t))
  *             bp[0] = TYPE_LONG
  */
       goto __pyx_L4;
     }
 
-    /* "rbfly/amqp/_message.pyx":521
+    /* "rbfly/amqp/_message.pyx":522
  *             bp[0] = TYPE_LONG
  *             pack_uint64(&bp[1], <int64_t> value)
  *         elif MAX_LONG < value <= MAX_ULONG:             # <<<<<<<<<<<<<<
  *             bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *             bp[0] = TYPE_ULONG
  */
-    __pyx_t_3 = PyObject_RichCompare(__pyx_int_9223372036854775808, __pyx_v_value, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 521, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_int_9223372036854775808, __pyx_v_value, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     if (__Pyx_PyObject_IsTrue(__pyx_t_3)) {
       __Pyx_DECREF(__pyx_t_3);
-      __pyx_t_3 = PyObject_RichCompare(__pyx_v_value, __pyx_int_18446744073709551615, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 521, __pyx_L1_error)
+      __pyx_t_3 = PyObject_RichCompare(__pyx_v_value, __pyx_int_18446744073709551615, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 521, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (likely(__pyx_t_2)) {
 
-      /* "rbfly/amqp/_message.pyx":522
+      /* "rbfly/amqp/_message.pyx":523
  *             pack_uint64(&bp[1], <int64_t> value)
  *         elif MAX_LONG < value <= MAX_ULONG:
  *             bp = buffer_claim(buffer, 1 + sizeof(uint64_t))             # <<<<<<<<<<<<<<
  *             bp[0] = TYPE_ULONG
  *             pack_uint64(&bp[1], value)
  */
-      __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(uint64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 522, __pyx_L1_error)
+      __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(uint64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 523, __pyx_L1_error)
       __pyx_v_bp = __pyx_t_7;
 
-      /* "rbfly/amqp/_message.pyx":523
+      /* "rbfly/amqp/_message.pyx":524
  *         elif MAX_LONG < value <= MAX_ULONG:
  *             bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *             bp[0] = TYPE_ULONG             # <<<<<<<<<<<<<<
  *             pack_uint64(&bp[1], value)
  *         else:
  */
       (__pyx_v_bp[0]) = 0x80;
 
-      /* "rbfly/amqp/_message.pyx":524
+      /* "rbfly/amqp/_message.pyx":525
  *             bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *             bp[0] = TYPE_ULONG
  *             pack_uint64(&bp[1], value)             # <<<<<<<<<<<<<<
  *         else:
  *             raise TypeError('Cannot encode message with value: {}'.format(value))
  */
-      __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_value); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 524, __pyx_L1_error)
-      __pyx_f_5rbfly_6_codec_pack_uint64((&(__pyx_v_bp[1])), __pyx_t_12); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 524, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_v_value); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 525, __pyx_L1_error)
+      __pyx_f_5rbfly_6_codec_pack_uint64((&(__pyx_v_bp[1])), __pyx_t_12); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 525, __pyx_L1_error)
 
-      /* "rbfly/amqp/_message.pyx":521
+      /* "rbfly/amqp/_message.pyx":522
  *             bp[0] = TYPE_LONG
  *             pack_uint64(&bp[1], <int64_t> value)
  *         elif MAX_LONG < value <= MAX_ULONG:             # <<<<<<<<<<<<<<
  *             bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *             bp[0] = TYPE_ULONG
  */
       goto __pyx_L4;
     }
 
-    /* "rbfly/amqp/_message.pyx":526
+    /* "rbfly/amqp/_message.pyx":527
  *             pack_uint64(&bp[1], value)
  *         else:
  *             raise TypeError('Cannot encode message with value: {}'.format(value))             # <<<<<<<<<<<<<<
  *     elif PyFloat_CheckExact(value):
  *         bp = buffer_claim(buffer, 1 + sizeof(double))
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_encode_message_with_value, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 526, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_encode_message_with_value, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 527, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -8345,187 +8361,187 @@
           __pyx_t_6 = 1;
         }
       }
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_value};
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 526, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 527, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 526, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 527, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(1, 526, __pyx_L1_error)
+      __PYX_ERR(1, 527, __pyx_L1_error)
     }
     __pyx_L4:;
 
-    /* "rbfly/amqp/_message.pyx":512
+    /* "rbfly/amqp/_message.pyx":513
  *         bp = buffer_claim(buffer, 1)
  *         bp[0] = BOOL_TRUE if value else BOOL_FALSE
  *     elif PyLong_CheckExact(value):             # <<<<<<<<<<<<<<
  *         if MIN_INT <= value <= MAX_INT:
  *             bp = buffer_claim(buffer, 1 + sizeof(int32_t))
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":527
+  /* "rbfly/amqp/_message.pyx":528
  *         else:
  *             raise TypeError('Cannot encode message with value: {}'.format(value))
  *     elif PyFloat_CheckExact(value):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 1 + sizeof(double))
  *         bp[0] = TYPE_DOUBLE
  */
   __pyx_t_2 = PyFloat_CheckExact(__pyx_v_value);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":528
+    /* "rbfly/amqp/_message.pyx":529
  *             raise TypeError('Cannot encode message with value: {}'.format(value))
  *     elif PyFloat_CheckExact(value):
  *         bp = buffer_claim(buffer, 1 + sizeof(double))             # <<<<<<<<<<<<<<
  *         bp[0] = TYPE_DOUBLE
  *         pack_double(&bp[1], value)
  */
-    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(double)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 528, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(double)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 529, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_7;
 
-    /* "rbfly/amqp/_message.pyx":529
+    /* "rbfly/amqp/_message.pyx":530
  *     elif PyFloat_CheckExact(value):
  *         bp = buffer_claim(buffer, 1 + sizeof(double))
  *         bp[0] = TYPE_DOUBLE             # <<<<<<<<<<<<<<
  *         pack_double(&bp[1], value)
  *     elif PySequence_Check(value):
  */
     (__pyx_v_bp[0]) = 0x82;
 
-    /* "rbfly/amqp/_message.pyx":530
+    /* "rbfly/amqp/_message.pyx":531
  *         bp = buffer_claim(buffer, 1 + sizeof(double))
  *         bp[0] = TYPE_DOUBLE
  *         pack_double(&bp[1], value)             # <<<<<<<<<<<<<<
  *     elif PySequence_Check(value):
  *         _encode_sequence(buffer, value)
  */
-    __pyx_t_13 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_13 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 530, __pyx_L1_error)
-    __pyx_f_5rbfly_6_codec_pack_double((&(__pyx_v_bp[1])), __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 530, __pyx_L1_error)
+    __pyx_t_13 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_13 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 531, __pyx_L1_error)
+    __pyx_f_5rbfly_6_codec_pack_double((&(__pyx_v_bp[1])), __pyx_t_13); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 531, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":527
+    /* "rbfly/amqp/_message.pyx":528
  *         else:
  *             raise TypeError('Cannot encode message with value: {}'.format(value))
  *     elif PyFloat_CheckExact(value):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 1 + sizeof(double))
  *         bp[0] = TYPE_DOUBLE
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":531
+  /* "rbfly/amqp/_message.pyx":532
  *         bp[0] = TYPE_DOUBLE
  *         pack_double(&bp[1], value)
  *     elif PySequence_Check(value):             # <<<<<<<<<<<<<<
  *         _encode_sequence(buffer, value)
  *     elif PyDict_Check(value):
  */
   __pyx_t_2 = PySequence_Check(__pyx_v_value);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":532
+    /* "rbfly/amqp/_message.pyx":533
  *         pack_double(&bp[1], value)
  *     elif PySequence_Check(value):
  *         _encode_sequence(buffer, value)             # <<<<<<<<<<<<<<
  *     elif PyDict_Check(value):
  *         _encode_dict(buffer, value)
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_sequence(__pyx_v_buffer, __pyx_v_value); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 532, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_sequence(__pyx_v_buffer, __pyx_v_value); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 533, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":531
+    /* "rbfly/amqp/_message.pyx":532
  *         bp[0] = TYPE_DOUBLE
  *         pack_double(&bp[1], value)
  *     elif PySequence_Check(value):             # <<<<<<<<<<<<<<
  *         _encode_sequence(buffer, value)
  *     elif PyDict_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":533
+  /* "rbfly/amqp/_message.pyx":534
  *     elif PySequence_Check(value):
  *         _encode_sequence(buffer, value)
  *     elif PyDict_Check(value):             # <<<<<<<<<<<<<<
  *         _encode_dict(buffer, value)
  *     elif isinstance(value, datetime.datetime):
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_value);
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":534
+    /* "rbfly/amqp/_message.pyx":535
  *         _encode_sequence(buffer, value)
  *     elif PyDict_Check(value):
  *         _encode_dict(buffer, value)             # <<<<<<<<<<<<<<
  *     elif isinstance(value, datetime.datetime):
  *         bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  */
-    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_dict(__pyx_v_buffer, __pyx_v_value); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 534, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_5rbfly_4amqp_8_message__encode_dict(__pyx_v_buffer, __pyx_v_value); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 535, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":533
+    /* "rbfly/amqp/_message.pyx":534
  *     elif PySequence_Check(value):
  *         _encode_sequence(buffer, value)
  *     elif PyDict_Check(value):             # <<<<<<<<<<<<<<
  *         _encode_dict(buffer, value)
  *     elif isinstance(value, datetime.datetime):
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":535
+  /* "rbfly/amqp/_message.pyx":536
  *     elif PyDict_Check(value):
  *         _encode_dict(buffer, value)
  *     elif isinstance(value, datetime.datetime):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *         bp[0] = TYPE_TIMESTAMP
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_datetime); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 535, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_datetime); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 536, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 535, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 536, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_value, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 535, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_value, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 536, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":536
+    /* "rbfly/amqp/_message.pyx":537
  *         _encode_dict(buffer, value)
  *     elif isinstance(value, datetime.datetime):
  *         bp = buffer_claim(buffer, 1 + sizeof(uint64_t))             # <<<<<<<<<<<<<<
  *         bp[0] = TYPE_TIMESTAMP
  *         pack_uint64(&bp[1], <uint64_t> (value.timestamp() * 1000))
  */
-    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(uint64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 536, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (1 + (sizeof(uint64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 537, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_7;
 
-    /* "rbfly/amqp/_message.pyx":537
+    /* "rbfly/amqp/_message.pyx":538
  *     elif isinstance(value, datetime.datetime):
  *         bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *         bp[0] = TYPE_TIMESTAMP             # <<<<<<<<<<<<<<
  *         pack_uint64(&bp[1], <uint64_t> (value.timestamp() * 1000))
  *     elif isinstance(value, uuid.UUID):
  */
     (__pyx_v_bp[0]) = 0x83;
 
-    /* "rbfly/amqp/_message.pyx":538
+    /* "rbfly/amqp/_message.pyx":539
  *         bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *         bp[0] = TYPE_TIMESTAMP
  *         pack_uint64(&bp[1], <uint64_t> (value.timestamp() * 1000))             # <<<<<<<<<<<<<<
  *     elif isinstance(value, uuid.UUID):
  *         bp = buffer_claim(buffer, 17)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_timestamp); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 538, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_timestamp); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 539, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -8535,116 +8551,116 @@
         __pyx_t_6 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[1] = {__pyx_t_5, };
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 538, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 539, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    __pyx_t_4 = __Pyx_PyInt_MultiplyObjC(__pyx_t_3, __pyx_int_1000, 0x3E8, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 538, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_MultiplyObjC(__pyx_t_3, __pyx_int_1000, 0x3E8, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 539, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_t_4); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 538, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_uint64_t(__pyx_t_4); if (unlikely((__pyx_t_12 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 539, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_f_5rbfly_6_codec_pack_uint64((&(__pyx_v_bp[1])), ((uint64_t)__pyx_t_12)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 538, __pyx_L1_error)
+    __pyx_f_5rbfly_6_codec_pack_uint64((&(__pyx_v_bp[1])), ((uint64_t)__pyx_t_12)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 539, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":535
+    /* "rbfly/amqp/_message.pyx":536
  *     elif PyDict_Check(value):
  *         _encode_dict(buffer, value)
  *     elif isinstance(value, datetime.datetime):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 1 + sizeof(uint64_t))
  *         bp[0] = TYPE_TIMESTAMP
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":539
+  /* "rbfly/amqp/_message.pyx":540
  *         bp[0] = TYPE_TIMESTAMP
  *         pack_uint64(&bp[1], <uint64_t> (value.timestamp() * 1000))
  *     elif isinstance(value, uuid.UUID):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 17)
  *         bp[0] = TYPE_UUID
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_uuid); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 539, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_uuid); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UUID); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 539, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_UUID); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_value, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 539, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_value, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 540, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_2) {
 
-    /* "rbfly/amqp/_message.pyx":540
+    /* "rbfly/amqp/_message.pyx":541
  *         pack_uint64(&bp[1], <uint64_t> (value.timestamp() * 1000))
  *     elif isinstance(value, uuid.UUID):
  *         bp = buffer_claim(buffer, 17)             # <<<<<<<<<<<<<<
  *         bp[0] = TYPE_UUID
  *         memcpy(&bp[1], <char*> value.bytes, 16)
  */
-    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 17); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 540, __pyx_L1_error)
+    __pyx_t_7 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 17); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 541, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_7;
 
-    /* "rbfly/amqp/_message.pyx":541
+    /* "rbfly/amqp/_message.pyx":542
  *     elif isinstance(value, uuid.UUID):
  *         bp = buffer_claim(buffer, 17)
  *         bp[0] = TYPE_UUID             # <<<<<<<<<<<<<<
  *         memcpy(&bp[1], <char*> value.bytes, 16)
  *     elif isinstance(value, Symbol):
  */
     (__pyx_v_bp[0]) = 0x98;
 
-    /* "rbfly/amqp/_message.pyx":542
+    /* "rbfly/amqp/_message.pyx":543
  *         bp = buffer_claim(buffer, 17)
  *         bp[0] = TYPE_UUID
  *         memcpy(&bp[1], <char*> value.bytes, 16)             # <<<<<<<<<<<<<<
  *     elif isinstance(value, Symbol):
  *         value_bin = value.name.encode('ascii')
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 542, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 542, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 543, __pyx_L1_error)
     (void)(memcpy((&(__pyx_v_bp[1])), ((char *)__pyx_t_7), 16));
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "rbfly/amqp/_message.pyx":539
+    /* "rbfly/amqp/_message.pyx":540
  *         bp[0] = TYPE_TIMESTAMP
  *         pack_uint64(&bp[1], <uint64_t> (value.timestamp() * 1000))
  *     elif isinstance(value, uuid.UUID):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, 17)
  *         bp[0] = TYPE_UUID
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":543
+  /* "rbfly/amqp/_message.pyx":544
  *         bp[0] = TYPE_UUID
  *         memcpy(&bp[1], <char*> value.bytes, 16)
  *     elif isinstance(value, Symbol):             # <<<<<<<<<<<<<<
  *         value_bin = value.name.encode('ascii')
  *         _encode_strb(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Symbol); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 543, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Symbol); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_value, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 543, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_value, __pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(1, 544, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (likely(__pyx_t_2)) {
 
-    /* "rbfly/amqp/_message.pyx":544
+    /* "rbfly/amqp/_message.pyx":545
  *         memcpy(&bp[1], <char*> value.bytes, 16)
  *     elif isinstance(value, Symbol):
  *         value_bin = value.name.encode('ascii')             # <<<<<<<<<<<<<<
  *         _encode_strb(
  *             buffer,
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 544, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 544, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
@@ -8655,76 +8671,76 @@
         __pyx_t_6 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_n_u_ascii};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 544, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 545, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_3))) __PYX_ERR(1, 544, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_3))) __PYX_ERR(1, 545, __pyx_L1_error)
     __pyx_v_value_bin = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "rbfly/amqp/_message.pyx":547
+    /* "rbfly/amqp/_message.pyx":548
  *         _encode_strb(
  *             buffer,
  *             value_bin,             # <<<<<<<<<<<<<<
  *             len(value_bin),
  *             TYPE_SYMBOL_SHORT,
  */
     if (unlikely(__pyx_v_value_bin == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(1, 547, __pyx_L1_error)
+      __PYX_ERR(1, 548, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_value_bin); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 547, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_value_bin); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":548
+    /* "rbfly/amqp/_message.pyx":549
  *             buffer,
  *             value_bin,
  *             len(value_bin),             # <<<<<<<<<<<<<<
  *             TYPE_SYMBOL_SHORT,
  *             TYPE_SYMBOL_LONG
  */
     if (unlikely(__pyx_v_value_bin == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(1, 548, __pyx_L1_error)
+      __PYX_ERR(1, 549, __pyx_L1_error)
     }
-    __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_value_bin); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 548, __pyx_L1_error)
+    __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_value_bin); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 549, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":545
+    /* "rbfly/amqp/_message.pyx":546
  *     elif isinstance(value, Symbol):
  *         value_bin = value.name.encode('ascii')
  *         _encode_strb(             # <<<<<<<<<<<<<<
  *             buffer,
  *             value_bin,
  */
-    __pyx_t_8 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_7, __pyx_t_1, 0xA3, 0xB3); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 545, __pyx_L1_error)
+    __pyx_t_8 = __pyx_f_5rbfly_4amqp_8_message__encode_strb(__pyx_v_buffer, __pyx_t_7, __pyx_t_1, 0xA3, 0xB3); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 546, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":543
+    /* "rbfly/amqp/_message.pyx":544
  *         bp[0] = TYPE_UUID
  *         memcpy(&bp[1], <char*> value.bytes, 16)
  *     elif isinstance(value, Symbol):             # <<<<<<<<<<<<<<
  *         value_bin = value.name.encode('ascii')
  *         _encode_strb(
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":553
+  /* "rbfly/amqp/_message.pyx":554
  *         )
  *     else:
  *         raise TypeError('Cannot encode message with body of type: {}'.format(type(value)))             # <<<<<<<<<<<<<<
  * 
  *     return buffer.offset - start
  */
   /*else*/ {
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_encode_message_with_body, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 553, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_encode_message_with_body, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 554, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_4 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -8734,38 +8750,38 @@
         __pyx_t_6 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, ((PyObject *)Py_TYPE(__pyx_v_value))};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 553, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 554, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 553, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 554, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(1, 553, __pyx_L1_error)
+    __PYX_ERR(1, 554, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "rbfly/amqp/_message.pyx":555
+  /* "rbfly/amqp/_message.pyx":556
  *         raise TypeError('Cannot encode message with body of type: {}'.format(type(value)))
  * 
  *     return buffer.offset - start             # <<<<<<<<<<<<<<
  * 
  * cdef inline Py_ssize_t _encode_sequence(Buffer *buffer, object value) except -1:
  */
   __pyx_r = (__pyx_v_buffer->offset - __pyx_v_start);
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":483
+  /* "rbfly/amqp/_message.pyx":484
  *     buffer[2] = code
  * 
  * cdef inline Py_ssize_t _encode_value(Buffer *buffer, object value) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Encode Python object into AMQP format.
  */
 
@@ -8778,15 +8794,15 @@
   __pyx_r = -1L;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_value_bin);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":557
+/* "rbfly/amqp/_message.pyx":558
  *     return buffer.offset - start
  * 
  * cdef inline Py_ssize_t _encode_sequence(Buffer *buffer, object value) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Encode Python sequence into AMQP format.
  */
 
@@ -8805,158 +8821,158 @@
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_encode_sequence", 0);
 
-  /* "rbfly/amqp/_message.pyx":562
+  /* "rbfly/amqp/_message.pyx":563
  *     """
  *     cdef:
  *         Py_ssize_t hlen = 1 + 2 * sizeof(uint32_t)             # <<<<<<<<<<<<<<
  *         Py_ssize_t start = buffer.offset + hlen
  *         Py_ssize_t blen
  */
   __pyx_v_hlen = (1 + (2 * (sizeof(uint32_t))));
 
-  /* "rbfly/amqp/_message.pyx":563
+  /* "rbfly/amqp/_message.pyx":564
  *     cdef:
  *         Py_ssize_t hlen = 1 + 2 * sizeof(uint32_t)
  *         Py_ssize_t start = buffer.offset + hlen             # <<<<<<<<<<<<<<
  *         Py_ssize_t blen
  *         char *bp
  */
   __pyx_v_start = (__pyx_v_buffer->offset + __pyx_v_hlen);
 
-  /* "rbfly/amqp/_message.pyx":569
+  /* "rbfly/amqp/_message.pyx":570
  * 
  * 
  *     bp = buffer_claim(buffer, hlen)             # <<<<<<<<<<<<<<
  *     bp[0] = TYPE_LIST32
  * 
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 569, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 570, __pyx_L1_error)
   __pyx_v_bp = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":570
+  /* "rbfly/amqp/_message.pyx":571
  * 
  *     bp = buffer_claim(buffer, hlen)
  *     bp[0] = TYPE_LIST32             # <<<<<<<<<<<<<<
  * 
  *     # number of sequence elements; reserve size of uint32_t for buffer
  */
   (__pyx_v_bp[0]) = 0xD0;
 
-  /* "rbfly/amqp/_message.pyx":574
+  /* "rbfly/amqp/_message.pyx":575
  *     # number of sequence elements; reserve size of uint32_t for buffer
  *     # length taken by the sequence
  *     pack_uint32(&bp[1 + sizeof(uint32_t)], len(value))             # <<<<<<<<<<<<<<
  * 
  *     for obj in value:
  */
-  __pyx_t_2 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 574, __pyx_L1_error)
-  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[(1 + (sizeof(uint32_t)))])), __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 574, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 575, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[(1 + (sizeof(uint32_t)))])), __pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 575, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":576
+  /* "rbfly/amqp/_message.pyx":577
  *     pack_uint32(&bp[1 + sizeof(uint32_t)], len(value))
  * 
  *     for obj in value:             # <<<<<<<<<<<<<<
  *         _encode_value(buffer, obj)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_value)) || PyTuple_CheckExact(__pyx_v_value)) {
     __pyx_t_3 = __pyx_v_value; __Pyx_INCREF(__pyx_t_3); __pyx_t_2 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 576, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 576, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 577, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_2); __Pyx_INCREF(__pyx_t_5); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 576, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_2); __Pyx_INCREF(__pyx_t_5); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 577, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 576, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 577, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_2); __Pyx_INCREF(__pyx_t_5); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 576, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_2); __Pyx_INCREF(__pyx_t_5); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 577, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 576, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 577, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_3);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 576, __pyx_L1_error)
+          else __PYX_ERR(1, 577, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_obj, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "rbfly/amqp/_message.pyx":577
+    /* "rbfly/amqp/_message.pyx":578
  * 
  *     for obj in value:
  *         _encode_value(buffer, obj)             # <<<<<<<<<<<<<<
  * 
  *     # encode the buffer length taken by the sequence
  */
-    __pyx_t_6 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_obj); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 577, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_obj); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 578, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":576
+    /* "rbfly/amqp/_message.pyx":577
  *     pack_uint32(&bp[1 + sizeof(uint32_t)], len(value))
  * 
  *     for obj in value:             # <<<<<<<<<<<<<<
  *         _encode_value(buffer, obj)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "rbfly/amqp/_message.pyx":580
+  /* "rbfly/amqp/_message.pyx":581
  * 
  *     # encode the buffer length taken by the sequence
  *     blen = buffer.offset - start             # <<<<<<<<<<<<<<
  *     pack_uint32(&bp[1], blen)
  *     return blen
  */
   __pyx_v_blen = (__pyx_v_buffer->offset - __pyx_v_start);
 
-  /* "rbfly/amqp/_message.pyx":581
+  /* "rbfly/amqp/_message.pyx":582
  *     # encode the buffer length taken by the sequence
  *     blen = buffer.offset - start
  *     pack_uint32(&bp[1], blen)             # <<<<<<<<<<<<<<
  *     return blen
  * 
  */
-  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 581, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 582, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":582
+  /* "rbfly/amqp/_message.pyx":583
  *     blen = buffer.offset - start
  *     pack_uint32(&bp[1], blen)
  *     return blen             # <<<<<<<<<<<<<<
  * 
  * cdef inline Py_ssize_t _encode_dict(Buffer *buffer, object value) except -1:
  */
   __pyx_r = __pyx_v_blen;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":557
+  /* "rbfly/amqp/_message.pyx":558
  *     return buffer.offset - start
  * 
  * cdef inline Py_ssize_t _encode_sequence(Buffer *buffer, object value) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Encode Python sequence into AMQP format.
  */
 
@@ -8968,15 +8984,15 @@
   __pyx_r = -1L;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":584
+/* "rbfly/amqp/_message.pyx":585
  *     return blen
  * 
  * cdef inline Py_ssize_t _encode_dict(Buffer *buffer, object value) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Encode Python dictionary into AMQP format.
  */
 
@@ -8999,138 +9015,138 @@
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_encode_dict", 0);
 
-  /* "rbfly/amqp/_message.pyx":589
+  /* "rbfly/amqp/_message.pyx":590
  *     """
  *     cdef:
  *         Py_ssize_t hlen = 1 + 2 * sizeof(uint32_t)             # <<<<<<<<<<<<<<
  *         Py_ssize_t start = buffer.offset + hlen
  *         Py_ssize_t blen
  */
   __pyx_v_hlen = (1 + (2 * (sizeof(uint32_t))));
 
-  /* "rbfly/amqp/_message.pyx":590
+  /* "rbfly/amqp/_message.pyx":591
  *     cdef:
  *         Py_ssize_t hlen = 1 + 2 * sizeof(uint32_t)
  *         Py_ssize_t start = buffer.offset + hlen             # <<<<<<<<<<<<<<
  *         Py_ssize_t blen
  *         char *bp
  */
   __pyx_v_start = (__pyx_v_buffer->offset + __pyx_v_hlen);
 
-  /* "rbfly/amqp/_message.pyx":596
+  /* "rbfly/amqp/_message.pyx":597
  * 
  *     # TODO: optimize for TYPE_MAP8
  *     bp = buffer_claim(buffer, hlen)             # <<<<<<<<<<<<<<
  *     bp[0] = TYPE_MAP32
  * 
  */
-  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 596, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 597, __pyx_L1_error)
   __pyx_v_bp = __pyx_t_1;
 
-  /* "rbfly/amqp/_message.pyx":597
+  /* "rbfly/amqp/_message.pyx":598
  *     # TODO: optimize for TYPE_MAP8
  *     bp = buffer_claim(buffer, hlen)
  *     bp[0] = TYPE_MAP32             # <<<<<<<<<<<<<<
  * 
  *     # number of map elements (both keys and values); reserve size of
  */
   (__pyx_v_bp[0]) = 0xD1;
 
-  /* "rbfly/amqp/_message.pyx":601
+  /* "rbfly/amqp/_message.pyx":602
  *     # number of map elements (both keys and values); reserve size of
  *     # uint32_t for buffer length taken by the dictionary
  *     pack_uint32(&bp[1 + sizeof(uint32_t)], len(value) * 2)             # <<<<<<<<<<<<<<
  * 
  *     for k, v in value.items():
  */
-  __pyx_t_2 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 601, __pyx_L1_error)
-  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[(1 + (sizeof(uint32_t)))])), (__pyx_t_2 * 2)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 601, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_value); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 602, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[(1 + (sizeof(uint32_t)))])), (__pyx_t_2 * 2)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 602, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":603
+  /* "rbfly/amqp/_message.pyx":604
  *     pack_uint32(&bp[1 + sizeof(uint32_t)], len(value) * 2)
  * 
  *     for k, v in value.items():             # <<<<<<<<<<<<<<
  *         _encode_value(buffer, k)
  *         _encode_value(buffer, v)
  */
   __pyx_t_2 = 0;
   if (unlikely(__pyx_v_value == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(1, 603, __pyx_L1_error)
+    __PYX_ERR(1, 604, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_value, 0, __pyx_n_s_items, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 603, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_value, 0, __pyx_n_s_items, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_3);
   __pyx_t_3 = __pyx_t_6;
   __pyx_t_6 = 0;
   while (1) {
     __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_4, &__pyx_t_2, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
     if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 603, __pyx_L1_error)
+    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 604, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "rbfly/amqp/_message.pyx":604
+    /* "rbfly/amqp/_message.pyx":605
  * 
  *     for k, v in value.items():
  *         _encode_value(buffer, k)             # <<<<<<<<<<<<<<
  *         _encode_value(buffer, v)
  * 
  */
-    __pyx_t_9 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_k); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 604, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_k); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 605, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":605
+    /* "rbfly/amqp/_message.pyx":606
  *     for k, v in value.items():
  *         _encode_value(buffer, k)
  *         _encode_value(buffer, v)             # <<<<<<<<<<<<<<
  * 
  *     # encode the buffer length taken by the dictionary
  */
-    __pyx_t_9 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_v); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 605, __pyx_L1_error)
+    __pyx_t_9 = __pyx_f_5rbfly_4amqp_8_message__encode_value(__pyx_v_buffer, __pyx_v_v); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 606, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "rbfly/amqp/_message.pyx":608
+  /* "rbfly/amqp/_message.pyx":609
  * 
  *     # encode the buffer length taken by the dictionary
  *     blen = buffer.offset - start             # <<<<<<<<<<<<<<
  *     pack_uint32(&bp[1], blen)
  *     return blen
  */
   __pyx_v_blen = (__pyx_v_buffer->offset - __pyx_v_start);
 
-  /* "rbfly/amqp/_message.pyx":609
+  /* "rbfly/amqp/_message.pyx":610
  *     # encode the buffer length taken by the dictionary
  *     blen = buffer.offset - start
  *     pack_uint32(&bp[1], blen)             # <<<<<<<<<<<<<<
  *     return blen
  * 
  */
-  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 609, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 610, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":610
+  /* "rbfly/amqp/_message.pyx":611
  *     blen = buffer.offset - start
  *     pack_uint32(&bp[1], blen)
  *     return blen             # <<<<<<<<<<<<<<
  * 
  * cdef inline Py_ssize_t _encode_strb(
  */
   __pyx_r = __pyx_v_blen;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":584
+  /* "rbfly/amqp/_message.pyx":585
  *     return blen
  * 
  * cdef inline Py_ssize_t _encode_dict(Buffer *buffer, object value) except -1:             # <<<<<<<<<<<<<<
  *     """
  *     Encode Python dictionary into AMQP format.
  */
 
@@ -9144,15 +9160,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_k);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":612
+/* "rbfly/amqp/_message.pyx":613
  *     return blen
  * 
  * cdef inline Py_ssize_t _encode_strb(             # <<<<<<<<<<<<<<
  *         Buffer *buffer,
  *         char *body,
  */
 
@@ -9172,164 +9188,164 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_encode_strb", 0);
 
-  /* "rbfly/amqp/_message.pyx":624
+  /* "rbfly/amqp/_message.pyx":625
  *         char *bp
  * 
  *     if size < 256:             # <<<<<<<<<<<<<<
  *         hlen = 2
  *         blen = hlen + size
  */
   __pyx_t_1 = (__pyx_v_size < 0x100);
   if (__pyx_t_1) {
 
-    /* "rbfly/amqp/_message.pyx":625
+    /* "rbfly/amqp/_message.pyx":626
  * 
  *     if size < 256:
  *         hlen = 2             # <<<<<<<<<<<<<<
  *         blen = hlen + size
  *         bp = buffer_claim(buffer, blen)
  */
     __pyx_v_hlen = 2;
 
-    /* "rbfly/amqp/_message.pyx":626
+    /* "rbfly/amqp/_message.pyx":627
  *     if size < 256:
  *         hlen = 2
  *         blen = hlen + size             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, blen)
  *         bp[0] = code_short
  */
     __pyx_v_blen = (__pyx_v_hlen + __pyx_v_size);
 
-    /* "rbfly/amqp/_message.pyx":627
+    /* "rbfly/amqp/_message.pyx":628
  *         hlen = 2
  *         blen = hlen + size
  *         bp = buffer_claim(buffer, blen)             # <<<<<<<<<<<<<<
  *         bp[0] = code_short
  *         bp[1] = size
  */
-    __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 627, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 628, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_2;
 
-    /* "rbfly/amqp/_message.pyx":628
+    /* "rbfly/amqp/_message.pyx":629
  *         blen = hlen + size
  *         bp = buffer_claim(buffer, blen)
  *         bp[0] = code_short             # <<<<<<<<<<<<<<
  *         bp[1] = size
  *     elif size <= MAX_UINT:
  */
     (__pyx_v_bp[0]) = __pyx_v_code_short;
 
-    /* "rbfly/amqp/_message.pyx":629
+    /* "rbfly/amqp/_message.pyx":630
  *         bp = buffer_claim(buffer, blen)
  *         bp[0] = code_short
  *         bp[1] = size             # <<<<<<<<<<<<<<
  *     elif size <= MAX_UINT:
  *         hlen = 1 + sizeof(uint32_t)
  */
     (__pyx_v_bp[1]) = __pyx_v_size;
 
-    /* "rbfly/amqp/_message.pyx":624
+    /* "rbfly/amqp/_message.pyx":625
  *         char *bp
  * 
  *     if size < 256:             # <<<<<<<<<<<<<<
  *         hlen = 2
  *         blen = hlen + size
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":630
+  /* "rbfly/amqp/_message.pyx":631
  *         bp[0] = code_short
  *         bp[1] = size
  *     elif size <= MAX_UINT:             # <<<<<<<<<<<<<<
  *         hlen = 1 + sizeof(uint32_t)
  *         blen = hlen + size
  */
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 630, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 630, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_int_4294967295, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 631, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 630, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 631, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (likely(__pyx_t_1)) {
 
-    /* "rbfly/amqp/_message.pyx":631
+    /* "rbfly/amqp/_message.pyx":632
  *         bp[1] = size
  *     elif size <= MAX_UINT:
  *         hlen = 1 + sizeof(uint32_t)             # <<<<<<<<<<<<<<
  *         blen = hlen + size
  *         bp = buffer_claim(buffer, blen)
  */
     __pyx_v_hlen = (1 + (sizeof(uint32_t)));
 
-    /* "rbfly/amqp/_message.pyx":632
+    /* "rbfly/amqp/_message.pyx":633
  *     elif size <= MAX_UINT:
  *         hlen = 1 + sizeof(uint32_t)
  *         blen = hlen + size             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, blen)
  *         bp[0] = code_long
  */
     __pyx_v_blen = (__pyx_v_hlen + __pyx_v_size);
 
-    /* "rbfly/amqp/_message.pyx":633
+    /* "rbfly/amqp/_message.pyx":634
  *         hlen = 1 + sizeof(uint32_t)
  *         blen = hlen + size
  *         bp = buffer_claim(buffer, blen)             # <<<<<<<<<<<<<<
  *         bp[0] = code_long
  *         pack_uint32(&bp[1], size)
  */
-    __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 633, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_blen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 634, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_2;
 
-    /* "rbfly/amqp/_message.pyx":634
+    /* "rbfly/amqp/_message.pyx":635
  *         blen = hlen + size
  *         bp = buffer_claim(buffer, blen)
  *         bp[0] = code_long             # <<<<<<<<<<<<<<
  *         pack_uint32(&bp[1], size)
  *     else:
  */
     (__pyx_v_bp[0]) = __pyx_v_code_long;
 
-    /* "rbfly/amqp/_message.pyx":635
+    /* "rbfly/amqp/_message.pyx":636
  *         bp = buffer_claim(buffer, blen)
  *         bp[0] = code_long
  *         pack_uint32(&bp[1], size)             # <<<<<<<<<<<<<<
  *     else:
  *         raise RbFlyBufferError('Data too long, size={}'.format(size))
  */
-    __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 635, __pyx_L1_error)
+    __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp[1])), __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L1_error)
 
-    /* "rbfly/amqp/_message.pyx":630
+    /* "rbfly/amqp/_message.pyx":631
  *         bp[0] = code_short
  *         bp[1] = size
  *     elif size <= MAX_UINT:             # <<<<<<<<<<<<<<
  *         hlen = 1 + sizeof(uint32_t)
  *         blen = hlen + size
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/amqp/_message.pyx":637
+  /* "rbfly/amqp/_message.pyx":638
  *         pack_uint32(&bp[1], size)
  *     else:
  *         raise RbFlyBufferError('Data too long, size={}'.format(size))             # <<<<<<<<<<<<<<
  * 
  *     memcpy(&bp[hlen], body, size)
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_RbFlyBufferError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 637, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_RbFlyBufferError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 638, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Data_too_long_size, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 637, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Data_too_long_size, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 638, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 637, __pyx_L1_error)
+    __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 638, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -9340,15 +9356,15 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_7};
       __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 637, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 638, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_t_6 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
@@ -9361,44 +9377,44 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 637, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 638, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(1, 637, __pyx_L1_error)
+    __PYX_ERR(1, 638, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "rbfly/amqp/_message.pyx":639
+  /* "rbfly/amqp/_message.pyx":640
  *         raise RbFlyBufferError('Data too long, size={}'.format(size))
  * 
  *     memcpy(&bp[hlen], body, size)             # <<<<<<<<<<<<<<
  *     return blen
  * 
  */
   (void)(memcpy((&(__pyx_v_bp[__pyx_v_hlen])), __pyx_v_body, __pyx_v_size));
 
-  /* "rbfly/amqp/_message.pyx":640
+  /* "rbfly/amqp/_message.pyx":641
  * 
  *     memcpy(&bp[hlen], body, size)
  *     return blen             # <<<<<<<<<<<<<<
  * 
  * #
  */
   __pyx_r = __pyx_v_blen;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":612
+  /* "rbfly/amqp/_message.pyx":613
  *     return blen
  * 
  * cdef inline Py_ssize_t _encode_strb(             # <<<<<<<<<<<<<<
  *         Buffer *buffer,
  *         char *body,
  */
 
@@ -9413,15 +9429,15 @@
   __Pyx_AddTraceback("rbfly.amqp._message._encode_strb", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1L;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":646
+/* "rbfly/amqp/_message.pyx":647
  * #
  * 
  * def set_message_ctx(msg: MessageCtx) -> None:             # <<<<<<<<<<<<<<
  *     """
  *     Set current context of AMQP message.
  */
 
@@ -9464,37 +9480,37 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_msg)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 646, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 647, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_message_ctx") < 0)) __PYX_ERR(1, 646, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_message_ctx") < 0)) __PYX_ERR(1, 647, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_msg = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_message_ctx", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 646, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_message_ctx", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 647, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.amqp._message.set_message_ctx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_msg), __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx, 0, "msg", 0))) __PYX_ERR(1, 646, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_msg), __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx, 0, "msg", 0))) __PYX_ERR(1, 647, __pyx_L1_error)
   __pyx_r = __pyx_pf_5rbfly_4amqp_8_message_4set_message_ctx(__pyx_self, __pyx_v_msg);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9510,24 +9526,24 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_message_ctx", 0);
 
-  /* "rbfly/amqp/_message.pyx":650
+  /* "rbfly/amqp/_message.pyx":651
  *     Set current context of AMQP message.
  *     """
  *     CTX_MESSAGE.set(msg)             # <<<<<<<<<<<<<<
  * 
  * def get_message_ctx() -> MessageCtx:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_CTX_MESSAGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 650, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_CTX_MESSAGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 650, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_set); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -9538,21 +9554,21 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, ((PyObject *)__pyx_v_msg)};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 650, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 651, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "rbfly/amqp/_message.pyx":646
+  /* "rbfly/amqp/_message.pyx":647
  * #
  * 
  * def set_message_ctx(msg: MessageCtx) -> None:             # <<<<<<<<<<<<<<
  *     """
  *     Set current context of AMQP message.
  */
 
@@ -9567,15 +9583,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/amqp/_message.pyx":652
+/* "rbfly/amqp/_message.pyx":653
  *     CTX_MESSAGE.set(msg)
  * 
  * def get_message_ctx() -> MessageCtx:             # <<<<<<<<<<<<<<
  *     """
  *     Get current context of AMQP message.
  */
 
@@ -9603,25 +9619,25 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_message_ctx", 0);
 
-  /* "rbfly/amqp/_message.pyx":656
+  /* "rbfly/amqp/_message.pyx":657
  *     Get current context of AMQP message.
  *     """
  *     return CTX_MESSAGE.get()             # <<<<<<<<<<<<<<
  * 
  * # vim: sw=4:et:ai
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_CTX_MESSAGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 656, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_CTX_MESSAGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 656, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 657, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -9632,24 +9648,24 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_2, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 656, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 657, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx))))) __PYX_ERR(1, 656, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx))))) __PYX_ERR(1, 657, __pyx_L1_error)
   __pyx_r = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "rbfly/amqp/_message.pyx":652
+  /* "rbfly/amqp/_message.pyx":653
  *     CTX_MESSAGE.set(msg)
  * 
  * def get_message_ctx() -> MessageCtx:             # <<<<<<<<<<<<<<
  *     """
  *     Get current context of AMQP message.
  */
 
@@ -10083,15 +10099,15 @@
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 368, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 369, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -10156,39 +10172,39 @@
   /* "rbfly/amqp/_message.pyx":197
  *     return c_encode_amqp(&buff, message)
  * 
  * def decode_amqp(bytes buffer) -> MessageCtx:             # <<<<<<<<<<<<<<
  *     """
  *     Decode AMQP message.
  */
-  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_buffer, __pyx_n_s_buff); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 197, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(3, __pyx_n_s_buffer, __pyx_n_s_size, __pyx_n_s_buff); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_amqp__message_pyx, __pyx_n_s_decode_amqp, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 197, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_amqp__message_pyx, __pyx_n_s_decode_amqp, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 197, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":646
+  /* "rbfly/amqp/_message.pyx":647
  * #
  * 
  * def set_message_ctx(msg: MessageCtx) -> None:             # <<<<<<<<<<<<<<
  *     """
  *     Set current context of AMQP message.
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_msg); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 646, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_msg); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_amqp__message_pyx, __pyx_n_s_set_message_ctx, 646, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 646, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_amqp__message_pyx, __pyx_n_s_set_message_ctx, 647, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 647, __pyx_L1_error)
 
-  /* "rbfly/amqp/_message.pyx":652
+  /* "rbfly/amqp/_message.pyx":653
  *     CTX_MESSAGE.set(msg)
  * 
  * def get_message_ctx() -> MessageCtx:             # <<<<<<<<<<<<<<
  *     """
  *     Get current context of AMQP message.
  */
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_amqp__message_pyx, __pyx_n_s_get_message_ctx, 652, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 652, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_amqp__message_pyx, __pyx_n_s_get_message_ctx, 653, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 653, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -10243,15 +10259,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   if (__Pyx_ExportFunction("c_encode_amqp", (void (*)(void))__pyx_f_5rbfly_4amqp_8_message_c_encode_amqp, "Py_ssize_t (struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("c_decode_amqp", (void (*)(void))__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp, "struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(struct __pyx_t_5rbfly_7_buffer_Buffer *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("c_decode_amqp", (void (*)(void))__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp, "struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -10874,47 +10890,47 @@
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_4amqp_8_message_3decode_amqp, 0, __pyx_n_s_decode_amqp, NULL, __pyx_n_s_rbfly_amqp__message, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_amqp, __pyx_t_2) < 0) __PYX_ERR(1, 197, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "rbfly/amqp/_message.pyx":646
+  /* "rbfly/amqp/_message.pyx":647
  * #
  * 
  * def set_message_ctx(msg: MessageCtx) -> None:             # <<<<<<<<<<<<<<
  *     """
  *     Set current context of AMQP message.
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 646, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_msg, __pyx_n_s_MessageCtx) < 0) __PYX_ERR(1, 646, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 646, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_4amqp_8_message_5set_message_ctx, 0, __pyx_n_s_set_message_ctx, NULL, __pyx_n_s_rbfly_amqp__message, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 646, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_msg, __pyx_n_s_MessageCtx) < 0) __PYX_ERR(1, 647, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 647, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_4amqp_8_message_5set_message_ctx, 0, __pyx_n_s_set_message_ctx, NULL, __pyx_n_s_rbfly_amqp__message, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_message_ctx, __pyx_t_4) < 0) __PYX_ERR(1, 646, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_set_message_ctx, __pyx_t_4) < 0) __PYX_ERR(1, 647, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "rbfly/amqp/_message.pyx":652
+  /* "rbfly/amqp/_message.pyx":653
  *     CTX_MESSAGE.set(msg)
  * 
  * def get_message_ctx() -> MessageCtx:             # <<<<<<<<<<<<<<
  *     """
  *     Get current context of AMQP message.
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 652, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_MessageCtx) < 0) __PYX_ERR(1, 652, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_4amqp_8_message_7get_message_ctx, 0, __pyx_n_s_get_message_ctx, NULL, __pyx_n_s_rbfly_amqp__message, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 652, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_MessageCtx) < 0) __PYX_ERR(1, 653, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_4amqp_8_message_7get_message_ctx, 0, __pyx_n_s_get_message_ctx, NULL, __pyx_n_s_rbfly_amqp__message, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_message_ctx, __pyx_t_2) < 0) __PYX_ERR(1, 652, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_message_ctx, __pyx_t_2) < 0) __PYX_ERR(1, 653, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "rbfly/amqp/_message.pyx":1
  * #             # <<<<<<<<<<<<<<
  * # rbfly - a library for RabbitMQ Streams using Python asyncio
  * #
  */
```

### Comparing `rbfly-0.7.1/rbfly/amqp/_message.pxd` & `rbfly-0.7.2/rbfly/amqp/_message.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -39,10 +39,10 @@
         public uint64_t stream_offset
         public double stream_timestamp
         public uint64_t stream_publish_id
         public uint8_t is_set_stream_publish_id
 
 cdef:
     Py_ssize_t c_encode_amqp(Buffer*, object) except -1
-    MessageCtx c_decode_amqp(Buffer*)
+    MessageCtx c_decode_amqp(Buffer*, Py_ssize_t)
 
 # vim: sw=4:et:ai
```

### Comparing `rbfly-0.7.1/rbfly/amqp/_message.pyi` & `rbfly-0.7.2/rbfly/amqp/_message.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/amqp/_message.pyx` & `rbfly-0.7.2/rbfly/amqp/_message.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -197,22 +197,23 @@
 def decode_amqp(bytes buffer) -> MessageCtx:
     """
     Decode AMQP message.
 
     :param buffer: Buffer to decode the message from.
     """
     cdef:
-        Buffer buff = Buffer(buffer, len(buffer), 0)
-    return c_decode_amqp(&buff)
+        cdef size = len(buffer)
+        Buffer buff = Buffer(buffer, size, 0)
+    return c_decode_amqp(&buff, size)
 
 #
 # functions to decode AMQP format
 #
 
-cdef MessageCtx c_decode_amqp(Buffer *buffer):
+cdef MessageCtx c_decode_amqp(Buffer *buffer, Py_ssize_t size):
     """
     Decode AMQP message.
 
     :param buffer: Buffer to decode the message from.
     """
     cdef:
         uint32_t desc_code
```

### Comparing `rbfly-0.7.1/rbfly/cm.py` & `rbfly-0.7.2/rbfly/cm.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/error.py` & `rbfly-0.7.2/rbfly/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/__init__.py` & `rbfly-0.7.2/rbfly/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/_client.c` & `rbfly-0.7.2/rbfly/streams/_client.c`

 * *Files 1% similar despite different names*

```diff
@@ -1352,15 +1352,15 @@
   int __pyx_n;
   uint64_t inc;
 };
 struct __pyx_defaults {
   PyObject *__pyx_arg_app_properties;
 };
 
-/* "rbfly/streams/_client.pyx":517
+/* "rbfly/streams/_client.pyx":548
  *         publisher._next_message_id()
  * 
  * async def _flush_messages(             # <<<<<<<<<<<<<<
  *         publisher: PublisherBatchTrait,
  *         data: list[MessageCtx],
  */
 struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages {
@@ -1368,24 +1368,25 @@
   PyObject *__pyx_v_amqp;
   Py_ssize_t __pyx_v_count;
   PyObject *__pyx_v_data;
   struct __pyx_obj_5rbfly_7streams_7_client_PublisherBatchTrait *__pyx_v_publisher;
 };
 
 
-/* "rbfly/streams/_client.pyx":482
- *         self._message: MessageCtx | None = None
+/* "rbfly/streams/_client.pyx":508
+ *         return offset
  * 
  *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:             # <<<<<<<<<<<<<<
  *         """
  *         Iterate over messages read from a stream.
  */
 struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ {
   PyObject_HEAD
   PyObject *__pyx_v_client;
+  PyObject *__pyx_v_ex;
   PyObject *__pyx_v_messages;
   PyObject *__pyx_v_protocol;
   struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self;
   PyObject *__pyx_v_task;
   float __pyx_v_timeout;
   PyObject *__pyx_t_0;
   PyObject *__pyx_t_1;
@@ -1529,21 +1530,23 @@
  * 
  * cdef class Subscriber:             # <<<<<<<<<<<<<<
  *     """
  *     RabbitMQ stream subscriber.
  */
 struct __pyx_obj_5rbfly_7streams_7_client_Subscriber {
   PyObject_HEAD
+  struct __pyx_vtabstruct_5rbfly_7streams_7_client_Subscriber *__pyx_vtab;
   PyObject *_client;
   PyObject *_stream;
   uint8_t _subscription_id;
   PyObject *_offset;
   float _timeout;
   char _amqp;
-  struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *_message;
+  PyObject *_messages;
+  PyObject *_last_message;
 };
 
 
 /* "rbfly/streams/_client.pyx":98
  *         ...
  * 
  * cdef class PublisherTrait:             # <<<<<<<<<<<<<<
@@ -1801,14 +1804,28 @@
  *     RabbitMQ Streams publisher for sending single message of binary data.
  */
 
 struct __pyx_vtabstruct_5rbfly_7streams_7_client_PublisherBin {
   struct __pyx_vtabstruct_5rbfly_7streams_7_client_PublisherTrait __pyx_base;
 };
 static struct __pyx_vtabstruct_5rbfly_7streams_7_client_PublisherBin *__pyx_vtabptr_5rbfly_7streams_7_client_PublisherBin;
+
+
+/* "rbfly/streams/_client.pyx":436
+ *         self._data = await _flush_messages(self, self._data, amqp=False)
+ * 
+ * cdef class Subscriber:             # <<<<<<<<<<<<<<
+ *     """
+ *     RabbitMQ stream subscriber.
+ */
+
+struct __pyx_vtabstruct_5rbfly_7streams_7_client_Subscriber {
+  PyObject *(*_next_message_offset)(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *, int __pyx_skip_dispatch);
+};
+static struct __pyx_vtabstruct_5rbfly_7streams_7_client_Subscriber *__pyx_vtabptr_5rbfly_7streams_7_client_Subscriber;
 /* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
@@ -2440,14 +2457,63 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
+/* PyIntBinop.proto */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_SubtractObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
+#else
+#define __Pyx_PyInt_SubtractObjC(op1, op2, intval, inplace, zerodivision_check)\
+    (inplace ? PyNumber_InPlaceSubtract(op1, op2) : PyNumber_Subtract(op1, op2))
+#endif
+
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
+
+/* ObjectGetItem.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
+#else
+#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
+#endif
+
+/* PyIntBinop.proto */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
+#else
+#define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
+    (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
+#endif
+
+/* PyObject_Str.proto */
+#define __Pyx_PyObject_Str(obj)\
+    (likely(PyString_CheckExact(obj)) ? __Pyx_NewRef(obj) : PyObject_Str(obj))
+
 /* StopAsyncIteration.proto */
 #define __Pyx_StopAsyncIteration_USED
 static PyObject *__Pyx_PyExc_StopAsyncIteration;
 static int __pyx_StopAsyncIteration_init(PyObject *module);
 
 /* SliceObject.proto */
 #define __Pyx_PyObject_DelSlice(obj, cstart, cstop, py_start, py_stop, py_slice, has_cstart, has_cstop, wraparound)\
@@ -2471,30 +2537,30 @@
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
-/* SetupReduce.proto */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_setup_reduce(PyObject* type_obj);
-#endif
-
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyTypeObject* typeptr , void* vtable);
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyTypeObject *type);
 
 /* MergeVTables.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_MergeVtables(PyTypeObject *type);
 #endif
 
+/* SetupReduce.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce(PyObject* type_obj);
+#endif
+
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
@@ -2668,14 +2734,15 @@
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static uint64_t __pyx_f_5rbfly_7streams_7_client_14PublisherTrait__next_message_id(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *__pyx_v_self, int __pyx_skip_dispatch, struct __pyx_opt_args_5rbfly_7streams_7_client_14PublisherTrait__next_message_id *__pyx_optional_args); /* proto*/
 static uint64_t __pyx_f_5rbfly_7streams_7_client_14PublisherTrait__reset_message_id(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *__pyx_v_self, uint64_t __pyx_v_message_id, int __pyx_skip_dispatch); /* proto*/
+static PyObject *__pyx_f_5rbfly_7streams_7_client_10Subscriber__next_message_offset(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 
 /* Module declarations from "cython" */
 
 /* Module declarations from "libc.stdint" */
 
 /* Module declarations from "rbfly._buffer" */
 
@@ -2697,15 +2764,15 @@
 static PyObject *__pyx_builtin_sorted;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_tp[] = "tp";
 static const char __pyx_k__10[] = "*";
 static const char __pyx_k__11[] = ".";
-static const char __pyx_k__52[] = "?";
+static const char __pyx_k__53[] = "?";
 static const char __pyx_k_ctx[] = "ctx";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_inc[] = "inc";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_pid[] = "pid";
 static const char __pyx_k_Lock[] = "Lock";
@@ -2737,14 +2804,15 @@
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_types[] = "types";
 static const char __pyx_k_Offset[] = "Offset";
 static const char __pyx_k_aenter[] = "__aenter__";
 static const char __pyx_k_client[] = "client";
 static const char __pyx_k_enable[] = "enable";
+static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_logger[] = "logger";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_offset[] = "offset";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_return[] = "return";
@@ -2794,16 +2862,18 @@
 static const char __pyx_k_read_stream[] = "read_stream";
 static const char __pyx_k_PublisherBin[] = "PublisherBin";
 static const char __pyx_k_get_protocol[] = "get_protocol";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_asyncio_tasks[] = "asyncio.tasks";
+static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_stream_offset[] = "stream_offset";
 static const char __pyx_k_KEY_PUBLISH_ID[] = "KEY_PUBLISH_ID";
 static const char __pyx_k_PublisherBatch[] = "PublisherBatch";
 static const char __pyx_k_PublisherTrait[] = "PublisherTrait";
 static const char __pyx_k_Publisher_send[] = "Publisher.send";
 static const char __pyx_k_app_properties[] = "app_properties";
 static const char __pyx_k_flush_messages[] = "_flush_messages";
 static const char __pyx_k_ConnectionError[] = "ConnectionError";
@@ -2822,14 +2892,15 @@
 static const char __pyx_k_Subscriber___aiter[] = "Subscriber.__aiter__";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_AMQPBody_MessageCtx[] = "AMQPBody | MessageCtx";
 static const char __pyx_k_PublisherBatchLimit[] = "PublisherBatchLimit";
 static const char __pyx_k_PublisherBatchTrait[] = "PublisherBatchTrait";
 static const char __pyx_k_batch_locals_lambda[] = "batch.<locals>.<lambda>";
+static const char __pyx_k_next_message_offset[] = "_next_message_offset";
 static const char __pyx_k_stream_messsage_ctx[] = "stream_messsage_ctx";
 static const char __pyx_k_rbfly_streams__client[] = "rbfly.streams._client";
 static const char __pyx_k_PublisherConstr___init[] = "PublisherConstr.__init__";
 static const char __pyx_k_PublisherBinBatch_batch[] = "PublisherBinBatch.batch";
 static const char __pyx_k_PublisherBinBatch_flush[] = "PublisherBinBatch.flush";
 static const char __pyx_k_PublisherTrait__publish[] = "PublisherTrait._publish";
 static const char __pyx_k_PublisherBatchFast_batch[] = "PublisherBatchFast.batch";
@@ -2845,28 +2916,30 @@
 static const char __pyx_k_Subscriber___setstate_cython[] = "Subscriber.__setstate_cython__";
 static const char __pyx_k_PublisherBatch___reduce_cython[] = "PublisherBatch.__reduce_cython__";
 static const char __pyx_k_PublisherBin___setstate_cython[] = "PublisherBin.__setstate_cython__";
 static const char __pyx_k_PublisherTrait___reduce_cython[] = "PublisherTrait.__reduce_cython__";
 static const char __pyx_k_Interface_for_publisher_classes[] = "\n    Interface for publisher classes constructor.\n    ";
 static const char __pyx_k_PublisherTrait__next_message_id[] = "PublisherTrait._next_message_id";
 static const char __pyx_k_RabbitMQ_Streams_publishers_pro[] = "\nRabbitMQ Streams publishers (producers) and subscribers (consumers).\n\nPublishers sending messages in AMQP format for two scenarios are implemented\n\n- sending single message\n- sending batch of messages\n\nThere are also publishers for sending opaque binary data implemented. These\nare used to measure overhead of AMQP 1.0 encoding with the official\npublishers. While these are not part of official API, they still can be\nused and are supported.\n\nSubscriber class implements RabbitMQ Streams message consumer. It supports\nboth AMQP 1.0 message format and opaque binary data.\n";
+static const char __pyx_k_Subscriber__next_message_offset[] = "Subscriber._next_message_offset";
 static const char __pyx_k_Connection_error_when_publishing[] = "Connection error when publishing messages";
 static const char __pyx_k_PublisherBatchFast___reduce_cyth[] = "PublisherBatchFast.__reduce_cython__";
 static const char __pyx_k_PublisherBatchFast___setstate_cy[] = "PublisherBatchFast.__setstate_cython__";
 static const char __pyx_k_PublisherBatchLimit___reduce_cyt[] = "PublisherBatchLimit.__reduce_cython__";
 static const char __pyx_k_PublisherBatchLimit___setstate_c[] = "PublisherBatchLimit.__setstate_cython__";
 static const char __pyx_k_PublisherBatchMem___reduce_cytho[] = "PublisherBatchMem.__reduce_cython__";
 static const char __pyx_k_PublisherBatchMem___setstate_cyt[] = "PublisherBatchMem.__setstate_cython__";
 static const char __pyx_k_PublisherBatchTrait___reduce_cyt[] = "PublisherBatchTrait.__reduce_cython__";
 static const char __pyx_k_PublisherBatchTrait___setstate_c[] = "PublisherBatchTrait.__setstate_cython__";
 static const char __pyx_k_PublisherBatch___setstate_cython[] = "PublisherBatch.__setstate_cython__";
 static const char __pyx_k_PublisherBinBatch___reduce_cytho[] = "PublisherBinBatch.__reduce_cython__";
 static const char __pyx_k_PublisherBinBatch___setstate_cyt[] = "PublisherBinBatch.__setstate_cython__";
 static const char __pyx_k_PublisherTrait___setstate_cython[] = "PublisherTrait.__setstate_cython__";
 static const char __pyx_k_PublisherTrait__reset_message_id[] = "PublisherTrait._reset_message_id";
+static const char __pyx_k_connection_error_received_id_ini[] = "connection error received, id={}, initial offset={}, error={}";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_5__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_pf_5rbfly_7streams_7_client_stream_messsage_ctx(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_body, PyObject *__pyx_v_publish_id, PyObject *__pyx_v_app_properties); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_15PublisherConstr___init__(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_client, CYTHON_UNUSED PyObject *__pyx_v_stream, CYTHON_UNUSED PyObject *__pyx_v_id, CYTHON_UNUSED PyObject *__pyx_v_name, CYTHON_UNUSED PyObject *__pyx_v_message_id); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_14PublisherTrait___cinit__(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *__pyx_v_self, PyObject *__pyx_v_client, PyObject *__pyx_v_stream, uint8_t __pyx_v_id, PyObject *__pyx_v_name, uint64_t __pyx_v_message_id); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_14PublisherTrait_2_next_message_id(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *__pyx_v_self, uint64_t __pyx_v_inc); /* proto */
@@ -2911,15 +2984,16 @@
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_12PublisherBin_3__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_PublisherBin *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_12PublisherBin_5__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_PublisherBin *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_batch(struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self, PyObject *__pyx_v_message); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_2flush(struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_5__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_17PublisherBinBatch_7__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_PublisherBinBatch *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber___cinit__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_client, PyObject *__pyx_v_stream, PyObject *__pyx_v_subscription_id, PyObject *__pyx_v_offset, double __pyx_v_timeout, PyObject *__pyx_v_amqp); /* proto */
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_2__aiter__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_2_next_message_offset(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_4__aiter__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_client_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_stream_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_16_subscription_id___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
@@ -2927,19 +3001,22 @@
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7_offset_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_timeout_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
 static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_5_amqp_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
-static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_9__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_7_client_2_flush_messages(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_5rbfly_7streams_7_client_PublisherBatchTrait *__pyx_v_publisher, PyObject *__pyx_v_data, PyObject *__pyx_v_amqp); /* proto */
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_6_flush(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_5_send(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_4_flush(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_3_batch(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -3085,18 +3162,19 @@
   PyObject *__pyx_n_s_Publisher___reduce_cython;
   PyObject *__pyx_n_s_Publisher___setstate_cython;
   PyObject *__pyx_n_s_Publisher_send;
   PyObject *__pyx_n_s_Subscriber;
   PyObject *__pyx_n_s_Subscriber___aiter;
   PyObject *__pyx_n_s_Subscriber___reduce_cython;
   PyObject *__pyx_n_s_Subscriber___setstate_cython;
+  PyObject *__pyx_n_s_Subscriber__next_message_offset;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s__10;
   PyObject *__pyx_kp_u__11;
-  PyObject *__pyx_n_s__52;
+  PyObject *__pyx_n_s__53;
   PyObject *__pyx_n_s_aenter;
   PyObject *__pyx_n_s_aexit;
   PyObject *__pyx_n_s_aiter;
   PyObject *__pyx_n_s_amqp;
   PyObject *__pyx_n_s_app_properties;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_asyncio;
@@ -3105,30 +3183,33 @@
   PyObject *__pyx_n_s_attrgetter;
   PyObject *__pyx_n_s_await;
   PyObject *__pyx_n_s_batch;
   PyObject *__pyx_n_s_batch_locals_lambda;
   PyObject *__pyx_n_s_body;
   PyObject *__pyx_n_s_bool;
   PyObject *__pyx_n_s_bytes;
+  PyObject *__pyx_n_s_class_getitem;
   PyObject *__pyx_n_s_client;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_close;
   PyObject *__pyx_n_s_collections;
   PyObject *__pyx_n_s_cond;
+  PyObject *__pyx_kp_u_connection_error_received_id_ini;
   PyObject *__pyx_n_s_count;
   PyObject *__pyx_n_s_ctx;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_debug;
   PyObject *__pyx_n_s_deque;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_s_doc;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_flush;
   PyObject *__pyx_n_s_flush_messages;
+  PyObject *__pyx_n_s_format;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_getLogger;
   PyObject *__pyx_n_s_get_protocol;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_id;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_inc;
@@ -3152,14 +3233,15 @@
   PyObject *__pyx_n_s_message_id;
   PyObject *__pyx_n_s_metaclass;
   PyObject *__pyx_n_s_module;
   PyObject *__pyx_n_s_mro_entries;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_name_2;
   PyObject *__pyx_n_s_next_message_id;
+  PyObject *__pyx_n_s_next_message_offset;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_notify_all;
   PyObject *__pyx_n_s_offset;
   PyObject *__pyx_n_s_operator;
   PyObject *__pyx_n_s_pid;
   PyObject *__pyx_n_s_popleft;
   PyObject *__pyx_n_s_prepare;
@@ -3184,14 +3266,15 @@
   PyObject *__pyx_n_s_set_name;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_sorted;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_stream;
   PyObject *__pyx_n_s_stream_messsage_ctx;
+  PyObject *__pyx_n_s_stream_offset;
   PyObject *__pyx_n_s_stream_publish_id;
   PyObject *__pyx_n_u_stream_publish_id;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_subscription_id;
   PyObject *__pyx_n_s_super;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_throw;
@@ -3213,15 +3296,15 @@
   PyObject *__pyx_tuple__22;
   PyObject *__pyx_tuple__23;
   PyObject *__pyx_tuple__25;
   PyObject *__pyx_tuple__29;
   PyObject *__pyx_tuple__32;
   PyObject *__pyx_tuple__36;
   PyObject *__pyx_tuple__37;
-  PyObject *__pyx_tuple__51;
+  PyObject *__pyx_tuple__52;
   PyObject *__pyx_codeobj__3;
   PyObject *__pyx_codeobj__4;
   PyObject *__pyx_codeobj__5;
   PyObject *__pyx_codeobj__6;
   PyObject *__pyx_codeobj__7;
   PyObject *__pyx_codeobj__8;
   PyObject *__pyx_codeobj__9;
@@ -3247,14 +3330,15 @@
   PyObject *__pyx_codeobj__44;
   PyObject *__pyx_codeobj__45;
   PyObject *__pyx_codeobj__46;
   PyObject *__pyx_codeobj__47;
   PyObject *__pyx_codeobj__48;
   PyObject *__pyx_codeobj__49;
   PyObject *__pyx_codeobj__50;
+  PyObject *__pyx_codeobj__51;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -3385,18 +3469,19 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Publisher___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Publisher___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Publisher_send);
   Py_CLEAR(clear_module_state->__pyx_n_s_Subscriber);
   Py_CLEAR(clear_module_state->__pyx_n_s_Subscriber___aiter);
   Py_CLEAR(clear_module_state->__pyx_n_s_Subscriber___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Subscriber___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Subscriber__next_message_offset);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s__10);
   Py_CLEAR(clear_module_state->__pyx_kp_u__11);
-  Py_CLEAR(clear_module_state->__pyx_n_s__52);
+  Py_CLEAR(clear_module_state->__pyx_n_s__53);
   Py_CLEAR(clear_module_state->__pyx_n_s_aenter);
   Py_CLEAR(clear_module_state->__pyx_n_s_aexit);
   Py_CLEAR(clear_module_state->__pyx_n_s_aiter);
   Py_CLEAR(clear_module_state->__pyx_n_s_amqp);
   Py_CLEAR(clear_module_state->__pyx_n_s_app_properties);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio);
@@ -3405,30 +3490,33 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_attrgetter);
   Py_CLEAR(clear_module_state->__pyx_n_s_await);
   Py_CLEAR(clear_module_state->__pyx_n_s_batch);
   Py_CLEAR(clear_module_state->__pyx_n_s_batch_locals_lambda);
   Py_CLEAR(clear_module_state->__pyx_n_s_body);
   Py_CLEAR(clear_module_state->__pyx_n_s_bool);
   Py_CLEAR(clear_module_state->__pyx_n_s_bytes);
+  Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
   Py_CLEAR(clear_module_state->__pyx_n_s_client);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_collections);
   Py_CLEAR(clear_module_state->__pyx_n_s_cond);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_connection_error_received_id_ini);
   Py_CLEAR(clear_module_state->__pyx_n_s_count);
   Py_CLEAR(clear_module_state->__pyx_n_s_ctx);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_debug);
   Py_CLEAR(clear_module_state->__pyx_n_s_deque);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_flush);
   Py_CLEAR(clear_module_state->__pyx_n_s_flush_messages);
+  Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_getLogger);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_protocol);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_id);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_inc);
@@ -3452,14 +3540,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_message_id);
   Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_module);
   Py_CLEAR(clear_module_state->__pyx_n_s_mro_entries);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_next_message_id);
+  Py_CLEAR(clear_module_state->__pyx_n_s_next_message_offset);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_notify_all);
   Py_CLEAR(clear_module_state->__pyx_n_s_offset);
   Py_CLEAR(clear_module_state->__pyx_n_s_operator);
   Py_CLEAR(clear_module_state->__pyx_n_s_pid);
   Py_CLEAR(clear_module_state->__pyx_n_s_popleft);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
@@ -3484,14 +3573,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_sorted);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_stream);
   Py_CLEAR(clear_module_state->__pyx_n_s_stream_messsage_ctx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_stream_offset);
   Py_CLEAR(clear_module_state->__pyx_n_s_stream_publish_id);
   Py_CLEAR(clear_module_state->__pyx_n_u_stream_publish_id);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_subscription_id);
   Py_CLEAR(clear_module_state->__pyx_n_s_super);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_throw);
@@ -3513,15 +3603,15 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__22);
   Py_CLEAR(clear_module_state->__pyx_tuple__23);
   Py_CLEAR(clear_module_state->__pyx_tuple__25);
   Py_CLEAR(clear_module_state->__pyx_tuple__29);
   Py_CLEAR(clear_module_state->__pyx_tuple__32);
   Py_CLEAR(clear_module_state->__pyx_tuple__36);
   Py_CLEAR(clear_module_state->__pyx_tuple__37);
-  Py_CLEAR(clear_module_state->__pyx_tuple__51);
+  Py_CLEAR(clear_module_state->__pyx_tuple__52);
   Py_CLEAR(clear_module_state->__pyx_codeobj__3);
   Py_CLEAR(clear_module_state->__pyx_codeobj__4);
   Py_CLEAR(clear_module_state->__pyx_codeobj__5);
   Py_CLEAR(clear_module_state->__pyx_codeobj__6);
   Py_CLEAR(clear_module_state->__pyx_codeobj__7);
   Py_CLEAR(clear_module_state->__pyx_codeobj__8);
   Py_CLEAR(clear_module_state->__pyx_codeobj__9);
@@ -3547,14 +3637,15 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__44);
   Py_CLEAR(clear_module_state->__pyx_codeobj__45);
   Py_CLEAR(clear_module_state->__pyx_codeobj__46);
   Py_CLEAR(clear_module_state->__pyx_codeobj__47);
   Py_CLEAR(clear_module_state->__pyx_codeobj__48);
   Py_CLEAR(clear_module_state->__pyx_codeobj__49);
   Py_CLEAR(clear_module_state->__pyx_codeobj__50);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__51);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3663,18 +3754,19 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Publisher___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Publisher___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Publisher_send);
   Py_VISIT(traverse_module_state->__pyx_n_s_Subscriber);
   Py_VISIT(traverse_module_state->__pyx_n_s_Subscriber___aiter);
   Py_VISIT(traverse_module_state->__pyx_n_s_Subscriber___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Subscriber___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Subscriber__next_message_offset);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s__10);
   Py_VISIT(traverse_module_state->__pyx_kp_u__11);
-  Py_VISIT(traverse_module_state->__pyx_n_s__52);
+  Py_VISIT(traverse_module_state->__pyx_n_s__53);
   Py_VISIT(traverse_module_state->__pyx_n_s_aenter);
   Py_VISIT(traverse_module_state->__pyx_n_s_aexit);
   Py_VISIT(traverse_module_state->__pyx_n_s_aiter);
   Py_VISIT(traverse_module_state->__pyx_n_s_amqp);
   Py_VISIT(traverse_module_state->__pyx_n_s_app_properties);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio);
@@ -3683,30 +3775,33 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_attrgetter);
   Py_VISIT(traverse_module_state->__pyx_n_s_await);
   Py_VISIT(traverse_module_state->__pyx_n_s_batch);
   Py_VISIT(traverse_module_state->__pyx_n_s_batch_locals_lambda);
   Py_VISIT(traverse_module_state->__pyx_n_s_body);
   Py_VISIT(traverse_module_state->__pyx_n_s_bool);
   Py_VISIT(traverse_module_state->__pyx_n_s_bytes);
+  Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
   Py_VISIT(traverse_module_state->__pyx_n_s_client);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_collections);
   Py_VISIT(traverse_module_state->__pyx_n_s_cond);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_connection_error_received_id_ini);
   Py_VISIT(traverse_module_state->__pyx_n_s_count);
   Py_VISIT(traverse_module_state->__pyx_n_s_ctx);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_debug);
   Py_VISIT(traverse_module_state->__pyx_n_s_deque);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_flush);
   Py_VISIT(traverse_module_state->__pyx_n_s_flush_messages);
+  Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_getLogger);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_protocol);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_id);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_inc);
@@ -3730,14 +3825,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_message_id);
   Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_module);
   Py_VISIT(traverse_module_state->__pyx_n_s_mro_entries);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_next_message_id);
+  Py_VISIT(traverse_module_state->__pyx_n_s_next_message_offset);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_notify_all);
   Py_VISIT(traverse_module_state->__pyx_n_s_offset);
   Py_VISIT(traverse_module_state->__pyx_n_s_operator);
   Py_VISIT(traverse_module_state->__pyx_n_s_pid);
   Py_VISIT(traverse_module_state->__pyx_n_s_popleft);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
@@ -3762,14 +3858,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_sorted);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_stream);
   Py_VISIT(traverse_module_state->__pyx_n_s_stream_messsage_ctx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_stream_offset);
   Py_VISIT(traverse_module_state->__pyx_n_s_stream_publish_id);
   Py_VISIT(traverse_module_state->__pyx_n_u_stream_publish_id);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_subscription_id);
   Py_VISIT(traverse_module_state->__pyx_n_s_super);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_throw);
@@ -3791,15 +3888,15 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__22);
   Py_VISIT(traverse_module_state->__pyx_tuple__23);
   Py_VISIT(traverse_module_state->__pyx_tuple__25);
   Py_VISIT(traverse_module_state->__pyx_tuple__29);
   Py_VISIT(traverse_module_state->__pyx_tuple__32);
   Py_VISIT(traverse_module_state->__pyx_tuple__36);
   Py_VISIT(traverse_module_state->__pyx_tuple__37);
-  Py_VISIT(traverse_module_state->__pyx_tuple__51);
+  Py_VISIT(traverse_module_state->__pyx_tuple__52);
   Py_VISIT(traverse_module_state->__pyx_codeobj__3);
   Py_VISIT(traverse_module_state->__pyx_codeobj__4);
   Py_VISIT(traverse_module_state->__pyx_codeobj__5);
   Py_VISIT(traverse_module_state->__pyx_codeobj__6);
   Py_VISIT(traverse_module_state->__pyx_codeobj__7);
   Py_VISIT(traverse_module_state->__pyx_codeobj__8);
   Py_VISIT(traverse_module_state->__pyx_codeobj__9);
@@ -3825,14 +3922,15 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__44);
   Py_VISIT(traverse_module_state->__pyx_codeobj__45);
   Py_VISIT(traverse_module_state->__pyx_codeobj__46);
   Py_VISIT(traverse_module_state->__pyx_codeobj__47);
   Py_VISIT(traverse_module_state->__pyx_codeobj__48);
   Py_VISIT(traverse_module_state->__pyx_codeobj__49);
   Py_VISIT(traverse_module_state->__pyx_codeobj__50);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__51);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3959,18 +4057,19 @@
 #define __pyx_n_s_Publisher___reduce_cython __pyx_mstate_global->__pyx_n_s_Publisher___reduce_cython
 #define __pyx_n_s_Publisher___setstate_cython __pyx_mstate_global->__pyx_n_s_Publisher___setstate_cython
 #define __pyx_n_s_Publisher_send __pyx_mstate_global->__pyx_n_s_Publisher_send
 #define __pyx_n_s_Subscriber __pyx_mstate_global->__pyx_n_s_Subscriber
 #define __pyx_n_s_Subscriber___aiter __pyx_mstate_global->__pyx_n_s_Subscriber___aiter
 #define __pyx_n_s_Subscriber___reduce_cython __pyx_mstate_global->__pyx_n_s_Subscriber___reduce_cython
 #define __pyx_n_s_Subscriber___setstate_cython __pyx_mstate_global->__pyx_n_s_Subscriber___setstate_cython
+#define __pyx_n_s_Subscriber__next_message_offset __pyx_mstate_global->__pyx_n_s_Subscriber__next_message_offset
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s__10 __pyx_mstate_global->__pyx_n_s__10
 #define __pyx_kp_u__11 __pyx_mstate_global->__pyx_kp_u__11
-#define __pyx_n_s__52 __pyx_mstate_global->__pyx_n_s__52
+#define __pyx_n_s__53 __pyx_mstate_global->__pyx_n_s__53
 #define __pyx_n_s_aenter __pyx_mstate_global->__pyx_n_s_aenter
 #define __pyx_n_s_aexit __pyx_mstate_global->__pyx_n_s_aexit
 #define __pyx_n_s_aiter __pyx_mstate_global->__pyx_n_s_aiter
 #define __pyx_n_s_amqp __pyx_mstate_global->__pyx_n_s_amqp
 #define __pyx_n_s_app_properties __pyx_mstate_global->__pyx_n_s_app_properties
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_asyncio __pyx_mstate_global->__pyx_n_s_asyncio
@@ -3979,30 +4078,33 @@
 #define __pyx_n_s_attrgetter __pyx_mstate_global->__pyx_n_s_attrgetter
 #define __pyx_n_s_await __pyx_mstate_global->__pyx_n_s_await
 #define __pyx_n_s_batch __pyx_mstate_global->__pyx_n_s_batch
 #define __pyx_n_s_batch_locals_lambda __pyx_mstate_global->__pyx_n_s_batch_locals_lambda
 #define __pyx_n_s_body __pyx_mstate_global->__pyx_n_s_body
 #define __pyx_n_s_bool __pyx_mstate_global->__pyx_n_s_bool
 #define __pyx_n_s_bytes __pyx_mstate_global->__pyx_n_s_bytes
+#define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
 #define __pyx_n_s_client __pyx_mstate_global->__pyx_n_s_client
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
 #define __pyx_n_s_collections __pyx_mstate_global->__pyx_n_s_collections
 #define __pyx_n_s_cond __pyx_mstate_global->__pyx_n_s_cond
+#define __pyx_kp_u_connection_error_received_id_ini __pyx_mstate_global->__pyx_kp_u_connection_error_received_id_ini
 #define __pyx_n_s_count __pyx_mstate_global->__pyx_n_s_count
 #define __pyx_n_s_ctx __pyx_mstate_global->__pyx_n_s_ctx
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_debug __pyx_mstate_global->__pyx_n_s_debug
 #define __pyx_n_s_deque __pyx_mstate_global->__pyx_n_s_deque
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_flush __pyx_mstate_global->__pyx_n_s_flush
 #define __pyx_n_s_flush_messages __pyx_mstate_global->__pyx_n_s_flush_messages
+#define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_getLogger __pyx_mstate_global->__pyx_n_s_getLogger
 #define __pyx_n_s_get_protocol __pyx_mstate_global->__pyx_n_s_get_protocol
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_id __pyx_mstate_global->__pyx_n_s_id
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_inc __pyx_mstate_global->__pyx_n_s_inc
@@ -4026,14 +4128,15 @@
 #define __pyx_n_s_message_id __pyx_mstate_global->__pyx_n_s_message_id
 #define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
 #define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
 #define __pyx_n_s_mro_entries __pyx_mstate_global->__pyx_n_s_mro_entries
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
 #define __pyx_n_s_next_message_id __pyx_mstate_global->__pyx_n_s_next_message_id
+#define __pyx_n_s_next_message_offset __pyx_mstate_global->__pyx_n_s_next_message_offset
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_notify_all __pyx_mstate_global->__pyx_n_s_notify_all
 #define __pyx_n_s_offset __pyx_mstate_global->__pyx_n_s_offset
 #define __pyx_n_s_operator __pyx_mstate_global->__pyx_n_s_operator
 #define __pyx_n_s_pid __pyx_mstate_global->__pyx_n_s_pid
 #define __pyx_n_s_popleft __pyx_mstate_global->__pyx_n_s_popleft
 #define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
@@ -4058,14 +4161,15 @@
 #define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_sorted __pyx_mstate_global->__pyx_n_s_sorted
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_stream __pyx_mstate_global->__pyx_n_s_stream
 #define __pyx_n_s_stream_messsage_ctx __pyx_mstate_global->__pyx_n_s_stream_messsage_ctx
+#define __pyx_n_s_stream_offset __pyx_mstate_global->__pyx_n_s_stream_offset
 #define __pyx_n_s_stream_publish_id __pyx_mstate_global->__pyx_n_s_stream_publish_id
 #define __pyx_n_u_stream_publish_id __pyx_mstate_global->__pyx_n_u_stream_publish_id
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_subscription_id __pyx_mstate_global->__pyx_n_s_subscription_id
 #define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
@@ -4087,15 +4191,15 @@
 #define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
 #define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
 #define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
 #define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
 #define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
 #define __pyx_tuple__36 __pyx_mstate_global->__pyx_tuple__36
 #define __pyx_tuple__37 __pyx_mstate_global->__pyx_tuple__37
-#define __pyx_tuple__51 __pyx_mstate_global->__pyx_tuple__51
+#define __pyx_tuple__52 __pyx_mstate_global->__pyx_tuple__52
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 #define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 #define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
 #define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
 #define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
@@ -4121,14 +4225,15 @@
 #define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
 #define __pyx_codeobj__45 __pyx_mstate_global->__pyx_codeobj__45
 #define __pyx_codeobj__46 __pyx_mstate_global->__pyx_codeobj__46
 #define __pyx_codeobj__47 __pyx_mstate_global->__pyx_codeobj__47
 #define __pyx_codeobj__48 __pyx_mstate_global->__pyx_codeobj__48
 #define __pyx_codeobj__49 __pyx_mstate_global->__pyx_codeobj__49
 #define __pyx_codeobj__50 __pyx_mstate_global->__pyx_codeobj__50
+#define __pyx_codeobj__51 __pyx_mstate_global->__pyx_codeobj__51
 /* #### Code section: module_code ### */
 
 /* "rbfly/streams/_client.pyx":55
  * KEY_PUBLISH_ID = operator.attrgetter('stream_publish_id')
  * 
  * def stream_messsage_ctx(             # <<<<<<<<<<<<<<
  *     body: AMQPBody,
@@ -11166,16 +11271,16 @@
   __Pyx_AddTraceback("rbfly.streams._client.PublisherBinBatch.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":462
- *         public MessageCtx _message
+/* "rbfly/streams/_client.pyx":466
+ *         public object _last_message
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *             self,
  *             client,
  */
 
 /* Python wrapper */
@@ -11216,55 +11321,55 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_client)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 462, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 466, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_stream)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 462, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 466, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 1); __PYX_ERR(1, 462, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 1); __PYX_ERR(1, 466, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_subscription_id)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 462, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 466, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 2); __PYX_ERR(1, 462, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 2); __PYX_ERR(1, 466, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_offset)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 462, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 466, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 3); __PYX_ERR(1, 462, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 3); __PYX_ERR(1, 466, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_timeout)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 462, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 466, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 4); __PYX_ERR(1, 462, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 4); __PYX_ERR(1, 466, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_amqp)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 462, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 466, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 5); __PYX_ERR(1, 462, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, 5); __PYX_ERR(1, 466, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 462, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 466, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 6)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
       values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
       values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
@@ -11272,27 +11377,27 @@
       values[4] = __Pyx_Arg_VARARGS(__pyx_args, 4);
       values[5] = __Pyx_Arg_VARARGS(__pyx_args, 5);
     }
     __pyx_v_client = values[0];
     __pyx_v_stream = ((PyObject*)values[1]);
     __pyx_v_subscription_id = ((PyObject*)values[2]);
     __pyx_v_offset = values[3];
-    __pyx_v_timeout = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_timeout == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 468, __pyx_L3_error)
+    __pyx_v_timeout = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_timeout == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 472, __pyx_L3_error)
     __pyx_v_amqp = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, __pyx_nargs); __PYX_ERR(1, 462, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 6, 6, __pyx_nargs); __PYX_ERR(1, 466, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.streams._client.Subscriber.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_stream), (&PyUnicode_Type), 0, "stream", 1))) __PYX_ERR(1, 465, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_subscription_id), (&PyInt_Type), 0, "subscription_id", 1))) __PYX_ERR(1, 466, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_stream), (&PyUnicode_Type), 0, "stream", 1))) __PYX_ERR(1, 469, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_subscription_id), (&PyInt_Type), 0, "subscription_id", 1))) __PYX_ERR(1, 470, __pyx_L1_error)
   __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber___cinit__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), __pyx_v_client, __pyx_v_stream, __pyx_v_subscription_id, __pyx_v_offset, __pyx_v_timeout, __pyx_v_amqp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -11306,97 +11411,110 @@
   uint8_t __pyx_t_1;
   char __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "rbfly/streams/_client.pyx":474
+  /* "rbfly/streams/_client.pyx":478
  *         Create RabbitMQ stream subscriber.
  *         """
  *         self._client = client             # <<<<<<<<<<<<<<
  *         self._stream = stream
  *         self._subscription_id = subscription_id
  */
   __Pyx_INCREF(__pyx_v_client);
   __Pyx_GIVEREF(__pyx_v_client);
   __Pyx_GOTREF(__pyx_v_self->_client);
   __Pyx_DECREF(__pyx_v_self->_client);
   __pyx_v_self->_client = __pyx_v_client;
 
-  /* "rbfly/streams/_client.pyx":475
+  /* "rbfly/streams/_client.pyx":479
  *         """
  *         self._client = client
  *         self._stream = stream             # <<<<<<<<<<<<<<
  *         self._subscription_id = subscription_id
  *         self._offset = offset
  */
   __Pyx_INCREF(__pyx_v_stream);
   __Pyx_GIVEREF(__pyx_v_stream);
   __Pyx_GOTREF(__pyx_v_self->_stream);
   __Pyx_DECREF(__pyx_v_self->_stream);
   __pyx_v_self->_stream = __pyx_v_stream;
 
-  /* "rbfly/streams/_client.pyx":476
+  /* "rbfly/streams/_client.pyx":480
  *         self._client = client
  *         self._stream = stream
  *         self._subscription_id = subscription_id             # <<<<<<<<<<<<<<
  *         self._offset = offset
  *         self._timeout = timeout
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_subscription_id); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 476, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_subscription_id); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 480, __pyx_L1_error)
   __pyx_v_self->_subscription_id = __pyx_t_1;
 
-  /* "rbfly/streams/_client.pyx":477
+  /* "rbfly/streams/_client.pyx":481
  *         self._stream = stream
  *         self._subscription_id = subscription_id
  *         self._offset = offset             # <<<<<<<<<<<<<<
  *         self._timeout = timeout
  *         self._amqp = amqp
  */
   __Pyx_INCREF(__pyx_v_offset);
   __Pyx_GIVEREF(__pyx_v_offset);
   __Pyx_GOTREF(__pyx_v_self->_offset);
   __Pyx_DECREF(__pyx_v_self->_offset);
   __pyx_v_self->_offset = __pyx_v_offset;
 
-  /* "rbfly/streams/_client.pyx":478
+  /* "rbfly/streams/_client.pyx":482
  *         self._subscription_id = subscription_id
  *         self._offset = offset
  *         self._timeout = timeout             # <<<<<<<<<<<<<<
  *         self._amqp = amqp
- *         self._message: MessageCtx | None = None
+ * 
  */
   __pyx_v_self->_timeout = __pyx_v_timeout;
 
-  /* "rbfly/streams/_client.pyx":479
+  /* "rbfly/streams/_client.pyx":483
  *         self._offset = offset
  *         self._timeout = timeout
  *         self._amqp = amqp             # <<<<<<<<<<<<<<
- *         self._message: MessageCtx | None = None
  * 
+ *         self._last_message = None
  */
-  __pyx_t_2 = __Pyx_PyInt_As_char(__pyx_v_amqp); if (unlikely((__pyx_t_2 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 479, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_char(__pyx_v_amqp); if (unlikely((__pyx_t_2 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 483, __pyx_L1_error)
   __pyx_v_self->_amqp = __pyx_t_2;
 
-  /* "rbfly/streams/_client.pyx":480
- *         self._timeout = timeout
+  /* "rbfly/streams/_client.pyx":485
  *         self._amqp = amqp
- *         self._message: MessageCtx | None = None             # <<<<<<<<<<<<<<
  * 
- *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:
+ *         self._last_message = None             # <<<<<<<<<<<<<<
+ *         self._messages = None
+ * 
+ */
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF(__pyx_v_self->_last_message);
+  __Pyx_DECREF(__pyx_v_self->_last_message);
+  __pyx_v_self->_last_message = Py_None;
+
+  /* "rbfly/streams/_client.pyx":486
+ * 
+ *         self._last_message = None
+ *         self._messages = None             # <<<<<<<<<<<<<<
+ * 
+ *     cpdef object _next_message_offset(self):
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  __Pyx_GOTREF((PyObject *)__pyx_v_self->_message);
-  __Pyx_DECREF((PyObject *)__pyx_v_self->_message);
-  __pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None);
+  __Pyx_GOTREF(__pyx_v_self->_messages);
+  __Pyx_DECREF(__pyx_v_self->_messages);
+  __pyx_v_self->_messages = Py_None;
 
-  /* "rbfly/streams/_client.pyx":462
- *         public MessageCtx _message
+  /* "rbfly/streams/_client.pyx":466
+ *         public object _last_message
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *             self,
  *             client,
  */
 
   /* function exit code */
@@ -11405,63 +11523,409 @@
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.streams._client.Subscriber.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_5rbfly_7streams_7_client_10Subscriber_4generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "rbfly/streams/_client.pyx":482
- *         self._message: MessageCtx | None = None
+/* "rbfly/streams/_client.pyx":488
+ *         self._messages = None
+ * 
+ *     cpdef object _next_message_offset(self):             # <<<<<<<<<<<<<<
+ *         """
+ *         Determine RabbitMQ Streams offset specification of next message to
+ */
+
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3_next_message_offset(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyObject *__pyx_f_5rbfly_7streams_7_client_10Subscriber__next_message_offset(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, int __pyx_skip_dispatch) {
+  PyObject *__pyx_v_offset = 0;
+  PyObject *__pyx_v_msg = NULL;
+  PyObject *__pyx_v_n = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  int __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_next_message_offset", 0);
+  /* Check if called by wrapper */
+  if (unlikely(__pyx_skip_dispatch)) ;
+  /* Check if overridden in Python */
+  else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
+    #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+    static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+    if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
+      PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      #endif
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_message_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 488, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      #ifdef __Pyx_CyFunction_USED
+      if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
+      #else
+      if (!PyCFunction_Check(__pyx_t_1)
+      #endif
+              || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3_next_message_offset)) {
+        __Pyx_XDECREF(__pyx_r);
+        __Pyx_INCREF(__pyx_t_1);
+        __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
+        __pyx_t_5 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_4)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_4);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_5 = 1;
+          }
+        }
+        {
+          PyObject *__pyx_callargs[1] = {__pyx_t_4, };
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 488, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        }
+        __pyx_r = __pyx_t_2;
+        __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        goto __pyx_L0;
+      }
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+      __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      __pyx_obj_dict_version = __Pyx_get_object_dict_version(((PyObject *)__pyx_v_self));
+      if (unlikely(__pyx_typedict_guard != __pyx_tp_dict_version)) {
+        __pyx_tp_dict_version = __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+      }
+      #endif
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+    }
+    #endif
+  }
+
+  /* "rbfly/streams/_client.pyx":495
+ *         cdef object offset
+ * 
+ *         if self._messages is None:             # <<<<<<<<<<<<<<
+ *             # no messages read yet, use the initial offset
+ *             offset = self._offset
+ */
+  __pyx_t_6 = (__pyx_v_self->_messages == Py_None);
+  if (__pyx_t_6) {
+
+    /* "rbfly/streams/_client.pyx":497
+ *         if self._messages is None:
+ *             # no messages read yet, use the initial offset
+ *             offset = self._offset             # <<<<<<<<<<<<<<
+ *         elif n := len(self._messages):
+ *             # eventually, the messages are to be read from the queue; use
+ */
+    __pyx_t_1 = __pyx_v_self->_offset;
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v_offset = __pyx_t_1;
+    __pyx_t_1 = 0;
+
+    /* "rbfly/streams/_client.pyx":495
+ *         cdef object offset
+ * 
+ *         if self._messages is None:             # <<<<<<<<<<<<<<
+ *             # no messages read yet, use the initial offset
+ *             offset = self._offset
+ */
+    goto __pyx_L3;
+  }
+
+  /* "rbfly/streams/_client.pyx":498
+ *             # no messages read yet, use the initial offset
+ *             offset = self._offset
+ *         elif n := len(self._messages):             # <<<<<<<<<<<<<<
+ *             # eventually, the messages are to be read from the queue; use
+ *             # the last message in the queue to determine next offset
+ */
+  __pyx_t_1 = __pyx_v_self->_messages;
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_7 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(1, 498, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 498, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_n = __pyx_t_1;
+  __pyx_t_1 = 0;
+  __pyx_t_6 = (__pyx_t_7 != 0);
+  if (__pyx_t_6) {
+
+    /* "rbfly/streams/_client.pyx":501
+ *             # eventually, the messages are to be read from the queue; use
+ *             # the last message in the queue to determine next offset
+ *             msg = self._messages[n - 1]             # <<<<<<<<<<<<<<
+ *             offset = Offset.offset(msg.stream_offset + 1)
+ *         else:
+ */
+    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_n, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 501, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_self->_messages, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 501, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_v_msg = __pyx_t_2;
+    __pyx_t_2 = 0;
+
+    /* "rbfly/streams/_client.pyx":502
+ *             # the last message in the queue to determine next offset
+ *             msg = self._messages[n - 1]
+ *             offset = Offset.offset(msg.stream_offset + 1)             # <<<<<<<<<<<<<<
+ *         else:
+ *             # queue is empty, use last message to determine next offset
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 502, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 502, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_stream_offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 502, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 502, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
+    __pyx_t_5 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_1);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_5 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_4};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 502, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
+    __pyx_v_offset = __pyx_t_2;
+    __pyx_t_2 = 0;
+
+    /* "rbfly/streams/_client.pyx":498
+ *             # no messages read yet, use the initial offset
+ *             offset = self._offset
+ *         elif n := len(self._messages):             # <<<<<<<<<<<<<<
+ *             # eventually, the messages are to be read from the queue; use
+ *             # the last message in the queue to determine next offset
+ */
+    goto __pyx_L3;
+  }
+
+  /* "rbfly/streams/_client.pyx":505
+ *         else:
+ *             # queue is empty, use last message to determine next offset
+ *             offset = Offset.offset(self._last_message.stream_offset + 1)             # <<<<<<<<<<<<<<
+ *         return offset
+ * 
+ */
+  /*else*/ {
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 505, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_offset); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 505, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_last_message, __pyx_n_s_stream_offset); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 505, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 505, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = NULL;
+    __pyx_t_5 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_3);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __pyx_t_5 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_1};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    }
+    __pyx_v_offset = __pyx_t_2;
+    __pyx_t_2 = 0;
+  }
+  __pyx_L3:;
+
+  /* "rbfly/streams/_client.pyx":506
+ *             # queue is empty, use last message to determine next offset
+ *             offset = Offset.offset(self._last_message.stream_offset + 1)
+ *         return offset             # <<<<<<<<<<<<<<
+ * 
+ *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_offset);
+  __pyx_r = __pyx_v_offset;
+  goto __pyx_L0;
+
+  /* "rbfly/streams/_client.pyx":488
+ *         self._messages = None
+ * 
+ *     cpdef object _next_message_offset(self):             # <<<<<<<<<<<<<<
+ *         """
+ *         Determine RabbitMQ Streams offset specification of next message to
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._next_message_offset", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_offset);
+  __Pyx_XDECREF(__pyx_v_msg);
+  __Pyx_XDECREF(__pyx_v_n);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3_next_message_offset(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_7_client_10Subscriber_2_next_message_offset, "Subscriber._next_message_offset(self)\n\n        Determine RabbitMQ Streams offset specification of next message to\n        be read from the stream.\n        ");
+static PyMethodDef __pyx_mdef_5rbfly_7streams_7_client_10Subscriber_3_next_message_offset = {"_next_message_offset", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3_next_message_offset, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_2_next_message_offset};
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3_next_message_offset(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("_next_message_offset (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("_next_message_offset", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "_next_message_offset", 0))) return NULL;
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_2_next_message_offset(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_2_next_message_offset(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_next_message_offset", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __pyx_f_5rbfly_7streams_7_client_10Subscriber__next_message_offset(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 488, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._next_message_offset", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+static PyObject *__pyx_gb_5rbfly_7streams_7_client_10Subscriber_6generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+
+/* "rbfly/streams/_client.pyx":508
+ *         return offset
  * 
  *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:             # <<<<<<<<<<<<<<
  *         """
  *         Iterate over messages read from a stream.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__(PyObject *__pyx_v_self); /*proto*/
-PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_7_client_10Subscriber_2__aiter__, "\n        Iterate over messages read from a stream.\n        ");
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_5__aiter__(PyObject *__pyx_v_self); /*proto*/
+PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_7_client_10Subscriber_4__aiter__, "\n        Iterate over messages read from a stream.\n        ");
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_2__aiter__;
+struct wrapperbase __pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_4__aiter__;
 #endif
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_5__aiter__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__aiter__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_2__aiter__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_4__aiter__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_2__aiter__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_4__aiter__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
   struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__aiter__", 0);
   __pyx_cur_scope = (struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ *)__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__(__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(1, 482, __pyx_L1_error)
+    __PYX_ERR(1, 508, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_AsyncGen_New((__pyx_coroutine_body_t) __pyx_gb_5rbfly_7streams_7_client_10Subscriber_4generator7, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_aiter, __pyx_n_s_Subscriber___aiter, __pyx_n_s_rbfly_streams__client); if (unlikely(!gen)) __PYX_ERR(1, 482, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_AsyncGen_New((__pyx_coroutine_body_t) __pyx_gb_5rbfly_7streams_7_client_10Subscriber_6generator7, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_aiter, __pyx_n_s_Subscriber___aiter, __pyx_n_s_rbfly_streams__client); if (unlikely(!gen)) __PYX_ERR(1, 508, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -11469,28 +11933,42 @@
   __pyx_r = NULL;
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_5rbfly_7streams_7_client_10Subscriber_4generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_5rbfly_7streams_7_client_10Subscriber_6generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ *__pyx_cur_scope = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   float __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  PyObject *__pyx_t_16 = NULL;
+  int __pyx_t_17;
+  char const *__pyx_t_18;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
+  PyObject *__pyx_t_23 = NULL;
+  PyObject *__pyx_t_24 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__aiter__", 0);
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
@@ -11498,70 +11976,70 @@
     case 2: goto __pyx_L16_resume_from_await;
     case 3: goto __pyx_L19_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 482, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 508, __pyx_L1_error)
 
-  /* "rbfly/streams/_client.pyx":487
+  /* "rbfly/streams/_client.pyx":513
  *         """
  *         cdef:
  *             float timeout = self._timeout             # <<<<<<<<<<<<<<
  *             object client = self._client
  *             object messages
  */
   __pyx_t_1 = __pyx_cur_scope->__pyx_v_self->_timeout;
   __pyx_cur_scope->__pyx_v_timeout = __pyx_t_1;
 
-  /* "rbfly/streams/_client.pyx":488
+  /* "rbfly/streams/_client.pyx":514
  *         cdef:
  *             float timeout = self._timeout
  *             object client = self._client             # <<<<<<<<<<<<<<
  *             object messages
  *             object protocol
  */
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self->_client;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_cur_scope->__pyx_v_client = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "rbfly/streams/_client.pyx":493
+  /* "rbfly/streams/_client.pyx":519
  *             object task
  * 
  *         while True:             # <<<<<<<<<<<<<<
  *             try:
  *                 protocol = await client.get_protocol()
  */
   while (1) {
 
-    /* "rbfly/streams/_client.pyx":494
+    /* "rbfly/streams/_client.pyx":520
  * 
  *         while True:
  *             try:             # <<<<<<<<<<<<<<
  *                 protocol = await client.get_protocol()
  *                 task = protocol.read_stream(self._subscription_id)
  */
     {
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "rbfly/streams/_client.pyx":495
+        /* "rbfly/streams/_client.pyx":521
  *         while True:
  *             try:
  *                 protocol = await client.get_protocol()             # <<<<<<<<<<<<<<
  *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:
  */
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_client, __pyx_n_s_get_protocol); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 495, __pyx_L6_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_client, __pyx_n_s_get_protocol); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 521, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = NULL;
         __pyx_t_8 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -11571,15 +12049,15 @@
             __pyx_t_8 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_7, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 495, __pyx_L6_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 521, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_2);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XGOTREF(__pyx_r);
         if (likely(__pyx_r)) {
@@ -11601,36 +12079,36 @@
           __Pyx_XGOTREF(__pyx_t_3);
           __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
           __pyx_cur_scope->__pyx_t_1 = 0;
           __Pyx_XGOTREF(__pyx_t_4);
           __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
           __pyx_cur_scope->__pyx_t_2 = 0;
           __Pyx_XGOTREF(__pyx_t_5);
-          if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 495, __pyx_L6_error)
+          if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 521, __pyx_L6_error)
           __pyx_t_2 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_2);
         } else {
           __pyx_t_2 = NULL;
-          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_2) < 0) __PYX_ERR(1, 495, __pyx_L6_error)
+          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_2) < 0) __PYX_ERR(1, 521, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_2);
         }
         __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_protocol);
         __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_protocol, __pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "rbfly/streams/_client.pyx":496
+        /* "rbfly/streams/_client.pyx":522
  *             try:
  *                 protocol = await client.get_protocol()
  *                 task = protocol.read_stream(self._subscription_id)             # <<<<<<<<<<<<<<
  *                 if timeout:
  *                     task = asyncio.wait_for(task, timeout)
  */
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_protocol, __pyx_n_s_read_stream); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 496, __pyx_L6_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_protocol, __pyx_n_s_read_stream); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 522, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_self->_subscription_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 496, __pyx_L6_error)
+        __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_self->_subscription_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 522, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_9 = NULL;
         __pyx_t_8 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -11641,46 +12119,46 @@
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_7};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 496, __pyx_L6_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 522, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
         __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_task);
         __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_task, __pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "rbfly/streams/_client.pyx":497
+        /* "rbfly/streams/_client.pyx":523
  *                 protocol = await client.get_protocol()
  *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:             # <<<<<<<<<<<<<<
  *                     task = asyncio.wait_for(task, timeout)
- *                 messages = await task
+ *                 messages = self._messages = await task
  */
         __pyx_t_10 = (__pyx_cur_scope->__pyx_v_timeout != 0);
         if (__pyx_t_10) {
 
-          /* "rbfly/streams/_client.pyx":498
+          /* "rbfly/streams/_client.pyx":524
  *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:
  *                     task = asyncio.wait_for(task, timeout)             # <<<<<<<<<<<<<<
- *                 messages = await task
- *             except ConnectionError:
+ *                 messages = self._messages = await task
+ *             except ConnectionError as ex:
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_asyncio); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 498, __pyx_L6_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_asyncio); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 524, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_wait_for); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 498, __pyx_L6_error)
+          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_wait_for); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 524, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-          __pyx_t_6 = PyFloat_FromDouble(__pyx_cur_scope->__pyx_v_timeout); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 498, __pyx_L6_error)
+          __pyx_t_6 = PyFloat_FromDouble(__pyx_cur_scope->__pyx_v_timeout); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 524, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_t_9 = NULL;
           __pyx_t_8 = 0;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
             __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
             if (likely(__pyx_t_9)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -11691,38 +12169,38 @@
             }
           }
           {
             PyObject *__pyx_callargs[3] = {__pyx_t_9, __pyx_cur_scope->__pyx_v_task, __pyx_t_6};
             __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 2+__pyx_t_8);
             __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-            if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 498, __pyx_L6_error)
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 524, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           }
           __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_task);
           __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_task, __pyx_t_2);
           __Pyx_GIVEREF(__pyx_t_2);
           __pyx_t_2 = 0;
 
-          /* "rbfly/streams/_client.pyx":497
+          /* "rbfly/streams/_client.pyx":523
  *                 protocol = await client.get_protocol()
  *                 task = protocol.read_stream(self._subscription_id)
  *                 if timeout:             # <<<<<<<<<<<<<<
  *                     task = asyncio.wait_for(task, timeout)
- *                 messages = await task
+ *                 messages = self._messages = await task
  */
         }
 
-        /* "rbfly/streams/_client.pyx":499
+        /* "rbfly/streams/_client.pyx":525
  *                 if timeout:
  *                     task = asyncio.wait_for(task, timeout)
- *                 messages = await task             # <<<<<<<<<<<<<<
- *             except ConnectionError:
- *                 pass
+ *                 messages = self._messages = await task             # <<<<<<<<<<<<<<
+ *             except ConnectionError as ex:
+ *                 logger.debug(
  */
         __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_cur_scope->__pyx_v_task);
         __Pyx_XGOTREF(__pyx_r);
         if (likely(__pyx_r)) {
           __Pyx_XGIVEREF(__pyx_t_3);
           __pyx_cur_scope->__pyx_t_0 = __pyx_t_3;
           __Pyx_XGIVEREF(__pyx_t_4);
@@ -11741,55 +12219,61 @@
           __Pyx_XGOTREF(__pyx_t_3);
           __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
           __pyx_cur_scope->__pyx_t_1 = 0;
           __Pyx_XGOTREF(__pyx_t_4);
           __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
           __pyx_cur_scope->__pyx_t_2 = 0;
           __Pyx_XGOTREF(__pyx_t_5);
-          if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 499, __pyx_L6_error)
+          if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 525, __pyx_L6_error)
           __pyx_t_2 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_2);
         } else {
           __pyx_t_2 = NULL;
-          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_2) < 0) __PYX_ERR(1, 499, __pyx_L6_error)
+          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_2) < 0) __PYX_ERR(1, 525, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_2);
         }
+        __Pyx_INCREF(__pyx_t_2);
         __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_messages);
         __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_messages, __pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_2);
-        __pyx_t_2 = 0;
+        __Pyx_INCREF(__pyx_t_2);
+        __Pyx_GIVEREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_self->_messages);
+        __Pyx_DECREF(__pyx_cur_scope->__pyx_v_self->_messages);
+        __pyx_cur_scope->__pyx_v_self->_messages = __pyx_t_2;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "rbfly/streams/_client.pyx":494
+        /* "rbfly/streams/_client.pyx":520
  * 
  *         while True:
  *             try:             # <<<<<<<<<<<<<<
  *                 protocol = await client.get_protocol()
  *                 task = protocol.read_stream(self._subscription_id)
  */
       }
 
-      /* "rbfly/streams/_client.pyx":503
- *                 pass
+      /* "rbfly/streams/_client.pyx":534
+ *                 )
  *             else:
  *                 while messages:             # <<<<<<<<<<<<<<
- *                     self._message = messages.popleft()
- *                     yield self._message
+ *                     self._last_message = messages.popleft()
+ *                     yield self._last_message
  */
       /*else:*/ {
         while (1) {
-          __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_messages); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(1, 503, __pyx_L8_except_error)
+          __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_messages); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(1, 534, __pyx_L8_except_error)
           if (!__pyx_t_10) break;
 
-          /* "rbfly/streams/_client.pyx":504
+          /* "rbfly/streams/_client.pyx":535
  *             else:
  *                 while messages:
- *                     self._message = messages.popleft()             # <<<<<<<<<<<<<<
- *                     yield self._message
+ *                     self._last_message = messages.popleft()             # <<<<<<<<<<<<<<
+ *                     yield self._last_message
  * 
  */
-          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_messages, __pyx_n_s_popleft); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 504, __pyx_L8_except_error)
+          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_messages, __pyx_n_s_popleft); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 535, __pyx_L8_except_error)
           __Pyx_GOTREF(__pyx_t_7);
           __pyx_t_6 = NULL;
           __pyx_t_8 = 0;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
             __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
             if (likely(__pyx_t_6)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -11799,34 +12283,33 @@
               __pyx_t_8 = 1;
             }
           }
           {
             PyObject *__pyx_callargs[1] = {__pyx_t_6, };
             __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
             __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-            if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 504, __pyx_L8_except_error)
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 535, __pyx_L8_except_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           }
-          if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx))))) __PYX_ERR(1, 504, __pyx_L8_except_error)
           __Pyx_GIVEREF(__pyx_t_2);
-          __Pyx_GOTREF((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
-          __Pyx_DECREF((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
-          __pyx_cur_scope->__pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_2);
+          __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_self->_last_message);
+          __Pyx_DECREF(__pyx_cur_scope->__pyx_v_self->_last_message);
+          __pyx_cur_scope->__pyx_v_self->_last_message = __pyx_t_2;
           __pyx_t_2 = 0;
 
-          /* "rbfly/streams/_client.pyx":505
+          /* "rbfly/streams/_client.pyx":536
  *                 while messages:
- *                     self._message = messages.popleft()
- *                     yield self._message             # <<<<<<<<<<<<<<
+ *                     self._last_message = messages.popleft()
+ *                     yield self._last_message             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  */
-          __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
-          __pyx_r = ((PyObject *)__pyx_cur_scope->__pyx_v_self->_message);
+          __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self->_last_message);
+          __pyx_r = __pyx_cur_scope->__pyx_v_self->_last_message;
           __Pyx_XGIVEREF(__pyx_t_3);
           __pyx_cur_scope->__pyx_t_0 = __pyx_t_3;
           __Pyx_XGIVEREF(__pyx_t_4);
           __pyx_cur_scope->__pyx_t_1 = __pyx_t_4;
           __Pyx_XGIVEREF(__pyx_t_5);
           __pyx_cur_scope->__pyx_t_2 = __pyx_t_5;
           __Pyx_XGIVEREF(__pyx_r);
@@ -11841,49 +12324,194 @@
           __Pyx_XGOTREF(__pyx_t_3);
           __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
           __pyx_cur_scope->__pyx_t_1 = 0;
           __Pyx_XGOTREF(__pyx_t_4);
           __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
           __pyx_cur_scope->__pyx_t_2 = 0;
           __Pyx_XGOTREF(__pyx_t_5);
-          if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 505, __pyx_L8_except_error)
+          if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 536, __pyx_L8_except_error)
         }
       }
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L13_try_end;
       __pyx_L6_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-      /* "rbfly/streams/_client.pyx":500
+      /* "rbfly/streams/_client.pyx":526
  *                     task = asyncio.wait_for(task, timeout)
- *                 messages = await task
- *             except ConnectionError:             # <<<<<<<<<<<<<<
- *                 pass
- *             else:
+ *                 messages = self._messages = await task
+ *             except ConnectionError as ex:             # <<<<<<<<<<<<<<
+ *                 logger.debug(
+ *                     'connection error received, id={}, initial offset={},'
  */
       __Pyx_ErrFetch(&__pyx_t_2, &__pyx_t_7, &__pyx_t_6);
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_ConnectionError); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 500, __pyx_L8_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_ConnectionError); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 526, __pyx_L8_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_2, __pyx_t_9);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_ErrRestore(__pyx_t_2, __pyx_t_7, __pyx_t_6);
       __pyx_t_2 = 0; __pyx_t_7 = 0; __pyx_t_6 = 0;
       if (__pyx_t_8) {
-        __Pyx_ErrRestore(0,0,0);
+        __Pyx_AddTraceback("rbfly.streams._client.Subscriber.__aiter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+        if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_2) < 0) __PYX_ERR(1, 526, __pyx_L8_except_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_7);
+        __Pyx_GIVEREF(__pyx_t_7);
+        __pyx_cur_scope->__pyx_v_ex = __pyx_t_7;
+        /*try:*/ {
+
+          /* "rbfly/streams/_client.pyx":527
+ *                 messages = self._messages = await task
+ *             except ConnectionError as ex:
+ *                 logger.debug(             # <<<<<<<<<<<<<<
+ *                     'connection error received, id={}, initial offset={},'
+ *                     ' error={}'.format(
+ */
+          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_logger); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 527, __pyx_L25_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_debug); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 527, __pyx_L25_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+
+          /* "rbfly/streams/_client.pyx":529
+ *                 logger.debug(
+ *                     'connection error received, id={}, initial offset={},'
+ *                     ' error={}'.format(             # <<<<<<<<<<<<<<
+ *                         self._subscription_id, self._offset, str(ex)
+ *                     )
+ */
+          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_connection_error_received_id_ini, __pyx_n_s_format); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 529, __pyx_L25_error)
+          __Pyx_GOTREF(__pyx_t_13);
+
+          /* "rbfly/streams/_client.pyx":530
+ *                     'connection error received, id={}, initial offset={},'
+ *                     ' error={}'.format(
+ *                         self._subscription_id, self._offset, str(ex)             # <<<<<<<<<<<<<<
+ *                     )
+ *                 )
+ */
+          __pyx_t_14 = __Pyx_PyInt_From_uint8_t(__pyx_cur_scope->__pyx_v_self->_subscription_id); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 530, __pyx_L25_error)
+          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_15 = __Pyx_PyObject_Str(__pyx_cur_scope->__pyx_v_ex); if (unlikely(!__pyx_t_15)) __PYX_ERR(1, 530, __pyx_L25_error)
+          __Pyx_GOTREF(__pyx_t_15);
+          __pyx_t_16 = NULL;
+          __pyx_t_8 = 0;
+          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
+            __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_13);
+            if (likely(__pyx_t_16)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
+              __Pyx_INCREF(__pyx_t_16);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_13, function);
+              __pyx_t_8 = 1;
+            }
+          }
+          {
+            PyObject *__pyx_callargs[4] = {__pyx_t_16, __pyx_t_14, __pyx_cur_scope->__pyx_v_self->_offset, __pyx_t_15};
+            __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_8, 3+__pyx_t_8);
+            __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+            __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+            __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+            if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 529, __pyx_L25_error)
+            __Pyx_GOTREF(__pyx_t_11);
+            __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+          }
+          __pyx_t_13 = NULL;
+          __pyx_t_8 = 0;
+          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+            __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
+            if (likely(__pyx_t_13)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+              __Pyx_INCREF(__pyx_t_13);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_12, function);
+              __pyx_t_8 = 1;
+            }
+          }
+          {
+            PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_t_11};
+            __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+            __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+            if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 527, __pyx_L25_error)
+            __Pyx_GOTREF(__pyx_t_9);
+            __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          }
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        }
+
+        /* "rbfly/streams/_client.pyx":526
+ *                     task = asyncio.wait_for(task, timeout)
+ *                 messages = self._messages = await task
+ *             except ConnectionError as ex:             # <<<<<<<<<<<<<<
+ *                 logger.debug(
+ *                     'connection error received, id={}, initial offset={},'
+ */
+        /*finally:*/ {
+          /*normal exit:*/{
+            __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_ex);
+            __Pyx_DECREF(__pyx_cur_scope->__pyx_v_ex); __pyx_cur_scope->__pyx_v_ex = 0;
+            goto __pyx_L26;
+          }
+          __pyx_L25_error:;
+          /*exception exit:*/{
+            __Pyx_PyThreadState_assign
+            __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0;
+            __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+            __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+            __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+            __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+            __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+            if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_22, &__pyx_t_23, &__pyx_t_24);
+            if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21) < 0)) __Pyx_ErrFetch(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21);
+            __Pyx_XGOTREF(__pyx_t_19);
+            __Pyx_XGOTREF(__pyx_t_20);
+            __Pyx_XGOTREF(__pyx_t_21);
+            __Pyx_XGOTREF(__pyx_t_22);
+            __Pyx_XGOTREF(__pyx_t_23);
+            __Pyx_XGOTREF(__pyx_t_24);
+            __pyx_t_8 = __pyx_lineno; __pyx_t_17 = __pyx_clineno; __pyx_t_18 = __pyx_filename;
+            {
+              __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_ex);
+              __Pyx_DECREF(__pyx_cur_scope->__pyx_v_ex); __pyx_cur_scope->__pyx_v_ex = 0;
+            }
+            if (PY_MAJOR_VERSION >= 3) {
+              __Pyx_XGIVEREF(__pyx_t_22);
+              __Pyx_XGIVEREF(__pyx_t_23);
+              __Pyx_XGIVEREF(__pyx_t_24);
+              __Pyx_ExceptionReset(__pyx_t_22, __pyx_t_23, __pyx_t_24);
+            }
+            __Pyx_XGIVEREF(__pyx_t_19);
+            __Pyx_XGIVEREF(__pyx_t_20);
+            __Pyx_XGIVEREF(__pyx_t_21);
+            __Pyx_ErrRestore(__pyx_t_19, __pyx_t_20, __pyx_t_21);
+            __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0; __pyx_t_24 = 0;
+            __pyx_lineno = __pyx_t_8; __pyx_clineno = __pyx_t_17; __pyx_filename = __pyx_t_18;
+            goto __pyx_L8_except_error;
+          }
+          __pyx_L26:;
+        }
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         goto __pyx_L7_exception_handled;
       }
       goto __pyx_L8_except_error;
       __pyx_L8_except_error:;
 
-      /* "rbfly/streams/_client.pyx":494
+      /* "rbfly/streams/_client.pyx":520
  * 
  *         while True:
  *             try:             # <<<<<<<<<<<<<<
  *                 protocol = await client.get_protocol()
  *                 task = protocol.read_stream(self._subscription_id)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -11897,16 +12525,16 @@
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       __pyx_L13_try_end:;
     }
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "rbfly/streams/_client.pyx":482
- *         self._message: MessageCtx | None = None
+  /* "rbfly/streams/_client.pyx":508
+ *         return offset
  * 
  *     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:             # <<<<<<<<<<<<<<
  *         """
  *         Iterate over messages read from a stream.
  */
 
   /* function exit code */
@@ -11914,27 +12542,33 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_Generator_Replace_StopIteration(1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_XDECREF(__pyx_t_14);
+  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_16);
   __Pyx_AddTraceback("__aiter__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_r); __pyx_r = 0;
   #if !CYTHON_USE_EXC_INFO_STACK
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":454
+/* "rbfly/streams/_client.pyx":456
  *     """
  *     cdef:
  *         public object _client             # <<<<<<<<<<<<<<
  *         public str _stream
  *         public uint8_t _subscription_id
  */
 
@@ -12024,15 +12658,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":455
+/* "rbfly/streams/_client.pyx":457
  *     cdef:
  *         public object _client
  *         public str _stream             # <<<<<<<<<<<<<<
  *         public uint8_t _subscription_id
  *         public object _offset
  */
 
@@ -12084,15 +12718,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(1, 455, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(1, 457, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_stream);
   __Pyx_DECREF(__pyx_v_self->_stream);
   __pyx_v_self->_stream = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -12135,15 +12769,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":456
+/* "rbfly/streams/_client.pyx":458
  *         public object _client
  *         public str _stream
  *         public uint8_t _subscription_id             # <<<<<<<<<<<<<<
  *         public object _offset
  *         public float _timeout
  */
 
@@ -12166,15 +12800,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_subscription_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 456, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_subscription_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12205,29 +12839,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   uint8_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 456, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 458, __pyx_L1_error)
   __pyx_v_self->_subscription_id = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.streams._client.Subscriber._subscription_id.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":457
+/* "rbfly/streams/_client.pyx":459
  *         public str _stream
  *         public uint8_t _subscription_id
  *         public object _offset             # <<<<<<<<<<<<<<
  *         public float _timeout
  *         public char _amqp
  */
 
@@ -12317,20 +12951,20 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":458
+/* "rbfly/streams/_client.pyx":460
  *         public uint8_t _subscription_id
  *         public object _offset
  *         public float _timeout             # <<<<<<<<<<<<<<
  *         public char _amqp
- *         public MessageCtx _message
+ * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_timeout_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
@@ -12348,15 +12982,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 458, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12387,34 +13021,34 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   float __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_value); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 458, __pyx_L1_error)
+  __pyx_t_1 = __pyx_PyFloat_AsFloat(__pyx_v_value); if (unlikely((__pyx_t_1 == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 460, __pyx_L1_error)
   __pyx_v_self->_timeout = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.streams._client.Subscriber._timeout.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":459
+/* "rbfly/streams/_client.pyx":461
  *         public object _offset
  *         public float _timeout
  *         public char _amqp             # <<<<<<<<<<<<<<
- *         public MessageCtx _message
  * 
+ *         public object _messages
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_5_amqp_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
@@ -12432,15 +13066,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_self->_amqp); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 459, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_self->_amqp); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -12471,156 +13105,241 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   char __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_char(__pyx_v_value); if (unlikely((__pyx_t_1 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 459, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_char(__pyx_v_value); if (unlikely((__pyx_t_1 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 461, __pyx_L1_error)
   __pyx_v_self->_amqp = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.streams._client.Subscriber._amqp.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":460
- *         public float _timeout
+/* "rbfly/streams/_client.pyx":463
  *         public char _amqp
- *         public MessageCtx _message             # <<<<<<<<<<<<<<
  * 
- *     def __cinit__(
+ *         public object _messages             # <<<<<<<<<<<<<<
+ *         public object _last_message
+ * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF((PyObject *)__pyx_v_self->_message);
-  __pyx_r = ((PyObject *)__pyx_v_self->_message);
+  __Pyx_INCREF(__pyx_v_self->_messages);
+  __pyx_r = __pyx_v_self->_messages;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx))))) __PYX_ERR(1, 460, __pyx_L1_error)
-  __pyx_t_1 = __pyx_v_value;
-  __Pyx_INCREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF((PyObject *)__pyx_v_self->_message);
-  __Pyx_DECREF((PyObject *)__pyx_v_self->_message);
-  __pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __Pyx_INCREF(__pyx_v_value);
+  __Pyx_GIVEREF(__pyx_v_value);
+  __Pyx_GOTREF(__pyx_v_self->_messages);
+  __Pyx_DECREF(__pyx_v_self->_messages);
+  __pyx_v_self->_messages = __pyx_v_value;
+
+  /* function exit code */
+  __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_5__del__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages_4__del__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9_messages_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__del__", 0);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  __Pyx_GOTREF(__pyx_v_self->_messages);
+  __Pyx_DECREF(__pyx_v_self->_messages);
+  __pyx_v_self->_messages = Py_None;
 
   /* function exit code */
   __pyx_r = 0;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "rbfly/streams/_client.pyx":464
+ * 
+ *         public object _messages
+ *         public object _last_message             # <<<<<<<<<<<<<<
+ * 
+ *     def __cinit__(
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_1__get__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message___get__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message___get__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->_last_message);
+  __pyx_r = __pyx_v_self->_last_message;
   goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rbfly.streams._client.Subscriber._message.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
+
+  /* function exit code */
   __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message_2__set__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message_2__set__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__", 0);
+  __Pyx_INCREF(__pyx_v_value);
+  __Pyx_GIVEREF(__pyx_v_value);
+  __Pyx_GOTREF(__pyx_v_self->_last_message);
+  __Pyx_DECREF(__pyx_v_self->_last_message);
+  __pyx_v_self->_last_message = __pyx_v_value;
+
+  /* function exit code */
+  __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_5__del__(PyObject *__pyx_v_self); /*proto*/
-static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_5__del__(PyObject *__pyx_v_self) {
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_5__del__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_4__del__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message_4__del__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_8_message_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+static int __pyx_pf_5rbfly_7streams_7_client_10Subscriber_13_last_message_4__del__(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__del__", 0);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  __Pyx_GOTREF((PyObject *)__pyx_v_self->_message);
-  __Pyx_DECREF((PyObject *)__pyx_v_self->_message);
-  __pyx_v_self->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None);
+  __Pyx_GOTREF(__pyx_v_self->_last_message);
+  __Pyx_DECREF(__pyx_v_self->_last_message);
+  __pyx_v_self->_last_message = Py_None;
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_6__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__, "Subscriber.__reduce_cython__(self)");
-static PyMethodDef __pyx_mdef_5rbfly_7streams_7_client_10Subscriber_6__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_6__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__};
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_6__reduce_cython__(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_7_client_10Subscriber_7__reduce_cython__, "Subscriber.__reduce_cython__(self)");
+static PyMethodDef __pyx_mdef_5rbfly_7streams_7_client_10Subscriber_8__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_7__reduce_cython__};
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -12629,22 +13348,22 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7__reduce_cython__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
@@ -12676,24 +13395,24 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_10__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__, "Subscriber.__setstate_cython__(self, __pyx_state)");
-static PyMethodDef __pyx_mdef_5rbfly_7streams_7_client_10Subscriber_8__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__};
-static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__setstate_cython__(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_7_client_10Subscriber_9__setstate_cython__, "Subscriber.__setstate_cython__(self, __pyx_state)");
+static PyMethodDef __pyx_mdef_5rbfly_7streams_7_client_10Subscriber_10__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_10__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_9__setstate_cython__};
+static PyObject *__pyx_pw_5rbfly_7streams_7_client_10Subscriber_10__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
@@ -12740,22 +13459,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 3, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.streams._client.Subscriber.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_5rbfly_7streams_7_client_10Subscriber_9__setstate_cython__(((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_5rbfly_7streams_7_client_10Subscriber_9__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
@@ -12779,70 +13498,70 @@
   __Pyx_AddTraceback("rbfly.streams._client.Subscriber.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_client.pyx":507
- *                     yield self._message
+/* "rbfly/streams/_client.pyx":538
+ *                     yield self._last_message
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):             # <<<<<<<<<<<<<<
  *     if not ctx.is_set_stream_publish_id:
  *         ctx.stream_publish_id = publisher.message_id
  */
 
 static CYTHON_INLINE void __pyx_f_5rbfly_7streams_7_client__before_ctx_publish(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *__pyx_v_publisher, struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_v_ctx) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   uint64_t __pyx_t_2;
   __Pyx_RefNannySetupContext("_before_ctx_publish", 0);
 
-  /* "rbfly/streams/_client.pyx":508
+  /* "rbfly/streams/_client.pyx":539
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  *     if not ctx.is_set_stream_publish_id:             # <<<<<<<<<<<<<<
  *         ctx.stream_publish_id = publisher.message_id
  * 
  */
   __pyx_t_1 = (!(__pyx_v_ctx->is_set_stream_publish_id != 0));
   if (__pyx_t_1) {
 
-    /* "rbfly/streams/_client.pyx":509
+    /* "rbfly/streams/_client.pyx":540
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  *     if not ctx.is_set_stream_publish_id:
  *         ctx.stream_publish_id = publisher.message_id             # <<<<<<<<<<<<<<
  * 
  * cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  */
     __pyx_t_2 = __pyx_v_publisher->message_id;
     __pyx_v_ctx->stream_publish_id = __pyx_t_2;
 
-    /* "rbfly/streams/_client.pyx":508
+    /* "rbfly/streams/_client.pyx":539
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  *     if not ctx.is_set_stream_publish_id:             # <<<<<<<<<<<<<<
  *         ctx.stream_publish_id = publisher.message_id
  * 
  */
   }
 
-  /* "rbfly/streams/_client.pyx":507
- *                     yield self._message
+  /* "rbfly/streams/_client.pyx":538
+ *                     yield self._last_message
  * 
  * cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):             # <<<<<<<<<<<<<<
  *     if not ctx.is_set_stream_publish_id:
  *         ctx.stream_publish_id = publisher.message_id
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "rbfly/streams/_client.pyx":511
+/* "rbfly/streams/_client.pyx":542
  *         ctx.stream_publish_id = publisher.message_id
  * 
  * cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):             # <<<<<<<<<<<<<<
  *     if ctx.is_set_stream_publish_id:
  *         publisher._reset_message_id(ctx.stream_publish_id)
  */
 
@@ -12850,56 +13569,56 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_after_ctx_publish", 0);
 
-  /* "rbfly/streams/_client.pyx":512
+  /* "rbfly/streams/_client.pyx":543
  * 
  * cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  *     if ctx.is_set_stream_publish_id:             # <<<<<<<<<<<<<<
  *         publisher._reset_message_id(ctx.stream_publish_id)
  *     else:
  */
   __pyx_t_1 = (__pyx_v_ctx->is_set_stream_publish_id != 0);
   if (__pyx_t_1) {
 
-    /* "rbfly/streams/_client.pyx":513
+    /* "rbfly/streams/_client.pyx":544
  * cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  *     if ctx.is_set_stream_publish_id:
  *         publisher._reset_message_id(ctx.stream_publish_id)             # <<<<<<<<<<<<<<
  *     else:
  *         publisher._next_message_id()
  */
-    ((struct __pyx_vtabstruct_5rbfly_7streams_7_client_PublisherTrait *)__pyx_v_publisher->__pyx_vtab)->_reset_message_id(__pyx_v_publisher, __pyx_v_ctx->stream_publish_id, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 513, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5rbfly_7streams_7_client_PublisherTrait *)__pyx_v_publisher->__pyx_vtab)->_reset_message_id(__pyx_v_publisher, __pyx_v_ctx->stream_publish_id, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 544, __pyx_L1_error)
 
-    /* "rbfly/streams/_client.pyx":512
+    /* "rbfly/streams/_client.pyx":543
  * 
  * cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
  *     if ctx.is_set_stream_publish_id:             # <<<<<<<<<<<<<<
  *         publisher._reset_message_id(ctx.stream_publish_id)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/streams/_client.pyx":515
+  /* "rbfly/streams/_client.pyx":546
  *         publisher._reset_message_id(ctx.stream_publish_id)
  *     else:
  *         publisher._next_message_id()             # <<<<<<<<<<<<<<
  * 
  * async def _flush_messages(
  */
   /*else*/ {
-    ((struct __pyx_vtabstruct_5rbfly_7streams_7_client_PublisherTrait *)__pyx_v_publisher->__pyx_vtab)->_next_message_id(__pyx_v_publisher, 0, NULL); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 515, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_5rbfly_7streams_7_client_PublisherTrait *)__pyx_v_publisher->__pyx_vtab)->_next_message_id(__pyx_v_publisher, 0, NULL); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 546, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "rbfly/streams/_client.pyx":511
+  /* "rbfly/streams/_client.pyx":542
  *         ctx.stream_publish_id = publisher.message_id
  * 
  * cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):             # <<<<<<<<<<<<<<
  *     if ctx.is_set_stream_publish_id:
  *         publisher._reset_message_id(ctx.stream_publish_id)
  */
 
@@ -12908,15 +13627,15 @@
   __pyx_L1_error:;
   __Pyx_AddTraceback("rbfly.streams._client._after_ctx_publish", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 static PyObject *__pyx_gb_5rbfly_7streams_7_client_4generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "rbfly/streams/_client.pyx":517
+/* "rbfly/streams/_client.pyx":548
  *         publisher._next_message_id()
  * 
  * async def _flush_messages(             # <<<<<<<<<<<<<<
  *         publisher: PublisherBatchTrait,
  *         data: list[MessageCtx],
  */
 
@@ -12950,15 +13669,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_flush_messages (wrapper)", 0);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_publisher,&__pyx_n_s_data,&__pyx_n_s_amqp,0};
     PyObject* values[3] = {0,0,0};
 
-    /* "rbfly/streams/_client.pyx":521
+    /* "rbfly/streams/_client.pyx":552
  *         data: list[MessageCtx],
  *         *,
  *         amqp: bool=True,             # <<<<<<<<<<<<<<
  * ) -> list[MessageCtx]:
  *     """
  */
     values[2] = ((PyObject *)((PyObject *)Py_True));
@@ -12972,57 +13691,57 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_publisher)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 517, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 517, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_flush_messages", 1, 2, 2, 1); __PYX_ERR(1, 517, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_flush_messages", 1, 2, 2, 1); __PYX_ERR(1, 548, __pyx_L3_error)
         }
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 2;
         PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
         if (value) { values[index] = value; kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 517, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 548, __pyx_L3_error)
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_flush_messages") < 0)) __PYX_ERR(1, 517, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_flush_messages") < 0)) __PYX_ERR(1, 548, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_publisher = ((struct __pyx_obj_5rbfly_7streams_7_client_PublisherBatchTrait *)values[0]);
     __pyx_v_data = ((PyObject*)values[1]);
     __pyx_v_amqp = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_flush_messages", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 517, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_flush_messages", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 548, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.streams._client._flush_messages", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_publisher), __pyx_ptype_5rbfly_7streams_7_client_PublisherBatchTrait, 0, "publisher", 0))) __PYX_ERR(1, 518, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyList_Type), 0, "data", 1))) __PYX_ERR(1, 519, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_publisher), __pyx_ptype_5rbfly_7streams_7_client_PublisherBatchTrait, 0, "publisher", 0))) __PYX_ERR(1, 549, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyList_Type), 0, "data", 1))) __PYX_ERR(1, 550, __pyx_L1_error)
   __pyx_r = __pyx_pf_5rbfly_7streams_7_client_2_flush_messages(__pyx_self, __pyx_v_publisher, __pyx_v_data, __pyx_v_amqp);
 
-  /* "rbfly/streams/_client.pyx":517
+  /* "rbfly/streams/_client.pyx":548
  *         publisher._next_message_id()
  * 
  * async def _flush_messages(             # <<<<<<<<<<<<<<
  *         publisher: PublisherBatchTrait,
  *         data: list[MessageCtx],
  */
 
@@ -13043,29 +13762,29 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_flush_messages", 0);
   __pyx_cur_scope = (struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages *)__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages(__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(1, 517, __pyx_L1_error)
+    __PYX_ERR(1, 548, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_publisher = __pyx_v_publisher;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_publisher);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_publisher);
   __pyx_cur_scope->__pyx_v_data = __pyx_v_data;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_data);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_data);
   __pyx_cur_scope->__pyx_v_amqp = __pyx_v_amqp;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_amqp);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_amqp);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_5rbfly_7streams_7_client_4generator8, __pyx_codeobj__9, (PyObject *) __pyx_cur_scope, __pyx_n_s_flush_messages, __pyx_n_s_flush_messages, __pyx_n_s_rbfly_streams__client); if (unlikely(!gen)) __PYX_ERR(1, 517, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_5rbfly_7streams_7_client_4generator8, __pyx_codeobj__9, (PyObject *) __pyx_cur_scope, __pyx_n_s_flush_messages, __pyx_n_s_flush_messages, __pyx_n_s_rbfly_streams__client); if (unlikely(!gen)) __PYX_ERR(1, 548, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13096,42 +13815,42 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_await;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 517, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 548, __pyx_L1_error)
 
-  /* "rbfly/streams/_client.pyx":529
+  /* "rbfly/streams/_client.pyx":560
  *         Py_ssize_t count
  * 
  *     while data:             # <<<<<<<<<<<<<<
  *         count = await publisher._publish(*data, amqp=amqp)
  *         del data[:count]
  */
   while (1) {
     __pyx_t_1 = (PyList_GET_SIZE(__pyx_cur_scope->__pyx_v_data) != 0);
     if (!__pyx_t_1) break;
 
-    /* "rbfly/streams/_client.pyx":530
+    /* "rbfly/streams/_client.pyx":561
  * 
  *     while data:
  *         count = await publisher._publish(*data, amqp=amqp)             # <<<<<<<<<<<<<<
  *         del data[:count]
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_publisher), __pyx_n_s_publish); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 530, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_publisher), __pyx_n_s_publish); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 561, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_Tuple(__pyx_cur_scope->__pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 530, __pyx_L1_error)
+    __pyx_t_3 = PySequence_Tuple(__pyx_cur_scope->__pyx_v_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 561, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 530, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 561, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_amqp, __pyx_cur_scope->__pyx_v_amqp) < 0) __PYX_ERR(1, 530, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 530, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_amqp, __pyx_cur_scope->__pyx_v_amqp) < 0) __PYX_ERR(1, 561, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 561, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_5);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -13139,48 +13858,48 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 1;
       return __pyx_r;
       __pyx_L6_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 530, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 561, __pyx_L1_error)
       __pyx_t_5 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_5);
     } else {
       __pyx_t_5 = NULL;
-      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_5) < 0) __PYX_ERR(1, 530, __pyx_L1_error)
+      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_5) < 0) __PYX_ERR(1, 561, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
     }
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 530, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 561, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_cur_scope->__pyx_v_count = __pyx_t_6;
 
-    /* "rbfly/streams/_client.pyx":531
+    /* "rbfly/streams/_client.pyx":562
  *     while data:
  *         count = await publisher._publish(*data, amqp=amqp)
  *         del data[:count]             # <<<<<<<<<<<<<<
  * 
  *     return data
  */
-    if (__Pyx_PyObject_DelSlice(__pyx_cur_scope->__pyx_v_data, 0, __pyx_cur_scope->__pyx_v_count, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(1, 531, __pyx_L1_error)
+    if (__Pyx_PyObject_DelSlice(__pyx_cur_scope->__pyx_v_data, 0, __pyx_cur_scope->__pyx_v_count, NULL, NULL, NULL, 0, 1, 0) < 0) __PYX_ERR(1, 562, __pyx_L1_error)
   }
 
-  /* "rbfly/streams/_client.pyx":533
+  /* "rbfly/streams/_client.pyx":564
  *         del data[:count]
  * 
  *     return data             # <<<<<<<<<<<<<<
  * 
  * # vim: sw=4:et:ai
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_cur_scope->__pyx_v_data);
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "rbfly/streams/_client.pyx":517
+  /* "rbfly/streams/_client.pyx":548
  *         publisher._next_message_id()
  * 
  * async def _flush_messages(             # <<<<<<<<<<<<<<
  *         publisher: PublisherBatchTrait,
  *         data: list[MessageCtx],
  */
 
@@ -13386,14 +14105,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_client);
+  Py_CLEAR(p->__pyx_v_ex);
   Py_CLEAR(p->__pyx_v_messages);
   Py_CLEAR(p->__pyx_v_protocol);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_task);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
   Py_CLEAR(p->__pyx_t_2);
@@ -13406,14 +14126,17 @@
 
 static int __pyx_tp_traverse_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ *p = (struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ *)o;
   if (p->__pyx_v_client) {
     e = (*v)(p->__pyx_v_client, a); if (e) return e;
   }
+  if (p->__pyx_v_ex) {
+    e = (*v)(p->__pyx_v_ex, a); if (e) return e;
+  }
   if (p->__pyx_v_messages) {
     e = (*v)(p->__pyx_v_messages, a); if (e) return e;
   }
   if (p->__pyx_v_protocol) {
     e = (*v)(p->__pyx_v_protocol, a); if (e) return e;
   }
   if (p->__pyx_v_self) {
@@ -14702,14 +15425,15 @@
   0, /*tp_watched*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
+static struct __pyx_vtabstruct_5rbfly_7streams_7_client_Subscriber __pyx_vtable_5rbfly_7streams_7_client_Subscriber;
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client_Subscriber(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
@@ -14718,18 +15442,20 @@
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   #endif
   p = ((struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)o);
+  p->__pyx_vtab = __pyx_vtabptr_5rbfly_7streams_7_client_Subscriber;
   p->_client = Py_None; Py_INCREF(Py_None);
   p->_stream = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->_offset = Py_None; Py_INCREF(Py_None);
-  p->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None); Py_INCREF(Py_None);
+  p->_messages = Py_None; Py_INCREF(Py_None);
+  p->_last_message = Py_None; Py_INCREF(Py_None);
   if (unlikely(__pyx_pw_5rbfly_7streams_7_client_10Subscriber_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
@@ -14742,44 +15468,51 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_client);
   Py_CLEAR(p->_stream);
   Py_CLEAR(p->_offset);
-  Py_CLEAR(p->_message);
+  Py_CLEAR(p->_messages);
+  Py_CLEAR(p->_last_message);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static int __pyx_tp_traverse_5rbfly_7streams_7_client_Subscriber(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *p = (struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)o;
   if (p->_client) {
     e = (*v)(p->_client, a); if (e) return e;
   }
   if (p->_offset) {
     e = (*v)(p->_offset, a); if (e) return e;
   }
-  if (p->_message) {
-    e = (*v)(((PyObject *)p->_message), a); if (e) return e;
+  if (p->_messages) {
+    e = (*v)(p->_messages, a); if (e) return e;
+  }
+  if (p->_last_message) {
+    e = (*v)(p->_last_message, a); if (e) return e;
   }
   return 0;
 }
 
 static int __pyx_tp_clear_5rbfly_7streams_7_client_Subscriber(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *p = (struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *)o;
   tmp = ((PyObject*)p->_client);
   p->_client = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_offset);
   p->_offset = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_message);
-  p->_message = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)Py_None); Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->_messages);
+  p->_messages = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->_last_message);
+  p->_last_message = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__client(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_7_client_1__get__(o);
 }
@@ -14857,53 +15590,67 @@
   }
   else {
     PyErr_SetString(PyExc_NotImplementedError, "__del__");
     return -1;
   }
 }
 
-static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__message(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_1__get__(o);
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__messages(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_1__get__(o);
+}
+
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__messages(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_3__set__(o, v);
+  }
+  else {
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_9_messages_5__del__(o);
+  }
+}
+
+static PyObject *__pyx_getprop_5rbfly_7streams_7_client_10Subscriber__last_message(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_1__get__(o);
 }
 
-static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__message(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+static int __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__last_message(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
   if (v) {
-    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_3__set__(o, v);
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_3__set__(o, v);
   }
   else {
-    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_8_message_5__del__(o);
+    return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_13_last_message_5__del__(o);
   }
 }
 
-static PyObject *__pyx_specialmethod___pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
-  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__(self);
+static PyObject *__pyx_specialmethod___pyx_pw_5rbfly_7streams_7_client_10Subscriber_5__aiter__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
+  return __pyx_pw_5rbfly_7streams_7_client_10Subscriber_5__aiter__(self);
 }
 
 static PyMethodDef __pyx_methods_5rbfly_7streams_7_client_Subscriber[] = {
-  {"__aiter__", (PyCFunction)__pyx_specialmethod___pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__, METH_NOARGS|METH_COEXIST, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_2__aiter__},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_6__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_5__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_7__setstate_cython__},
+  {"__aiter__", (PyCFunction)__pyx_specialmethod___pyx_pw_5rbfly_7streams_7_client_10Subscriber_5__aiter__, METH_NOARGS|METH_COEXIST, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_4__aiter__},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_8__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_7__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_10__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_7_client_10Subscriber_9__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_5rbfly_7streams_7_client_Subscriber[] = {
   {(char *)"_client", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__client, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__client, (char *)PyDoc_STR("_client: object"), 0},
   {(char *)"_stream", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__stream, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__stream, (char *)PyDoc_STR("_stream: unicode"), 0},
   {(char *)"_subscription_id", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__subscription_id, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__subscription_id, (char *)PyDoc_STR("_subscription_id: 'uint8_t'"), 0},
   {(char *)"_offset", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__offset, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__offset, (char *)PyDoc_STR("_offset: object"), 0},
   {(char *)"_timeout", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__timeout, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__timeout, (char *)PyDoc_STR("_timeout: 'float'"), 0},
   {(char *)"_amqp", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__amqp, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__amqp, (char *)PyDoc_STR("_amqp: 'char'"), 0},
-  {(char *)"_message", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__message, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__message, (char *)PyDoc_STR("_message: rbfly.amqp._message.MessageCtx"), 0},
+  {(char *)"_messages", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__messages, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__messages, (char *)PyDoc_STR("_messages: object"), 0},
+  {(char *)"_last_message", __pyx_getprop_5rbfly_7streams_7_client_10Subscriber__last_message, __pyx_setprop_5rbfly_7streams_7_client_10Subscriber__last_message, (char *)PyDoc_STR("_last_message: object"), 0},
   {0, 0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_5rbfly_7streams_7_client_Subscriber_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_5rbfly_7streams_7_client_Subscriber},
-  {Py_am_aiter, (void *)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__},
-  {Py_tp_doc, (void *)PyDoc_STR("\n    RabbitMQ stream subscriber.\n\n    A stream subscriber holds information about RabbitMQ stream\n    subscription and is used to iterate over messages read from a stream.\n\n    :var client: RabbitMQ Streams client.\n    :var stream: RabbitMQ stream name.\n    :var subscription_id: RabbitMQ stream subscription id.\n    :var offset: RabbitMQ Streams offset specification.\n    :var timeout: Raise timeout error if no message within specified time\n        (in seconds).\n    :var message: Last received message or null.\n    :var amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP\n        decoding.\n    ")},
+  {Py_am_aiter, (void *)__pyx_pw_5rbfly_7streams_7_client_10Subscriber_5__aiter__},
+  {Py_tp_doc, (void *)PyDoc_STR("\n    RabbitMQ stream subscriber.\n\n    A stream subscriber holds information about RabbitMQ stream\n    subscription and is used to iterate over messages read from a stream.\n\n    :var _client: RabbitMQ Streams client.\n    :var _stream: RabbitMQ stream name.\n    :var _subscription_id: RabbitMQ stream subscription id.\n    :var _offset: RabbitMQ Streams offset specification used on first\n        subscription.\n    :var _timeout: Raise timeout error if no message within specified time\n        (in seconds).\n    :var _amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP\n        decoding.\n    :var _last_message: Last received message or null.\n    :var _messages: Current queue of messages or null.\n    ")},
   {Py_tp_traverse, (void *)__pyx_tp_traverse_5rbfly_7streams_7_client_Subscriber},
   {Py_tp_clear, (void *)__pyx_tp_clear_5rbfly_7streams_7_client_Subscriber},
   {Py_tp_methods, (void *)__pyx_methods_5rbfly_7streams_7_client_Subscriber},
   {Py_tp_getset, (void *)__pyx_getsets_5rbfly_7streams_7_client_Subscriber},
   {Py_tp_new, (void *)__pyx_tp_new_5rbfly_7streams_7_client_Subscriber},
   {0, 0},
 };
@@ -14915,15 +15662,15 @@
   __pyx_type_5rbfly_7streams_7_client_Subscriber_slots,
 };
 #else
 
 #if PY_MAJOR_VERSION >= 3
 static __Pyx_PyAsyncMethodsStruct __pyx_tp_as_async_Subscriber = {
   0, /*am_await*/
-  __pyx_pw_5rbfly_7streams_7_client_10Subscriber_3__aiter__, /*am_aiter*/
+  __pyx_pw_5rbfly_7streams_7_client_10Subscriber_5__aiter__, /*am_aiter*/
   0, /*am_anext*/
   #if PY_VERSION_HEX >= 0x030A00A3
   0, /*am_send*/
   #endif
 };
 #endif
 
@@ -14954,15 +15701,15 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  PyDoc_STR("\n    RabbitMQ stream subscriber.\n\n    A stream subscriber holds information about RabbitMQ stream\n    subscription and is used to iterate over messages read from a stream.\n\n    :var client: RabbitMQ Streams client.\n    :var stream: RabbitMQ stream name.\n    :var subscription_id: RabbitMQ stream subscription id.\n    :var offset: RabbitMQ Streams offset specification.\n    :var timeout: Raise timeout error if no message within specified time\n        (in seconds).\n    :var message: Last received message or null.\n    :var amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP\n        decoding.\n    "), /*tp_doc*/
+  PyDoc_STR("\n    RabbitMQ stream subscriber.\n\n    A stream subscriber holds information about RabbitMQ stream\n    subscription and is used to iterate over messages read from a stream.\n\n    :var _client: RabbitMQ Streams client.\n    :var _stream: RabbitMQ stream name.\n    :var _subscription_id: RabbitMQ stream subscription id.\n    :var _offset: RabbitMQ Streams offset specification used on first\n        subscription.\n    :var _timeout: Raise timeout error if no message within specified time\n        (in seconds).\n    :var _amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP\n        decoding.\n    :var _last_message: Last received message or null.\n    :var _messages: Current queue of messages or null.\n    "), /*tp_doc*/
   __pyx_tp_traverse_5rbfly_7streams_7_client_Subscriber, /*tp_traverse*/
   __pyx_tp_clear_5rbfly_7streams_7_client_Subscriber, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_5rbfly_7streams_7_client_Subscriber, /*tp_methods*/
@@ -16344,18 +17091,19 @@
     {&__pyx_n_s_Publisher___reduce_cython, __pyx_k_Publisher___reduce_cython, sizeof(__pyx_k_Publisher___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Publisher___setstate_cython, __pyx_k_Publisher___setstate_cython, sizeof(__pyx_k_Publisher___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Publisher_send, __pyx_k_Publisher_send, sizeof(__pyx_k_Publisher_send), 0, 0, 1, 1},
     {&__pyx_n_s_Subscriber, __pyx_k_Subscriber, sizeof(__pyx_k_Subscriber), 0, 0, 1, 1},
     {&__pyx_n_s_Subscriber___aiter, __pyx_k_Subscriber___aiter, sizeof(__pyx_k_Subscriber___aiter), 0, 0, 1, 1},
     {&__pyx_n_s_Subscriber___reduce_cython, __pyx_k_Subscriber___reduce_cython, sizeof(__pyx_k_Subscriber___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Subscriber___setstate_cython, __pyx_k_Subscriber___setstate_cython, sizeof(__pyx_k_Subscriber___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Subscriber__next_message_offset, __pyx_k_Subscriber__next_message_offset, sizeof(__pyx_k_Subscriber__next_message_offset), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
     {&__pyx_kp_u__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 1, 0, 0},
-    {&__pyx_n_s__52, __pyx_k__52, sizeof(__pyx_k__52), 0, 0, 1, 1},
+    {&__pyx_n_s__53, __pyx_k__53, sizeof(__pyx_k__53), 0, 0, 1, 1},
     {&__pyx_n_s_aenter, __pyx_k_aenter, sizeof(__pyx_k_aenter), 0, 0, 1, 1},
     {&__pyx_n_s_aexit, __pyx_k_aexit, sizeof(__pyx_k_aexit), 0, 0, 1, 1},
     {&__pyx_n_s_aiter, __pyx_k_aiter, sizeof(__pyx_k_aiter), 0, 0, 1, 1},
     {&__pyx_n_s_amqp, __pyx_k_amqp, sizeof(__pyx_k_amqp), 0, 0, 1, 1},
     {&__pyx_n_s_app_properties, __pyx_k_app_properties, sizeof(__pyx_k_app_properties), 0, 0, 1, 1},
     {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio, __pyx_k_asyncio, sizeof(__pyx_k_asyncio), 0, 0, 1, 1},
@@ -16364,30 +17112,33 @@
     {&__pyx_n_s_attrgetter, __pyx_k_attrgetter, sizeof(__pyx_k_attrgetter), 0, 0, 1, 1},
     {&__pyx_n_s_await, __pyx_k_await, sizeof(__pyx_k_await), 0, 0, 1, 1},
     {&__pyx_n_s_batch, __pyx_k_batch, sizeof(__pyx_k_batch), 0, 0, 1, 1},
     {&__pyx_n_s_batch_locals_lambda, __pyx_k_batch_locals_lambda, sizeof(__pyx_k_batch_locals_lambda), 0, 0, 1, 1},
     {&__pyx_n_s_body, __pyx_k_body, sizeof(__pyx_k_body), 0, 0, 1, 1},
     {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
     {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
+    {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
     {&__pyx_n_s_client, __pyx_k_client, sizeof(__pyx_k_client), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
     {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
     {&__pyx_n_s_cond, __pyx_k_cond, sizeof(__pyx_k_cond), 0, 0, 1, 1},
+    {&__pyx_kp_u_connection_error_received_id_ini, __pyx_k_connection_error_received_id_ini, sizeof(__pyx_k_connection_error_received_id_ini), 0, 1, 0, 0},
     {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
     {&__pyx_n_s_ctx, __pyx_k_ctx, sizeof(__pyx_k_ctx), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_s_debug, __pyx_k_debug, sizeof(__pyx_k_debug), 0, 0, 1, 1},
     {&__pyx_n_s_deque, __pyx_k_deque, sizeof(__pyx_k_deque), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_flush, __pyx_k_flush, sizeof(__pyx_k_flush), 0, 0, 1, 1},
     {&__pyx_n_s_flush_messages, __pyx_k_flush_messages, sizeof(__pyx_k_flush_messages), 0, 0, 1, 1},
+    {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_getLogger, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
     {&__pyx_n_s_get_protocol, __pyx_k_get_protocol, sizeof(__pyx_k_get_protocol), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_inc, __pyx_k_inc, sizeof(__pyx_k_inc), 0, 0, 1, 1},
@@ -16411,14 +17162,15 @@
     {&__pyx_n_s_message_id, __pyx_k_message_id, sizeof(__pyx_k_message_id), 0, 0, 1, 1},
     {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
     {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
     {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
     {&__pyx_n_s_next_message_id, __pyx_k_next_message_id, sizeof(__pyx_k_next_message_id), 0, 0, 1, 1},
+    {&__pyx_n_s_next_message_offset, __pyx_k_next_message_offset, sizeof(__pyx_k_next_message_offset), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_notify_all, __pyx_k_notify_all, sizeof(__pyx_k_notify_all), 0, 0, 1, 1},
     {&__pyx_n_s_offset, __pyx_k_offset, sizeof(__pyx_k_offset), 0, 0, 1, 1},
     {&__pyx_n_s_operator, __pyx_k_operator, sizeof(__pyx_k_operator), 0, 0, 1, 1},
     {&__pyx_n_s_pid, __pyx_k_pid, sizeof(__pyx_k_pid), 0, 0, 1, 1},
     {&__pyx_n_s_popleft, __pyx_k_popleft, sizeof(__pyx_k_popleft), 0, 0, 1, 1},
     {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
@@ -16443,14 +17195,15 @@
     {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_sorted, __pyx_k_sorted, sizeof(__pyx_k_sorted), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_stream, __pyx_k_stream, sizeof(__pyx_k_stream), 0, 0, 1, 1},
     {&__pyx_n_s_stream_messsage_ctx, __pyx_k_stream_messsage_ctx, sizeof(__pyx_k_stream_messsage_ctx), 0, 0, 1, 1},
+    {&__pyx_n_s_stream_offset, __pyx_k_stream_offset, sizeof(__pyx_k_stream_offset), 0, 0, 1, 1},
     {&__pyx_n_s_stream_publish_id, __pyx_k_stream_publish_id, sizeof(__pyx_k_stream_publish_id), 0, 0, 1, 1},
     {&__pyx_n_u_stream_publish_id, __pyx_k_stream_publish_id, sizeof(__pyx_k_stream_publish_id), 0, 1, 0, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_subscription_id, __pyx_k_subscription_id, sizeof(__pyx_k_subscription_id), 0, 0, 1, 1},
     {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
@@ -16784,40 +17537,49 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 3, __pyx_L1_error)
 
+  /* "rbfly/streams/_client.pyx":488
+ *         self._messages = None
+ * 
+ *     cpdef object _next_message_offset(self):             # <<<<<<<<<<<<<<
+ *         """
+ *         Determine RabbitMQ Streams offset specification of next message to
+ */
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__client_pyx, __pyx_n_s_next_message_offset, 488, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(1, 488, __pyx_L1_error)
+
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "rbfly/streams/_client.pyx":517
+  /* "rbfly/streams/_client.pyx":548
  *         publisher._next_message_id()
  * 
  * async def _flush_messages(             # <<<<<<<<<<<<<<
  *         publisher: PublisherBatchTrait,
  *         data: list[MessageCtx],
  */
-  __pyx_tuple__51 = PyTuple_Pack(4, __pyx_n_s_publisher, __pyx_n_s_data, __pyx_n_s_amqp, __pyx_n_s_count); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(1, 517, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 1, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_COROUTINE, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__client_pyx, __pyx_n_s_flush_messages, 517, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 517, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(4, __pyx_n_s_publisher, __pyx_n_s_data, __pyx_n_s_amqp, __pyx_n_s_count); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(1, 548, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 1, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_COROUTINE, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__client_pyx, __pyx_n_s_flush_messages, 548, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -16874,42 +17636,42 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages_spec, NULL); if (unlikely(!__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages)) __PYX_ERR(1, 517, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages_spec, __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
+  __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages_spec, NULL); if (unlikely(!__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages)) __PYX_ERR(1, 548, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages_spec, __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
   #else
   __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages = &__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages->tp_dictoffset && __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_8__flush_messages->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter___spec, NULL); if (unlikely(!__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__)) __PYX_ERR(1, 482, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter___spec, __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__) < 0) __PYX_ERR(1, 482, __pyx_L1_error)
+  __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter___spec, NULL); if (unlikely(!__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__)) __PYX_ERR(1, 508, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter___spec, __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__) < 0) __PYX_ERR(1, 508, __pyx_L1_error)
   #else
   __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__ = &__pyx_type_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__) < 0) __PYX_ERR(1, 482, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__) < 0) __PYX_ERR(1, 508, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__->tp_dictoffset && __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct_7___aiter__->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -17044,14 +17806,16 @@
   __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct___publish->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct___publish->tp_dictoffset && __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct___publish->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_5rbfly_7streams_7_client___pyx_scope_struct___publish->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
+  __pyx_vtabptr_5rbfly_7streams_7_client_Subscriber = &__pyx_vtable_5rbfly_7streams_7_client_Subscriber;
+  __pyx_vtable_5rbfly_7streams_7_client_Subscriber._next_message_offset = (PyObject *(*)(struct __pyx_obj_5rbfly_7streams_7_client_Subscriber *, int __pyx_skip_dispatch))__pyx_f_5rbfly_7streams_7_client_10Subscriber__next_message_offset;
   #if CYTHON_USE_TYPE_SPECS
   __pyx_ptype_5rbfly_7streams_7_client_Subscriber = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_5rbfly_7streams_7_client_Subscriber_spec, NULL); if (unlikely(!__pyx_ptype_5rbfly_7streams_7_client_Subscriber)) __PYX_ERR(1, 436, __pyx_L1_error)
   if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_5rbfly_7streams_7_client_Subscriber_spec, __pyx_ptype_5rbfly_7streams_7_client_Subscriber) < 0) __PYX_ERR(1, 436, __pyx_L1_error)
   #else
   __pyx_ptype_5rbfly_7streams_7_client_Subscriber = &__pyx_type_5rbfly_7streams_7_client_Subscriber;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
@@ -17067,20 +17831,24 @@
     __pyx_ptype_5rbfly_7streams_7_client_Subscriber->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)__pyx_ptype_5rbfly_7streams_7_client_Subscriber, "__aiter__"); if (unlikely(!wrapper)) __PYX_ERR(1, 436, __pyx_L1_error)
     if (__Pyx_IS_TYPE(wrapper, &PyWrapperDescr_Type)) {
-      __pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_2__aiter__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_2__aiter__.doc = __pyx_doc_5rbfly_7streams_7_client_10Subscriber_2__aiter__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_2__aiter__;
+      __pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_4__aiter__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_4__aiter__.doc = __pyx_doc_5rbfly_7streams_7_client_10Subscriber_4__aiter__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_5rbfly_7streams_7_client_10Subscriber_4__aiter__;
     }
   }
   #endif
+  if (__Pyx_SetVtable(__pyx_ptype_5rbfly_7streams_7_client_Subscriber, __pyx_vtabptr_5rbfly_7streams_7_client_Subscriber) < 0) __PYX_ERR(1, 436, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_MergeVtables(__pyx_ptype_5rbfly_7streams_7_client_Subscriber) < 0) __PYX_ERR(1, 436, __pyx_L1_error)
+  #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Subscriber, (PyObject *) __pyx_ptype_5rbfly_7streams_7_client_Subscriber) < 0) __PYX_ERR(1, 436, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_5rbfly_7streams_7_client_Subscriber) < 0) __PYX_ERR(1, 436, __pyx_L1_error)
   #endif
   __pyx_vtabptr_5rbfly_7streams_7_client_PublisherTrait = &__pyx_vtable_5rbfly_7streams_7_client_PublisherTrait;
   __pyx_vtable_5rbfly_7streams_7_client_PublisherTrait._next_message_id = (uint64_t (*)(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *, int __pyx_skip_dispatch, struct __pyx_opt_args_5rbfly_7streams_7_client_14PublisherTrait__next_message_id *__pyx_optional_args))__pyx_f_5rbfly_7streams_7_client_14PublisherTrait__next_message_id;
   __pyx_vtable_5rbfly_7streams_7_client_PublisherTrait._reset_message_id = (uint64_t (*)(struct __pyx_obj_5rbfly_7streams_7_client_PublisherTrait *, uint64_t, int __pyx_skip_dispatch))__pyx_f_5rbfly_7streams_7_client_14PublisherTrait__reset_message_id;
@@ -18346,58 +19114,71 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_17PublisherBinBatch_8__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PublisherBinBatch___setstate_cyt, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_5) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
+  /* "rbfly/streams/_client.pyx":488
+ *         self._messages = None
+ * 
+ *     cpdef object _next_message_offset(self):             # <<<<<<<<<<<<<<
+ *         """
+ *         Determine RabbitMQ Streams offset specification of next message to
+ */
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_10Subscriber_3_next_message_offset, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Subscriber__next_message_offset, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 488, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_5rbfly_7streams_7_client_Subscriber->tp_dict, __pyx_n_s_next_message_offset, __pyx_t_5) < 0) __PYX_ERR(1, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  PyType_Modified(__pyx_ptype_5rbfly_7streams_7_client_Subscriber);
+
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_10Subscriber_6__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Subscriber___reduce_cython, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_10Subscriber_8__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Subscriber___reduce_cython, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_10Subscriber_8__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Subscriber___setstate_cython, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_10Subscriber_10__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Subscriber___setstate_cython, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_5) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "rbfly/streams/_client.pyx":517
+  /* "rbfly/streams/_client.pyx":548
  *         publisher._next_message_id()
  * 
  * async def _flush_messages(             # <<<<<<<<<<<<<<
  *         publisher: PublisherBatchTrait,
  *         data: list[MessageCtx],
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 517, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_amqp, ((PyObject *)Py_True)) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 517, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_amqp, ((PyObject *)Py_True)) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_publisher, __pyx_n_s_PublisherBatchTrait) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_kp_s_list_MessageCtx) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_amqp, __pyx_n_s_bool) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_list_MessageCtx) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_3_flush_messages, __Pyx_CYFUNCTION_COROUTINE, __pyx_n_s_flush_messages, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 517, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_publisher, __pyx_n_s_PublisherBatchTrait) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_kp_s_list_MessageCtx) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_amqp, __pyx_n_s_bool) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_list_MessageCtx) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_7_client_3_flush_messages, __Pyx_CYFUNCTION_COROUTINE, __pyx_n_s_flush_messages, NULL, __pyx_n_s_rbfly_streams__client, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_4, __pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_flush_messages, __pyx_t_4) < 0) __PYX_ERR(1, 517, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_flush_messages, __pyx_t_4) < 0) __PYX_ERR(1, 548, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "rbfly/streams/_client.pyx":1
  * #             # <<<<<<<<<<<<<<
  * # rbfly - a library for RabbitMQ Streams using Python asyncio
  * #
  */
@@ -22684,14 +23465,425 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
+/* PyIntBinop */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_SubtractObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
+    CYTHON_MAYBE_UNUSED_VAR(intval);
+    CYTHON_MAYBE_UNUSED_VAR(inplace);
+    CYTHON_UNUSED_VAR(zerodivision_check);
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long x;
+        long a = PyInt_AS_LONG(op1);
+        
+            x = (long)((unsigned long)a - b);
+            if (likely((x^a) >= 0 || (x^~b) >= 0))
+                return PyInt_FromLong(x);
+            return PyLong_Type.tp_as_number->nb_subtract(op1, op2);
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        const long b = intval;
+        long a, x;
+#ifdef HAVE_LONG_LONG
+        const PY_LONG_LONG llb = intval;
+        PY_LONG_LONG lla, llx;
+#endif
+        const digit* digits = __Pyx_PyLong_Digits(op1);
+        const Py_ssize_t size = Py_SIZE(op1);
+        if (unlikely(size == 0)) {
+            return PyLong_FromLong(-intval);
+        }
+        if (likely(__Pyx_sst_abs(size) <= 1)) {
+            a = likely(size) ? digits[0] : 0;
+            if (size == -1) a = -a;
+        } else {
+            switch (size) {
+                case -2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                default: return PyLong_Type.tp_as_number->nb_subtract(op1, op2);
+            }
+        }
+                x = a - b;
+            return PyLong_FromLong(x);
+#ifdef HAVE_LONG_LONG
+        long_long:
+                llx = lla - llb;
+            return PyLong_FromLongLong(llx);
+#endif
+        
+        
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        double a = __pyx_PyFloat_AsDouble(op1);
+#else
+        double a = PyFloat_AS_DOUBLE(op1);
+#endif
+            double result;
+            
+            PyFPE_START_PROTECT("subtract", return NULL)
+            result = ((double)a) - (double)b;
+            PyFPE_END_PROTECT(result)
+            return PyFloat_FromDouble(result);
+    }
+    return (inplace ? PyNumber_InPlaceSubtract : PyNumber_Subtract)(op1, op2);
+}
+#endif
+
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (unlikely(!j)) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return sm->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
+    PyObject *runerr = NULL;
+    Py_ssize_t key_value;
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError,
+            "cannot fit '" __Pyx_FMT_TYPENAME "' into an index-sized integer", index_type_name);
+        __Pyx_DECREF_TypeName(index_type_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
+    __Pyx_TypeName obj_type_name;
+    if (likely(PyType_Check(obj))) {
+        PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
+        if (meth) {
+            PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
+            Py_DECREF(meth);
+            return result;
+        }
+    }
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+        "'" __Pyx_FMT_TYPENAME "' object is not subscriptable", obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key) {
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyMappingMethods *mm = tp->tp_as_mapping;
+    PySequenceMethods *sm = tp->tp_as_sequence;
+    if (likely(mm && mm->mp_subscript)) {
+        return mm->mp_subscript(obj, key);
+    }
+    if (likely(sm && sm->sq_item)) {
+        return __Pyx_PyObject_GetIndex(obj, key);
+    }
+    return __Pyx_PyObject_GetItem_Slow(obj, key);
+}
+#endif
+
+/* PyIntBinop */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
+    CYTHON_MAYBE_UNUSED_VAR(intval);
+    CYTHON_MAYBE_UNUSED_VAR(inplace);
+    CYTHON_UNUSED_VAR(zerodivision_check);
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long x;
+        long a = PyInt_AS_LONG(op1);
+        
+            x = (long)((unsigned long)a + b);
+            if (likely((x^a) >= 0 || (x^b) >= 0))
+                return PyInt_FromLong(x);
+            return PyLong_Type.tp_as_number->nb_add(op1, op2);
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        const long b = intval;
+        long a, x;
+#ifdef HAVE_LONG_LONG
+        const PY_LONG_LONG llb = intval;
+        PY_LONG_LONG lla, llx;
+#endif
+        const digit* digits = __Pyx_PyLong_Digits(op1);
+        const Py_ssize_t size = Py_SIZE(op1);
+        if (unlikely(size == 0)) {
+            return __Pyx_NewRef(op2);
+        }
+        if (likely(__Pyx_sst_abs(size) <= 1)) {
+            a = likely(size) ? digits[0] : 0;
+            if (size == -1) a = -a;
+        } else {
+            switch (size) {
+                case -2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+                    #ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+                    #endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
+            }
+        }
+                x = a + b;
+            return PyLong_FromLong(x);
+#ifdef HAVE_LONG_LONG
+        long_long:
+                llx = lla + llb;
+            return PyLong_FromLongLong(llx);
+#endif
+        
+        
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        double a = __pyx_PyFloat_AsDouble(op1);
+#else
+        double a = PyFloat_AS_DOUBLE(op1);
+#endif
+            double result;
+            
+            PyFPE_START_PROTECT("add", return NULL)
+            result = ((double)a) + (double)b;
+            PyFPE_END_PROTECT(result)
+            return PyFloat_FromDouble(result);
+    }
+    return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
+}
+#endif
+
 /* StopAsyncIteration */
 #if PY_VERSION_HEX < 0x030500B1
 #if CYTHON_USE_TYPE_SPECS
 #error Using async coroutines with type specs requires Python 3.5 or later.
 #else
 static PyTypeObject __Pyx__PyExc_StopAsyncIteration_type = {
     PyVarObject_HEAD_INIT(0, 0)
@@ -23028,14 +24220,105 @@
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
+/* SetVTable */
+static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
+    PyObject *ob = PyCapsule_New(vtable, 0, 0);
+    if (unlikely(!ob))
+        goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
+#else
+    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
+#endif
+        goto bad;
+    Py_DECREF(ob);
+    return 0;
+bad:
+    Py_XDECREF(ob);
+    return -1;
+}
+
+/* GetVTable */
+static void* __Pyx_GetVtable(PyTypeObject *type) {
+    void* ptr;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
+#else
+    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
+#endif
+    if (!ob)
+        goto bad;
+    ptr = PyCapsule_GetPointer(ob, 0);
+    if (!ptr && !PyErr_Occurred())
+        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
+    Py_DECREF(ob);
+    return ptr;
+bad:
+    Py_XDECREF(ob);
+    return NULL;
+}
+
+/* MergeVTables */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type) {
+    int i;
+    void** base_vtables;
+    __Pyx_TypeName tp_base_name;
+    __Pyx_TypeName base_name;
+    void* unknown = (void*)-1;
+    PyObject* bases = type->tp_bases;
+    int base_depth = 0;
+    {
+        PyTypeObject* base = type->tp_base;
+        while (base) {
+            base_depth += 1;
+            base = base->tp_base;
+        }
+    }
+    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
+    base_vtables[0] = unknown;
+    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
+        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
+        if (base_vtable != NULL) {
+            int j;
+            PyTypeObject* base = type->tp_base;
+            for (j = 0; j < base_depth; j++) {
+                if (base_vtables[j] == unknown) {
+                    base_vtables[j] = __Pyx_GetVtable(base);
+                    base_vtables[j + 1] = unknown;
+                }
+                if (base_vtables[j] == base_vtable) {
+                    break;
+                } else if (base_vtables[j] == NULL) {
+                    goto bad;
+                }
+                base = base->tp_base;
+            }
+        }
+    }
+    PyErr_Clear();
+    free(base_vtables);
+    return 0;
+bad:
+    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
+    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
+    PyErr_Format(PyExc_TypeError,
+        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
+    __Pyx_DECREF_TypeName(tp_base_name);
+    __Pyx_DECREF_TypeName(base_name);
+    free(base_vtables);
+    return -1;
+}
+#endif
+
 /* SetupReduce */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
@@ -23139,105 +24422,14 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
-/* SetVTable */
-static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
-    PyObject *ob = PyCapsule_New(vtable, 0, 0);
-    if (unlikely(!ob))
-        goto bad;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
-#else
-    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
-#endif
-        goto bad;
-    Py_DECREF(ob);
-    return 0;
-bad:
-    Py_XDECREF(ob);
-    return -1;
-}
-
-/* GetVTable */
-static void* __Pyx_GetVtable(PyTypeObject *type) {
-    void* ptr;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
-#else
-    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
-#endif
-    if (!ob)
-        goto bad;
-    ptr = PyCapsule_GetPointer(ob, 0);
-    if (!ptr && !PyErr_Occurred())
-        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
-    Py_DECREF(ob);
-    return ptr;
-bad:
-    Py_XDECREF(ob);
-    return NULL;
-}
-
-/* MergeVTables */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_MergeVtables(PyTypeObject *type) {
-    int i;
-    void** base_vtables;
-    __Pyx_TypeName tp_base_name;
-    __Pyx_TypeName base_name;
-    void* unknown = (void*)-1;
-    PyObject* bases = type->tp_bases;
-    int base_depth = 0;
-    {
-        PyTypeObject* base = type->tp_base;
-        while (base) {
-            base_depth += 1;
-            base = base->tp_base;
-        }
-    }
-    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
-    base_vtables[0] = unknown;
-    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
-        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
-        if (base_vtable != NULL) {
-            int j;
-            PyTypeObject* base = type->tp_base;
-            for (j = 0; j < base_depth; j++) {
-                if (base_vtables[j] == unknown) {
-                    base_vtables[j] = __Pyx_GetVtable(base);
-                    base_vtables[j + 1] = unknown;
-                }
-                if (base_vtables[j] == base_vtable) {
-                    break;
-                } else if (base_vtables[j] == NULL) {
-                    goto bad;
-                }
-                base = base->tp_base;
-            }
-        }
-    }
-    PyErr_Clear();
-    free(base_vtables);
-    return 0;
-bad:
-    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
-    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
-    PyErr_Format(PyExc_TypeError,
-        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
-    __Pyx_DECREF_TypeName(tp_base_name);
-    __Pyx_DECREF_TypeName(base_name);
-    free(base_vtables);
-    return -1;
-}
-#endif
-
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
     size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
@@ -24948,15 +26140,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__52));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__53));
     }
     return name;
 }
 #endif
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
```

### Comparing `rbfly-0.7.1/rbfly/streams/_client.pyi` & `rbfly-0.7.2/rbfly/streams/_client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing as tp
+from collections import deque
 
 from ..types import AMQPBody, AMQPAppProperties
 from ..amqp import MessageCtx
 from .client import StreamsClient
 from .offset import Offset
 
 class PublisherConstr(tp.Protocol):
@@ -72,27 +73,29 @@
 
 class Subscriber:
     _stream: str
     _subscription_id: int
     _offset: Offset
     _timeout: float
     _amqp: bool
-    _message: MessageCtx | None
+    _last_message: MessageCtx | None
+    _messages: deque[MessageCtx] | None
 
     def __init__(
         self,
         client: StreamsClient,
         stream: str,
         subscription_id: int,
         offset: Offset,
         timeout: float,
         amqp: bool,
     ) -> None:
         ...
 
+    def _next_message_offset(self) -> Offset: ...
     def __aiter__(self) -> tp.AsyncIterator[MessageCtx]: ...
 
 def stream_messsage_ctx(
     body: AMQPBody,
     *,
     publish_id: int | None=None,
     app_properties: AMQPAppProperties={},
```

### Comparing `rbfly-0.7.1/rbfly/streams/_client.pyx` & `rbfly-0.7.2/rbfly/streams/_client.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -436,32 +436,36 @@
 cdef class Subscriber:
     """
     RabbitMQ stream subscriber.
 
     A stream subscriber holds information about RabbitMQ stream
     subscription and is used to iterate over messages read from a stream.
 
-    :var client: RabbitMQ Streams client.
-    :var stream: RabbitMQ stream name.
-    :var subscription_id: RabbitMQ stream subscription id.
-    :var offset: RabbitMQ Streams offset specification.
-    :var timeout: Raise timeout error if no message within specified time
+    :var _client: RabbitMQ Streams client.
+    :var _stream: RabbitMQ stream name.
+    :var _subscription_id: RabbitMQ stream subscription id.
+    :var _offset: RabbitMQ Streams offset specification used on first
+        subscription.
+    :var _timeout: Raise timeout error if no message within specified time
         (in seconds).
-    :var message: Last received message or null.
-    :var amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP
+    :var _amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP
         decoding.
+    :var _last_message: Last received message or null.
+    :var _messages: Current queue of messages or null.
     """
     cdef:
         public object _client
         public str _stream
         public uint8_t _subscription_id
         public object _offset
         public float _timeout
         public char _amqp
-        public MessageCtx _message
+
+        public object _messages
+        public object _last_message
 
     def __cinit__(
             self,
             client,
             stream: str,
             subscription_id: int,
             offset: Offset,
@@ -473,15 +477,37 @@
         """
         self._client = client
         self._stream = stream
         self._subscription_id = subscription_id
         self._offset = offset
         self._timeout = timeout
         self._amqp = amqp
-        self._message: MessageCtx | None = None
+
+        self._last_message = None
+        self._messages = None
+
+    cpdef object _next_message_offset(self):
+        """
+        Determine RabbitMQ Streams offset specification of next message to
+        be read from the stream.
+        """
+        cdef object offset
+
+        if self._messages is None:
+            # no messages read yet, use the initial offset
+            offset = self._offset
+        elif n := len(self._messages):
+            # eventually, the messages are to be read from the queue; use
+            # the last message in the queue to determine next offset
+            msg = self._messages[n - 1]
+            offset = Offset.offset(msg.stream_offset + 1) 
+        else:
+            # queue is empty, use last message to determine next offset
+            offset = Offset.offset(self._last_message.stream_offset + 1)
+        return offset
 
     async def __aiter__(self) -> tp.AsyncIterator[MessageCtx]:
         """
         Iterate over messages read from a stream.
         """
         cdef:
             float timeout = self._timeout
@@ -492,21 +518,26 @@
 
         while True:
             try:
                 protocol = await client.get_protocol()
                 task = protocol.read_stream(self._subscription_id)
                 if timeout:
                     task = asyncio.wait_for(task, timeout)
-                messages = await task
-            except ConnectionError:
-                pass
+                messages = self._messages = await task
+            except ConnectionError as ex:
+                logger.debug(
+                    'connection error received, id={}, initial offset={},'
+                    ' error={}'.format(
+                        self._subscription_id, self._offset, str(ex)
+                    )
+                )
             else:
                 while messages:
-                    self._message = messages.popleft()
-                    yield self._message
+                    self._last_message = messages.popleft()
+                    yield self._last_message
 
 cdef inline void _before_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
     if not ctx.is_set_stream_publish_id:
         ctx.stream_publish_id = publisher.message_id
 
 cdef inline void _after_ctx_publish(PublisherTrait publisher, MessageCtx ctx):
     if ctx.is_set_stream_publish_id:
```

### Comparing `rbfly-0.7.1/rbfly/streams/_codec.c` & `rbfly-0.7.2/rbfly/streams/_codec.c`

 * *Files 1% similar despite different names*

```diff
@@ -1405,27 +1405,27 @@
   __pyx_e_5rbfly_7streams_6_codec_LEN_FRAME_SIZE = (sizeof(uint32_t))
 };
 
 /* "rbfly/streams/_codec.pyx":48
  *     LEN_FRAME_SIZE = sizeof(uint32_t)
  * 
  * ctypedef Py_ssize_t (*t_func_encode)(Buffer*, object) except -1             # <<<<<<<<<<<<<<
- * ctypedef MessageCtx (*t_func_decode)(Buffer*)
+ * ctypedef MessageCtx (*t_func_decode)(Buffer*, Py_ssize_t)
  * 
  */
 typedef Py_ssize_t (*__pyx_t_5rbfly_7streams_6_codec_t_func_encode)(struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *);
 
 /* "rbfly/streams/_codec.pyx":49
  * 
  * ctypedef Py_ssize_t (*t_func_encode)(Buffer*, object) except -1
- * ctypedef MessageCtx (*t_func_decode)(Buffer*)             # <<<<<<<<<<<<<<
+ * ctypedef MessageCtx (*t_func_decode)(Buffer*, Py_ssize_t)             # <<<<<<<<<<<<<<
  * 
  * cdef class FrameDecoder:
  */
-typedef struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(*__pyx_t_5rbfly_7streams_6_codec_t_func_decode)(struct __pyx_t_5rbfly_7_buffer_Buffer *);
+typedef struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(*__pyx_t_5rbfly_7streams_6_codec_t_func_decode)(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t);
 
 /* "rbfly/streams/_codec.pyx":63
  *         self.data = b''
  * 
  *     def commands(self, chunk: bytes) -> tp.Iterator:  # [tuple[int, int]]:             # <<<<<<<<<<<<<<
  *         """
  *         Iterate over indices of each frame in the data buffer.
@@ -1451,21 +1451,20 @@
  * cdef class FrameEncoder:             # <<<<<<<<<<<<<<
  *     """
  *     RabbitMQ Streams protocol frame encoder.
  */
 struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder {
   PyObject_HEAD
   arrayobject *buffer;
-  char *mv;
   int size;
 };
 
 
 /* "rbfly/streams/_codec.pyx":51
- * ctypedef MessageCtx (*t_func_decode)(Buffer*)
+ * ctypedef MessageCtx (*t_func_decode)(Buffer*, Py_ssize_t)
  * 
  * cdef class FrameDecoder:             # <<<<<<<<<<<<<<
  *     """
  *     RabbitMQ Streams protocol frame decoder.
  */
 struct __pyx_obj_5rbfly_7streams_6_codec_FrameDecoder {
   PyObject_HEAD
@@ -2193,27 +2192,27 @@
 #if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntFromPy.proto */
+static CYTHON_INLINE uint8_t __Pyx_PyInt_As_uint8_t(PyObject *);
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint16_t(uint16_t value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE uint16_t __Pyx_PyInt_As_uint16_t(PyObject *);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
-
-/* CIntFromPy.proto */
 static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint64_t(uint64_t value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value);
@@ -2434,27 +2433,27 @@
 
 /* Module declarations from "rbfly._buffer" */
 static char *(*__pyx_f_5rbfly_7_buffer_buffer_claim)(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t); /*proto*/
 static char (*__pyx_f_5rbfly_7_buffer_buffer_check_size)(struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t); /*proto*/
 
 /* Module declarations from "rbfly.amqp._message" */
 static Py_ssize_t (*__pyx_f_5rbfly_4amqp_8_message_c_encode_amqp)(struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *); /*proto*/
-static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(*__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp)(struct __pyx_t_5rbfly_7_buffer_Buffer *); /*proto*/
+static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(*__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp)(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t); /*proto*/
 
 /* Module declarations from "rbfly._codec" */
 static uint16_t (*__pyx_f_5rbfly_6_codec_unpack_uint16)(char const *); /*proto*/
 static uint32_t (*__pyx_f_5rbfly_6_codec_unpack_uint32)(char const *); /*proto*/
 static uint64_t (*__pyx_f_5rbfly_6_codec_unpack_uint64)(char const *); /*proto*/
 static void (*__pyx_f_5rbfly_6_codec_pack_uint16)(char *, uint16_t); /*proto*/
 static void (*__pyx_f_5rbfly_6_codec_pack_uint32)(char *, uint32_t); /*proto*/
 static void (*__pyx_f_5rbfly_6_codec_pack_uint64)(char *, uint64_t); /*proto*/
 
 /* Module declarations from "rbfly.streams._codec" */
 static CYTHON_INLINE Py_ssize_t __pyx_f_5rbfly_7streams_6_codec_encode_body(struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *); /*proto*/
-static CYTHON_INLINE struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_7streams_6_codec_decode_body(struct __pyx_t_5rbfly_7_buffer_Buffer *); /*proto*/
+static CYTHON_INLINE struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_7streams_6_codec_decode_body(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "rbfly.streams._codec"
 extern int __pyx_module_is_main_rbfly__streams___codec;
 int __pyx_module_is_main_rbfly__streams___codec = 0;
 
 /* Implementation of "rbfly.streams._codec" */
@@ -2524,14 +2523,15 @@
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_VERSION[] = "VERSION";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_k_entry[] = "k_entry";
 static const char __pyx_k_logging[] = "logging";
 static const char __pyx_k_msg_len[] = "msg_len";
+static const char __pyx_k_uint8_t[] = "uint8_t";
 static const char __pyx_k_version[] = "version";
 static const char __pyx_k_warning[] = "warning";
 static const char __pyx_k_calc_crc[] = "calc_crc";
 static const char __pyx_k_commands[] = "commands";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_messages[] = "messages";
 static const char __pyx_k_msg_size[] = "msg_size";
@@ -2611,15 +2611,15 @@
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameDecoder_4data___get__(struct __pyx_obj_5rbfly_7streams_6_codec_FrameDecoder *__pyx_v_self); /* proto */
 static int __pyx_pf_5rbfly_7streams_6_codec_12FrameDecoder_4data_2__set__(struct __pyx_obj_5rbfly_7streams_6_codec_FrameDecoder *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_5rbfly_7streams_6_codec_12FrameDecoder_4data_4__del__(struct __pyx_obj_5rbfly_7streams_6_codec_FrameDecoder *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameDecoder_5__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_6_codec_FrameDecoder *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameDecoder_7__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_6_codec_FrameDecoder *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder___cinit__(struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self, int __pyx_v_size); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_2encode(struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish(struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self, PyObject *__pyx_v_publisher_id, PyObject *__pyx_v_amqp, PyObject *__pyx_v_messages); /* proto */
+static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish(struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self, uint8_t __pyx_v_publisher_id, PyObject *__pyx_v_amqp, PyObject *__pyx_v_messages); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_decode_publish_confirm(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_start); /* proto */
 static PyObject *__pyx_pf_5rbfly_7streams_6_codec_2decode_messages(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_start, PyObject *__pyx_v_offset_start, PyObject *__pyx_v_queue, PyObject *__pyx_v_amqp); /* proto */
 static PyObject *__pyx_tp_new_5rbfly_7streams_6_codec___pyx_scope_struct__commands(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_6_codec_FrameEncoder(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_5rbfly_7streams_6_codec_FrameDecoder(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -2889,14 +2889,15 @@
   PyObject *__pyx_n_s_timestamp;
   PyObject *__pyx_n_s_tp;
   PyObject *__pyx_kp_s_tp_Iterator;
   PyObject *__pyx_kp_s_tp_Optional_int;
   PyObject *__pyx_kp_s_tuple_int_bytes;
   PyObject *__pyx_kp_s_tuple_int_object;
   PyObject *__pyx_n_s_typing;
+  PyObject *__pyx_n_s_uint8_t;
   PyObject *__pyx_kp_u_unknown_frame_version_version;
   PyObject *__pyx_kp_u_unknown_magic_version_0x_02x;
   PyObject *__pyx_n_s_version;
   PyObject *__pyx_n_s_warning;
   PyObject *__pyx_n_s_zlib;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_14;
@@ -3101,14 +3102,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_timestamp);
   Py_CLEAR(clear_module_state->__pyx_n_s_tp);
   Py_CLEAR(clear_module_state->__pyx_kp_s_tp_Iterator);
   Py_CLEAR(clear_module_state->__pyx_kp_s_tp_Optional_int);
   Py_CLEAR(clear_module_state->__pyx_kp_s_tuple_int_bytes);
   Py_CLEAR(clear_module_state->__pyx_kp_s_tuple_int_object);
   Py_CLEAR(clear_module_state->__pyx_n_s_typing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_uint8_t);
   Py_CLEAR(clear_module_state->__pyx_kp_u_unknown_frame_version_version);
   Py_CLEAR(clear_module_state->__pyx_kp_u_unknown_magic_version_0x_02x);
   Py_CLEAR(clear_module_state->__pyx_n_s_version);
   Py_CLEAR(clear_module_state->__pyx_n_s_warning);
   Py_CLEAR(clear_module_state->__pyx_n_s_zlib);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_14);
@@ -3291,14 +3293,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_timestamp);
   Py_VISIT(traverse_module_state->__pyx_n_s_tp);
   Py_VISIT(traverse_module_state->__pyx_kp_s_tp_Iterator);
   Py_VISIT(traverse_module_state->__pyx_kp_s_tp_Optional_int);
   Py_VISIT(traverse_module_state->__pyx_kp_s_tuple_int_bytes);
   Py_VISIT(traverse_module_state->__pyx_kp_s_tuple_int_object);
   Py_VISIT(traverse_module_state->__pyx_n_s_typing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_uint8_t);
   Py_VISIT(traverse_module_state->__pyx_kp_u_unknown_frame_version_version);
   Py_VISIT(traverse_module_state->__pyx_kp_u_unknown_magic_version_0x_02x);
   Py_VISIT(traverse_module_state->__pyx_n_s_version);
   Py_VISIT(traverse_module_state->__pyx_n_s_warning);
   Py_VISIT(traverse_module_state->__pyx_n_s_zlib);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_14);
@@ -3587,14 +3590,15 @@
 #define __pyx_n_s_timestamp __pyx_mstate_global->__pyx_n_s_timestamp
 #define __pyx_n_s_tp __pyx_mstate_global->__pyx_n_s_tp
 #define __pyx_kp_s_tp_Iterator __pyx_mstate_global->__pyx_kp_s_tp_Iterator
 #define __pyx_kp_s_tp_Optional_int __pyx_mstate_global->__pyx_kp_s_tp_Optional_int
 #define __pyx_kp_s_tuple_int_bytes __pyx_mstate_global->__pyx_kp_s_tuple_int_bytes
 #define __pyx_kp_s_tuple_int_object __pyx_mstate_global->__pyx_kp_s_tuple_int_object
 #define __pyx_n_s_typing __pyx_mstate_global->__pyx_n_s_typing
+#define __pyx_n_s_uint8_t __pyx_mstate_global->__pyx_n_s_uint8_t
 #define __pyx_kp_u_unknown_frame_version_version __pyx_mstate_global->__pyx_kp_u_unknown_frame_version_version
 #define __pyx_kp_u_unknown_magic_version_0x_02x __pyx_mstate_global->__pyx_kp_u_unknown_magic_version_0x_02x
 #define __pyx_n_s_version __pyx_mstate_global->__pyx_n_s_version
 #define __pyx_n_s_warning __pyx_mstate_global->__pyx_n_s_warning
 #define __pyx_n_s_zlib __pyx_mstate_global->__pyx_n_s_zlib
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_14 __pyx_mstate_global->__pyx_int_14
@@ -5401,15 +5405,15 @@
   __Pyx_AddTraceback("rbfly.streams._codec.FrameDecoder.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_codec.pyx":117
+/* "rbfly/streams/_codec.pyx":116
  *     cdef int size
  * 
  *     def __cinit__(self, int size):             # <<<<<<<<<<<<<<
  *         # check encoding method if this changes
  *         if size < 32:
  */
 
@@ -5436,31 +5440,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_size)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 117, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 116, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 117, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 116, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
-    __pyx_v_size = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 117, __pyx_L3_error)
+    __pyx_v_size = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 116, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 117, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 116, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.streams._codec.FrameEncoder.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder___cinit__(((struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *)__pyx_v_self), __pyx_v_size);
 
@@ -5476,89 +5480,89 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "rbfly/streams/_codec.pyx":119
+  /* "rbfly/streams/_codec.pyx":118
  *     def __cinit__(self, int size):
  *         # check encoding method if this changes
  *         if size < 32:             # <<<<<<<<<<<<<<
  *             raise ValueError('Encoder buffer minimum size is 32 bytes')
  * 
  */
   __pyx_t_1 = (__pyx_v_size < 32);
   if (unlikely(__pyx_t_1)) {
 
-    /* "rbfly/streams/_codec.pyx":120
+    /* "rbfly/streams/_codec.pyx":119
  *         # check encoding method if this changes
  *         if size < 32:
  *             raise ValueError('Encoder buffer minimum size is 32 bytes')             # <<<<<<<<<<<<<<
  * 
  *         self.buffer = array.array('b', [0] * size)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 120, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 119, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 120, __pyx_L1_error)
+    __PYX_ERR(1, 119, __pyx_L1_error)
 
-    /* "rbfly/streams/_codec.pyx":119
+    /* "rbfly/streams/_codec.pyx":118
  *     def __cinit__(self, int size):
  *         # check encoding method if this changes
  *         if size < 32:             # <<<<<<<<<<<<<<
  *             raise ValueError('Encoder buffer minimum size is 32 bytes')
  * 
  */
   }
 
-  /* "rbfly/streams/_codec.pyx":122
+  /* "rbfly/streams/_codec.pyx":121
  *             raise ValueError('Encoder buffer minimum size is 32 bytes')
  * 
  *         self.buffer = array.array('b', [0] * size)             # <<<<<<<<<<<<<<
  *         self.size = size
  * 
  */
-  __pyx_t_2 = PyList_New(1 * ((__pyx_v_size<0) ? 0:__pyx_v_size)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 122, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1 * ((__pyx_v_size<0) ? 0:__pyx_v_size)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   { Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < __pyx_v_size; __pyx_temp++) {
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
       PyList_SET_ITEM(__pyx_t_2, __pyx_temp, __pyx_int_0);
     }
   }
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 122, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_u_b);
   __Pyx_GIVEREF(__pyx_n_u_b);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_u_b);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 122, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->buffer);
   __Pyx_DECREF((PyObject *)__pyx_v_self->buffer);
   __pyx_v_self->buffer = ((arrayobject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "rbfly/streams/_codec.pyx":123
+  /* "rbfly/streams/_codec.pyx":122
  * 
  *         self.buffer = array.array('b', [0] * size)
  *         self.size = size             # <<<<<<<<<<<<<<
  * 
  *     def encode(self, data: bytes) -> bytes:
  */
   __pyx_v_self->size = __pyx_v_size;
 
-  /* "rbfly/streams/_codec.pyx":117
+  /* "rbfly/streams/_codec.pyx":116
  *     cdef int size
  * 
  *     def __cinit__(self, int size):             # <<<<<<<<<<<<<<
  *         # check encoding method if this changes
  *         if size < 32:
  */
 
@@ -5571,15 +5575,15 @@
   __Pyx_AddTraceback("rbfly.streams._codec.FrameEncoder.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_codec.pyx":125
+/* "rbfly/streams/_codec.pyx":124
  *         self.size = size
  * 
  *     def encode(self, data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *         """
  *         Encode RabbitMQ Streams protocol frame.
  */
 
@@ -5622,37 +5626,37 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 125, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 124, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encode") < 0)) __PYX_ERR(1, 125, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encode") < 0)) __PYX_ERR(1, 124, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_data = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 125, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 124, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.streams._codec.FrameEncoder.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(1, 125, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(1, 124, __pyx_L1_error)
   __pyx_r = __pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_2encode(((struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *)__pyx_v_self), __pyx_v_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5672,116 +5676,116 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 0);
 
-  /* "rbfly/streams/_codec.pyx":130
+  /* "rbfly/streams/_codec.pyx":129
  *         """
  *         cdef:
  *             Py_ssize_t size = len(data)             # <<<<<<<<<<<<<<
  *             Py_ssize_t blen = LEN_FRAME_SIZE + size
  *             char *bp = self.buffer.data.as_chars
  */
-  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 130, __pyx_L1_error)
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 129, __pyx_L1_error)
   __pyx_v_size = __pyx_t_1;
 
-  /* "rbfly/streams/_codec.pyx":131
+  /* "rbfly/streams/_codec.pyx":130
  *         cdef:
  *             Py_ssize_t size = len(data)
  *             Py_ssize_t blen = LEN_FRAME_SIZE + size             # <<<<<<<<<<<<<<
  *             char *bp = self.buffer.data.as_chars
  * 
  */
   __pyx_v_blen = (__pyx_e_5rbfly_7streams_6_codec_LEN_FRAME_SIZE + __pyx_v_size);
 
-  /* "rbfly/streams/_codec.pyx":132
+  /* "rbfly/streams/_codec.pyx":131
  *             Py_ssize_t size = len(data)
  *             Py_ssize_t blen = LEN_FRAME_SIZE + size
  *             char *bp = self.buffer.data.as_chars             # <<<<<<<<<<<<<<
  * 
  *         if blen <= self.size:
  */
   __pyx_t_2 = __pyx_v_self->buffer->data.as_chars;
   __pyx_v_bp = __pyx_t_2;
 
-  /* "rbfly/streams/_codec.pyx":134
+  /* "rbfly/streams/_codec.pyx":133
  *             char *bp = self.buffer.data.as_chars
  * 
  *         if blen <= self.size:             # <<<<<<<<<<<<<<
  *             pack_uint32(bp, size)
  *             memcpy(&bp[LEN_FRAME_SIZE], <char*> data, size)
  */
   __pyx_t_3 = (__pyx_v_blen <= __pyx_v_self->size);
   if (likely(__pyx_t_3)) {
 
-    /* "rbfly/streams/_codec.pyx":135
+    /* "rbfly/streams/_codec.pyx":134
  * 
  *         if blen <= self.size:
  *             pack_uint32(bp, size)             # <<<<<<<<<<<<<<
  *             memcpy(&bp[LEN_FRAME_SIZE], <char*> data, size)
  *         else:
  */
-    __pyx_f_5rbfly_6_codec_pack_uint32(__pyx_v_bp, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 135, __pyx_L1_error)
+    __pyx_f_5rbfly_6_codec_pack_uint32(__pyx_v_bp, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 134, __pyx_L1_error)
 
-    /* "rbfly/streams/_codec.pyx":136
+    /* "rbfly/streams/_codec.pyx":135
  *         if blen <= self.size:
  *             pack_uint32(bp, size)
  *             memcpy(&bp[LEN_FRAME_SIZE], <char*> data, size)             # <<<<<<<<<<<<<<
  *         else:
  *             # TODO: how this should fit into RbFlyBufferError and
  */
-    __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 136, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 135, __pyx_L1_error)
     (void)(memcpy((&(__pyx_v_bp[__pyx_e_5rbfly_7streams_6_codec_LEN_FRAME_SIZE])), ((char *)__pyx_t_2), __pyx_v_size));
 
-    /* "rbfly/streams/_codec.pyx":134
+    /* "rbfly/streams/_codec.pyx":133
  *             char *bp = self.buffer.data.as_chars
  * 
  *         if blen <= self.size:             # <<<<<<<<<<<<<<
  *             pack_uint32(bp, size)
  *             memcpy(&bp[LEN_FRAME_SIZE], <char*> data, size)
  */
     goto __pyx_L3;
   }
 
-  /* "rbfly/streams/_codec.pyx":140
+  /* "rbfly/streams/_codec.pyx":139
  *             # TODO: how this should fit into RbFlyBufferError and
  *             # AMQP*Error?
  *             raise ProtocolError(0x0e, 'Frame too large')             # <<<<<<<<<<<<<<
  * 
  *         return bp[:blen]
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_ProtocolError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 140, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_ProtocolError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 140, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(1, 140, __pyx_L1_error)
+    __PYX_ERR(1, 139, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "rbfly/streams/_codec.pyx":142
+  /* "rbfly/streams/_codec.pyx":141
  *             raise ProtocolError(0x0e, 'Frame too large')
  * 
  *         return bp[:blen]             # <<<<<<<<<<<<<<
  * 
  *     def encode_publish(
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_bp + 0, __pyx_v_blen - 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 142, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_bp + 0, __pyx_v_blen - 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "rbfly/streams/_codec.pyx":125
+  /* "rbfly/streams/_codec.pyx":124
  *         self.size = size
  * 
  *     def encode(self, data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *         """
  *         Encode RabbitMQ Streams protocol frame.
  */
 
@@ -5793,40 +5797,40 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_codec.pyx":144
+/* "rbfly/streams/_codec.pyx":143
  *         return bp[:blen]
  * 
  *     def encode_publish(             # <<<<<<<<<<<<<<
  *             self,
- *             publisher_id: int,
+ *             publisher_id: uint8_t,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5rbfly_7streams_6_codec_12FrameEncoder_5encode_publish(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish, "FrameEncoder.encode_publish(self, int publisher_id: int, *messages: MessageCtx, amqp: bool = True) -> tuple[int, bytes]\n\n        Encode frame with publish RabbitMQ Streams protocol command.\n\n        :param publisher_id: Publisher id.\n        :param messages: List of messages to be published to a stream.\n        ");
+PyDoc_STRVAR(__pyx_doc_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish, "FrameEncoder.encode_publish(self, uint8_t publisher_id: uint8_t, *messages: MessageCtx, amqp: bool = True) -> tuple[int, bytes]\n\n        Encode frame with publish RabbitMQ Streams protocol command.\n\n        :param publisher_id: Publisher id.\n        :param messages: List of messages to be published to a stream.\n        ");
 static PyMethodDef __pyx_mdef_5rbfly_7streams_6_codec_12FrameEncoder_5encode_publish = {"encode_publish", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5rbfly_7streams_6_codec_12FrameEncoder_5encode_publish, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish};
 static PyObject *__pyx_pw_5rbfly_7streams_6_codec_12FrameEncoder_5encode_publish(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
-  PyObject *__pyx_v_publisher_id = 0;
+  uint8_t __pyx_v_publisher_id;
   PyObject *__pyx_v_amqp = 0;
   PyObject *__pyx_v_messages = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
@@ -5841,16 +5845,16 @@
     return NULL;
   }
   __Pyx_GOTREF(__pyx_v_messages);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_publisher_id,&__pyx_n_s_amqp,0};
     PyObject* values[2] = {0,0};
 
-    /* "rbfly/streams/_codec.pyx":148
- *             publisher_id: int,
+    /* "rbfly/streams/_codec.pyx":147
+ *             publisher_id: uint8_t,
  *             *messages: MessageCtx,
  *             amqp: bool=True,             # <<<<<<<<<<<<<<
  *     ) -> tuple[int, bytes]:
  *         """
  */
     values[1] = ((PyObject *)Py_True);
     if (__pyx_kwds) {
@@ -5861,67 +5865,62 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_publisher_id)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 144, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 143, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (kw_args == 1) {
         const Py_ssize_t index = 1;
         PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
         if (value) { values[index] = value; kw_args--; }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 144, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 143, __pyx_L3_error)
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, used_pos_args, "encode_publish") < 0)) __PYX_ERR(1, 144, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, used_pos_args, "encode_publish") < 0)) __PYX_ERR(1, 143, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_publisher_id = ((PyObject*)values[0]);
+    __pyx_v_publisher_id = __Pyx_PyInt_As_uint8_t(values[0]); if (unlikely((__pyx_v_publisher_id == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 145, __pyx_L3_error)
     __pyx_v_amqp = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode_publish", 0, 1, 1, __pyx_nargs); __PYX_ERR(1, 144, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode_publish", 0, 1, 1, __pyx_nargs); __PYX_ERR(1, 143, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_messages); __pyx_v_messages = 0;
   __Pyx_AddTraceback("rbfly.streams._codec.FrameEncoder.encode_publish", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_publisher_id), (&PyInt_Type), 0, "publisher_id", 1))) __PYX_ERR(1, 146, __pyx_L1_error)
   __pyx_r = __pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish(((struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *)__pyx_v_self), __pyx_v_publisher_id, __pyx_v_amqp, __pyx_v_messages);
 
-  /* "rbfly/streams/_codec.pyx":144
+  /* "rbfly/streams/_codec.pyx":143
  *         return bp[:blen]
  * 
  *     def encode_publish(             # <<<<<<<<<<<<<<
  *             self,
- *             publisher_id: int,
+ *             publisher_id: uint8_t,
  */
 
   /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
   __Pyx_DECREF(__pyx_v_messages);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish(struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self, PyObject *__pyx_v_publisher_id, PyObject *__pyx_v_amqp, PyObject *__pyx_v_messages) {
+static PyObject *__pyx_pf_5rbfly_7streams_6_codec_12FrameEncoder_4encode_publish(struct __pyx_obj_5rbfly_7streams_6_codec_FrameEncoder *__pyx_v_self, uint8_t __pyx_v_publisher_id, PyObject *__pyx_v_amqp, PyObject *__pyx_v_messages) {
   struct __pyx_t_5rbfly_7_buffer_Buffer __pyx_v_b;
   struct __pyx_t_5rbfly_7_buffer_Buffer *__pyx_v_buffer;
   char *__pyx_v_bp_hdr;
   char *__pyx_v_bp_msg;
   Py_ssize_t __pyx_v_offset;
   __pyx_t_5rbfly_7streams_6_codec_t_func_encode __pyx_v_encode_msg;
   Py_ssize_t __pyx_v_i;
@@ -5938,477 +5937,475 @@
   struct __pyx_t_5rbfly_7_buffer_Buffer __pyx_t_1;
   Py_ssize_t (*__pyx_t_2)(struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *);
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   char *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   uint16_t __pyx_t_7;
-  char __pyx_t_8;
+  Py_ssize_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   Py_ssize_t __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
+  PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  PyObject *__pyx_t_14 = NULL;
-  uint64_t __pyx_t_15;
+  uint64_t __pyx_t_14;
+  PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
-  PyObject *__pyx_t_18 = NULL;
-  int __pyx_t_19;
+  int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_publish", 0);
 
-  /* "rbfly/streams/_codec.pyx":157
+  /* "rbfly/streams/_codec.pyx":156
  *         """
  *         cdef:
  *             Buffer b = Buffer(self.buffer.data.as_chars, self.size, 0)             # <<<<<<<<<<<<<<
  *             Buffer *buffer = &b
  *             char *bp_hdr
  */
   __pyx_t_1.buffer = __pyx_v_self->buffer->data.as_chars;
   __pyx_t_1.size = __pyx_v_self->size;
   __pyx_t_1.offset = 0;
   __pyx_v_b = __pyx_t_1;
 
-  /* "rbfly/streams/_codec.pyx":158
+  /* "rbfly/streams/_codec.pyx":157
  *         cdef:
  *             Buffer b = Buffer(self.buffer.data.as_chars, self.size, 0)
  *             Buffer *buffer = &b             # <<<<<<<<<<<<<<
  *             char *bp_hdr
  *             char *bp_msg
  */
   __pyx_v_buffer = (&__pyx_v_b);
 
-  /* "rbfly/streams/_codec.pyx":161
+  /* "rbfly/streams/_codec.pyx":160
  *             char *bp_hdr
  *             char *bp_msg
  *             Py_ssize_t offset = LEN_FRAME_SIZE             # <<<<<<<<<<<<<<
  * 
  *             t_func_encode encode_msg = c_encode_amqp if amqp else encode_body
  */
   __pyx_v_offset = __pyx_e_5rbfly_7streams_6_codec_LEN_FRAME_SIZE;
 
-  /* "rbfly/streams/_codec.pyx":163
+  /* "rbfly/streams/_codec.pyx":162
  *             Py_ssize_t offset = LEN_FRAME_SIZE
  * 
  *             t_func_encode encode_msg = c_encode_amqp if amqp else encode_body             # <<<<<<<<<<<<<<
  * 
  *             Py_ssize_t i, count
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_amqp); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(1, 163, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_amqp); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(1, 162, __pyx_L1_error)
   if (__pyx_t_3) {
     __pyx_t_2 = __pyx_f_5rbfly_4amqp_8_message_c_encode_amqp;
   } else {
     __pyx_t_2 = __pyx_f_5rbfly_7streams_6_codec_encode_body;
   }
   __pyx_v_encode_msg = __pyx_t_2;
 
-  /* "rbfly/streams/_codec.pyx":170
+  /* "rbfly/streams/_codec.pyx":169
  *             Py_ssize_t last_offset, num_offset, frame_size
  * 
  *         msg_len = len(messages)             # <<<<<<<<<<<<<<
  *         bp_hdr = buffer.buffer
  * 
  */
-  __pyx_t_4 = PyTuple_GET_SIZE(__pyx_v_messages); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_GET_SIZE(__pyx_v_messages); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 169, __pyx_L1_error)
   __pyx_v_msg_len = __pyx_t_4;
 
-  /* "rbfly/streams/_codec.pyx":171
+  /* "rbfly/streams/_codec.pyx":170
  * 
  *         msg_len = len(messages)
  *         bp_hdr = buffer.buffer             # <<<<<<<<<<<<<<
  * 
  *         # buffer is 32 bytes long at least, so no buffer bounds checking
  */
   __pyx_t_5 = __pyx_v_buffer->buffer;
   __pyx_v_bp_hdr = __pyx_t_5;
 
-  /* "rbfly/streams/_codec.pyx":175
+  /* "rbfly/streams/_codec.pyx":174
  *         # buffer is 32 bytes long at least, so no buffer bounds checking
  *         # here
  *         pack_uint16(&bp_hdr[offset], KEY_PUBLISH)             # <<<<<<<<<<<<<<
  *         offset += sizeof(uint16_t)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_KEY_PUBLISH); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 175, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_KEY_PUBLISH); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_t_6); if (unlikely((__pyx_t_7 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 175, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_t_6); if (unlikely((__pyx_t_7 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 174, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_f_5rbfly_6_codec_pack_uint16((&(__pyx_v_bp_hdr[__pyx_v_offset])), __pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 175, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint16((&(__pyx_v_bp_hdr[__pyx_v_offset])), __pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 174, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":176
+  /* "rbfly/streams/_codec.pyx":175
  *         # here
  *         pack_uint16(&bp_hdr[offset], KEY_PUBLISH)
  *         offset += sizeof(uint16_t)             # <<<<<<<<<<<<<<
  * 
  *         pack_uint16(&bp_hdr[offset], VERSION)
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint16_t)));
 
-  /* "rbfly/streams/_codec.pyx":178
+  /* "rbfly/streams/_codec.pyx":177
  *         offset += sizeof(uint16_t)
  * 
  *         pack_uint16(&bp_hdr[offset], VERSION)             # <<<<<<<<<<<<<<
  *         offset += sizeof(uint16_t)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_VERSION); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 178, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_VERSION); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_t_6); if (unlikely((__pyx_t_7 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_t_6); if (unlikely((__pyx_t_7 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 177, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_f_5rbfly_6_codec_pack_uint16((&(__pyx_v_bp_hdr[__pyx_v_offset])), __pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint16((&(__pyx_v_bp_hdr[__pyx_v_offset])), __pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 177, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":179
+  /* "rbfly/streams/_codec.pyx":178
  * 
  *         pack_uint16(&bp_hdr[offset], VERSION)
  *         offset += sizeof(uint16_t)             # <<<<<<<<<<<<<<
  * 
  *         bp_hdr[offset] = publisher_id
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint16_t)));
 
-  /* "rbfly/streams/_codec.pyx":181
+  /* "rbfly/streams/_codec.pyx":180
  *         offset += sizeof(uint16_t)
  * 
  *         bp_hdr[offset] = publisher_id             # <<<<<<<<<<<<<<
  *         offset += 1
  * 
  */
-  __pyx_t_8 = __Pyx_PyInt_As_char(__pyx_v_publisher_id); if (unlikely((__pyx_t_8 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 181, __pyx_L1_error)
-  (__pyx_v_bp_hdr[__pyx_v_offset]) = __pyx_t_8;
+  (__pyx_v_bp_hdr[__pyx_v_offset]) = __pyx_v_publisher_id;
 
-  /* "rbfly/streams/_codec.pyx":182
+  /* "rbfly/streams/_codec.pyx":181
  * 
  *         bp_hdr[offset] = publisher_id
  *         offset += 1             # <<<<<<<<<<<<<<
  * 
  *         # mark buffer position for number of messages
  */
   __pyx_v_offset = (__pyx_v_offset + 1);
 
-  /* "rbfly/streams/_codec.pyx":185
+  /* "rbfly/streams/_codec.pyx":184
  * 
  *         # mark buffer position for number of messages
  *         num_offset = offset             # <<<<<<<<<<<<<<
  *         offset += sizeof(uint32_t)
  * 
  */
   __pyx_v_num_offset = __pyx_v_offset;
 
-  /* "rbfly/streams/_codec.pyx":186
+  /* "rbfly/streams/_codec.pyx":185
  *         # mark buffer position for number of messages
  *         num_offset = offset
  *         offset += sizeof(uint32_t)             # <<<<<<<<<<<<<<
  * 
  *         buffer.offset = offset
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint32_t)));
 
-  /* "rbfly/streams/_codec.pyx":188
+  /* "rbfly/streams/_codec.pyx":187
  *         offset += sizeof(uint32_t)
  * 
  *         buffer.offset = offset             # <<<<<<<<<<<<<<
  *         for i in range(msg_len):
  *             msg = messages[i]
  */
   __pyx_v_buffer->offset = __pyx_v_offset;
 
-  /* "rbfly/streams/_codec.pyx":189
+  /* "rbfly/streams/_codec.pyx":188
  * 
  *         buffer.offset = offset
  *         for i in range(msg_len):             # <<<<<<<<<<<<<<
  *             msg = messages[i]
  *             # mark offset of last message, which was successfuly encoded
  */
   __pyx_t_4 = __pyx_v_msg_len;
-  __pyx_t_9 = __pyx_t_4;
-  for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
-    __pyx_v_i = __pyx_t_10;
+  __pyx_t_8 = __pyx_t_4;
+  for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
+    __pyx_v_i = __pyx_t_9;
 
-    /* "rbfly/streams/_codec.pyx":190
+    /* "rbfly/streams/_codec.pyx":189
  *         buffer.offset = offset
  *         for i in range(msg_len):
  *             msg = messages[i]             # <<<<<<<<<<<<<<
  *             # mark offset of last message, which was successfuly encoded
  *             last_offset = buffer.offset
  */
     __pyx_t_6 = PyTuple_GET_ITEM(__pyx_v_messages, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_6);
     __Pyx_XDECREF_SET(__pyx_v_msg, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "rbfly/streams/_codec.pyx":192
+    /* "rbfly/streams/_codec.pyx":191
  *             msg = messages[i]
  *             # mark offset of last message, which was successfuly encoded
  *             last_offset = buffer.offset             # <<<<<<<<<<<<<<
  * 
  *             try:
  */
-    __pyx_t_11 = __pyx_v_buffer->offset;
-    __pyx_v_last_offset = __pyx_t_11;
+    __pyx_t_10 = __pyx_v_buffer->offset;
+    __pyx_v_last_offset = __pyx_t_10;
 
-    /* "rbfly/streams/_codec.pyx":194
+    /* "rbfly/streams/_codec.pyx":193
  *             last_offset = buffer.offset
  * 
  *             try:             # <<<<<<<<<<<<<<
  *                 # pack message id
  *                 bp_msg = buffer_claim(buffer, sizeof(uint64_t))
  */
     {
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
-      __Pyx_ExceptionSave(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
+      __Pyx_ExceptionSave(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
+      __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_13);
-      __Pyx_XGOTREF(__pyx_t_14);
       /*try:*/ {
 
-        /* "rbfly/streams/_codec.pyx":196
+        /* "rbfly/streams/_codec.pyx":195
  *             try:
  *                 # pack message id
  *                 bp_msg = buffer_claim(buffer, sizeof(uint64_t))             # <<<<<<<<<<<<<<
  *                 pack_uint64(bp_msg, msg.stream_publish_id)
  * 
  */
-        __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L5_error)
+        __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 195, __pyx_L5_error)
         __pyx_v_bp_msg = __pyx_t_5;
 
-        /* "rbfly/streams/_codec.pyx":197
+        /* "rbfly/streams/_codec.pyx":196
  *                 # pack message id
  *                 bp_msg = buffer_claim(buffer, sizeof(uint64_t))
  *                 pack_uint64(bp_msg, msg.stream_publish_id)             # <<<<<<<<<<<<<<
  * 
  *                 # pack message itself and then its size
  */
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_stream_publish_id); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 197, __pyx_L5_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_stream_publish_id); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 196, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_15 = __Pyx_PyInt_As_uint64_t(__pyx_t_6); if (unlikely((__pyx_t_15 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 197, __pyx_L5_error)
+        __pyx_t_14 = __Pyx_PyInt_As_uint64_t(__pyx_t_6); if (unlikely((__pyx_t_14 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L5_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __pyx_f_5rbfly_6_codec_pack_uint64(__pyx_v_bp_msg, __pyx_t_15); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 197, __pyx_L5_error)
+        __pyx_f_5rbfly_6_codec_pack_uint64(__pyx_v_bp_msg, __pyx_t_14); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L5_error)
 
-        /* "rbfly/streams/_codec.pyx":200
+        /* "rbfly/streams/_codec.pyx":199
  * 
  *                 # pack message itself and then its size
  *                 bp_msg = buffer_claim(buffer, sizeof(uint32_t))             # <<<<<<<<<<<<<<
  *                 msg_size = encode_msg(buffer, msg)
  *                 pack_uint32(bp_msg, msg_size)
  */
-        __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L5_error)
+        __pyx_t_5 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 199, __pyx_L5_error)
         __pyx_v_bp_msg = __pyx_t_5;
 
-        /* "rbfly/streams/_codec.pyx":201
+        /* "rbfly/streams/_codec.pyx":200
  *                 # pack message itself and then its size
  *                 bp_msg = buffer_claim(buffer, sizeof(uint32_t))
  *                 msg_size = encode_msg(buffer, msg)             # <<<<<<<<<<<<<<
  *                 pack_uint32(bp_msg, msg_size)
  *             except RbFlyBufferError as ex:
  */
-        __pyx_t_11 = __pyx_v_encode_msg(__pyx_v_buffer, __pyx_v_msg); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 201, __pyx_L5_error)
-        __pyx_v_msg_size = __pyx_t_11;
+        __pyx_t_10 = __pyx_v_encode_msg(__pyx_v_buffer, __pyx_v_msg); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 200, __pyx_L5_error)
+        __pyx_v_msg_size = __pyx_t_10;
 
-        /* "rbfly/streams/_codec.pyx":202
+        /* "rbfly/streams/_codec.pyx":201
  *                 bp_msg = buffer_claim(buffer, sizeof(uint32_t))
  *                 msg_size = encode_msg(buffer, msg)
  *                 pack_uint32(bp_msg, msg_size)             # <<<<<<<<<<<<<<
  *             except RbFlyBufferError as ex:
  *                 count = i
  */
-        __pyx_f_5rbfly_6_codec_pack_uint32(__pyx_v_bp_msg, __pyx_v_msg_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 202, __pyx_L5_error)
+        __pyx_f_5rbfly_6_codec_pack_uint32(__pyx_v_bp_msg, __pyx_v_msg_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 201, __pyx_L5_error)
 
-        /* "rbfly/streams/_codec.pyx":194
+        /* "rbfly/streams/_codec.pyx":193
  *             last_offset = buffer.offset
  * 
  *             try:             # <<<<<<<<<<<<<<
  *                 # pack message id
  *                 bp_msg = buffer_claim(buffer, sizeof(uint64_t))
  */
       }
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
       goto __pyx_L12_try_end;
       __pyx_L5_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "rbfly/streams/_codec.pyx":203
+      /* "rbfly/streams/_codec.pyx":202
  *                 msg_size = encode_msg(buffer, msg)
  *                 pack_uint32(bp_msg, msg_size)
  *             except RbFlyBufferError as ex:             # <<<<<<<<<<<<<<
  *                 count = i
  *                 break
  */
-      __Pyx_ErrFetch(&__pyx_t_6, &__pyx_t_16, &__pyx_t_17);
-      __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_RbFlyBufferError); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 203, __pyx_L7_except_error)
-      __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_19 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_6, __pyx_t_18);
-      __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      __Pyx_ErrRestore(__pyx_t_6, __pyx_t_16, __pyx_t_17);
-      __pyx_t_6 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0;
-      if (__pyx_t_19) {
+      __Pyx_ErrFetch(&__pyx_t_6, &__pyx_t_15, &__pyx_t_16);
+      __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_RbFlyBufferError); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 202, __pyx_L7_except_error)
+      __Pyx_GOTREF(__pyx_t_17);
+      __pyx_t_18 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_6, __pyx_t_17);
+      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+      __Pyx_ErrRestore(__pyx_t_6, __pyx_t_15, __pyx_t_16);
+      __pyx_t_6 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
+      if (__pyx_t_18) {
         __Pyx_AddTraceback("rbfly.streams._codec.FrameEncoder.encode_publish", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_17, &__pyx_t_16, &__pyx_t_6) < 0) __PYX_ERR(1, 203, __pyx_L7_except_error)
-        __Pyx_GOTREF(__pyx_t_17);
+        if (__Pyx_GetException(&__pyx_t_16, &__pyx_t_15, &__pyx_t_6) < 0) __PYX_ERR(1, 202, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_16);
+        __Pyx_GOTREF(__pyx_t_15);
         __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_16);
-        __pyx_v_ex = __pyx_t_16;
+        __Pyx_INCREF(__pyx_t_15);
+        __pyx_v_ex = __pyx_t_15;
         /*try:*/ {
 
-          /* "rbfly/streams/_codec.pyx":204
+          /* "rbfly/streams/_codec.pyx":203
  *                 pack_uint32(bp_msg, msg_size)
  *             except RbFlyBufferError as ex:
  *                 count = i             # <<<<<<<<<<<<<<
  *                 break
  *         else:
  */
           __pyx_v_count = __pyx_v_i;
 
-          /* "rbfly/streams/_codec.pyx":205
+          /* "rbfly/streams/_codec.pyx":204
  *             except RbFlyBufferError as ex:
  *                 count = i
  *                 break             # <<<<<<<<<<<<<<
  *         else:
  *             count = msg_len
  */
           goto __pyx_L16_break;
         }
 
-        /* "rbfly/streams/_codec.pyx":203
+        /* "rbfly/streams/_codec.pyx":202
  *                 msg_size = encode_msg(buffer, msg)
  *                 pack_uint32(bp_msg, msg_size)
  *             except RbFlyBufferError as ex:             # <<<<<<<<<<<<<<
  *                 count = i
  *                 break
  */
         /*finally:*/ {
           __pyx_L16_break: {
             __Pyx_DECREF(__pyx_v_ex); __pyx_v_ex = 0;
             goto __pyx_L13_except_break;
           }
         }
         __pyx_L13_except_break:;
-        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         goto __pyx_L10_try_break;
       }
       goto __pyx_L7_except_error;
       __pyx_L7_except_error:;
 
-      /* "rbfly/streams/_codec.pyx":194
+      /* "rbfly/streams/_codec.pyx":193
  *             last_offset = buffer.offset
  * 
  *             try:             # <<<<<<<<<<<<<<
  *                 # pack message id
  *                 bp_msg = buffer_claim(buffer, sizeof(uint64_t))
  */
+      __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_XGIVEREF(__pyx_t_13);
-      __Pyx_XGIVEREF(__pyx_t_14);
-      __Pyx_ExceptionReset(__pyx_t_12, __pyx_t_13, __pyx_t_14);
+      __Pyx_ExceptionReset(__pyx_t_11, __pyx_t_12, __pyx_t_13);
       goto __pyx_L1_error;
       __pyx_L10_try_break:;
+      __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_XGIVEREF(__pyx_t_13);
-      __Pyx_XGIVEREF(__pyx_t_14);
-      __Pyx_ExceptionReset(__pyx_t_12, __pyx_t_13, __pyx_t_14);
+      __Pyx_ExceptionReset(__pyx_t_11, __pyx_t_12, __pyx_t_13);
       goto __pyx_L4_break;
       __pyx_L12_try_end:;
     }
   }
   /*else*/ {
 
-    /* "rbfly/streams/_codec.pyx":207
+    /* "rbfly/streams/_codec.pyx":206
  *                 break
  *         else:
  *             count = msg_len             # <<<<<<<<<<<<<<
  *             last_offset = buffer.offset
  * 
  */
     __pyx_v_count = __pyx_v_msg_len;
 
-    /* "rbfly/streams/_codec.pyx":208
+    /* "rbfly/streams/_codec.pyx":207
  *         else:
  *             count = msg_len
  *             last_offset = buffer.offset             # <<<<<<<<<<<<<<
  * 
  *         pack_uint32(&bp_hdr[num_offset], count)  # TODO: int32 really
  */
-    __pyx_t_10 = __pyx_v_buffer->offset;
-    __pyx_v_last_offset = __pyx_t_10;
+    __pyx_t_9 = __pyx_v_buffer->offset;
+    __pyx_v_last_offset = __pyx_t_9;
   }
   __pyx_L4_break:;
 
-  /* "rbfly/streams/_codec.pyx":210
+  /* "rbfly/streams/_codec.pyx":209
  *             last_offset = buffer.offset
  * 
  *         pack_uint32(&bp_hdr[num_offset], count)  # TODO: int32 really             # <<<<<<<<<<<<<<
  * 
  *         frame_size = last_offset - LEN_FRAME_SIZE
  */
-  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp_hdr[__pyx_v_num_offset])), __pyx_v_count); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 210, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint32((&(__pyx_v_bp_hdr[__pyx_v_num_offset])), __pyx_v_count); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 209, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":212
+  /* "rbfly/streams/_codec.pyx":211
  *         pack_uint32(&bp_hdr[num_offset], count)  # TODO: int32 really
  * 
  *         frame_size = last_offset - LEN_FRAME_SIZE             # <<<<<<<<<<<<<<
  *         pack_uint32(buffer.buffer, frame_size)
  *         return count, buffer.buffer[:last_offset]
  */
   __pyx_v_frame_size = (__pyx_v_last_offset - __pyx_e_5rbfly_7streams_6_codec_LEN_FRAME_SIZE);
 
-  /* "rbfly/streams/_codec.pyx":213
+  /* "rbfly/streams/_codec.pyx":212
  * 
  *         frame_size = last_offset - LEN_FRAME_SIZE
  *         pack_uint32(buffer.buffer, frame_size)             # <<<<<<<<<<<<<<
  *         return count, buffer.buffer[:last_offset]
  * 
  */
-  __pyx_f_5rbfly_6_codec_pack_uint32(__pyx_v_buffer->buffer, __pyx_v_frame_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 213, __pyx_L1_error)
+  __pyx_f_5rbfly_6_codec_pack_uint32(__pyx_v_buffer->buffer, __pyx_v_frame_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 212, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":214
+  /* "rbfly/streams/_codec.pyx":213
  *         frame_size = last_offset - LEN_FRAME_SIZE
  *         pack_uint32(buffer.buffer, frame_size)
  *         return count, buffer.buffer[:last_offset]             # <<<<<<<<<<<<<<
  * 
  * def decode_publish_confirm(data: bytes, start: int) -> tuple[int, object]:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_count); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 214, __pyx_L1_error)
+  __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_count); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_16 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buffer->buffer + 0, __pyx_v_last_offset - 0); if (unlikely(!__pyx_t_16)) __PYX_ERR(1, 214, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buffer->buffer + 0, __pyx_v_last_offset - 0); if (unlikely(!__pyx_t_15)) __PYX_ERR(1, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_15);
+  __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(1, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_17 = PyTuple_New(2); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 214, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_17);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_16);
-  PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_16);
+  PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_15);
+  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_15);
   __pyx_t_6 = 0;
+  __pyx_t_15 = 0;
+  __pyx_r = ((PyObject*)__pyx_t_16);
   __pyx_t_16 = 0;
-  __pyx_r = ((PyObject*)__pyx_t_17);
-  __pyx_t_17 = 0;
   goto __pyx_L0;
 
-  /* "rbfly/streams/_codec.pyx":144
+  /* "rbfly/streams/_codec.pyx":143
  *         return bp[:blen]
  * 
  *     def encode_publish(             # <<<<<<<<<<<<<<
  *             self,
- *             publisher_id: int,
+ *             publisher_id: uint8_t,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_15);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
-  __Pyx_XDECREF(__pyx_t_18);
   __Pyx_AddTraceback("rbfly.streams._codec.FrameEncoder.encode_publish", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_msg);
   __Pyx_XDECREF(__pyx_v_ex);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -6594,15 +6591,15 @@
   __Pyx_AddTraceback("rbfly.streams._codec.FrameEncoder.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_codec.pyx":216
+/* "rbfly/streams/_codec.pyx":215
  *         return count, buffer.buffer[:last_offset]
  * 
  * def decode_publish_confirm(data: bytes, start: int) -> tuple[int, object]:             # <<<<<<<<<<<<<<
  *     """
  *     Decode publisher id and published messages ids from confirmation data
  */
 
@@ -6648,47 +6645,47 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 216, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 215, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 216, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 215, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("decode_publish_confirm", 1, 2, 2, 1); __PYX_ERR(1, 216, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("decode_publish_confirm", 1, 2, 2, 1); __PYX_ERR(1, 215, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_publish_confirm") < 0)) __PYX_ERR(1, 216, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_publish_confirm") < 0)) __PYX_ERR(1, 215, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_data = ((PyObject*)values[0]);
     __pyx_v_start = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode_publish_confirm", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 216, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("decode_publish_confirm", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 215, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.streams._codec.decode_publish_confirm", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(1, 216, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), (&PyInt_Type), 0, "start", 1))) __PYX_ERR(1, 216, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(1, 215, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), (&PyInt_Type), 0, "start", 1))) __PYX_ERR(1, 215, __pyx_L1_error)
   __pyx_r = __pyx_pf_5rbfly_7streams_6_codec_decode_publish_confirm(__pyx_self, __pyx_v_data, __pyx_v_start);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6722,103 +6719,103 @@
   uint32_t __pyx_t_12;
   PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_publish_confirm", 0);
 
-  /* "rbfly/streams/_codec.pyx":225
+  /* "rbfly/streams/_codec.pyx":224
  *     """
  *     cdef:
  *         Buffer b = Buffer(data, len(data), start)             # <<<<<<<<<<<<<<
  *         Buffer *buffer = &b
  *         char *bp
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 224, __pyx_L1_error)
   __pyx_t_1.buffer = __pyx_t_2;
-  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 224, __pyx_L1_error)
   __pyx_t_1.size = __pyx_t_3;
-  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_start); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_start); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 224, __pyx_L1_error)
   __pyx_t_1.offset = __pyx_t_3;
   __pyx_v_b = __pyx_t_1;
 
-  /* "rbfly/streams/_codec.pyx":226
+  /* "rbfly/streams/_codec.pyx":225
  *     cdef:
  *         Buffer b = Buffer(data, len(data), start)
  *         Buffer *buffer = &b             # <<<<<<<<<<<<<<
  *         char *bp
  * 
  */
   __pyx_v_buffer = (&__pyx_v_b);
 
-  /* "rbfly/streams/_codec.pyx":229
+  /* "rbfly/streams/_codec.pyx":228
  *         char *bp
  * 
  *         Py_ssize_t offset = 0             # <<<<<<<<<<<<<<
  *         Py_ssize_t hlen = sizeof(uint8_t) + sizeof(uint32_t)
  * 
  */
   __pyx_v_offset = 0;
 
-  /* "rbfly/streams/_codec.pyx":230
+  /* "rbfly/streams/_codec.pyx":229
  * 
  *         Py_ssize_t offset = 0
  *         Py_ssize_t hlen = sizeof(uint8_t) + sizeof(uint32_t)             # <<<<<<<<<<<<<<
  * 
  *         uint32_t i, n
  */
   __pyx_v_hlen = ((sizeof(uint8_t)) + (sizeof(uint32_t)));
 
-  /* "rbfly/streams/_codec.pyx":236
+  /* "rbfly/streams/_codec.pyx":235
  *         object publish_ids
  * 
  *     bp = buffer_claim(buffer, hlen)             # <<<<<<<<<<<<<<
  *     publisher_id = bp[0]
  *     n = unpack_uint32(&bp[1])  # TODO: int32 really
  */
-  __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 236, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 235, __pyx_L1_error)
   __pyx_v_bp = __pyx_t_2;
 
-  /* "rbfly/streams/_codec.pyx":237
+  /* "rbfly/streams/_codec.pyx":236
  * 
  *     bp = buffer_claim(buffer, hlen)
  *     publisher_id = bp[0]             # <<<<<<<<<<<<<<
  *     n = unpack_uint32(&bp[1])  # TODO: int32 really
  * 
  */
   __pyx_v_publisher_id = (__pyx_v_bp[0]);
 
-  /* "rbfly/streams/_codec.pyx":238
+  /* "rbfly/streams/_codec.pyx":237
  *     bp = buffer_claim(buffer, hlen)
  *     publisher_id = bp[0]
  *     n = unpack_uint32(&bp[1])  # TODO: int32 really             # <<<<<<<<<<<<<<
  * 
  *     if n == 0:
  */
-  __pyx_t_4 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[1]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[1]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 237, __pyx_L1_error)
   __pyx_v_n = __pyx_t_4;
 
-  /* "rbfly/streams/_codec.pyx":240
+  /* "rbfly/streams/_codec.pyx":239
  *     n = unpack_uint32(&bp[1])  # TODO: int32 really
  * 
  *     if n == 0:             # <<<<<<<<<<<<<<
  *         raise RbFlyBufferError('Received zero publish ids')
  * 
  */
   __pyx_t_5 = (__pyx_v_n == 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "rbfly/streams/_codec.pyx":241
+    /* "rbfly/streams/_codec.pyx":240
  * 
  *     if n == 0:
  *         raise RbFlyBufferError('Received zero publish ids')             # <<<<<<<<<<<<<<
  * 
  *     bp = buffer_claim(buffer, n * sizeof(uint64_t))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_RbFlyBufferError); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 241, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_RbFlyBufferError); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -6828,123 +6825,123 @@
         __pyx_t_9 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_kp_u_Received_zero_publish_ids};
       __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 241, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(1, 241, __pyx_L1_error)
+    __PYX_ERR(1, 240, __pyx_L1_error)
 
-    /* "rbfly/streams/_codec.pyx":240
+    /* "rbfly/streams/_codec.pyx":239
  *     n = unpack_uint32(&bp[1])  # TODO: int32 really
  * 
  *     if n == 0:             # <<<<<<<<<<<<<<
  *         raise RbFlyBufferError('Received zero publish ids')
  * 
  */
   }
 
-  /* "rbfly/streams/_codec.pyx":243
+  /* "rbfly/streams/_codec.pyx":242
  *         raise RbFlyBufferError('Received zero publish ids')
  * 
  *     bp = buffer_claim(buffer, n * sizeof(uint64_t))             # <<<<<<<<<<<<<<
  *     offset = 0
  * 
  */
-  __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (__pyx_v_n * (sizeof(uint64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (__pyx_v_n * (sizeof(uint64_t)))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 242, __pyx_L1_error)
   __pyx_v_bp = __pyx_t_2;
 
-  /* "rbfly/streams/_codec.pyx":244
+  /* "rbfly/streams/_codec.pyx":243
  * 
  *     bp = buffer_claim(buffer, n * sizeof(uint64_t))
  *     offset = 0             # <<<<<<<<<<<<<<
  * 
  *     if n == 1:
  */
   __pyx_v_offset = 0;
 
-  /* "rbfly/streams/_codec.pyx":246
+  /* "rbfly/streams/_codec.pyx":245
  *     offset = 0
  * 
  *     if n == 1:             # <<<<<<<<<<<<<<
  *         publish_ids = {unpack_uint64(bp)}
  *     else:
  */
   __pyx_t_5 = (__pyx_v_n == 1);
   if (__pyx_t_5) {
 
-    /* "rbfly/streams/_codec.pyx":247
+    /* "rbfly/streams/_codec.pyx":246
  * 
  *     if n == 1:
  *         publish_ids = {unpack_uint64(bp)}             # <<<<<<<<<<<<<<
  *     else:
  *         publish_ids = set()
  */
-    __pyx_t_10 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_v_bp); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 247, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyInt_From_uint64_t(__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 247, __pyx_L1_error)
+    __pyx_t_10 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_v_bp); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 246, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint64_t(__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PySet_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 247, __pyx_L1_error)
+    __pyx_t_7 = PySet_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PySet_Add(__pyx_t_7, __pyx_t_6) < 0) __PYX_ERR(1, 247, __pyx_L1_error)
+    if (PySet_Add(__pyx_t_7, __pyx_t_6) < 0) __PYX_ERR(1, 246, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_publish_ids = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "rbfly/streams/_codec.pyx":246
+    /* "rbfly/streams/_codec.pyx":245
  *     offset = 0
  * 
  *     if n == 1:             # <<<<<<<<<<<<<<
  *         publish_ids = {unpack_uint64(bp)}
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "rbfly/streams/_codec.pyx":249
+  /* "rbfly/streams/_codec.pyx":248
  *         publish_ids = {unpack_uint64(bp)}
  *     else:
  *         publish_ids = set()             # <<<<<<<<<<<<<<
  *         for i in range(n):
  *             publish_ids.add(unpack_uint64(&bp[offset]))
  */
   /*else*/ {
-    __pyx_t_7 = PySet_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_t_7 = PySet_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_v_publish_ids = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "rbfly/streams/_codec.pyx":250
+    /* "rbfly/streams/_codec.pyx":249
  *     else:
  *         publish_ids = set()
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             publish_ids.add(unpack_uint64(&bp[offset]))
  *             offset += sizeof(uint64_t)
  */
     __pyx_t_4 = __pyx_v_n;
     __pyx_t_11 = __pyx_t_4;
     for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
       __pyx_v_i = __pyx_t_12;
 
-      /* "rbfly/streams/_codec.pyx":251
+      /* "rbfly/streams/_codec.pyx":250
  *         publish_ids = set()
  *         for i in range(n):
  *             publish_ids.add(unpack_uint64(&bp[offset]))             # <<<<<<<<<<<<<<
  *             offset += sizeof(uint64_t)
  * 
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_publish_ids, __pyx_n_s_add); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 251, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_publish_ids, __pyx_n_s_add); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 250, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 251, __pyx_L1_error)
-      __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 251, __pyx_L1_error)
+      __pyx_t_10 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 250, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_From_uint64_t(__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 250, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_13 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_13)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -6955,55 +6952,55 @@
         }
       }
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_t_8};
         __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 251, __pyx_L1_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "rbfly/streams/_codec.pyx":252
+      /* "rbfly/streams/_codec.pyx":251
  *         for i in range(n):
  *             publish_ids.add(unpack_uint64(&bp[offset]))
  *             offset += sizeof(uint64_t)             # <<<<<<<<<<<<<<
  * 
  *     return publisher_id, publish_ids
  */
       __pyx_v_offset = (__pyx_v_offset + (sizeof(uint64_t)));
     }
   }
   __pyx_L4:;
 
-  /* "rbfly/streams/_codec.pyx":254
+  /* "rbfly/streams/_codec.pyx":253
  *             offset += sizeof(uint64_t)
  * 
  *     return publisher_id, publish_ids             # <<<<<<<<<<<<<<
  * 
  * def decode_messages(
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_v_publisher_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 254, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_uint8_t(__pyx_v_publisher_id); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 254, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
   __Pyx_INCREF(__pyx_v_publish_ids);
   __Pyx_GIVEREF(__pyx_v_publish_ids);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_publish_ids);
   __pyx_t_7 = 0;
   __pyx_r = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "rbfly/streams/_codec.pyx":216
+  /* "rbfly/streams/_codec.pyx":215
  *         return count, buffer.buffer[:last_offset]
  * 
  * def decode_publish_confirm(data: bytes, start: int) -> tuple[int, object]:             # <<<<<<<<<<<<<<
  *     """
  *     Decode publisher id and published messages ids from confirmation data
  */
 
@@ -7018,15 +7015,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_publish_ids);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_codec.pyx":256
+/* "rbfly/streams/_codec.pyx":255
  *     return publisher_id, publish_ids
  * 
  * def decode_messages(             # <<<<<<<<<<<<<<
  *         data: bytes,
  *         start: int,
  */
 
@@ -7081,48 +7078,48 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_start)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 1); __PYX_ERR(1, 256, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 1); __PYX_ERR(1, 255, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_offset_start)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 2); __PYX_ERR(1, 256, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 2); __PYX_ERR(1, 255, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_queue)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 3); __PYX_ERR(1, 256, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 3); __PYX_ERR(1, 255, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_amqp)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 256, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 255, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 4); __PYX_ERR(1, 256, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, 4); __PYX_ERR(1, 255, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_messages") < 0)) __PYX_ERR(1, 256, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_messages") < 0)) __PYX_ERR(1, 255, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -7133,23 +7130,23 @@
     __pyx_v_start = ((PyObject*)values[1]);
     __pyx_v_offset_start = ((PyObject*)values[2]);
     __pyx_v_queue = values[3];
     __pyx_v_amqp = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, __pyx_nargs); __PYX_ERR(1, 256, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("decode_messages", 1, 5, 5, __pyx_nargs); __PYX_ERR(1, 255, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("rbfly.streams._codec.decode_messages", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(1, 257, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), (&PyInt_Type), 0, "start", 1))) __PYX_ERR(1, 258, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_offset_start), (&PyInt_Type), 1, "offset_start", 1))) __PYX_ERR(1, 259, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 0, "data", 1))) __PYX_ERR(1, 256, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_start), (&PyInt_Type), 0, "start", 1))) __PYX_ERR(1, 257, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_offset_start), (&PyInt_Type), 1, "offset_start", 1))) __PYX_ERR(1, 258, __pyx_L1_error)
   __pyx_r = __pyx_pf_5rbfly_7streams_6_codec_2decode_messages(__pyx_self, __pyx_v_data, __pyx_v_start, __pyx_v_offset_start, __pyx_v_queue, __pyx_v_amqp);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7180,15 +7177,15 @@
   __pyx_t_5rbfly_7streams_6_codec_t_func_decode __pyx_v_decode_msg;
   PyObject *__pyx_v_ex = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   struct __pyx_t_5rbfly_7_buffer_Buffer __pyx_t_1;
   char *__pyx_t_2;
   Py_ssize_t __pyx_t_3;
-  struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(*__pyx_t_4)(struct __pyx_t_5rbfly_7_buffer_Buffer *);
+  struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(*__pyx_t_4)(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t);
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
@@ -7216,124 +7213,124 @@
   PyObject *__pyx_t_33 = NULL;
   PyObject *__pyx_t_34 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_messages", 0);
 
-  /* "rbfly/streams/_codec.pyx":273
+  /* "rbfly/streams/_codec.pyx":272
  *     """
  *     cdef:
  *         Buffer b = Buffer(data, len(data), start)             # <<<<<<<<<<<<<<
  *         Buffer *buffer = &b
  *         Py_ssize_t offset = 0
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(1, 272, __pyx_L1_error)
   __pyx_t_1.buffer = __pyx_t_2;
-  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 272, __pyx_L1_error)
   __pyx_t_1.size = __pyx_t_3;
-  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_start); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_start); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 272, __pyx_L1_error)
   __pyx_t_1.offset = __pyx_t_3;
   __pyx_v_b = __pyx_t_1;
 
-  /* "rbfly/streams/_codec.pyx":274
+  /* "rbfly/streams/_codec.pyx":273
  *     cdef:
  *         Buffer b = Buffer(data, len(data), start)
  *         Buffer *buffer = &b             # <<<<<<<<<<<<<<
  *         Py_ssize_t offset = 0
  *         Py_ssize_t hlen = (
  */
   __pyx_v_buffer = (&__pyx_v_b);
 
-  /* "rbfly/streams/_codec.pyx":275
+  /* "rbfly/streams/_codec.pyx":274
  *         Buffer b = Buffer(data, len(data), start)
  *         Buffer *buffer = &b
  *         Py_ssize_t offset = 0             # <<<<<<<<<<<<<<
  *         Py_ssize_t hlen = (
  *             2
  */
   __pyx_v_offset = 0;
 
-  /* "rbfly/streams/_codec.pyx":281
+  /* "rbfly/streams/_codec.pyx":280
  *             + sizeof(uint32_t)  # num_records
  *             + sizeof(uint64_t)  * 3  # chunk_first_offset
  *             + sizeof(uint32_t)  * 4  # reserved             # <<<<<<<<<<<<<<
  *         )
  *         char *bp
  */
   __pyx_v_hlen = ((((2 + (sizeof(uint16_t))) + (sizeof(uint32_t))) + ((sizeof(uint64_t)) * 3)) + ((sizeof(uint32_t)) * 4));
 
-  /* "rbfly/streams/_codec.pyx":291
+  /* "rbfly/streams/_codec.pyx":290
  * 
  *         MessageCtx msg
  *         t_func_decode decode_msg = c_decode_amqp if amqp else decode_body             # <<<<<<<<<<<<<<
  * 
  *     bp = buffer_claim(buffer, hlen)
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_amqp); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_amqp); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(1, 290, __pyx_L1_error)
   if (__pyx_t_5) {
     __pyx_t_4 = __pyx_f_5rbfly_4amqp_8_message_c_decode_amqp;
   } else {
     __pyx_t_4 = __pyx_f_5rbfly_7streams_6_codec_decode_body;
   }
   __pyx_v_decode_msg = __pyx_t_4;
 
-  /* "rbfly/streams/_codec.pyx":293
+  /* "rbfly/streams/_codec.pyx":292
  *         t_func_decode decode_msg = c_decode_amqp if amqp else decode_body
  * 
  *     bp = buffer_claim(buffer, hlen)             # <<<<<<<<<<<<<<
  *     magic_version = bp[offset]
  *     offset += 1
  */
-  __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 293, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_hlen); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 292, __pyx_L1_error)
   __pyx_v_bp = __pyx_t_2;
 
-  /* "rbfly/streams/_codec.pyx":294
+  /* "rbfly/streams/_codec.pyx":293
  * 
  *     bp = buffer_claim(buffer, hlen)
  *     magic_version = bp[offset]             # <<<<<<<<<<<<<<
  *     offset += 1
  *     if magic_version != 0x50:  # or 'P'
  */
   __pyx_v_magic_version = (__pyx_v_bp[__pyx_v_offset]);
 
-  /* "rbfly/streams/_codec.pyx":295
+  /* "rbfly/streams/_codec.pyx":294
  *     bp = buffer_claim(buffer, hlen)
  *     magic_version = bp[offset]
  *     offset += 1             # <<<<<<<<<<<<<<
  *     if magic_version != 0x50:  # or 'P'
  *         logger.warning('unknown magic version: 0x{:02x}'.format(magic_version))
  */
   __pyx_v_offset = (__pyx_v_offset + 1);
 
-  /* "rbfly/streams/_codec.pyx":296
+  /* "rbfly/streams/_codec.pyx":295
  *     magic_version = bp[offset]
  *     offset += 1
  *     if magic_version != 0x50:  # or 'P'             # <<<<<<<<<<<<<<
  *         logger.warning('unknown magic version: 0x{:02x}'.format(magic_version))
  *         return
  */
   __pyx_t_5 = (__pyx_v_magic_version != 0x50);
   if (__pyx_t_5) {
 
-    /* "rbfly/streams/_codec.pyx":297
+    /* "rbfly/streams/_codec.pyx":296
  *     offset += 1
  *     if magic_version != 0x50:  # or 'P'
  *         logger.warning('unknown magic version: 0x{:02x}'.format(magic_version))             # <<<<<<<<<<<<<<
  *         return
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 297, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 296, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_warning); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 297, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_warning); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 296, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_unknown_magic_version_0x_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 297, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_unknown_magic_version_0x_02x, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 296, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyInt_From_signed__char(__pyx_v_magic_version); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 297, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_signed__char(__pyx_v_magic_version); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 296, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_11 = NULL;
     __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_11)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -7344,15 +7341,15 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_11, __pyx_t_10};
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 297, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 296, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __pyx_t_9 = NULL;
     __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
@@ -7365,272 +7362,272 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_7};
       __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 297, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 296, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "rbfly/streams/_codec.pyx":298
+    /* "rbfly/streams/_codec.pyx":297
  *     if magic_version != 0x50:  # or 'P'
  *         logger.warning('unknown magic version: 0x{:02x}'.format(magic_version))
  *         return             # <<<<<<<<<<<<<<
  * 
  *     chunk_type = bp[offset]
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "rbfly/streams/_codec.pyx":296
+    /* "rbfly/streams/_codec.pyx":295
  *     magic_version = bp[offset]
  *     offset += 1
  *     if magic_version != 0x50:  # or 'P'             # <<<<<<<<<<<<<<
  *         logger.warning('unknown magic version: 0x{:02x}'.format(magic_version))
  *         return
  */
   }
 
-  /* "rbfly/streams/_codec.pyx":300
+  /* "rbfly/streams/_codec.pyx":299
  *         return
  * 
  *     chunk_type = bp[offset]             # <<<<<<<<<<<<<<
  *     offset += 1
  * 
  */
   __pyx_v_chunk_type = (__pyx_v_bp[__pyx_v_offset]);
 
-  /* "rbfly/streams/_codec.pyx":301
+  /* "rbfly/streams/_codec.pyx":300
  * 
  *     chunk_type = bp[offset]
  *     offset += 1             # <<<<<<<<<<<<<<
  * 
  *     num_entries = unpack_uint16(&bp[offset])
  */
   __pyx_v_offset = (__pyx_v_offset + 1);
 
-  /* "rbfly/streams/_codec.pyx":303
+  /* "rbfly/streams/_codec.pyx":302
  *     offset += 1
  * 
  *     num_entries = unpack_uint16(&bp[offset])             # <<<<<<<<<<<<<<
  *     offset += sizeof(uint16_t)
  * 
  */
-  __pyx_t_13 = __pyx_f_5rbfly_6_codec_unpack_uint16((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 303, __pyx_L1_error)
+  __pyx_t_13 = __pyx_f_5rbfly_6_codec_unpack_uint16((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 302, __pyx_L1_error)
   __pyx_v_num_entries = __pyx_t_13;
 
-  /* "rbfly/streams/_codec.pyx":304
+  /* "rbfly/streams/_codec.pyx":303
  * 
  *     num_entries = unpack_uint16(&bp[offset])
  *     offset += sizeof(uint16_t)             # <<<<<<<<<<<<<<
  * 
  *     num_records = unpack_uint32(&bp[offset])
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint16_t)));
 
-  /* "rbfly/streams/_codec.pyx":306
+  /* "rbfly/streams/_codec.pyx":305
  *     offset += sizeof(uint16_t)
  * 
  *     num_records = unpack_uint32(&bp[offset])             # <<<<<<<<<<<<<<
  *     offset += sizeof(uint32_t)
  * 
  */
-  __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 306, __pyx_L1_error)
+  __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 305, __pyx_L1_error)
   __pyx_v_num_records = __pyx_t_14;
 
-  /* "rbfly/streams/_codec.pyx":307
+  /* "rbfly/streams/_codec.pyx":306
  * 
  *     num_records = unpack_uint32(&bp[offset])
  *     offset += sizeof(uint32_t)             # <<<<<<<<<<<<<<
  * 
  *     timestamp = unpack_uint64(&bp[offset])
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint32_t)));
 
-  /* "rbfly/streams/_codec.pyx":309
+  /* "rbfly/streams/_codec.pyx":308
  *     offset += sizeof(uint32_t)
  * 
  *     timestamp = unpack_uint64(&bp[offset])             # <<<<<<<<<<<<<<
  *     offset += sizeof(uint64_t)
  * 
  */
-  __pyx_t_15 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 309, __pyx_L1_error)
+  __pyx_t_15 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L1_error)
   __pyx_v_timestamp = __pyx_t_15;
 
-  /* "rbfly/streams/_codec.pyx":310
+  /* "rbfly/streams/_codec.pyx":309
  * 
  *     timestamp = unpack_uint64(&bp[offset])
  *     offset += sizeof(uint64_t)             # <<<<<<<<<<<<<<
  * 
  *     epoch = unpack_uint64(&bp[offset])
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint64_t)));
 
-  /* "rbfly/streams/_codec.pyx":312
+  /* "rbfly/streams/_codec.pyx":311
  *     offset += sizeof(uint64_t)
  * 
  *     epoch = unpack_uint64(&bp[offset])             # <<<<<<<<<<<<<<
  *     offset += sizeof(uint64_t)
  * 
  */
-  __pyx_t_15 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 312, __pyx_L1_error)
+  __pyx_t_15 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 311, __pyx_L1_error)
   __pyx_v_epoch = __pyx_t_15;
 
-  /* "rbfly/streams/_codec.pyx":313
+  /* "rbfly/streams/_codec.pyx":312
  * 
  *     epoch = unpack_uint64(&bp[offset])
  *     offset += sizeof(uint64_t)             # <<<<<<<<<<<<<<
  * 
  *     chunk_first_offset = unpack_uint64(&bp[offset])
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint64_t)));
 
-  /* "rbfly/streams/_codec.pyx":315
+  /* "rbfly/streams/_codec.pyx":314
  *     offset += sizeof(uint64_t)
  * 
  *     chunk_first_offset = unpack_uint64(&bp[offset])             # <<<<<<<<<<<<<<
  *     offset += sizeof(uint64_t)
  * 
  */
-  __pyx_t_15 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 315, __pyx_L1_error)
+  __pyx_t_15 = __pyx_f_5rbfly_6_codec_unpack_uint64((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 314, __pyx_L1_error)
   __pyx_v_chunk_first_offset = __pyx_t_15;
 
-  /* "rbfly/streams/_codec.pyx":316
+  /* "rbfly/streams/_codec.pyx":315
  * 
  *     chunk_first_offset = unpack_uint64(&bp[offset])
  *     offset += sizeof(uint64_t)             # <<<<<<<<<<<<<<
  * 
  *     # offset: 32
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint64_t)));
 
-  /* "rbfly/streams/_codec.pyx":319
+  /* "rbfly/streams/_codec.pyx":318
  * 
  *     # offset: 32
  *     chunk_crc = unpack_uint32(&bp[offset])             # <<<<<<<<<<<<<<
  *     offset += sizeof(uint32_t)
  * 
  */
-  __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 319, __pyx_L1_error)
+  __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 318, __pyx_L1_error)
   __pyx_v_chunk_crc = __pyx_t_14;
 
-  /* "rbfly/streams/_codec.pyx":320
+  /* "rbfly/streams/_codec.pyx":319
  *     # offset: 32
  *     chunk_crc = unpack_uint32(&bp[offset])
  *     offset += sizeof(uint32_t)             # <<<<<<<<<<<<<<
  * 
  *     data_size = unpack_uint32(&bp[offset])
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint32_t)));
 
-  /* "rbfly/streams/_codec.pyx":322
+  /* "rbfly/streams/_codec.pyx":321
  *     offset += sizeof(uint32_t)
  * 
  *     data_size = unpack_uint32(&bp[offset])             # <<<<<<<<<<<<<<
  *     offset += sizeof(uint32_t)
  * 
  */
-  __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 322, __pyx_L1_error)
+  __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32((&(__pyx_v_bp[__pyx_v_offset]))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 321, __pyx_L1_error)
   __pyx_v_data_size = __pyx_t_14;
 
-  /* "rbfly/streams/_codec.pyx":323
+  /* "rbfly/streams/_codec.pyx":322
  * 
  *     data_size = unpack_uint32(&bp[offset])
  *     offset += sizeof(uint32_t)             # <<<<<<<<<<<<<<
  * 
  *     offset += sizeof(uint32_t) * 2  # skip for the fields below
  */
   __pyx_v_offset = (__pyx_v_offset + (sizeof(uint32_t)));
 
-  /* "rbfly/streams/_codec.pyx":325
+  /* "rbfly/streams/_codec.pyx":324
  *     offset += sizeof(uint32_t)
  * 
  *     offset += sizeof(uint32_t) * 2  # skip for the fields below             # <<<<<<<<<<<<<<
  *     # trailer_len = unpack_uint32(&bp[offset])
  *     # offset += sizeof(uint32_t)
  */
   __pyx_v_offset = (__pyx_v_offset + ((sizeof(uint32_t)) * 2));
 
-  /* "rbfly/streams/_codec.pyx":331
+  /* "rbfly/streams/_codec.pyx":330
  *     # offset += sizeof(uint32_t)
  * 
  *     if not buffer_check_size(buffer, data_size):             # <<<<<<<<<<<<<<
  *         logger.warning(
  *             'chunk data size invalid, chunk first offset={},'
  */
-  __pyx_t_16 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_data_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 331, __pyx_L1_error)
+  __pyx_t_16 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_data_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 330, __pyx_L1_error)
   __pyx_t_5 = (!(__pyx_t_16 != 0));
   if (__pyx_t_5) {
 
-    /* "rbfly/streams/_codec.pyx":332
+    /* "rbfly/streams/_codec.pyx":331
  * 
  *     if not buffer_check_size(buffer, data_size):
  *         logger.warning(             # <<<<<<<<<<<<<<
  *             'chunk data size invalid, chunk first offset={},'
  *             ' timestamp={}, data size={}, buffer size={}'.format(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logger); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 332, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logger); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_warning); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 332, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_warning); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "rbfly/streams/_codec.pyx":334
+    /* "rbfly/streams/_codec.pyx":333
  *         logger.warning(
  *             'chunk data size invalid, chunk first offset={},'
  *             ' timestamp={}, data size={}, buffer size={}'.format(             # <<<<<<<<<<<<<<
  *                 chunk_first_offset,
  *                 timestamp,
  */
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_chunk_data_size_invalid_chunk_fi, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 334, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_chunk_data_size_invalid_chunk_fi, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
 
-    /* "rbfly/streams/_codec.pyx":335
+    /* "rbfly/streams/_codec.pyx":334
  *             'chunk data size invalid, chunk first offset={},'
  *             ' timestamp={}, data size={}, buffer size={}'.format(
  *                 chunk_first_offset,             # <<<<<<<<<<<<<<
  *                 timestamp,
  *                 data_size,
  */
-    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_chunk_first_offset); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 335, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_uint64_t(__pyx_v_chunk_first_offset); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
 
-    /* "rbfly/streams/_codec.pyx":336
+    /* "rbfly/streams/_codec.pyx":335
  *             ' timestamp={}, data size={}, buffer size={}'.format(
  *                 chunk_first_offset,
  *                 timestamp,             # <<<<<<<<<<<<<<
  *                 data_size,
  *                 buffer.size
  */
-    __pyx_t_11 = __Pyx_PyInt_From_uint64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 336, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_From_uint64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
 
-    /* "rbfly/streams/_codec.pyx":337
+    /* "rbfly/streams/_codec.pyx":336
  *                 chunk_first_offset,
  *                 timestamp,
  *                 data_size,             # <<<<<<<<<<<<<<
  *                 buffer.size
  *             )
  */
-    __pyx_t_17 = __Pyx_PyInt_From_uint32_t(__pyx_v_data_size); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 337, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_From_uint32_t(__pyx_v_data_size); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_17);
 
-    /* "rbfly/streams/_codec.pyx":338
+    /* "rbfly/streams/_codec.pyx":337
  *                 timestamp,
  *                 data_size,
  *                 buffer.size             # <<<<<<<<<<<<<<
  *             )
  *         )
  */
-    __pyx_t_18 = PyInt_FromSsize_t(__pyx_v_buffer->size); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 338, __pyx_L1_error)
+    __pyx_t_18 = PyInt_FromSsize_t(__pyx_v_buffer->size); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __pyx_t_19 = NULL;
     __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_19)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -7644,15 +7641,15 @@
       PyObject *__pyx_callargs[5] = {__pyx_t_19, __pyx_t_10, __pyx_t_11, __pyx_t_17, __pyx_t_18};
       __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_12, 4+__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 334, __pyx_L1_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 333, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __pyx_t_9 = NULL;
     __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
@@ -7665,53 +7662,53 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
       __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 332, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 331, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "rbfly/streams/_codec.pyx":341
+    /* "rbfly/streams/_codec.pyx":340
  *             )
  *         )
  *         return             # <<<<<<<<<<<<<<
  * 
  *     calc_crc = zlib.crc32(bp[offset:offset + data_size])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "rbfly/streams/_codec.pyx":331
+    /* "rbfly/streams/_codec.pyx":330
  *     # offset += sizeof(uint32_t)
  * 
  *     if not buffer_check_size(buffer, data_size):             # <<<<<<<<<<<<<<
  *         logger.warning(
  *             'chunk data size invalid, chunk first offset={},'
  */
   }
 
-  /* "rbfly/streams/_codec.pyx":343
+  /* "rbfly/streams/_codec.pyx":342
  *         return
  * 
  *     calc_crc = zlib.crc32(bp[offset:offset + data_size])             # <<<<<<<<<<<<<<
  *     if chunk_crc != calc_crc:
  *         logger.warning(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_zlib); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_zlib); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_crc32); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_crc32); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_bp + __pyx_v_offset, (__pyx_v_offset + __pyx_v_data_size) - __pyx_v_offset); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_bp + __pyx_v_offset, (__pyx_v_offset + __pyx_v_data_size) - __pyx_v_offset); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_9 = NULL;
   __pyx_t_12 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -7722,67 +7719,67 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_7};
     __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 343, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 342, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
-  __pyx_t_14 = __Pyx_PyInt_As_uint32_t(__pyx_t_6); if (unlikely((__pyx_t_14 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_As_uint32_t(__pyx_t_6); if (unlikely((__pyx_t_14 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_calc_crc = __pyx_t_14;
 
-  /* "rbfly/streams/_codec.pyx":344
+  /* "rbfly/streams/_codec.pyx":343
  * 
  *     calc_crc = zlib.crc32(bp[offset:offset + data_size])
  *     if chunk_crc != calc_crc:             # <<<<<<<<<<<<<<
  *         logger.warning(
  *             'chunk crc validation failed, chunk first offset={},'
  */
   __pyx_t_5 = (__pyx_v_chunk_crc != __pyx_v_calc_crc);
   if (__pyx_t_5) {
 
-    /* "rbfly/streams/_codec.pyx":345
+    /* "rbfly/streams/_codec.pyx":344
  *     calc_crc = zlib.crc32(bp[offset:offset + data_size])
  *     if chunk_crc != calc_crc:
  *         logger.warning(             # <<<<<<<<<<<<<<
  *             'chunk crc validation failed, chunk first offset={},'
  *             ' timestamp={}, crc={}'.format(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logger); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 345, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logger); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_warning); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 345, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_warning); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "rbfly/streams/_codec.pyx":347
+    /* "rbfly/streams/_codec.pyx":346
  *         logger.warning(
  *             'chunk crc validation failed, chunk first offset={},'
  *             ' timestamp={}, crc={}'.format(             # <<<<<<<<<<<<<<
  *                 chunk_first_offset, timestamp, calc_crc
  *             )
  */
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_chunk_crc_validation_failed_chun, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 347, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_chunk_crc_validation_failed_chun, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 346, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
 
-    /* "rbfly/streams/_codec.pyx":348
+    /* "rbfly/streams/_codec.pyx":347
  *             'chunk crc validation failed, chunk first offset={},'
  *             ' timestamp={}, crc={}'.format(
  *                 chunk_first_offset, timestamp, calc_crc             # <<<<<<<<<<<<<<
  *             )
  *         )
  */
-    __pyx_t_18 = __Pyx_PyInt_From_uint64_t(__pyx_v_chunk_first_offset); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 348, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyInt_From_uint64_t(__pyx_v_chunk_first_offset); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
-    __pyx_t_17 = __Pyx_PyInt_From_uint64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 348, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_From_uint64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_17);
-    __pyx_t_11 = __Pyx_PyInt_From_uint32_t(__pyx_v_calc_crc); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 348, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_From_uint32_t(__pyx_v_calc_crc); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __pyx_t_10 = NULL;
     __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -7795,15 +7792,15 @@
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_10, __pyx_t_18, __pyx_t_17, __pyx_t_11};
       __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_12, 3+__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 347, __pyx_L1_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 346, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __pyx_t_9 = NULL;
     __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
@@ -7816,179 +7813,179 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
       __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 345, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 344, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "rbfly/streams/_codec.pyx":351
+    /* "rbfly/streams/_codec.pyx":350
  *             )
  *         )
  *         return             # <<<<<<<<<<<<<<
  * 
  *     for k_entry in range(num_entries):
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "rbfly/streams/_codec.pyx":344
+    /* "rbfly/streams/_codec.pyx":343
  * 
  *     calc_crc = zlib.crc32(bp[offset:offset + data_size])
  *     if chunk_crc != calc_crc:             # <<<<<<<<<<<<<<
  *         logger.warning(
  *             'chunk crc validation failed, chunk first offset={},'
  */
   }
 
-  /* "rbfly/streams/_codec.pyx":353
+  /* "rbfly/streams/_codec.pyx":352
  *         return
  * 
  *     for k_entry in range(num_entries):             # <<<<<<<<<<<<<<
  *         bp = buffer_claim(buffer, sizeof(uint32_t))
  *         size = unpack_uint32(bp)
  */
   __pyx_t_13 = __pyx_v_num_entries;
   __pyx_t_20 = __pyx_t_13;
   for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
     __pyx_v_k_entry = __pyx_t_21;
 
-    /* "rbfly/streams/_codec.pyx":354
+    /* "rbfly/streams/_codec.pyx":353
  * 
  *     for k_entry in range(num_entries):
  *         bp = buffer_claim(buffer, sizeof(uint32_t))             # <<<<<<<<<<<<<<
  *         size = unpack_uint32(bp)
  *         if buffer_check_size(buffer, size):
  */
-    __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 354, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint32_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 353, __pyx_L1_error)
     __pyx_v_bp = __pyx_t_2;
 
-    /* "rbfly/streams/_codec.pyx":355
+    /* "rbfly/streams/_codec.pyx":354
  *     for k_entry in range(num_entries):
  *         bp = buffer_claim(buffer, sizeof(uint32_t))
  *         size = unpack_uint32(bp)             # <<<<<<<<<<<<<<
  *         if buffer_check_size(buffer, size):
  *             current_offset = chunk_first_offset + k_entry
  */
-    __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_v_bp); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 355, __pyx_L1_error)
+    __pyx_t_14 = __pyx_f_5rbfly_6_codec_unpack_uint32(__pyx_v_bp); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 354, __pyx_L1_error)
     __pyx_v_size = __pyx_t_14;
 
-    /* "rbfly/streams/_codec.pyx":356
+    /* "rbfly/streams/_codec.pyx":355
  *         bp = buffer_claim(buffer, sizeof(uint32_t))
  *         size = unpack_uint32(bp)
  *         if buffer_check_size(buffer, size):             # <<<<<<<<<<<<<<
  *             current_offset = chunk_first_offset + k_entry
  *             if offset_start is None or current_offset >= offset_start:
  */
-    __pyx_t_16 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 356, __pyx_L1_error)
+    __pyx_t_16 = __pyx_f_5rbfly_7_buffer_buffer_check_size(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 355, __pyx_L1_error)
     __pyx_t_5 = (__pyx_t_16 != 0);
     if (__pyx_t_5) {
 
-      /* "rbfly/streams/_codec.pyx":357
+      /* "rbfly/streams/_codec.pyx":356
  *         size = unpack_uint32(bp)
  *         if buffer_check_size(buffer, size):
  *             current_offset = chunk_first_offset + k_entry             # <<<<<<<<<<<<<<
  *             if offset_start is None or current_offset >= offset_start:
  *                 try:
  */
       __pyx_v_current_offset = (__pyx_v_chunk_first_offset + __pyx_v_k_entry);
 
-      /* "rbfly/streams/_codec.pyx":358
+      /* "rbfly/streams/_codec.pyx":357
  *         if buffer_check_size(buffer, size):
  *             current_offset = chunk_first_offset + k_entry
  *             if offset_start is None or current_offset >= offset_start:             # <<<<<<<<<<<<<<
  *                 try:
- *                     msg = decode_msg(buffer)
+ *                     msg = decode_msg(buffer, size)
  */
       __pyx_t_22 = (__pyx_v_offset_start == ((PyObject*)Py_None));
       if (!__pyx_t_22) {
       } else {
         __pyx_t_5 = __pyx_t_22;
         goto __pyx_L10_bool_binop_done;
       }
-      __pyx_t_6 = __Pyx_PyInt_From_uint64_t(__pyx_v_current_offset); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 358, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_uint64_t(__pyx_v_current_offset); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 357, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = PyObject_RichCompare(__pyx_t_6, __pyx_v_offset_start, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 358, __pyx_L1_error)
+      __pyx_t_7 = PyObject_RichCompare(__pyx_t_6, __pyx_v_offset_start, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 357, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_22 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_22 < 0))) __PYX_ERR(1, 358, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_22 < 0))) __PYX_ERR(1, 357, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_5 = __pyx_t_22;
       __pyx_L10_bool_binop_done:;
       if (__pyx_t_5) {
 
-        /* "rbfly/streams/_codec.pyx":359
+        /* "rbfly/streams/_codec.pyx":358
  *             current_offset = chunk_first_offset + k_entry
  *             if offset_start is None or current_offset >= offset_start:
  *                 try:             # <<<<<<<<<<<<<<
- *                     msg = decode_msg(buffer)
+ *                     msg = decode_msg(buffer, size)
  *                     msg.stream_offset = current_offset
  */
         {
           __Pyx_PyThreadState_declare
           __Pyx_PyThreadState_assign
           __Pyx_ExceptionSave(&__pyx_t_23, &__pyx_t_24, &__pyx_t_25);
           __Pyx_XGOTREF(__pyx_t_23);
           __Pyx_XGOTREF(__pyx_t_24);
           __Pyx_XGOTREF(__pyx_t_25);
           /*try:*/ {
 
-            /* "rbfly/streams/_codec.pyx":360
+            /* "rbfly/streams/_codec.pyx":359
  *             if offset_start is None or current_offset >= offset_start:
  *                 try:
- *                     msg = decode_msg(buffer)             # <<<<<<<<<<<<<<
+ *                     msg = decode_msg(buffer, size)             # <<<<<<<<<<<<<<
  *                     msg.stream_offset = current_offset
  *                     msg.stream_timestamp = <double> timestamp / 1000
  */
-            __pyx_t_7 = ((PyObject *)__pyx_v_decode_msg(__pyx_v_buffer)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 360, __pyx_L12_error)
+            __pyx_t_7 = ((PyObject *)__pyx_v_decode_msg(__pyx_v_buffer, __pyx_v_size)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 359, __pyx_L12_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_XDECREF_SET(__pyx_v_msg, ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_7));
             __pyx_t_7 = 0;
 
-            /* "rbfly/streams/_codec.pyx":361
+            /* "rbfly/streams/_codec.pyx":360
  *                 try:
- *                     msg = decode_msg(buffer)
+ *                     msg = decode_msg(buffer, size)
  *                     msg.stream_offset = current_offset             # <<<<<<<<<<<<<<
  *                     msg.stream_timestamp = <double> timestamp / 1000
  *                 except AMQPDecoderError as ex:
  */
             __pyx_v_msg->stream_offset = __pyx_v_current_offset;
 
-            /* "rbfly/streams/_codec.pyx":362
- *                     msg = decode_msg(buffer)
+            /* "rbfly/streams/_codec.pyx":361
+ *                     msg = decode_msg(buffer, size)
  *                     msg.stream_offset = current_offset
  *                     msg.stream_timestamp = <double> timestamp / 1000             # <<<<<<<<<<<<<<
  *                 except AMQPDecoderError as ex:
  *                     logger.warning('cannot decode amqp message: {}'.format(ex))
  */
             __pyx_v_msg->stream_timestamp = (((double)__pyx_v_timestamp) / 1000.0);
 
-            /* "rbfly/streams/_codec.pyx":359
+            /* "rbfly/streams/_codec.pyx":358
  *             current_offset = chunk_first_offset + k_entry
  *             if offset_start is None or current_offset >= offset_start:
  *                 try:             # <<<<<<<<<<<<<<
- *                     msg = decode_msg(buffer)
+ *                     msg = decode_msg(buffer, size)
  *                     msg.stream_offset = current_offset
  */
           }
 
-          /* "rbfly/streams/_codec.pyx":366
+          /* "rbfly/streams/_codec.pyx":365
  *                     logger.warning('cannot decode amqp message: {}'.format(ex))
  *                 else:
  *                     queue.put(msg)             # <<<<<<<<<<<<<<
  *             else:
  *                 buffer.offset += size  # skip message
  */
           /*else:*/ {
-            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_queue, __pyx_n_s_put); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 366, __pyx_L14_except_error)
+            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_queue, __pyx_n_s_put); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 365, __pyx_L14_except_error)
             __Pyx_GOTREF(__pyx_t_6);
             __pyx_t_8 = NULL;
             __pyx_t_12 = 0;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
               __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
               if (likely(__pyx_t_8)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -7998,15 +7995,15 @@
                 __pyx_t_12 = 1;
               }
             }
             {
               PyObject *__pyx_callargs[2] = {__pyx_t_8, ((PyObject *)__pyx_v_msg)};
               __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
               __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-              if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 366, __pyx_L14_except_error)
+              if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 365, __pyx_L14_except_error)
               __Pyx_GOTREF(__pyx_t_7);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
             }
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           }
           __Pyx_XDECREF(__pyx_t_23); __pyx_t_23 = 0;
           __Pyx_XDECREF(__pyx_t_24); __pyx_t_24 = 0;
@@ -8019,51 +8016,51 @@
           __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
           __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-          /* "rbfly/streams/_codec.pyx":363
+          /* "rbfly/streams/_codec.pyx":362
  *                     msg.stream_offset = current_offset
  *                     msg.stream_timestamp = <double> timestamp / 1000
  *                 except AMQPDecoderError as ex:             # <<<<<<<<<<<<<<
  *                     logger.warning('cannot decode amqp message: {}'.format(ex))
  *                 else:
  */
           __Pyx_ErrFetch(&__pyx_t_7, &__pyx_t_6, &__pyx_t_8);
-          __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 363, __pyx_L14_except_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 362, __pyx_L14_except_error)
           __Pyx_GOTREF(__pyx_t_9);
           __pyx_t_12 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_7, __pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_ErrRestore(__pyx_t_7, __pyx_t_6, __pyx_t_8);
           __pyx_t_7 = 0; __pyx_t_6 = 0; __pyx_t_8 = 0;
           if (__pyx_t_12) {
             __Pyx_AddTraceback("rbfly.streams._codec.decode_messages", __pyx_clineno, __pyx_lineno, __pyx_filename);
-            if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 363, __pyx_L14_except_error)
+            if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 362, __pyx_L14_except_error)
             __Pyx_GOTREF(__pyx_t_8);
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_INCREF(__pyx_t_6);
             __pyx_v_ex = __pyx_t_6;
             /*try:*/ {
 
-              /* "rbfly/streams/_codec.pyx":364
+              /* "rbfly/streams/_codec.pyx":363
  *                     msg.stream_timestamp = <double> timestamp / 1000
  *                 except AMQPDecoderError as ex:
  *                     logger.warning('cannot decode amqp message: {}'.format(ex))             # <<<<<<<<<<<<<<
  *                 else:
  *                     queue.put(msg)
  */
-              __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_logger); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 364, __pyx_L25_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_logger); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 363, __pyx_L25_error)
               __Pyx_GOTREF(__pyx_t_11);
-              __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_warning); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 364, __pyx_L25_error)
+              __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_warning); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 363, __pyx_L25_error)
               __Pyx_GOTREF(__pyx_t_17);
               __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-              __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_cannot_decode_amqp_message, __pyx_n_s_format); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 364, __pyx_L25_error)
+              __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_cannot_decode_amqp_message, __pyx_n_s_format); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 363, __pyx_L25_error)
               __Pyx_GOTREF(__pyx_t_18);
               __pyx_t_10 = NULL;
               __pyx_t_12 = 0;
               if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_18))) {
                 __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_18);
                 if (likely(__pyx_t_10)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_18);
@@ -8073,15 +8070,15 @@
                   __pyx_t_12 = 1;
                 }
               }
               {
                 PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_v_ex};
                 __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_18, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
                 __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-                if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 364, __pyx_L25_error)
+                if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 363, __pyx_L25_error)
                 __Pyx_GOTREF(__pyx_t_11);
                 __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
               }
               __pyx_t_18 = NULL;
               __pyx_t_12 = 0;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_17))) {
                 __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_17);
@@ -8094,22 +8091,22 @@
                 }
               }
               {
                 PyObject *__pyx_callargs[2] = {__pyx_t_18, __pyx_t_11};
                 __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_17, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
                 __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
                 __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-                if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 364, __pyx_L25_error)
+                if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 363, __pyx_L25_error)
                 __Pyx_GOTREF(__pyx_t_9);
                 __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
               }
               __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
             }
 
-            /* "rbfly/streams/_codec.pyx":363
+            /* "rbfly/streams/_codec.pyx":362
  *                     msg.stream_offset = current_offset
  *                     msg.stream_timestamp = <double> timestamp / 1000
  *                 except AMQPDecoderError as ex:             # <<<<<<<<<<<<<<
  *                     logger.warning('cannot decode amqp message: {}'.format(ex))
  *                 else:
  */
             /*finally:*/ {
@@ -8160,19 +8157,19 @@
             __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
             __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
             goto __pyx_L13_exception_handled;
           }
           goto __pyx_L14_except_error;
           __pyx_L14_except_error:;
 
-          /* "rbfly/streams/_codec.pyx":359
+          /* "rbfly/streams/_codec.pyx":358
  *             current_offset = chunk_first_offset + k_entry
  *             if offset_start is None or current_offset >= offset_start:
  *                 try:             # <<<<<<<<<<<<<<
- *                     msg = decode_msg(buffer)
+ *                     msg = decode_msg(buffer, size)
  *                     msg.stream_offset = current_offset
  */
           __Pyx_XGIVEREF(__pyx_t_23);
           __Pyx_XGIVEREF(__pyx_t_24);
           __Pyx_XGIVEREF(__pyx_t_25);
           __Pyx_ExceptionReset(__pyx_t_23, __pyx_t_24, __pyx_t_25);
           goto __pyx_L1_error;
@@ -8180,118 +8177,118 @@
           __Pyx_XGIVEREF(__pyx_t_23);
           __Pyx_XGIVEREF(__pyx_t_24);
           __Pyx_XGIVEREF(__pyx_t_25);
           __Pyx_ExceptionReset(__pyx_t_23, __pyx_t_24, __pyx_t_25);
           __pyx_L19_try_end:;
         }
 
-        /* "rbfly/streams/_codec.pyx":358
+        /* "rbfly/streams/_codec.pyx":357
  *         if buffer_check_size(buffer, size):
  *             current_offset = chunk_first_offset + k_entry
  *             if offset_start is None or current_offset >= offset_start:             # <<<<<<<<<<<<<<
  *                 try:
- *                     msg = decode_msg(buffer)
+ *                     msg = decode_msg(buffer, size)
  */
         goto __pyx_L9;
       }
 
-      /* "rbfly/streams/_codec.pyx":368
+      /* "rbfly/streams/_codec.pyx":367
  *                     queue.put(msg)
  *             else:
  *                 buffer.offset += size  # skip message             # <<<<<<<<<<<<<<
  *         else:
  *             logger.warning(
  */
       /*else*/ {
         __pyx_v_buffer->offset = (__pyx_v_buffer->offset + __pyx_v_size);
       }
       __pyx_L9:;
 
-      /* "rbfly/streams/_codec.pyx":356
+      /* "rbfly/streams/_codec.pyx":355
  *         bp = buffer_claim(buffer, sizeof(uint32_t))
  *         size = unpack_uint32(bp)
  *         if buffer_check_size(buffer, size):             # <<<<<<<<<<<<<<
  *             current_offset = chunk_first_offset + k_entry
  *             if offset_start is None or current_offset >= offset_start:
  */
       goto __pyx_L8;
     }
 
-    /* "rbfly/streams/_codec.pyx":370
+    /* "rbfly/streams/_codec.pyx":369
  *                 buffer.offset += size  # skip message
  *         else:
  *             logger.warning(             # <<<<<<<<<<<<<<
  *                 'message data size invalid, chunk first offset={},'
  *                 ' timestamp={}, offset={}, message size={}, buffer size={}'.format(
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_logger); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 370, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_logger); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 369, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_warning); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 370, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_warning); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 369, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "rbfly/streams/_codec.pyx":372
+      /* "rbfly/streams/_codec.pyx":371
  *             logger.warning(
  *                 'message data size invalid, chunk first offset={},'
  *                 ' timestamp={}, offset={}, message size={}, buffer size={}'.format(             # <<<<<<<<<<<<<<
  *                     chunk_first_offset,
  *                     timestamp,
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_message_data_size_invalid_chunk, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 372, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_message_data_size_invalid_chunk, __pyx_n_s_format); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 371, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
 
-      /* "rbfly/streams/_codec.pyx":373
+      /* "rbfly/streams/_codec.pyx":372
  *                 'message data size invalid, chunk first offset={},'
  *                 ' timestamp={}, offset={}, message size={}, buffer size={}'.format(
  *                     chunk_first_offset,             # <<<<<<<<<<<<<<
  *                     timestamp,
  *                     buffer.offset,
  */
-      __pyx_t_17 = __Pyx_PyInt_From_uint64_t(__pyx_v_chunk_first_offset); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 373, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyInt_From_uint64_t(__pyx_v_chunk_first_offset); if (unlikely(!__pyx_t_17)) __PYX_ERR(1, 372, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_17);
 
-      /* "rbfly/streams/_codec.pyx":374
+      /* "rbfly/streams/_codec.pyx":373
  *                 ' timestamp={}, offset={}, message size={}, buffer size={}'.format(
  *                     chunk_first_offset,
  *                     timestamp,             # <<<<<<<<<<<<<<
  *                     buffer.offset,
  *                     size,
  */
-      __pyx_t_11 = __Pyx_PyInt_From_uint64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 374, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_From_uint64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 373, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
 
-      /* "rbfly/streams/_codec.pyx":375
+      /* "rbfly/streams/_codec.pyx":374
  *                     chunk_first_offset,
  *                     timestamp,
  *                     buffer.offset,             # <<<<<<<<<<<<<<
  *                     size,
  *                     buffer.size
  */
-      __pyx_t_18 = PyInt_FromSsize_t(__pyx_v_buffer->offset); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 375, __pyx_L1_error)
+      __pyx_t_18 = PyInt_FromSsize_t(__pyx_v_buffer->offset); if (unlikely(!__pyx_t_18)) __PYX_ERR(1, 374, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
 
-      /* "rbfly/streams/_codec.pyx":376
+      /* "rbfly/streams/_codec.pyx":375
  *                     timestamp,
  *                     buffer.offset,
  *                     size,             # <<<<<<<<<<<<<<
  *                     buffer.size
  *                 )
  */
-      __pyx_t_10 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 376, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 375, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
 
-      /* "rbfly/streams/_codec.pyx":377
+      /* "rbfly/streams/_codec.pyx":376
  *                     buffer.offset,
  *                     size,
  *                     buffer.size             # <<<<<<<<<<<<<<
  *                 )
  *             )
  */
-      __pyx_t_19 = PyInt_FromSsize_t(__pyx_v_buffer->size); if (unlikely(!__pyx_t_19)) __PYX_ERR(1, 377, __pyx_L1_error)
+      __pyx_t_19 = PyInt_FromSsize_t(__pyx_v_buffer->size); if (unlikely(!__pyx_t_19)) __PYX_ERR(1, 376, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
       __pyx_t_34 = NULL;
       __pyx_t_26 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_34 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_34)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -8306,15 +8303,15 @@
         __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_26, 5+__pyx_t_26);
         __Pyx_XDECREF(__pyx_t_34); __pyx_t_34 = 0;
         __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-        if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 372, __pyx_L1_error)
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 371, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __pyx_t_9 = NULL;
       __pyx_t_26 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
@@ -8327,35 +8324,35 @@
         }
       }
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_6};
         __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_26, 1+__pyx_t_26);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 370, __pyx_L1_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 369, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "rbfly/streams/_codec.pyx":380
+      /* "rbfly/streams/_codec.pyx":379
  *                 )
  *             )
  *             return             # <<<<<<<<<<<<<<
  * 
  * cdef inline Py_ssize_t encode_body(Buffer *buffer, object message) except -1:
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
     }
     __pyx_L8:;
   }
 
-  /* "rbfly/streams/_codec.pyx":256
+  /* "rbfly/streams/_codec.pyx":255
  *     return publisher_id, publish_ids
  * 
  * def decode_messages(             # <<<<<<<<<<<<<<
  *         data: bytes,
  *         start: int,
  */
 
@@ -8379,15 +8376,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_msg);
   __Pyx_XDECREF(__pyx_v_ex);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_codec.pyx":382
+/* "rbfly/streams/_codec.pyx":381
  *             return
  * 
  * cdef inline Py_ssize_t encode_body(Buffer *buffer, object message) except -1:             # <<<<<<<<<<<<<<
  *     cdef:
  *         object body = message.body
  */
 
@@ -8396,72 +8393,73 @@
   Py_ssize_t __pyx_v_size;
   char *__pyx_v_bp;
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   char *__pyx_t_3;
+  uint8_t *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_body", 0);
 
-  /* "rbfly/streams/_codec.pyx":384
+  /* "rbfly/streams/_codec.pyx":383
  * cdef inline Py_ssize_t encode_body(Buffer *buffer, object message) except -1:
  *     cdef:
  *         object body = message.body             # <<<<<<<<<<<<<<
  *         Py_ssize_t size = len(body)
  *         char *bp
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_message, __pyx_n_s_body); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 384, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_message, __pyx_n_s_body); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_body = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "rbfly/streams/_codec.pyx":385
+  /* "rbfly/streams/_codec.pyx":384
  *     cdef:
  *         object body = message.body
  *         Py_ssize_t size = len(body)             # <<<<<<<<<<<<<<
  *         char *bp
  * 
  */
-  __pyx_t_2 = PyObject_Length(__pyx_v_body); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 385, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_v_body); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(1, 384, __pyx_L1_error)
   __pyx_v_size = __pyx_t_2;
 
-  /* "rbfly/streams/_codec.pyx":388
+  /* "rbfly/streams/_codec.pyx":387
  *         char *bp
  * 
  *     bp = buffer_claim(buffer, size)             # <<<<<<<<<<<<<<
- *     memcpy(bp, <char*> body, size)
+ *     memcpy(bp, <uint8_t*> body, size)
  *     return size
  */
-  __pyx_t_3 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 388, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 387, __pyx_L1_error)
   __pyx_v_bp = __pyx_t_3;
 
-  /* "rbfly/streams/_codec.pyx":389
+  /* "rbfly/streams/_codec.pyx":388
  * 
  *     bp = buffer_claim(buffer, size)
- *     memcpy(bp, <char*> body, size)             # <<<<<<<<<<<<<<
+ *     memcpy(bp, <uint8_t*> body, size)             # <<<<<<<<<<<<<<
  *     return size
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_body); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(1, 389, __pyx_L1_error)
-  (void)(memcpy(__pyx_v_bp, ((char *)__pyx_t_3), __pyx_v_size));
+  __pyx_t_4 = __Pyx_PyObject_AsWritableUString(__pyx_v_body); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 388, __pyx_L1_error)
+  (void)(memcpy(__pyx_v_bp, ((uint8_t *)__pyx_t_4), __pyx_v_size));
 
-  /* "rbfly/streams/_codec.pyx":390
+  /* "rbfly/streams/_codec.pyx":389
  *     bp = buffer_claim(buffer, size)
- *     memcpy(bp, <char*> body, size)
+ *     memcpy(bp, <uint8_t*> body, size)
  *     return size             # <<<<<<<<<<<<<<
  * 
- * cdef inline MessageCtx decode_body(Buffer *buffer):
+ * cdef inline MessageCtx decode_body(Buffer *buffer, Py_ssize_t size):
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "rbfly/streams/_codec.pyx":382
+  /* "rbfly/streams/_codec.pyx":381
  *             return
  * 
  * cdef inline Py_ssize_t encode_body(Buffer *buffer, object message) except -1:             # <<<<<<<<<<<<<<
  *     cdef:
  *         object body = message.body
  */
 
@@ -8472,61 +8470,73 @@
   __pyx_r = -1L;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_body);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "rbfly/streams/_codec.pyx":392
+/* "rbfly/streams/_codec.pyx":391
  *     return size
  * 
- * cdef inline MessageCtx decode_body(Buffer *buffer):             # <<<<<<<<<<<<<<
- *     return MessageCtx(buffer.buffer[buffer.offset:buffer.size])
- * 
+ * cdef inline MessageCtx decode_body(Buffer *buffer, Py_ssize_t size):             # <<<<<<<<<<<<<<
+ *     cdef:
+ *         char *bp = buffer_claim(buffer, size)
  */
 
-static CYTHON_INLINE struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_7streams_6_codec_decode_body(struct __pyx_t_5rbfly_7_buffer_Buffer *__pyx_v_buffer) {
+static CYTHON_INLINE struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_f_5rbfly_7streams_6_codec_decode_body(struct __pyx_t_5rbfly_7_buffer_Buffer *__pyx_v_buffer, Py_ssize_t __pyx_v_size) {
+  char *__pyx_v_bp;
   struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_body", 0);
 
   /* "rbfly/streams/_codec.pyx":393
+ * cdef inline MessageCtx decode_body(Buffer *buffer, Py_ssize_t size):
+ *     cdef:
+ *         char *bp = buffer_claim(buffer, size)             # <<<<<<<<<<<<<<
  * 
- * cdef inline MessageCtx decode_body(Buffer *buffer):
- *     return MessageCtx(buffer.buffer[buffer.offset:buffer.size])             # <<<<<<<<<<<<<<
+ *     return MessageCtx(bp[:size])
+ */
+  __pyx_t_1 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, __pyx_v_size); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L1_error)
+  __pyx_v_bp = __pyx_t_1;
+
+  /* "rbfly/streams/_codec.pyx":395
+ *         char *bp = buffer_claim(buffer, size)
+ * 
+ *     return MessageCtx(bp[:size])             # <<<<<<<<<<<<<<
  * 
  * # vim: sw=4:et:ai
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_buffer->buffer + __pyx_v_buffer->offset, __pyx_v_buffer->size - __pyx_v_buffer->offset); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 393, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 393, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_bp + 0, __pyx_v_size - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_r = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 395, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)__pyx_t_3);
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "rbfly/streams/_codec.pyx":392
+  /* "rbfly/streams/_codec.pyx":391
  *     return size
  * 
- * cdef inline MessageCtx decode_body(Buffer *buffer):             # <<<<<<<<<<<<<<
- *     return MessageCtx(buffer.buffer[buffer.offset:buffer.size])
- * 
+ * cdef inline MessageCtx decode_body(Buffer *buffer, Py_ssize_t size):             # <<<<<<<<<<<<<<
+ *     cdef:
+ *         char *bp = buffer_claim(buffer, size)
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("rbfly.streams._codec.decode_body", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9147,58 +9157,59 @@
     {&__pyx_n_s_timestamp, __pyx_k_timestamp, sizeof(__pyx_k_timestamp), 0, 0, 1, 1},
     {&__pyx_n_s_tp, __pyx_k_tp, sizeof(__pyx_k_tp), 0, 0, 1, 1},
     {&__pyx_kp_s_tp_Iterator, __pyx_k_tp_Iterator, sizeof(__pyx_k_tp_Iterator), 0, 0, 1, 0},
     {&__pyx_kp_s_tp_Optional_int, __pyx_k_tp_Optional_int, sizeof(__pyx_k_tp_Optional_int), 0, 0, 1, 0},
     {&__pyx_kp_s_tuple_int_bytes, __pyx_k_tuple_int_bytes, sizeof(__pyx_k_tuple_int_bytes), 0, 0, 1, 0},
     {&__pyx_kp_s_tuple_int_object, __pyx_k_tuple_int_object, sizeof(__pyx_k_tuple_int_object), 0, 0, 1, 0},
     {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
+    {&__pyx_n_s_uint8_t, __pyx_k_uint8_t, sizeof(__pyx_k_uint8_t), 0, 0, 1, 1},
     {&__pyx_kp_u_unknown_frame_version_version, __pyx_k_unknown_frame_version_version, sizeof(__pyx_k_unknown_frame_version_version), 0, 1, 0, 0},
     {&__pyx_kp_u_unknown_magic_version_0x_02x, __pyx_k_unknown_magic_version_0x_02x, sizeof(__pyx_k_unknown_magic_version_0x_02x), 0, 1, 0, 0},
     {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
     {&__pyx_n_s_warning, __pyx_k_warning, sizeof(__pyx_k_warning), 0, 0, 1, 1},
     {&__pyx_n_s_zlib, __pyx_k_zlib, sizeof(__pyx_k_zlib), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 120, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 189, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 119, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 188, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(3, 120, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "rbfly/streams/_codec.pyx":120
+  /* "rbfly/streams/_codec.pyx":119
  *         # check encoding method if this changes
  *         if size < 32:
  *             raise ValueError('Encoder buffer minimum size is 32 bytes')             # <<<<<<<<<<<<<<
  * 
  *         self.buffer = array.array('b', [0] * size)
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Encoder_buffer_minimum_size_is_3); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 120, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Encoder_buffer_minimum_size_is_3); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "rbfly/streams/_codec.pyx":140
+  /* "rbfly/streams/_codec.pyx":139
  *             # TODO: how this should fit into RbFlyBufferError and
  *             # AMQP*Error?
  *             raise ProtocolError(0x0e, 'Frame too large')             # <<<<<<<<<<<<<<
  * 
  *         return bp[:blen]
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_int_14, __pyx_kp_u_Frame_too_large); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_int_14, __pyx_kp_u_Frame_too_large); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "rbfly/streams/_codec.pyx":63
  *         self.data = b''
  * 
  *     def commands(self, chunk: bytes) -> tp.Iterator:  # [tuple[int, int]]:             # <<<<<<<<<<<<<<
@@ -9227,37 +9238,37 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_tuple__10 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
   __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":125
+  /* "rbfly/streams/_codec.pyx":124
  *         self.size = size
  * 
  *     def encode(self, data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *         """
  *         Encode RabbitMQ Streams protocol frame.
  */
-  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_size, __pyx_n_s_blen, __pyx_n_s_bp); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 125, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_size, __pyx_n_s_blen, __pyx_n_s_bp); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_encode, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 125, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_encode, 124, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 124, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":144
+  /* "rbfly/streams/_codec.pyx":143
  *         return bp[:blen]
  * 
  *     def encode_publish(             # <<<<<<<<<<<<<<
  *             self,
- *             publisher_id: int,
+ *             publisher_id: uint8_t,
  */
-  __pyx_tuple__14 = PyTuple_Pack(19, __pyx_n_s_self, __pyx_n_s_publisher_id, __pyx_n_s_amqp, __pyx_n_s_messages, __pyx_n_s_b, __pyx_n_s_buffer, __pyx_n_s_bp_hdr, __pyx_n_s_bp_msg, __pyx_n_s_offset, __pyx_n_s_encode_msg, __pyx_n_s_i, __pyx_n_s_count, __pyx_n_s_msg, __pyx_n_s_msg_size, __pyx_n_s_msg_len, __pyx_n_s_last_offset, __pyx_n_s_num_offset, __pyx_n_s_frame_size, __pyx_n_s_ex); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 144, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(19, __pyx_n_s_self, __pyx_n_s_publisher_id, __pyx_n_s_amqp, __pyx_n_s_messages, __pyx_n_s_b, __pyx_n_s_buffer, __pyx_n_s_bp_hdr, __pyx_n_s_bp_msg, __pyx_n_s_offset, __pyx_n_s_encode_msg, __pyx_n_s_i, __pyx_n_s_count, __pyx_n_s_msg, __pyx_n_s_msg_size, __pyx_n_s_msg_len, __pyx_n_s_last_offset, __pyx_n_s_num_offset, __pyx_n_s_frame_size, __pyx_n_s_ex); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 1, 19, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_encode_publish, 144, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 144, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 1, 19, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_encode_publish, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 143, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
   __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -9266,37 +9277,37 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":216
+  /* "rbfly/streams/_codec.pyx":215
  *         return count, buffer.buffer[:last_offset]
  * 
  * def decode_publish_confirm(data: bytes, start: int) -> tuple[int, object]:             # <<<<<<<<<<<<<<
  *     """
  *     Decode publisher id and published messages ids from confirmation data
  */
-  __pyx_tuple__18 = PyTuple_Pack(11, __pyx_n_s_data, __pyx_n_s_start, __pyx_n_s_b, __pyx_n_s_buffer, __pyx_n_s_bp, __pyx_n_s_offset, __pyx_n_s_hlen, __pyx_n_s_i, __pyx_n_s_n, __pyx_n_s_publisher_id, __pyx_n_s_publish_ids); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 216, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(11, __pyx_n_s_data, __pyx_n_s_start, __pyx_n_s_b, __pyx_n_s_buffer, __pyx_n_s_bp, __pyx_n_s_offset, __pyx_n_s_hlen, __pyx_n_s_i, __pyx_n_s_n, __pyx_n_s_publisher_id, __pyx_n_s_publish_ids); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_decode_publish_confirm, 216, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 216, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_decode_publish_confirm, 215, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 215, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":256
+  /* "rbfly/streams/_codec.pyx":255
  *     return publisher_id, publish_ids
  * 
  * def decode_messages(             # <<<<<<<<<<<<<<
  *         data: bytes,
  *         start: int,
  */
-  __pyx_tuple__20 = PyTuple_Pack(26, __pyx_n_s_data, __pyx_n_s_start, __pyx_n_s_offset_start, __pyx_n_s_queue, __pyx_n_s_amqp, __pyx_n_s_b, __pyx_n_s_buffer, __pyx_n_s_offset, __pyx_n_s_hlen, __pyx_n_s_bp, __pyx_n_s_magic_version, __pyx_n_s_chunk_type, __pyx_n_s_k_entry, __pyx_n_s_num_entries, __pyx_n_s_num_records, __pyx_n_s_chunk_crc, __pyx_n_s_calc_crc, __pyx_n_s_size, __pyx_n_s_data_size, __pyx_n_s_timestamp, __pyx_n_s_epoch, __pyx_n_s_chunk_first_offset, __pyx_n_s_current_offset, __pyx_n_s_msg, __pyx_n_s_decode_msg, __pyx_n_s_ex); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 256, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(26, __pyx_n_s_data, __pyx_n_s_start, __pyx_n_s_offset_start, __pyx_n_s_queue, __pyx_n_s_amqp, __pyx_n_s_b, __pyx_n_s_buffer, __pyx_n_s_offset, __pyx_n_s_hlen, __pyx_n_s_bp, __pyx_n_s_magic_version, __pyx_n_s_chunk_type, __pyx_n_s_k_entry, __pyx_n_s_num_entries, __pyx_n_s_num_records, __pyx_n_s_chunk_crc, __pyx_n_s_calc_crc, __pyx_n_s_size, __pyx_n_s_data_size, __pyx_n_s_timestamp, __pyx_n_s_epoch, __pyx_n_s_chunk_first_offset, __pyx_n_s_current_offset, __pyx_n_s_msg, __pyx_n_s_decode_msg, __pyx_n_s_ex); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_decode_messages, 256, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 256, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_rbfly_streams__codec_pyx, __pyx_n_s_decode_messages, 255, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 255, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -9500,15 +9511,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_ImportFunction(__pyx_t_1, "buffer_claim", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_claim, "char *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   if (__Pyx_ImportFunction(__pyx_t_1, "buffer_check_size", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_check_size, "char (struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rbfly.amqp._message"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_ImportFunction(__pyx_t_1, "c_encode_amqp", (void (**)(void))&__pyx_f_5rbfly_4amqp_8_message_c_encode_amqp, "Py_ssize_t (struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "c_decode_amqp", (void (**)(void))&__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp, "struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(struct __pyx_t_5rbfly_7_buffer_Buffer *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "c_decode_amqp", (void (**)(void))&__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp, "struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rbfly._codec"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_ImportFunction(__pyx_t_1, "unpack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint16, "uint16_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   if (__Pyx_ImportFunction(__pyx_t_1, "unpack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint32, "uint32_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   if (__Pyx_ImportFunction(__pyx_t_1, "unpack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint64, "uint64_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   if (__Pyx_ImportFunction(__pyx_t_1, "pack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint16, "void (char *, uint16_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -10008,72 +10019,72 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_12FrameDecoder_8__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FrameDecoder___setstate_cython, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "rbfly/streams/_codec.pyx":125
+  /* "rbfly/streams/_codec.pyx":124
  *         self.size = size
  * 
  *     def encode(self, data: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *         """
  *         Encode RabbitMQ Streams protocol frame.
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 125, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 125, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 125, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_12FrameEncoder_3encode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FrameEncoder_encode, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 125, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 124, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 124, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_12FrameEncoder_3encode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FrameEncoder_encode, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_5rbfly_7streams_6_codec_FrameEncoder->tp_dict, __pyx_n_s_encode, __pyx_t_4) < 0) __PYX_ERR(1, 125, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_5rbfly_7streams_6_codec_FrameEncoder->tp_dict, __pyx_n_s_encode, __pyx_t_4) < 0) __PYX_ERR(1, 124, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   PyType_Modified(__pyx_ptype_5rbfly_7streams_6_codec_FrameEncoder);
 
-  /* "rbfly/streams/_codec.pyx":144
+  /* "rbfly/streams/_codec.pyx":143
  *         return bp[:blen]
  * 
  *     def encode_publish(             # <<<<<<<<<<<<<<
  *             self,
- *             publisher_id: int,
+ *             publisher_id: uint8_t,
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 144, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "rbfly/streams/_codec.pyx":148
- *             publisher_id: int,
+  /* "rbfly/streams/_codec.pyx":147
+ *             publisher_id: uint8_t,
  *             *messages: MessageCtx,
  *             amqp: bool=True,             # <<<<<<<<<<<<<<
  *     ) -> tuple[int, bytes]:
  *         """
  */
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_amqp, Py_True) < 0) __PYX_ERR(1, 144, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_amqp, Py_True) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
 
-  /* "rbfly/streams/_codec.pyx":144
+  /* "rbfly/streams/_codec.pyx":143
  *         return bp[:blen]
  * 
  *     def encode_publish(             # <<<<<<<<<<<<<<
  *             self,
- *             publisher_id: int,
+ *             publisher_id: uint8_t,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 144, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_publisher_id, __pyx_n_s_int) < 0) __PYX_ERR(1, 144, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_amqp, __pyx_n_s_bool) < 0) __PYX_ERR(1, 144, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_messages, __pyx_n_s_MessageCtx) < 0) __PYX_ERR(1, 144, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_int_bytes) < 0) __PYX_ERR(1, 144, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_12FrameEncoder_5encode_publish, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FrameEncoder_encode_publish, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 144, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_publisher_id, __pyx_n_s_uint8_t) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_amqp, __pyx_n_s_bool) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_messages, __pyx_n_s_MessageCtx) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_int_bytes) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_12FrameEncoder_5encode_publish, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FrameEncoder_encode_publish, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_3, __pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_5rbfly_7streams_6_codec_FrameEncoder->tp_dict, __pyx_n_s_encode_publish, __pyx_t_3) < 0) __PYX_ERR(1, 144, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_5rbfly_7streams_6_codec_FrameEncoder->tp_dict, __pyx_n_s_encode_publish, __pyx_t_3) < 0) __PYX_ERR(1, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_5rbfly_7streams_6_codec_FrameEncoder);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -10090,53 +10101,53 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_12FrameEncoder_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FrameEncoder___setstate_cython, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "rbfly/streams/_codec.pyx":216
+  /* "rbfly/streams/_codec.pyx":215
  *         return count, buffer.buffer[:last_offset]
  * 
  * def decode_publish_confirm(data: bytes, start: int) -> tuple[int, object]:             # <<<<<<<<<<<<<<
  *     """
  *     Decode publisher id and published messages ids from confirmation data
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 216, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 216, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_start, __pyx_n_s_int) < 0) __PYX_ERR(1, 216, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_int_object) < 0) __PYX_ERR(1, 216, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_1decode_publish_confirm, 0, __pyx_n_s_decode_publish_confirm, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 216, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 215, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_start, __pyx_n_s_int) < 0) __PYX_ERR(1, 215, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_int_object) < 0) __PYX_ERR(1, 215, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_1decode_publish_confirm, 0, __pyx_n_s_decode_publish_confirm, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_publish_confirm, __pyx_t_2) < 0) __PYX_ERR(1, 216, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_publish_confirm, __pyx_t_2) < 0) __PYX_ERR(1, 215, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "rbfly/streams/_codec.pyx":256
+  /* "rbfly/streams/_codec.pyx":255
  *     return publisher_id, publish_ids
  * 
  * def decode_messages(             # <<<<<<<<<<<<<<
  *         data: bytes,
  *         start: int,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 256, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 256, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_start, __pyx_n_s_int) < 0) __PYX_ERR(1, 256, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_offset_start, __pyx_kp_s_tp_Optional_int) < 0) __PYX_ERR(1, 256, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_queue, __pyx_n_s_MessageQueue) < 0) __PYX_ERR(1, 256, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_amqp, __pyx_n_s_bool) < 0) __PYX_ERR(1, 256, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 256, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_3decode_messages, 0, __pyx_n_s_decode_messages, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 256, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_n_s_bytes) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_start, __pyx_n_s_int) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_offset_start, __pyx_kp_s_tp_Optional_int) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_queue, __pyx_n_s_MessageQueue) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_amqp, __pyx_n_s_bool) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_5rbfly_7streams_6_codec_3decode_messages, 0, __pyx_n_s_decode_messages, NULL, __pyx_n_s_rbfly_streams__codec, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_messages, __pyx_t_3) < 0) __PYX_ERR(1, 256, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_decode_messages, __pyx_t_3) < 0) __PYX_ERR(1, 255, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "rbfly/streams/_codec.pyx":1
  * #             # <<<<<<<<<<<<<<
  * # rbfly - a library for RabbitMQ Streams using Python asyncio
  * #
  */
@@ -13909,14 +13920,210 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntFromPy */
+static CYTHON_INLINE uint8_t __Pyx_PyInt_As_uint8_t(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const uint8_t neg_one = (uint8_t) -1, const_zero = (uint8_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if ((sizeof(uint8_t) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(uint8_t, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (uint8_t) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = __Pyx_PyLong_Digits(x);
+            switch (Py_SIZE(x)) {
+                case  0: return (uint8_t) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(uint8_t, digit, digits[0])
+                case 2:
+                    if ((8 * sizeof(uint8_t) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) >= 2 * PyLong_SHIFT)) {
+                            return (uint8_t) (((((uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
+                        }
+                    }
+                    break;
+                case 3:
+                    if ((8 * sizeof(uint8_t) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) >= 3 * PyLong_SHIFT)) {
+                            return (uint8_t) (((((((uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
+                        }
+                    }
+                    break;
+                case 4:
+                    if ((8 * sizeof(uint8_t) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT)) {
+                            return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
+                        }
+                    }
+                    break;
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (uint8_t) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if ((sizeof(uint8_t) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(uint8_t) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = __Pyx_PyLong_Digits(x);
+            switch (Py_SIZE(x)) {
+                case  0: return (uint8_t) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(uint8_t, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(uint8_t,  digit, +digits[0])
+                case -2:
+                    if ((8 * sizeof(uint8_t) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) - 1 > 2 * PyLong_SHIFT)) {
+                            return (uint8_t) (((uint8_t)-1)*(((((uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 2:
+                    if ((8 * sizeof(uint8_t) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) - 1 > 2 * PyLong_SHIFT)) {
+                            return (uint8_t) ((((((uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case -3:
+                    if ((8 * sizeof(uint8_t) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) - 1 > 3 * PyLong_SHIFT)) {
+                            return (uint8_t) (((uint8_t)-1)*(((((((uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 3:
+                    if ((8 * sizeof(uint8_t) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) - 1 > 3 * PyLong_SHIFT)) {
+                            return (uint8_t) ((((((((uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case -4:
+                    if ((8 * sizeof(uint8_t) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) - 1 > 4 * PyLong_SHIFT)) {
+                            return (uint8_t) (((uint8_t)-1)*(((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 4:
+                    if ((8 * sizeof(uint8_t) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if ((8 * sizeof(uint8_t) - 1 > 4 * PyLong_SHIFT)) {
+                            return (uint8_t) ((((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+            }
+#endif
+            if ((sizeof(uint8_t) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(uint8_t) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
+            PyErr_SetString(PyExc_RuntimeError,
+                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
+#else
+            uint8_t val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+ #if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+ #endif
+            if (likely(v)) {
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                int ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                              bytes, sizeof(val),
+                                              is_little, !is_unsigned);
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+#endif
+            return (uint8_t) -1;
+        }
+    } else {
+        uint8_t val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (uint8_t) -1;
+        val = __Pyx_PyInt_As_uint8_t(tmp);
+        Py_DECREF(tmp);
+        return val;
+    }
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to uint8_t");
+    return (uint8_t) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to uint8_t");
+    return (uint8_t) -1;
+}
+
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint16_t(uint16_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint16_t neg_one = (uint16_t) -1, const_zero = (uint16_t) 0;
@@ -14182,210 +14389,14 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint16_t");
     return (uint16_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const char neg_one = (char) -1, const_zero = (char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if ((sizeof(char) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(char, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (char) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (char) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(char, digit, digits[0])
-                case 2:
-                    if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) >= 2 * PyLong_SHIFT)) {
-                            return (char) (((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) >= 3 * PyLong_SHIFT)) {
-                            return (char) (((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) >= 4 * PyLong_SHIFT)) {
-                            return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (char) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if ((sizeof(char) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if ((sizeof(char) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = __Pyx_PyLong_Digits(x);
-            switch (Py_SIZE(x)) {
-                case  0: return (char) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(char, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(char,  digit, +digits[0])
-                case -2:
-                    if ((8 * sizeof(char) - 1 > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
-                            return (char) (((char)-1)*(((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
-                            return (char) ((((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
-                            return (char) (((char)-1)*(((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
-                            return (char) ((((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
-                            return (char) (((char)-1)*(((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
-                        if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                            __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
-                            return (char) ((((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if ((sizeof(char) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if ((sizeof(char) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if (CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available, cannot convert large numbers");
-#else
-            char val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (char) -1;
-        }
-    } else {
-        char val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (char) -1;
-        val = __Pyx_PyInt_As_char(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to char");
-    return (char) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to char");
-    return (char) -1;
-}
-
-/* CIntFromPy */
 static CYTHON_INLINE uint64_t __Pyx_PyInt_As_uint64_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint64_t neg_one = (uint64_t) -1, const_zero = (uint64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `rbfly-0.7.1/rbfly/streams/_codec.pyi` & `rbfly-0.7.2/rbfly/streams/_codec.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/_codec.pyx` & `rbfly-0.7.2/rbfly/streams/_codec.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 logger = logging.getLogger(__name__)
 
 cdef enum:
     LEN_FRAME_SIZE = sizeof(uint32_t)
 
 ctypedef Py_ssize_t (*t_func_encode)(Buffer*, object) except -1
-ctypedef MessageCtx (*t_func_decode)(Buffer*)
+ctypedef MessageCtx (*t_func_decode)(Buffer*, Py_ssize_t)
 
 cdef class FrameDecoder:
     """
     RabbitMQ Streams protocol frame decoder.
 
     :var data: Buffer receiving data.
     """
@@ -107,15 +107,14 @@
         self.data = self.data[offset:]
 
 cdef class FrameEncoder:
     """
     RabbitMQ Streams protocol frame encoder.
     """
     cdef array.array buffer
-    cdef char *mv
     cdef int size
 
     def __cinit__(self, int size):
         # check encoding method if this changes
         if size < 32:
             raise ValueError('Encoder buffer minimum size is 32 bytes')
 
@@ -139,15 +138,15 @@
             # AMQP*Error?
             raise ProtocolError(0x0e, 'Frame too large')
 
         return bp[:blen]
 
     def encode_publish(
             self,
-            publisher_id: int,
+            publisher_id: uint8_t,
             *messages: MessageCtx,
             amqp: bool=True,
     ) -> tuple[int, bytes]:
         """
         Encode frame with publish RabbitMQ Streams protocol command.
 
         :param publisher_id: Publisher id.
@@ -353,15 +352,15 @@
     for k_entry in range(num_entries):
         bp = buffer_claim(buffer, sizeof(uint32_t))
         size = unpack_uint32(bp)
         if buffer_check_size(buffer, size):
             current_offset = chunk_first_offset + k_entry
             if offset_start is None or current_offset >= offset_start:
                 try:
-                    msg = decode_msg(buffer)
+                    msg = decode_msg(buffer, size)
                     msg.stream_offset = current_offset
                     msg.stream_timestamp = <double> timestamp / 1000
                 except AMQPDecoderError as ex:
                     logger.warning('cannot decode amqp message: {}'.format(ex))
                 else:
                     queue.put(msg)
             else:
@@ -382,14 +381,17 @@
 cdef inline Py_ssize_t encode_body(Buffer *buffer, object message) except -1:
     cdef:
         object body = message.body
         Py_ssize_t size = len(body)
         char *bp
 
     bp = buffer_claim(buffer, size)
-    memcpy(bp, <char*> body, size)
+    memcpy(bp, <uint8_t*> body, size)
     return size
 
-cdef inline MessageCtx decode_body(Buffer *buffer):
-    return MessageCtx(buffer.buffer[buffer.offset:buffer.size])
+cdef inline MessageCtx decode_body(Buffer *buffer, Py_ssize_t size):
+    cdef:
+        char *bp = buffer_claim(buffer, size)
+
+    return MessageCtx(bp[:size])
 
 # vim: sw=4:et:ai
```

### Comparing `rbfly-0.7.1/rbfly/streams/_mqueue.c` & `rbfly-0.7.2/rbfly/streams/_mqueue.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/_mqueue.pyi` & `rbfly-0.7.2/rbfly/streams/_mqueue.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/_mqueue.pyx` & `rbfly-0.7.2/rbfly/streams/_mqueue.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/client.py` & `rbfly-0.7.2/rbfly/streams/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,23 +126,19 @@
 
         for publisher in self._publishers.values():
             await self._create_publisher(
                 protocol, publisher.stream, publisher._id, publisher.name
             )
 
         for subscriber in self._subscribers.values():
-            msg = subscriber._message
-            proto_offset = subscriber._offset if msg is None \
-                else Offset.offset(msg.stream_offset + 1)
-
             await self._subscribe(
                 protocol,
                 subscriber._stream,
                 subscriber._subscription_id,
-                proto_offset,
+                subscriber._next_message_offset(),
                 subscriber._amqp
             )
 
     async def _disconnect(self, protocol: RabbitMQStreamsProtocol) -> None:
         await protocol.send_close()
         logger.info(
             'rabbitmq streams client disconnected: {}'.format(self._cinfo)
@@ -266,15 +262,16 @@
         """
         Subscribe to the stream and iterate over messages.
 
         :param stream: Name of RabbitMQ stream to subscribe to.
         :param offset: RabbitMQ Streams offset specification.
         :param timeout: Raise timeout error if no message received within
             specified time (in seconds).
-        :param amqp: Messages are in AMQP 1.0 format if true. Otherwise no AMQP decoding.
+        :param amqp: Messages are in AMQP 1.0 format if true. Otherwise no
+            AMQP decoding.
         """
         self._subscription_id += 1
         sid = self._subscription_id
 
         protocol = await self.get_protocol()
         proto_offset = await self._get_offset_reference(stream, offset)
         await self._subscribe(protocol, stream, sid, proto_offset, amqp)
@@ -344,17 +341,19 @@
         subscription_id: int,
         offset: Offset,
         amqp: bool,
     ) -> None:
         """
         Subscribe to RabbitMQ stream.
 
+        :param protocol: RabbitMQ Streams protocol instance.
         :param stream: RabbitMQ stream name.
         :param subscription_id: RabbitMQ stream subscription id.
         :param offset: RabbitMQ Streams offset specification.
+        :param amqp: Parse message data with AMQP parser if true.
         """
         await protocol.subscribe(stream, subscription_id, offset, amqp)
         logger.info(
             '(re)subscribed to stream, name={}, subscription id={},'
             ' offset={}'.format(stream, subscription_id, offset) 
         )
```

### Comparing `rbfly-0.7.1/rbfly/streams/codec.py` & `rbfly-0.7.2/rbfly/streams/codec.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/const.py` & `rbfly-0.7.2/rbfly/streams/const.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/error.py` & `rbfly-0.7.2/rbfly/streams/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/offset.py` & `rbfly-0.7.2/rbfly/streams/offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/protocol.py` & `rbfly-0.7.2/rbfly/streams/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -339,15 +339,14 @@
         """
         sid = subscription_id
         value = tp.cast(
             tp.Optional[int],
             offset.value if offset.type == OffsetType.OFFSET else None
         )
 
-        task = self._loop.create_future()
         data = codec.encode_subscribe(sid, stream, offset, const.INITIAL_CREDIT)
 
         queue = MessageQueue(const.INITIAL_CREDIT, const.QUEUE_MAX_SIZE)
         self._subscriptions[sid] = ReceivedMessages(queue, value, amqp)
         return await self.send_request(const.KEY_SUBSCRIBE, data)
 
     async def read_stream(self, subscription_id: int) -> deque[MessageCtx]:
@@ -363,15 +362,15 @@
         # process_message_delivery method; it might not happen there if
         # message queue is full, so check if it needs to be updated before
         # we start waiting for new messages
         if queue.empty():
             self.renew_credit(subscription_id, queue)
 
         await queue.wait()
-        self._subscriptions[subscription_id] = dtc.replace(rm, offset=None)
+        self._update_subscription(subscription_id, rm, offset=None)
         return queue.data
 
     async def unsubscribe(self, subscription_id: int) -> tp.Any:
         """
         Unsubscribe from RabbitMQ stream using the subscription id.
 
         :param subscription_id: Subscription id.
@@ -552,18 +551,22 @@
         self._published_messages.clear()
         self._subscriptions.clear()
 
         logger.info('connection is closed')
 
     def abort(self) -> None:
         """
-        Close Asyncio transport used by the protocol.
+        Close asyncio transport used by the protocol.
         """
         if not self.transport.empty:
-            self.transport.value.abort()
+            transport = self.transport.value
+            transport.abort()
+
+            if __debug__:
+                logger.debug('transport closed')
 
     def timestamp_callback(self) -> None:
         """
         Callback to watch timing of RabbitMQ Streams broker last response.
         """
         heartbeat = self.heartbeat
         delta = self._loop.time() - self._timestamp
@@ -681,15 +684,15 @@
                 'request sent, key=0x{:02x}, correlation_id={}'
                 .format(key, correlation_id)
             )
         return await task
 
     def create_waiter(self, key: int) -> asyncio.Future[None]:
         """
-        Create Asyncio future to wait for specific RabbitMQ Streams
+        Create asyncio future to wait for specific RabbitMQ Streams
         request.
 
         :param key: Key of request to wait for.
         """
         assert key not in self._waiters
         task = self._loop.create_future()
         self._waiters[key] = task
@@ -833,8 +836,36 @@
         logger.info(
             'tune frame sent: frame size={}, heartbeat={}'
             .format(self.frame_size, self.heartbeat)
         )
 
         assert const.KEY_TUNE not in self._waiters
 
+    #
+    # utility methods
+    #
+    def _update_subscription(
+            self,
+            subscription_id: int,
+            rm: ReceivedMessages,
+            *,
+            offset: int | None,
+    ) -> None:
+        """
+        Update subscription data.
+
+        If subscription does not exist then raise connection error. This is
+        the most likely reason for an invalid subscription.
+        """
+        data = self._subscriptions
+        if subscription_id in data:
+            data[subscription_id] = dtc.replace(rm, offset=offset)
+        else:
+            if __debug__:
+                logger.debug(
+                    'subscription no longer valid, id={}'.format(
+                        subscription_id
+                    )
+                )
+            raise ConnectionError('subscription no longer valid')
+
 # vim: sw=4:et:ai
```

### Comparing `rbfly-0.7.1/rbfly/streams/types.py` & `rbfly-0.7.2/rbfly/streams/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/streams/util.py` & `rbfly-0.7.2/rbfly/streams/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/tests/__init__.py` & `rbfly-0.7.2/rbfly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/tests/amqp/__init__.py` & `rbfly-0.7.2/rbfly/tests/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/tests/amqp/test_message.py` & `rbfly-0.7.2/rbfly/tests/amqp/test_message.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/tests/streams/__init__.py` & `rbfly-0.7.2/rbfly/tests/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/tests/streams/test_client.py` & `rbfly-0.7.2/rbfly/tests/streams/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,25 @@
 """
 
 import asyncio
 import copy
 import inspect
 import operator
 import typing as tp
+from collections import deque
 from collections.abc import AsyncIterator, AsyncGenerator
 from functools import partial
 
 from rbfly.amqp import MessageCtx
 from rbfly.error import RbFlyError
 from rbfly.streams.client import Scheme, StreamsClient, streams_client, \
     connection
 from rbfly.streams._client import PublisherTrait, Publisher, \
     PublisherBatchFast, PublisherBatchLimit, PublisherBin, \
-    PublisherBinBatch, stream_messsage_ctx
+    PublisherBinBatch, Subscriber, stream_messsage_ctx
 from rbfly.streams.offset import Offset, OffsetType
 from rbfly.streams.protocol import ProtocolError
 
 import pytest
 from unittest import mock
 
 TEST_CLIENT_URI = [
@@ -378,14 +379,61 @@
     ]
     assert call_recorder == expected
 
     # last message id is increased by 2
     assert publisher.message_id == 13
     assert publisher._data == []
 
+def test_subscriber_next_offset_initial() -> None:
+    """
+    Test next offset of a subscriber using initial offset.
+    """
+    subscriber = Subscriber(
+        mock.MagicMock(),
+        'a-stream',
+        1,
+        Offset.NEXT,
+        1,
+        True
+    )
+    assert subscriber._next_message_offset() == Offset.NEXT
+
+def test_subscriber_next_offset_non_empty() -> None:
+    """
+    Test next offset of a subscriber with non-empty queue.
+    """
+    subscriber = Subscriber(
+        mock.MagicMock(),
+        'a-stream',
+        1,
+        Offset.NEXT,
+        1,
+        True
+    )
+    subscriber._messages = deque([])
+    subscriber._messages.append(MessageCtx('abc', stream_offset=10))
+    subscriber._messages.append(MessageCtx('abc', stream_offset=11))
+    assert subscriber._next_message_offset() == Offset.offset(12)
+
+def test_subscriber_next_offset_empty() -> None:
+    """
+    Test next offset of a subscriber with empty queue.
+    """
+    subscriber = Subscriber(
+        mock.MagicMock(),
+        'a-stream',
+        1,
+        Offset.NEXT,
+        1,
+        True
+    )
+    subscriber._messages = deque([])
+    subscriber._last_message = MessageCtx('abc', stream_offset=10)
+    assert subscriber._next_message_offset() == Offset.offset(11)
+
 def test_connection_coroutine() -> None:
     """
     Test if connection decorator returns coroutine function.
     """
     # pylint: disable=invalid-name
 
     async def f() -> None:
```

### Comparing `rbfly-0.7.1/rbfly/tests/streams/test_codec.py` & `rbfly-0.7.2/rbfly/tests/streams/test_codec.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,14 +75,53 @@
     (
         DELIVERED_MSG_DATA_2,
         975,
         [MessageCtx(b'0000000065', stream_offset=975, stream_timestamp=1636900128.714)]
     ),
 )
 
+DELIVERED_DATA_BIN = (  # type: ignore
+    (
+        DELIVERED_MSG_DATA_1,
+        None,
+        [
+            MessageCtx(
+                b'\x00Su\xa0\n3210000123',
+                stream_offset=0,
+                stream_timestamp=1636891987.216
+            )
+        ]
+    ),
+    (
+        DELIVERED_MSG_DATA_1,
+        0,
+        [
+            MessageCtx(
+                b'\x00Su\xa0\n3210000123',
+                stream_offset=0,
+                stream_timestamp=1636891987.216
+            )
+        ]
+        ),
+    (DELIVERED_MSG_DATA_1, 1, []),  # request offset > 0
+    (
+        DELIVERED_MSG_DATA_2,
+        974,
+        [
+            MessageCtx(b'\x00Su\xa0\n0000000064', stream_offset=974, stream_timestamp=1636900128.714),
+            MessageCtx(b'\x00Su\xa0\n0000000065', stream_offset=975, stream_timestamp=1636900128.714),
+        ],
+    ),
+    (
+        DELIVERED_MSG_DATA_2,
+        975,
+        [MessageCtx(b'\x00Su\xa0\n0000000065', stream_offset=975, stream_timestamp=1636900128.714)]
+    ),
+)
+
 OFFSET_DATA = (
     (Offset.FIRST, b'\x00\x01'),
     (Offset.LAST, b'\x00\x02'),
     (Offset.NEXT, b'\x00\x03'),
     (Offset.offset(1024), b'\x00\x04\x00\x00\x00\x00\x00\x00\x04\x00'),
 
     # timestamp is encoded in milliseconds
@@ -204,15 +243,15 @@
     encoder = codec.FrameEncoder(1024)
     messages = [
         MessageCtx(b'123', stream_publish_id=10),
         MessageCtx(b'9876', stream_publish_id=11)
     ]
     count, data = encoder.encode_publish(5, *messages)
 
-    expected = b'\x00\x00\x002' \
+    expected = b'\x00\x00\x00\x32' \
         + b'\x00\x02\x00\x01\x05\x00\x00\x00\x02' \
         + b'\x00\x00\x00\x00\x00\x00\x00\x0a\x00\x00\x00\x08\x00Su\xa0\x03123' \
         + b'\x00\x00\x00\x00\x00\x00\x00\x0b\x00\x00\x00\x09\x00Su\xa0\x049876'
 
     assert count == 2
     assert data == expected
 
@@ -323,15 +362,47 @@
         offset: tp.Optional[int],
         expected: list[MessageCtx]
 ) -> None:
     """
     Test decoding delivered messages.
     """
     result = MessageQueue(2, 16)
-    codec.decode_messages(data, 0, offset, result, True)
+    codec.decode_messages(data, 0, offset, result, amqp=True)
+    assert list(result.data) == expected
+
+def test_encode_publish_bin_multi() -> None:
+    """
+    Test encoding multiple published messages, no AMQP 1.0 format.
+    """
+    encoder = codec.FrameEncoder(1024)
+    messages = [
+        MessageCtx(b'123', stream_publish_id=10),
+        MessageCtx(b'9876', stream_publish_id=11),
+    ]
+    count, data = encoder.encode_publish(5, *messages, amqp=False)
+
+    expected = b'\x00\x00\x00(' \
+        + b'\x00\x02\x00\x01\x05\x00\x00\x00\x02' \
+        + b'\x00\x00\x00\x00\x00\x00\x00\x0a\x00\x00\x00\x03123' \
+        + b'\x00\x00\x00\x00\x00\x00\x00\x0b\x00\x00\x00\x049876'
+
+    assert count == 2
+    assert data == expected
+
+@pytest.mark.parametrize('data, offset, expected', DELIVERED_DATA_BIN)
+def test_decode_delivered_message_bin(
+        data: bytes,
+        offset: tp.Optional[int],
+        expected: list[MessageCtx]
+) -> None:
+    """
+    Test decoding delivered messages, no AMQP 1.0 format.
+    """
+    result = MessageQueue(2, 16)
+    codec.decode_messages(data, 0, offset, result, amqp=False)
     assert list(result.data) == expected
 
 @pytest.mark.parametrize('offset, expected', OFFSET_DATA)
 def test_encode_offset(offset: Offset, expected: bytes) -> None:
     """
     Test encoding RabbitMQ Streams offset specification.
     """
```

### Comparing `rbfly-0.7.1/rbfly/tests/streams/test_mqueue.py` & `rbfly-0.7.2/rbfly/tests/streams/test_mqueue.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/tests/streams/test_offset.py` & `rbfly-0.7.2/rbfly/tests/streams/test_offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/tests/test_util.py` & `rbfly-0.7.2/rbfly/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/types.py` & `rbfly-0.7.2/rbfly/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly/util.py` & `rbfly-0.7.2/rbfly/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/rbfly.egg-info/PKG-INFO` & `rbfly-0.7.2/rbfly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.7.1
+Version: 0.7.2
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
```

### Comparing `rbfly-0.7.1/rbfly.egg-info/SOURCES.txt` & `rbfly-0.7.2/rbfly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbfly-0.7.1/setup.cfg` & `rbfly-0.7.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rbfly
-version = 0.7.1
+version = 0.7.2
 author = Artur Wroblewski
 author_email = wrobell@riseup.net
 license = GPLv3+
 description = RbFly - a library for RabbitMQ Streams using Python asyncio
 long_description = file: README
 long_description_content_type = text/x-rst
 url = https://wrobell.dcmod.org/rbfly/
@@ -29,30 +29,30 @@
 	*.pyx
 	*.pxd
 	*.h
 
 [options.extras_require]
 tests = 
 	cython-lint
-	mypy == 1.3.0
+	mypy == 1.4.1
 	bandit
 	toml  # required by bandit, not needed when using Python 3.11?
 	pika  # required for integration tests
 	pylint
 	pytest-cov
 	pytest-timeout
 	pytest-asyncio
 	pytest-lazy-fixture
 	uvloop
 	types-pkg-resources
 	types-setuptools
 performance = 
 	msgpack
 	aiokafka == 0.8.0
-	rstream == 0.7.0
+	rstream == 0.10.1
 
 [tool:pytest]
 addopts = --cov rbfly --cov-report=term-missing --cov-fail-under=71
 
 [tool:coverage:report]
 show_missing = 1
 partial_branches = 1
```

### Comparing `rbfly-0.7.1/setup.py` & `rbfly-0.7.2/setup.py`

 * *Files identical despite different names*

