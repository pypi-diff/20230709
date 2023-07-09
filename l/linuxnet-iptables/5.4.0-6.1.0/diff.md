# Comparing `tmp/linuxnet-iptables-5.4.0.tar.gz` & `tmp/linuxnet-iptables-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxnet-iptables-5.4.0.tar", last modified: Mon Jun 19 04:01:18 2023, max compression
+gzip compressed data, was "linuxnet-iptables-6.1.0.tar", last modified: Sun Jul  9 21:00:05 2023, max compression
```

## Comparing `linuxnet-iptables-5.4.0.tar` & `linuxnet-iptables-6.1.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/
--rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)     2943 2023-06-19 03:07:11.000000 linuxnet-iptables-5.4.0/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-5.4.0/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/README.md
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.338386 linuxnet-iptables-5.4.0/docs/
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-5.4.0/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/docs/chain.rst
--rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-5.4.0/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/exception.rst
--rw-r--r--   0 panos     (1001) users      (100)     8374 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/docs/iptables_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     3176 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/match-example.py
--rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/docs/match.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.341386 linuxnet-iptables-5.4.0/docs/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 03:00:51.000000 linuxnet-iptables-5.4.0/docs/matches/addrtypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/commentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-5.4.0/docs/matches/connmarkmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/conntrackmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/icmpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-5.4.0/docs/matches/limitmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/markmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/ownermatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/docs/matches/packetmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/packettypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/statematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1492 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/tcpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/tcpmssmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/ttlmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/matches/udpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/docs/rule.rst
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-5.4.0/docs/table.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/target-example.py
--rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/docs/target.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.343387 linuxnet-iptables-5.4.0/docs/targets/
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/chaintarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/connmarktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/dnattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/logtarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/marktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/masqueradetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/docs/targets/notracktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/rejecttarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/snattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/docs/targets/tracetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/docs/targets/ttltarget.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.343387 linuxnet-iptables-5.4.0/linuxnet/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.344386 linuxnet-iptables-5.4.0/linuxnet/iptables/
--rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    25234 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/chain.py
--rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/extension.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.346387 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1339 2023-06-19 03:00:49.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     5239 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/addrtypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     2889 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/commentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2271 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/connmarkmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5226 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/conntrackmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9769 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/icmpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4667 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/limitmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3852 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/markmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    14678 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/match.py
--rw-r--r--   0 panos     (1001) users      (100)     7798 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ownermatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7343 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packetmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2844 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packettypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     3155 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/statematch.py
--rw-r--r--   0 panos     (1001) users      (100)    10665 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3833 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmssmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4322 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ttlmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2724 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/udpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5782 2023-06-19 03:00:49.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/matches/util.py
--rw-r--r--   0 panos     (1001) users      (100)      918 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/parsing.py
--rw-r--r--   0 panos     (1001) users      (100)    16442 2023-03-01 20:08:53.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/rule.py
--rw-r--r--   0 panos     (1001) users      (100)    29087 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/table.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.348387 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/
--rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/connmarktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/logtarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/marktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/masqueradetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/nattarget.py
--rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 03:00:49.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/notracktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/rejecttarget.py
--rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/target.py
--rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/tracetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-5.4.0/linuxnet/iptables/targets/ttltarget.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     2699 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-06-19 04:01:18.000000 linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/top_level.txt
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/setup.cfg
--rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-5.4.0/setup.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-19 04:01:18.349387 linuxnet-iptables-5.4.0/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.4.0/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    61555 2023-06-19 03:00:50.000000 linuxnet-iptables-5.4.0/tests/iptables_test.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/
+-rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)     3549 2023-07-09 20:53:09.000000 linuxnet-iptables-6.1.0/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-6.1.0/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.589427 linuxnet-iptables-6.1.0/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-6.1.0/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/docs/chain.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-6.1.0/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/exception.rst
+-rw-r--r--   0 panos     (1001) users      (100)     7952 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/docs/iptables_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3047 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/docs/match-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/docs/match.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.591427 linuxnet-iptables-6.1.0/docs/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/docs/matches/addrtypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/commentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-6.1.0/docs/matches/connmarkmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/conntrackmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/icmpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-6.1.0/docs/matches/limitmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/markmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/ownermatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/docs/matches/packetmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/packettypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/statematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1746 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/docs/matches/tcpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/tcpmssmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/ttlmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/udpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/docs/rule.rst
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-6.1.0/docs/table.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/target-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/docs/target.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.593427 linuxnet-iptables-6.1.0/docs/targets/
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/chaintarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/connmarktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/dnattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/logtarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/marktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/masqueradetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-6.1.0/docs/targets/notracktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/rejecttarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/snattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-6.1.0/docs/targets/tracetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/ttltarget.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.593427 linuxnet-iptables-6.1.0/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.594427 linuxnet-iptables-6.1.0/linuxnet/iptables/
+-rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    27815 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/chain.py
+-rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.598427 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1339 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     4978 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/addrtypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2879 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/commentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2285 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/connmarkmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5113 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/conntrackmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9761 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/icmpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4559 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/limitmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3872 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/markmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    16427 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/match.py
+-rw-r--r--   0 panos     (1001) users      (100)     7640 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ownermatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     7077 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packetmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2827 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packettypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3167 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/statematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    11625 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3776 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmssmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4317 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ttlmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2597 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/udpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5782 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/util.py
+-rw-r--r--   0 panos     (1001) users      (100)      918 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/parsing.py
+-rw-r--r--   0 panos     (1001) users      (100)    17490 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/rule.py
+-rw-r--r--   0 panos     (1001) users      (100)    29276 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/table.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.600427 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/
+-rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/connmarktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/logtarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/marktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/masqueradetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/nattarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/notracktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/rejecttarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/target.py
+-rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/tracetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/ttltarget.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.600427 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     2699 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-6.1.0/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    65961 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/tests/iptables_test.py
```

### Comparing `linuxnet-iptables-5.4.0/.pylintrc` & `linuxnet-iptables-6.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/CHANGELOG.md` & `linuxnet-iptables-6.1.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 Change Log
 ==========
 
+6.1.0 (2023-07-09)
+------------------
+
+- this version maintains user API backwards-compatibility;
+  however the major version was changed because the Match/Criterion
+  implementation was updated in a way that breaks
+  backwards-compatibility with out-of-tree Match subclasses
+
+- the Chain and ChainRule classes are now iterable
+
+- added ability to zero the packet/byte counters of individual rules
+
+- the Chain.iter_rules() can now return rules that match a number of
+  conditions: have a chain as a target, have a specific match, etc.
+
+- added support for TCP option matching (--tcp-option) to TcpMatch
+
+
 5.4.0 (2023-06-18)
 ------------------
 
 - added AddressTypeMatch class to support the 'addrtype' match
 - added Chain.has_rules() method
 
 5.3.0 (2023-06-04)
```

### Comparing `linuxnet-iptables-5.4.0/LICENSE` & `linuxnet-iptables-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/Makefile` & `linuxnet-iptables-6.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/PKG-INFO` & `linuxnet-iptables-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.4.0
+Version: 6.1.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-5.4.0/README.md` & `linuxnet-iptables-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/Makefile` & `linuxnet-iptables-6.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/chain.rst` & `linuxnet-iptables-6.1.0/docs/chain.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/conf.py` & `linuxnet-iptables-6.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/exception.rst` & `linuxnet-iptables-6.1.0/docs/exception.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/extensibility.rst` & `linuxnet-iptables-6.1.0/docs/extensibility.rst`

 * *Files 4% similar despite different names*

```diff
@@ -57,25 +57,19 @@
 
 
 Adding a Match subclass
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 A new :class:`Match` subclass **must** implement the following methods:
 
-#. :meth:`to_iptables_args`: this method should return the **iptables(8)**
-   arguments for the match. In our example, the return value might look
-   like this::
+#. :meth:`get_match_name`: this method returns the **iptables(8)** match
+   extension name
 
-      ['-m', 'tcpmss', '--mss', '500']
-  
-   if the :class:`MssCriterion` value was set to ``500``.
-
-   Notice the use of the :meth:`Match.build_iptables_args` method; this
-   is a helper method that will generate an empty list if none of
-   the criteria in its argument list have been set.
+#. :meth:`get_criteria`: this method returns an iterable with the
+   new match's criteria
 
 #. :meth:`parse`: this is a classmethod that takes a single argument of type
    :class:`MatchParser` and returns an instance of the new subclass.
    This method is responsible for parsing the ``iptables -Lxnv`` output
    for this match.  Notice the use of the ``-Lxnv`` options when
    implementing this method.
 
@@ -86,18 +80,14 @@
    the match parsing process.
 
 #. One or more methods returning instances of the match-specific criteria.
    In the example, the relevant method is :meth:`TcpmssMatch.mss()`
    (the :class:`TcpmssMatch` supports a single criterion)
    which returns an instance of the :class:`MssCriterion` class.
 
-The new subclass **should** implement the special :meth:`__eq__`
-method; two :class:`Match` objects should compare equal if they are
-instances of the same :class:`Match` subclass and their criteria are equal.
-
 Finally, the new subclass **must** be registered with the :class:`MatchParser`
 class by invoking the method :meth:`MatchParser.register_class`, and specifying
 the keyword in the **iptables(8)** output that identifies the particular
 match (in this example, that keyword is ``tcpmss``)
 
 
 Adding a Criterion subclass
@@ -200,14 +190,15 @@
 Objects of subclasses of :class:`Criterion` are never directly instantiated
 by the user; they are instantiated
 as needed by the :class:`Match` subclasses.
 
 .. autoclass:: Criterion
     :members:
     :member-order: bysource
+    :private-members: to_iptables_args, _crit_iptables_args
 
 
 Target
 ~~~~~~
 
 .. autoclass:: Target
     :members:
```

### Comparing `linuxnet-iptables-5.4.0/docs/index.rst` & `linuxnet-iptables-6.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/iptables_api.rst` & `linuxnet-iptables-6.1.0/docs/iptables_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/match-example.py` & `linuxnet-iptables-6.1.0/docs/match-example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2021-2023, Panagiotis Tsirigotis
 
 """
 Example module implementing matching against the TCP MSS
 """
 
 from typing import List, Optional, Tuple
+
 from linuxnet.iptables.extension import (
         Match,
         Criterion,
         MatchParser,
         IptablesError)
 
 class TcpmssMatch(Match):
@@ -16,29 +17,32 @@
     """
     def __init__(self):
         """This match uses a single criterion of type MssCritetion defined
         below
         """
         self.__mss_crit = None
 
-    def __eq__(self, other):
-        return isinstance(other, TcpmssMatch) and self.mss() == other.mss()
+    @staticmethod
+    def get_match_name():
+        """Returns the match extension name
+        """
+        return 'tcpmss'
+
+    def get_criteria(self):
+        """Returns the tcpmss criteria.
+        """
+        return (self.__mss_crit,)
 
     def mss(self) -> 'MssCriterion':
         """Match against the MSS field of the TCP header
         """
         if self.__mss_crit is None:
             self.__mss_crit = MssCriterion(self)
         return self.__mss_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('tcpmss', [self.__mss_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse tcpmss; example::
 
             tcpmss match !10:20
 
         The 'tcpmss' field has already been consumed by the parser.
@@ -80,16 +84,14 @@
     def equals(self, mssval: int, endval: Optional[int] =None) -> Match:
         """Check for equality against ``mssval``, or range equality
         if ``endval`` is present.
 
         :param mssval: the MSS value
         :param endval: range of MSS values from ``mssval`` to this value
         """
-        if mssval is None:
-            raise IptablesError('mssval is None')
         self.__mssval = mssval
         if endval is not None and endval < mssval:
             raise IptablesError('bad range: endval < mssval')
         self.__endval = endval
         return self._set_polarity(True)
 
     def _crit_iptables_args(self) -> List[str]:
```

### Comparing `linuxnet-iptables-5.4.0/docs/match.rst` & `linuxnet-iptables-6.1.0/docs/match.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/addrtypematch.rst` & `linuxnet-iptables-6.1.0/docs/matches/addrtypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/commentmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/commentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/connmarkmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/connmarkmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/conntrackmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/conntrackmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/icmpmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/icmpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/limitmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/limitmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/markmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/markmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/ownermatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/ownermatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/packetmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/packetmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/packettypematch.rst` & `linuxnet-iptables-6.1.0/docs/matches/packettypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/statematch.rst` & `linuxnet-iptables-6.1.0/docs/matches/statematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/tcpmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/tcpmatch.rst`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 ~~~~~~~~~~~~~~~~~
 
 .. autoclass:: TcpFlagsCriterion
     :class-doc-from: class
     :inherited-members:
     :member-order: bysource
 
+.. autoclass:: TcpFlag
+    :class-doc-from: class
+    :members:
+    :member-order: bysource
+
 -------
 
 .. _source_port_criterion:
 
 SourcePortCriterion
 ~~~~~~~~~~~~~~~~~~~
 
@@ -58,7 +63,16 @@
 ~~~~~~~~~~~~~~~~~
 
 .. autoclass:: DestPortCriterion
     :class-doc-from: class
     :inherited-members:
     :member-order: bysource
 
+-------
+
+TcpOptionCriterion
+~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: TcpOptionCriterion
+    :class-doc-from: class
+    :inherited-members:
+    :member-order: bysource
```

### Comparing `linuxnet-iptables-5.4.0/docs/matches/tcpmssmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/tcpmssmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/ttlmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/ttlmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/matches/udpmatch.rst` & `linuxnet-iptables-6.1.0/docs/matches/udpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/rule.rst` & `linuxnet-iptables-6.1.0/docs/rule.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/table.rst` & `linuxnet-iptables-6.1.0/docs/table.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/target-example.py` & `linuxnet-iptables-6.1.0/docs/target-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/target.rst` & `linuxnet-iptables-6.1.0/docs/target.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/chaintarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/chaintarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/connmarktarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/connmarktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/dnattarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/dnattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/logtarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/logtarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/marktarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/marktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/masqueradetarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/masqueradetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/notracktarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/notracktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/rejecttarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/rejecttarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/snattarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/snattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/tracetarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/tracetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/docs/targets/ttltarget.rst` & `linuxnet-iptables-6.1.0/docs/targets/ttltarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/__init__.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/chain.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 # pylint: disable=too-many-instance-attributes,too-many-public-methods
 
 class Chain:
     """This class is used to represent an iptables chain.
     A chain contains a list of rules which can be referenced by
     number (rule numbers start with 1).
+
+    A :class:`Chain` object is iterable, returning the chain's rules.
     """
 
     def __init__(self, chain_name: str):
         """
         :param chain_name: real chain name
         """
         self.__real_chain_name = chain_name
@@ -47,14 +49,19 @@
         self.__byte_count = 0
         self.__rule_list = []
         self.__pft = None
 
     def __str__(self):
         return f'Chain({self.__real_chain_name})'
 
+    def __iter__(self):
+        """Iterator for the chain's rules
+        """
+        return iter(self.__rule_list)
+
     def is_builtin(self) -> bool:       # pylint: disable=no-self-use
         """Returns ``True`` if this is a built-in chain (e.g. ``INPUT``)
         """
         return False
 
     def has_rules(self) -> bool:
         """Returns ``True`` if the chain contains any rules
@@ -102,22 +109,73 @@
         """
         count = 0
         for rule in self.__rule_list:
             if rule.parsing_failed():
                 count += 1
         return count
 
+    def get_rule_count(self) -> int:
+        """Returns the number of rules in the chain
+        """
+        return len(self.__rule_list)
+
     def get_rules(self) -> List[ChainRule]:
         """Returns a list that contains the chain rules.
         """
         return self.__rule_list[:]
 
-    def iter_rules(self) -> Iterator[ChainRule]:
-        """Returns an iterator for the chain rules.
-        """
+    def iter_rules(self, *, chain_target=False, uses_goto=False,
+                    match_count: Optional[int] =None,
+                    match: Optional['Match'] =None) -> Iterator[ChainRule]:
+        """Returns an iterator for the chain rules. The rules returned
+        by the iterator depend on the arguments:
+
+        :param chain_target: if ``True``, return rules where the target
+            is a chain
+        :param uses_goto: if ``True``, return rules that use goto
+        :param match_count: if not ``None``, return rules that have that
+            number of matches
+        :param match: if not ``None``, return rules that have a matching
+            :class:`Match` in their match list
+        """
+        if (chain_target or uses_goto or match_count is not None or
+                                                match is not None):
+            match_klass = type(None)
+            if match:
+                # Perform a match class comparison
+                match_klass = type(match)
+                for crit in match.get_criteria():
+                    if crit is not None and crit.is_set():
+                        # Perform a match value comparison
+                        match_klass = type(None)
+                        break
+            # Define the filter function
+            def rule_filter(    # pylint: disable=too-many-return-statements
+                        rule: ChainRule) -> bool:
+                """Returns True/False based on whether the specified rule
+                satisfies the specified criteria.
+                """
+                if chain_target or uses_goto:
+                    target_chain = rule.get_target_chain()
+                    if target_chain is None:
+                        return False
+                    if uses_goto and not rule.uses_goto():
+                        return False
+                if (match_count is not None and
+                                        rule.get_match_count() != match_count):
+                    return False
+                if match is None:
+                    return True
+                for rule_match in rule:
+                    if match_klass is type(rule_match):
+                        return True
+                    if rule_match == match:
+                        return True
+                return False
+            return filter(rule_filter, self.__rule_list)
         return iter(self.__rule_list)
 
     def _set_rule_list(self, rule_list: List[ChainRule]) -> None:
         """Set the rule list.
         This method is only used by the parsing code, so it does not
         update any chain reference counts.
         """
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/deps.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/exceptions.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/extension.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/extension.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/__init__.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/addrtypematch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/addrtypematch.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against the address type
 """
 
-from typing import List
+from typing import Iterable
 
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .util import GenericCriterion, BooleanCriterion
 
 _logger = get_logger('linuxnet.iptables.matches.addrtype')
@@ -34,20 +34,25 @@
     """
     def __init__(self):
         self.__src_addr_type_crit = None
         self.__dst_addr_type_crit = None
         self.__limit_iface_in = None
         self.__limit_iface_out = None
 
-    def __eq__(self, other):
-        return (isinstance(other, AddressTypeMatch) and
-                self.src_addr_type() == other.src_addr_type() and
-                self.dst_addr_type() == other.dst_addr_type() and
-                self.limit_iface_in() == other.limit_iface_in() and
-                self.limit_iface_out() == other.limit_iface_out())
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'addrtype'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the addrtype match criteria.
+        """
+        return (self.__src_addr_type_crit, self.__dst_addr_type_crit,
+                        self.__limit_iface_in, self.__limit_iface_out)
 
     def src_addr_type(self) -> GenericCriterion:
         """Compare with the source address type.
 
         The comparison value is a string and should be one of the
         address type values listed in the documentation of the **addrtype**
         module in **iptables(8)**
@@ -88,21 +93,14 @@
         will raise an :exc:`IptablesError`
         """
         if self.__limit_iface_out is None:
             self.__limit_iface_out = BooleanCriterion(self, '--limit-iface-out',
                                                 supports_negation=False)
         return self.__limit_iface_out
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('addrtype',
-                    [self.__src_addr_type_crit, self.__dst_addr_type_crit,
-                        self.__limit_iface_in, self.__limit_iface_out])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse ADDRTYPE; the expected form is::
 
             ADDRTYPE match src-type UNICAST dst-type !UNICAST
             ADDRTYPE match src-type !BLACKHOLE dst-type !UNICAST limit-in
             ADDRTYPE match src-type MULTICAST limit-out
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/commentmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/commentmatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module supports matching against comments
 """
 
-from typing import List
+from typing import Iterable
 
 from ..exceptions import IptablesError
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .util import GenericCriterion
 
@@ -52,30 +52,32 @@
 
 class CommentMatch(Match):
     """Provide a way to add a comment to a rule
     """
     def __init__(self):
         self.__comment_crit = None
 
-    def __eq__(self, other):
-        return (isinstance(other, CommentMatch) and
-                self.comment() == other.comment())
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'comment'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the comment match criteria (only one).
+        """
+        return (self.__comment_crit,)
 
     def comment(self) -> CommentCriterion:
         """The rule comment
         """
         if self.__comment_crit is None:
             self.__comment_crit = CommentCriterion(self)
         return self.__comment_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('comment', [self.__comment_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse a comment. The comment has the form::
 
             /* some comment text */
 
         The leading '/*' has already been consumed when this method
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/connmarkmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/connmarkmatch.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module supports matching against the CT mark
 """
 
-from typing import List
+from typing import Iterable
 
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .markmatch import MarkCriterion
 
 _logger = get_logger('linuxnet.iptables.matches.connmarkmatch')
@@ -31,29 +31,32 @@
 
 class ConnmarkMatch(Match):
     """Match against the ctmark
     """
     def __init__(self):
         self.__mark_crit = None
 
-    def __eq__(self, other):
-        return isinstance(other, ConnmarkMatch) and self.mark() == other.mark()
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'connmark'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the connmark match criteria (only one).
+        """
+        return (self.__mark_crit,)
 
     def mark(self) -> MarkCriterion:
         """Match against the packet's ctmark
         """
         if self.__mark_crit is None:
             self.__mark_crit = MarkCriterion(self)
         return self.__mark_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('connmark', [self.__mark_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse the mark criteria::
 
             connmark match [!]<num>[/<num>]
 
         The 'connmark' field has already been consumed.
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/conntrackmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/conntrackmatch.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against connection tracking attributes
 """
 
-from typing import List
+from typing import Iterable
 
 from ..exceptions import IptablesParsingError
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .util import GenericCriterion
 
@@ -51,19 +51,24 @@
 class ConntrackMatch(Match):
     """Match against the connection tracking attributes.
     """
     def __init__(self):
         self.__ctstate_crit = None
         self.__ctstatus_crit = None
 
-    def __eq__(self, other):
-        return (isinstance(other, ConntrackMatch) and
-                    self.ctstate() == other.ctstate() and
-                    self.ctstatus() == other.ctstatus()
-                    )
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'conntrack'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the conntrack match criteria: ctstate, ctstatus
+        """
+        return (self.__ctstate_crit, self.__ctstatus_crit)
 
     def ctstate(self) -> CtStateCriterion:
         """Match against the connection tracking state
         """
         if self.__ctstate_crit is None:
             self.__ctstate_crit = CtStateCriterion(self)
         return self.__ctstate_crit
@@ -71,20 +76,14 @@
     def ctstatus(self) -> CtStatusCriterion:
         """Matching against the connection tracking status
         """
         if self.__ctstatus_crit is None:
             self.__ctstatus_crit = CtStatusCriterion(self)
         return self.__ctstatus_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('conntrack',
-                        [self.__ctstate_crit, self.__ctstatus_crit])
-
     # pylint: disable=too-many-branches
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Match against ctstate, ctstatus::
 
             [!] ctstate <state>
             [!] ctstatus <status>
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/icmpmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/icmpmatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against ICMP attributes
 """
 
-from typing import List, Optional, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 from ..exceptions import IptablesError, IptablesParsingError
 from ..deps import get_logger
 
 from .match import Match, Criterion, MatchParser
 
 
@@ -177,30 +177,32 @@
 
 class IcmpMatch(Match):
     """Match against the fields of the ICMP header
     """
     def __init__(self):
         self.__icmp_type_crit = None
 
-    def __eq__(self, other):
-        return (isinstance(other, IcmpMatch) and
-                        self.icmp_type() == other.icmp_type())
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'icmp'
+
+    def get_criteria(self) -> Iterable[Criterion]:
+        """Returns the ICMP match criteria (only one): icmp-type
+        """
+        return (self.__icmp_type_crit,)
 
     def icmp_type(self) -> IcmpTypeCriterion:
         """Criterion for matching against the ICMP type
         """
         if self.__icmp_type_crit is None:
             self.__icmp_type_crit = IcmpTypeCriterion(self)
         return self.__icmp_type_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('icmp', [self.__icmp_type_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse the ICMP criteria
 
         :meta private:
         """
         # iptables 1.4.7 output:
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/limitmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/limitmatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against rate limits
 """
 
-
-from typing import List
+from typing import Iterable, List
 
 from ..exceptions import IptablesError
 from ..deps import get_logger
 
 from .match import Match, Criterion, MatchParser
 from .util import GenericCriterion
 from .util import Rate as UtilRate
@@ -89,20 +88,31 @@
     # Make this available to users
     Rate = UtilRate
 
     def __init__(self):
         self.__rate_limit_crit = None
         self.__limit_burst_crit = None
 
-    def __eq__(self, other):
-        return (
-                isinstance(other, LimitMatch) and
-                self.limit() == other.limit() and
-                self.burst() == other.burst()
-                )
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'limit'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the limit match criteria: rate-limit, burst
+        Note that the burst criterion will be ``None`` if the rate-limit
+        criterion has not been set.
+        """
+        if (self.__rate_limit_crit is not None and
+                        self.__rate_limit_crit.is_set()):
+            burst_crit = self.__limit_burst_crit
+        else:
+            burst_crit = None
+        return (self.__rate_limit_crit, burst_crit)
 
     def limit(self) -> RateLimitCriterion:
         """Compare with the rate limit
         """
         if self.__rate_limit_crit is None:
             self.__rate_limit_crit = RateLimitCriterion(self)
         return self.__rate_limit_crit
@@ -110,27 +120,14 @@
     def burst(self) -> BurstCriterion:
         """Compare with the burst limit
         """
         if self.__limit_burst_crit is None:
             self.__limit_burst_crit = BurstCriterion(self)
         return self.__limit_burst_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        # The burst criterion can be included only if the limit criterion
-        # has been set.
-        if (self.__rate_limit_crit is not None and
-                        self.__rate_limit_crit.is_set()):
-            burst_crit = self.__limit_burst_crit
-        else:
-            burst_crit = None
-        return self.build_iptables_args('limit',
-                                        (self.__rate_limit_crit, burst_crit))
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse limit match::
 
             limit: avg <num>/<interval> burst <num>
 
         The 'limit:' has already been consumed.
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/markmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/markmatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module supports matching against the FW mark
 """
 
-from typing import List, Optional, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 from ..exceptions import IptablesError
 from ..deps import get_logger
 
 from .match import Match, Criterion, MatchParser
 
 _logger = get_logger('linuxnet.iptables.matches.markmatch')
@@ -79,29 +79,32 @@
 
 class MarkMatch(Match):
     """Match against the fwmark
     """
     def __init__(self):
         self.__mark_crit = None
 
-    def __eq__(self, other):
-        return isinstance(other, MarkMatch) and self.mark() == other.mark()
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'mark'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the mark match criteria (only one).
+        """
+        return (self.__mark_crit,)
 
     def mark(self) -> MarkCriterion:
         """Match against the packet's fwmark.
         """
         if self.__mark_crit is None:
             self.__mark_crit = MarkCriterion(self)
         return self.__mark_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('mark', [self.__mark_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse the mark criteria::
 
             mark match [!]<num>[/<num>]
 
         The 'mark' field has already been consumed.
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/match.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/match.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 A class derived from Match (with the exception of PacketMatch) corresponds
 to an iptables(8) extension match module, with the options of that module
 mapping to Criterion subclasses.
 The PacketMatch class is also derived from Match and offers matching
 against the common criteria (source/dest address etc.)
 """
 
-from typing import Any, List, Optional, Tuple
+from typing import Any, Iterable, List, Optional, Tuple
 
 from ..exceptions import IptablesError, IptablesParsingError
 from ..deps import get_logger
 from ..parsing import LookaheadIterator
 
 _logger = get_logger('linuxnet.iptables.matches.match')
 
@@ -40,74 +40,81 @@
 class Criterion:
     """
     This class is used to *express* an **iptables(8)** match criterion;
     it does not perform any comparisons.
 
     :class:`Criterion` is a superclass that serves the following purposes:
         1) it provides an :meth:`equals` method and a :meth:`not_equals`
-           method to express comparison against a value
+           method to express a ``==`` or a ``!=`` comparison against a value
         2) it keeps track of whether the criterion has been set;
            a criterion is set when either the :meth:`equals` or
            :meth:`not_equals` method is invoked; **a criterion may only**
            **be set once**
-        3) it keeps track of whether a criterion is negated or not
-        4) its :meth:`iptables_to_args` method generates the '!'
-           **iptables(8)** argument, and also checks if the criterion was set
+        3) it keeps track of whether a criterion is negated or not;
+           this is the criterion's **polarity** (a criterion that
+           performs a ``!=`` comparison has negative polarity)
+        4) it provides a :meth:`to_iptables_args` method to generate the
+           ``!`` (negation) **iptables(8)** argument, and to also check
+           if the criterion was set
 
     The :meth:`equals`/:meth:`not_equals` methods of :class:`Criterion`
     subclasses **must** invoke the :meth:`_set_polarity` method of
     :class:`Criterion` to indicate the polarity of the test.
     These methods are also responsible for saving the comparison value
     in the subclass object.
 
     A :class:`Criterion` has an owner which is an object of a subclass
     of :class:`Match`. The :meth:`equals`/:meth:`not_equals` methods return
     this object to facilitate building a criteria list:
 
     ::
 
-        match.crit1().equals('foo').crit2().not_equals('bar')
+        pkt_match.protocol().equals('tcp').input_interface().equals('eth0')
 
     """
     def __init__(self, match: 'Match'):
         """
         :param match: the :class:`Match` object that owns this ``Criterion``
         """
         self.__match: 'Match' = match
         self.__positive = None
+        self._any = False
 
     def __eq__(self, other: 'Criterion') -> bool:
         """Returns ``True`` iff:
 
              * both criteria are of the same type
              * both criteria are set or both criteria are not set
              * if both criteria are set, they have the same polarity,
                and the same value
         """
         if not isinstance(other, type(self)):
             return False
         if self.is_set() ^ other.is_set():
+            # One set, the other not set, so not equal
             return False
-        if self.is_set():
-            # Both set, so compare boolean values
-            return (self.is_positive() == other.is_positive() and
-                        self.get_value() == other.get_value())
-        # None set, so equal
-        return True
+        if not self.is_set():
+            # None set, so equal
+            return True
+        # Both set, so compare boolean values
+        if self._any or other._any:
+            return True
+        return (self.is_positive() == other.is_positive() and
+                                self.get_value() == other.get_value())
 
     def __ne__(self, other: 'Criterion'):
         return not self.__eq__(other)
 
     def is_set(self) -> bool:
         """Returns ``True`` if the criterion has been set
         """
         return self.__positive is not None
 
     def is_positive(self) -> bool:
-        """Returns the 'polarity' of the criterion; ``True`` for
+        """Returns the 'polarity' of the criterion: ``True`` for
         :meth:`equals` or ``False`` for :meth:`not_equals`
 
         Raises :class:`IptablesError` if the criterion is not set
         """
         if not self.is_set():
             raise IptablesError('criterion not set')
         return self.__positive
@@ -145,14 +152,26 @@
         Returns this object.
         """
         if self.__positive is not None:
             raise IptablesError(f"attempt to modify {self.__class__.__name__}")
         self.__positive = polarity
         return self.__match
 
+    def any(self) -> 'Match':
+        """Match any value.
+
+        This method is used when creating a :class:`Criterion` in order
+        to search the rules of the existing chains for ones that try
+        to match against specific packet properties (e.g. input interface)
+        without being particular about the property value (e.g. eth0).
+        """
+        self._any = True
+        self._set_polarity(True)
+        return self.__match
+
     def equals(self, *args, **kwargs) -> 'Match':
         """Express equality comparison against the argument values.
 
         Subclasses will implement this method to express comparisons
         against a specific value (or values). These values will be the
         arguments of the subclass method and will be stored in the
         subclass object.
@@ -196,93 +215,122 @@
         if is_equal:            # pylint: disable=no-else-return
             return self.equals(*args, **kwargs)
         else:
             return self.not_equals(*args, **kwargs)
 
     def _crit_iptables_args(self) -> List[str]:
         """Returns a list of **iptables(8)** arguments for the criterion,
-        except for polarity
+        except for polarity.
+
+        **Subclasses must implement this method.**
         """
         raise NotImplementedError
 
     def to_iptables_args(self) -> List[str]:
         """Returns a list of **iptables(8)** arguments
 
         This method should be invoked only for criteria that are set,
         i.e. the caller is expected to check with :meth:`Criterion.is_set`
         prior to invoking this method.
 
         :meta private:
         """
+        if self._any:
+            raise IptablesError(
+                f'{self.__class__.__name__} has value set to ANY')
         retval = [] if self.is_positive() else ['!']
         retval += self._crit_iptables_args()
         return retval
 
 
 class Match:
     """Parent class for all match-specific subclasses.
     """
 
-    @staticmethod
-    def build_iptables_args(match_name: Optional[str],
-                                crit_iterable) -> List[str]:
-        """Helper method to build an **iptables(8)** argument list from
-        a match name and a list of :class:`Criterion` objects.
-        **iptables(8)** arguments will be extracted from each
-        criterion that is set.
-
-        :param match_name: optional match name that will result
-            in adding ``-m match_name`` at the beginning of
-            the argument list; there must be at least one set
-            criterion for the match name to be included in the
-            return value
-        :param crit_iterable: an iterable containing
-            :class:`Criterion` objects
+    def get_match_name(self) -> Optional[str]:
+        """Returns the **iptables(8)** match extension name
+        """
+        raise NotImplementedError
+
+    def get_criteria(self) -> Iterable[Optional[Criterion]]:
+        """Returns an iterable containing instances of
+        :class:`Criterion` subclasses, or ``None`` values.
+        """
+        raise NotImplementedError
+
+    def has_criteria(self) -> bool:
+        """Returns ``True`` if the match has any criteria set
+        """
+        for crit in self.get_criteria():
+            if crit is not None and crit.is_set():
+                return True
+        return False
+
+    def to_iptables_args(self) -> List[str]:
+        """Returns a list of **iptables(8)** arguments for the match
+        and its criteria. If no criteria are set, an empty list is
+        returned.
         """
         args = []
-        for crit in crit_iterable:
+        for crit in self.get_criteria():
             if crit is not None and crit.is_set():
                 args += crit.to_iptables_args()
         if not args:
             return args
+        match_name = self.get_match_name()
         if not match_name:
             return args
         return ['-m', match_name] + args
 
-    def has_criteria(self) -> bool:
-        """Returns ``True`` if the match has any criteria set
-        """
-        return bool(self.to_iptables_args())
-
-    def to_iptables_args(self) -> List[str]:
-        """Returns a list of **iptables(8)** arguments
-
-        This method must be implemented by subclasses.
-        """
-        raise NotImplementedError
-
     def __eq__(self, other: 'Match'):
         """We rely on subclasses to define equality by value
         """
-        return self is other
+        if not isinstance(other, type(self)):
+            return False
+        for s_crit, o_crit in zip(self.get_criteria(),
+                                            other.get_criteria()):
+            s_crit_set = s_crit is not None and s_crit.is_set()
+            o_crit_set = o_crit is not None and o_crit.is_set()
+            if not s_crit_set:
+                if o_crit_set:
+                    return False
+                continue
+            if not o_crit_set:
+                return False
+            if s_crit != o_crit:
+                return False
+        return True
 
     def __ne__(self, other: 'Match'):
         return not self.__eq__(other)
 
 
 class MatchNone(Match):
     """This is a special class to indicate the absence of any
     :class:`Match` objects.
     This class is intended to be used for comparison purposes.
     """
 
+    @staticmethod
+    def get_match_name() -> Optional[str]:
+        """There is no name for :class:`MatchNone`
+        """
+        return None
+
+    @staticmethod
+    def get_criteria() -> Iterable[Criterion]:
+        """:class:`MatchNone` has no criteria.
+        """
+        return tuple()
+
     def to_iptables_args(self) -> List[str]:
-        """Returns a list of **iptables(8)** arguments
+        """:class:`MatchNone` is not a real **iptables(8)** match extension,
+        so invoking this method raises an :exc:`IptablesError`
         """
-        return []
+        raise IptablesError("MatchNone is not a real match")
 
 
 
 class CriteriaExhaustedError(Exception):
     """Exception raised to indicate that criteria parsing has completed
     """
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ownermatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ownermatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against UID/GID
 """
 
-from typing import List, Optional, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 from ..exceptions import IptablesParsingError
 from ..deps import get_logger
 
 from .match import Match, Criterion, MatchParser
 from .util import BooleanCriterion
 
@@ -95,21 +95,24 @@
     """
 
     def __init__(self):
         self.__uid_crit = None
         self.__gid_crit = None
         self.__socket_exists_crit = None
 
-    def __eq__(self, other):
-        return (
-                isinstance(other, OwnerMatch) and
-                self.uid() == other.uid() and
-                self.gid() == other.gid() and
-                self.socket_exists() == other.socket_exists()
-                )
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'owner'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the owner match criteria: uid, gid, socket-exists
+        """
+        return (self.__uid_crit, self.__gid_crit, self.__socket_exists_crit)
 
     def uid(self) -> UidCriterion:
         """Compare with the UID
         """
         if self.__uid_crit is None:
             self.__uid_crit = UidCriterion(self)
         return self.__uid_crit
@@ -124,20 +127,14 @@
     def socket_exists(self) -> SocketExistsCriterion:
         """Match if there is a socket for this packet
         """
         if self.__socket_exists_crit is None:
             self.__socket_exists_crit = SocketExistsCriterion(self)
         return self.__socket_exists_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        criteria = (self.__uid_crit, self.__gid_crit, self.__socket_exists_crit)
-        return self.build_iptables_args('owner', criteria)
-
     def _parse_criteria(self, criteria_iter, is_equal) -> bool:
         """Parse the owner criteria.
         Returns ``False`` if the same criterion is encountered again
         (example: owner UID 10-100 ! owner UID 20)
         This is an indication of a new match.
         """
         token = next(criteria_iter)
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packetmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packetmatch.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 This module provides the PacketMatch class which supports
 matching against standard packet attributes
 """
 
 from ipaddress import IPv4Network
-from typing import List, Optional
+from typing import Iterable, Optional
 
 from ..exceptions import IptablesParsingError
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .util import BooleanCriterion, GenericCriterion
 
@@ -102,24 +102,33 @@
         self.__iif_crit = None
         self.__oif_crit = None
         self.__proto_crit = None
         self.__frag_crit = None
         self.__source_crit = None
         self.__dest_crit = None
 
-    def __eq__(self, other):
+    @staticmethod
+    def get_match_name() -> Optional[str]:
+        """Returns the **iptables(8)** match extension name. In the case of
+        the standard packet match, there is no name.
+        """
+        return None
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the packet match criteria: input-interface, output-interface,
+        protocol, fragmented, source, destination.
+        """
         return (
-                isinstance(other, PacketMatch) and
-                self.input_interface() == other.input_interface() and
-                self.output_interface() == other.output_interface() and
-                self.protocol() == other.protocol() and
-                self.fragment() == other.fragment() and
-                self.source_address() == other.source_address() and
-                self.dest_address() == other.dest_address()
-                )
+                            self.__iif_crit,
+                            self.__oif_crit,
+                            self.__proto_crit,
+                            self.__frag_crit,
+                            self.__source_crit,
+                            self.__dest_crit,
+                        )
 
     def protocol(self) -> ProtocolCriterion:
         """Match against the protocol
         """
         if self.__proto_crit is None:
             self.__proto_crit = ProtocolCriterion(self)
         return self.__proto_crit
@@ -155,27 +164,14 @@
     def fragment(self) -> FragmentCriterion:
         """Match if packet has (or has not) the fragment bit set
         """
         if self.__frag_crit is None:
             self.__frag_crit = FragmentCriterion(self)
         return self.__frag_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Generate an **iptables(8)** arguments list for the set criteria
-        """
-        criteria = (
-                            self.__iif_crit,
-                            self.__oif_crit,
-                            self.__proto_crit,
-                            self.__frag_crit,
-                            self.__source_crit,
-                            self.__dest_crit,
-                        )
-        return self.build_iptables_args(None, criteria)
-
     @classmethod
     def _parse(cls, field_iter) -> Optional['PacketMatch']:
         """Parse the following fields, which will be returned in-order
         from field_iter:
             protocol, options, input-interface, output-interface,
             source, destination
         Returns a :class:`PacketMatch` object if any criteria for the above
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/packettypematch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packettypematch.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against the packet type
 """
 
-from typing import List
+from typing import Iterable
 
 from ..exceptions import IptablesParsingError
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .util import GenericCriterion
 
@@ -41,30 +41,32 @@
 
 class PacketTypeMatch(Match):
     """Match against the packet type
     """
     def __init__(self):
         self.__packet_type_crit = None
 
-    def __eq__(self, other):
-        return (isinstance(other, PacketTypeMatch) and
-                self.packet_type() == other.packet_type())
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'pkttype'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the packet type match criteria (only one).
+        """
+        return (self.__packet_type_crit,)
 
     def packet_type(self) -> PacketTypeCriterion:
         """Compare with the packet type
         """
         if self.__packet_type_crit is None:
             self.__packet_type_crit = PacketTypeCriterion(self)
         return self.__packet_type_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('pkttype', [self.__packet_type_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse PKTTYPE; the expected form is::
 
             PKTTYPE op <packet-type>
 
         where op is '=' or '!='.
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/statematch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/statematch.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against the connection tracking state
 """
 
 
-from typing import List
+from typing import Iterable
 
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .util import GenericCriterion
 
 _logger = get_logger('linuxnet.iptables.matches.statematch')
@@ -51,29 +51,32 @@
     This match is accessed via the **state** module, but it is not clear
     how its functionality is different from the **conntrack** module's
     --ctstate option.
     """
     def __init__(self):
         self.__state_crit = None
 
-    def __eq__(self, other):
-        return isinstance(other, StateMatch) and self.state() == other.state()
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'state'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the state match criteria (only one).
+        """
+        return (self.__state_crit,)
 
     def state(self) -> StateCriterion:
         """Match against the connection tracking state
         """
         if self.__state_crit is None:
             self.__state_crit = StateCriterion(self)
         return self.__state_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('state', [self.__state_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Match against state::
 
             state RELATED,ESTABLISHED
 
         The 'state' field has already been consumed.
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,70 +16,78 @@
 # <https://www.gnu.org/licenses/>.
 
 """
 This module supports matching against TCP packets
 """
 
 from enum import IntFlag
-from typing import List, Optional, Set, Tuple
+from typing import Iterable, List, Optional, Set, Tuple
 
 from ..exceptions import IptablesError, IptablesParsingError
 from ..deps import get_logger
 
 from .match import Match, Criterion, MatchParser
+from .util import GenericCriterion
 
 _logger = get_logger('linuxnet.iptables.matches.tcpmatch')
 
 
 class TcpFlag(IntFlag):
     """Names and values for the TCP flags.
     """
+    #: ``FIN`` bit
     FIN = 0x1
+    #: ``SYN`` bit
     SYN = 0x2
+    #: ``RST`` bit
     RST = 0x4
+    #: ``PSH`` bit
     PSH = 0x8
+    #: ``ACK`` bit
     ACK = 0x10
+    #: ``URG`` bit
     URG = 0x20
 
 
 class TcpFlagsCriterion(Criterion):
     """A criterion for comparing against packets with an arbitrary set of
-    TCP flags set, or for comparing against SYN packets. This is
+    TCP flags set, or for comparing against ``SYN`` packets. This is
     an either-or use, determined at the time of object instantiation.
 
     The value is the tuple (flags-checked, flags-set); both flags-checked
-    and flags-set are comma-separated lists of TCP flag names.
+    and flags-set are comma-separated lists of TCP flag names as defined
+    in :class:`TcpFlag`
     """
     def __init__(self, match: Match, syn_only=False):
         """
         :param match: the :class:`Match` object that owns this object
         :param syn_only: optional boolean value indicating a check only
-            against the **SYN** flag
+            against the ``SYN`` flag
         """
         super().__init__(match)
         # If syn_only is True, then flags_checked/flags_set will be None
         self.__syn_only = syn_only
         self.__flags_checked = None
         self.__flags_set = None
 
     def __eq__(self, other):
         if not isinstance(other, TcpFlagsCriterion):
             return False
-        if self.is_syn_only() ^ other.is_syn_only():
-            return False
         if not self._may_be_equal(other):
             return False
+        if self.is_syn_only() ^ other.is_syn_only():
+            return self._any or other._any
         return self.get_value() == other.get_value()
 
     def get_value(self) -> Tuple[Set[TcpFlag], Set[TcpFlag]]:
         """Returns the value that the criterion is comparing against
         """
         return (self.__flags_checked, self.__flags_set)
 
-    def is_syn_only(self):
+    def is_syn_only(self) -> bool:
         """Returns ``True`` if the criterion is only meant to check
         for the SYN flag (but note that it may not be set yet)
         """
         return self.__syn_only
 
     def bit_set(self) -> Match:
         """This method can be used if this criterion implements a
@@ -154,29 +162,38 @@
             port_spec += f':{self.__last_port}'
         return [self.__option, port_spec]
 
 
 class SourcePortCriterion(_PortCriterion):
     """Compare with a source port or check for inclusion in port-range
 
-    The value is a the tuple (port, last_port) where last_port may be ``None``
+    The value is the tuple (port, last_port) where last_port may be ``None``
     """
     def __init__(self, match: Match):
         super().__init__(match, '--sport')
 
 
 class DestPortCriterion(_PortCriterion):
     """Compare against a destination port or check for inclusion in port-range
 
-    The value is a the tuple (port, last_port) where last_port may be ``None``
+    The value is the tuple (port, last_port) where last_port may be ``None``
     """
     def __init__(self, match: Match):
         super().__init__(match, '--dport')
 
 
+class TcpOptionCriterion(GenericCriterion):
+    """Compare against a TCP option number.
+
+    The value is an integer.
+    """
+    def __init__(self, match: Match):
+        super().__init__(match, '--tcp-option')
+
+
 class _PortParser:      # pylint: disable=too-few-public-methods
     """Helper class used to parse TCP/UDP port criteria
     """
 
     SOURCE_PORT_PREFIX = ('spt:', 'spts:')
     DEST_PORT_PREFIX = ('dpt:', 'dpts:')
     PORT_PREFIX = SOURCE_PORT_PREFIX + DEST_PORT_PREFIX
@@ -202,22 +219,27 @@
     """Match against the fields of the TCP header
     """
 
     def __init__(self):
         self.__flags_crit = None
         self.__src_port_crit = None
         self.__dest_port_crit = None
+        self.__tcp_option_crit = None
 
-    def __eq__(self, other):
-        return (
-                isinstance(other, TcpMatch) and
-                self.tcp_flags() == other.tcp_flags() and
-                self.source_port() == other.source_port() and
-                self.dest_port() == other.dest_port()
-                )
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'tcp'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the TCP match criteria: flags, source-port, dest-port
+        """
+        return (self.__flags_crit, self.__src_port_crit,
+                        self.__dest_port_crit, self.__tcp_option_crit)
 
     def syn(self) -> TcpFlagsCriterion:
         """Criterion for matching against a SYN packet
         """
         if self.__flags_crit is None:
             self.__flags_crit = TcpFlagsCriterion(self, syn_only=True)
         return self.__flags_crit
@@ -239,36 +261,42 @@
     def dest_port(self) -> DestPortCriterion:
         """Match against the destination port
         """
         if self.__dest_port_crit is None:
             self.__dest_port_crit = DestPortCriterion(self)
         return self.__dest_port_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
+    def tcp_option(self) -> TcpOptionCriterion:
+        """Match against a TCP option
         """
-        criteria = (self.__flags_crit, self.__src_port_crit,
-                                                self.__dest_port_crit)
-        return self.build_iptables_args('tcp', criteria)
+        if self.__tcp_option_crit is None:
+            self.__tcp_option_crit = TcpOptionCriterion(self)
+        return self.__tcp_option_crit
 
-    @classmethod
-    def __parse_tcp_flags_num(cls, numstr: int) -> Set[TcpFlag]:
+    @staticmethod
+    def __parse_tcp_flags_num(numstr: int) -> Set[TcpFlag]:
         """Parse a hex-value numstr (e.g. 0x11) into a set of TCP flags.
         """
         try:
             flag_mask = int(numstr, 16)
             flags = {flag for flag in TcpFlag if flag_mask & flag}
             return flags
         except ValueError as valerr:
             raise IptablesParsingError(
                         "Bad TCP flag mask: " + numstr) from valerr
 
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
-        """Parse the TCP criteria
+        """Parse the TCP criteria. The iptables output looks like this::
+
+                tcp dpt:20 option=!10 flags:0x17/0x02
+
+        The 'tcp' field has already been consumed.
+
+        :meta private:
         """
         criteria_iter = parser.get_iter()
         match = TcpMatch()
         for val in criteria_iter:
             if val.startswith('flags:'):
                 flag_spec = val.split(':', 1)[1]
                 is_equal, flag_spec = parser.parse_value(flag_spec)
@@ -283,14 +311,18 @@
                                                 TcpFlag.RST, TcpFlag.ACK}):
                     match.syn().compare(is_equal)
                 else:
                     match.tcp_flags().compare(is_equal,
                                                 flags_checked, flags_set)
             elif val.startswith(_PortParser.PORT_PREFIX):
                 _PortParser.parse(val, match)
+            elif val.startswith('option'):
+                # The comparison looks either like 'option=10' or 'option=!10'
+                is_equal, value = parser.parse_value(val[len('option')+1:])
+                match.tcp_option().compare(is_equal, int(value))
             else:
                 criteria_iter.put_back(val)
                 break
         return match
 
 
 MatchParser.register_match('tcp', TcpMatch)
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/tcpmssmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmssmatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module supports matching against the TCP MSS
 """
 
-from typing import List, Optional, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 from ..exceptions import IptablesError
 from ..deps import get_logger
 
 from .match import Match, Criterion, MatchParser
 
 _logger = get_logger('linuxnet.iptables.matches.tcpmssmatch')
@@ -51,16 +51,14 @@
                     mssval: int, endval: Optional[int] =None) -> Match:
         """Check for equality against ``mssval``, or range equality
         if ``endval`` is present.
 
         :param mssval: the MSS value
         :param endval: range of MSS values from ``mssval`` to this value
         """
-        if mssval is None:
-            raise IptablesError('mssval is None')
         self.__mssval = mssval
         if endval is not None and endval < mssval:
             raise IptablesError('bad range: endval < mssval')
         self.__endval = endval
         return self._set_polarity(True)
 
     def _crit_iptables_args(self) -> List[str]:
@@ -74,29 +72,32 @@
 
 class TcpmssMatch(Match):
     """Match against the MSS field of the TCP header
     """
     def __init__(self):
         self.__mss_crit = None
 
-    def __eq__(self, other):
-        return isinstance(other, TcpmssMatch) and self.mss() == other.mss()
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'tcpmss'
+
+    def get_criteria(self) -> Iterable[Criterion]:
+        """Returns the TCPMSS match criteria (only one).
+        """
+        return (self.__mss_crit,)
 
     def mss(self) -> MssCriterion:
         """Match against the MSS field of the TCP header
         """
         if self.__mss_crit is None:
             self.__mss_crit = MssCriterion(self)
         return self.__mss_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('tcpmss', [self.__mss_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse tcpmss::
 
             tcpmss match !10:20
 
         'tcpmss' has already been consumed when this method
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/ttlmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ttlmatch.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against the packet TTL
 """
 
-from typing import List, Tuple
+from typing import Iterable, List, Tuple
 
 from ..exceptions import IptablesParsingError
 from ..deps import get_logger
 
 from .match import Match, Criterion, MatchParser, CriteriaExhaustedError
 
 _logger = get_logger('linuxnet.iptables.matches.ttlmatch')
@@ -89,30 +89,32 @@
 
 class TtlMatch(Match):
     """Match against the packet TTL value
     """
     def __init__(self):
         self.__ttl_crit = None
 
-    def __eq__(self, other):
-        return (isinstance(other, TtlMatch) and
-                self.ttl() == other.ttl())
+    @staticmethod
+    def get_match_name():
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'ttl'
+
+    def get_criteria(self) -> Iterable[Criterion]:
+        """Returns the TTL match criteria (only one).
+        """
+        return (self.__ttl_crit,)
 
     def ttl(self) -> TtlCriterion:
         """Returns the TTL criterion
         """
         if self.__ttl_crit is None:
             self.__ttl_crit = TtlCriterion(self)
         return self.__ttl_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        return self.build_iptables_args('ttl', [self.__ttl_crit])
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse the TTL criterion::
 
             TTL match TTL > 5
 
         :meta private:
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/udpmatch.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/udpmatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module supports matching against UDP packets
 """
 
-from typing import List
+from typing import Iterable
 
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .tcpmatch import _PortParser, SourcePortCriterion, DestPortCriterion
 
 _logger = get_logger('linuxnet.iptables.matches.udpmatch')
@@ -32,20 +32,24 @@
 class UdpMatch(Match):
     """Match against the source/destination UDP ports.
     """
     def __init__(self):
         self.__src_port_crit = None
         self.__dest_port_crit = None
 
-    def __eq__(self, other):
-        return (
-                isinstance(other, UdpMatch) and
-                self.source_port() == other.source_port() and
-                self.dest_port() == other.dest_port()
-                )
+    @staticmethod
+    def get_match_name() -> str:
+        """Returns the **iptables(8)** match extension name
+        """
+        return 'udp'
+
+    def get_criteria(self) -> Iterable['Criterion']:
+        """Returns the UDP match criteria: source-port, dest-port
+        """
+        return (self.__src_port_crit, self.__dest_port_crit)
 
     def source_port(self) -> SourcePortCriterion:
         """Match against the source port
         """
         if self.__src_port_crit is None:
             self.__src_port_crit = SourcePortCriterion(self)
         return self.__src_port_crit
@@ -53,20 +57,14 @@
     def dest_port(self) -> DestPortCriterion:
         """Match against the destination port
         """
         if self.__dest_port_crit is None:
             self.__dest_port_crit = DestPortCriterion(self)
         return self.__dest_port_crit
 
-    def to_iptables_args(self) -> List[str]:
-        """Returns **iptables(8)** arguments for this match
-        """
-        criteria = (self.__src_port_crit, self.__dest_port_crit)
-        return self.build_iptables_args('udp', criteria)
-
     @classmethod
     def parse(cls, parser: MatchParser) -> Match:
         """Parse the UDP criteria::
 
             udp spts:!1:1024 dpt:53
 
         The 'udp' field has already been consumed.
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/matches/util.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/util.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/metadata.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """
 Metadata information intended to be used by setup.py and the
 Sphinx conf.py
 """
 
 # pylint: disable=invalid-name
 
-_version_ = "5.4.0"
+_version_ = "6.1.0"
 _author_ = "Panagiotis (Panos) Tsirigotis"
 _package_ = "linuxnet.iptables"
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/parsing.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/parsing.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/rule.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Affero General
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """This module provides the ChainRule class
 """
 
-from typing import List, Optional
+from typing import Iterator, List, Optional
 
 from .exceptions import IptablesError, IptablesParsingError
 from .matches import Match, MatchNone, PacketMatch, CommentMatch
 from .matches.match import MatchParser
 from .parsing import LookaheadIterator, RuleFieldIterator
 from .targets import Target, ChainTarget, UnparsedTarget, TargetNone
 from .targets.target import TargetParser
@@ -37,14 +37,17 @@
     A :class:`ChainRule` has a (possibly empty) list of :class:`Match`
     objects and an optional :class:`Target` object.
 
     Multiple :class:`Match` objects of the same type can be included
     in a rule. Since multiple :class:`Match` objects imply a logical-AND,
     including objects of the same type may be useful when using negation.
     However, there can be at most one :class:`PacketMatch` object included.
+
+    A :class:`ChainRule` object is iterable, returning the rule's
+    :class:`Match` instances.
     """
 
     def __init__(self, *,
                 match:Optional[Match] =None,
                 match_list:Optional[List[Match]] =None,
                 target:Optional[Target] =None,
                 uses_goto:Optional[bool] =False):
@@ -87,14 +90,19 @@
     def __str__(self):
         if self.parsing_failed():
             rule_str = f"UNPARSED: {self.__iptables_line}"
         else:
             rule_str = ' '.join(self.to_iptables_args())
         return f"ChainRule('{rule_str}')"
 
+    def __iter__(self):
+        """Iterator for the rule's matches
+        """
+        return iter(self.__match_list)
+
     def _set_stats(self, *, packet_count: int, byte_count: int):
         """Set the rule stats
         This method is only used by the parsing code.
         """
         self.__packet_count = packet_count
         self.__byte_count = byte_count
 
@@ -187,14 +195,24 @@
     def set_target(self, target: Target) -> None:
         """Set the rule target
         """
         if self.__owner_chain is not None:
             raise IptablesError('attempt to replace target of active rule')
         self.__target = target
 
+    def iter_match_list(self) -> Iterator[Match]:
+        """Returns an iterator for the matches of this rule.
+        """
+        return iter(self.__match_list)
+
+    def get_match_count(self) -> int:
+        """Returns the number of matches.
+        """
+        return len(self.__match_list)
+
     def get_match_list(self) -> List[Match]:
         """Returns the match list of this rule.
         """
         return self.__match_list[:]
 
     def has_match(self, match: Match, is_only_match=True) -> bool:
         """Returns ``True`` if the match list of this rule consists only
@@ -251,15 +269,17 @@
         # chain object; try to resolve it
         pft = self.__owner_chain.get_pft()
         if pft is None:
             raise IptablesError("rule is not in IptablesPacketFilterTable")
         return self.__target.resolve_chain(pft)
 
     def matches_all_packets(self) -> bool:
-        """Returns ``True`` iff this rule matches all packets
+        """Returns ``True`` iff this rule matches all packets. This
+        can be because the rule has no matches, or because the only
+        matches are comments.
         """
         for match in self.__match_list:
             if not isinstance(match, CommentMatch):
                 return False
         return True
 
     def to_iptables_args(self) -> List[str]:
@@ -316,14 +336,24 @@
         if self.__owner_chain is not None:
             rcn = self.__owner_chain.get_real_name()
             raise IptablesError(f'rule already inserted in chain {rcn}')
         self.__target = ChainTarget(chain=chain)
         self.__uses_goto = True
         return self
 
+    def zero_counters(self) -> None:
+        """Zero the packet and byte counters of this rule
+        """
+        if self.__owner_chain is None:
+            raise IptablesError('rule not in a chain')
+        pft = self.__owner_chain.get_pft()
+        if pft is None:
+            raise IptablesError('rule belongs to chain that is not in kernel')
+        pft.zero_counters(chain=self.__owner_chain, rulenum=self.__rulenum)
+
     __PROTO_NAMES = set(('tcp', 'udp', 'udplite', 'icmp',
                                 'esp', 'ah', 'sctp', 'all'))
 
     @classmethod
     def __parse_target_name(cls, field_iter: LookaheadIterator):
         """Returns the target_name if present, otherwise None
         """
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/table.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """A programmatic interface to the iptables command
 """
 
 import logging
 import subprocess
 import time
 
-from typing import Dict, Iterator, List, Optional, Tuple
+from typing import Iterator, List, Mapping, Optional, Tuple
 
 from .exceptions import (
                 IptablesError, IptablesParsingError, IptablesExecutionError)
 from .chain import Chain, BuiltinChain
 from .targets import Target, ChainTarget, UnparsedTarget
 from .deps import get_logger
 
@@ -241,15 +241,15 @@
     def get_rcn(self, lcn: str) -> str:
         """Returns the real chain name for the given logical chain name
 
         :param lcn: logical chain name
         """
         return self.__rcn(lcn)
 
-    def get_chain_map(self) -> Dict[str, Chain]:
+    def get_chain_map(self) -> Mapping[str, Chain]:
         """Returns a dictionary containing all accessible chains;
         the key is the real chain name (if the
         :class:`IptablesPacketFilterTable` uses a prefix, only chains
         with that prefix, and the builtin chains, will be included)
         """
         return self.__chain_map.copy()
 
@@ -478,15 +478,15 @@
                         builtin_chain.get_real_name(),
                         logging.WARNING,
                         iter(builtin_chain.get_rules()),
                         log_stat_failures)
             builtin_chain._set_stats(    # pylint: disable=protected-access
                         chain_packet_count, chain_byte_count)
 
-    def __clear_chain_info(self):
+    def __clear_chain_info(self) -> None:
         """Disassociate from all known chains
         """
         for chain in self.__chain_map.values():
             chain._clear_pft()          # pylint: disable=protected-access
         for chain in self.__other_chain_map.values():
             chain._clear_pft()          # pylint: disable=protected-access
 
@@ -640,26 +640,29 @@
                         self.delete_chain.__qualname__,
                                 self, n_deleted, real_chain_name)
         chain.flush()
         _ = self.iptables_run(['-X', real_chain_name], check=True)
         self.__chain_map.pop(real_chain_name, None)
         chain._clear_pft()              # pylint: disable=protected-access
 
-    def zero_counters(self, chain: Optional[Chain] =None) -> None:
+    def zero_counters(self, chain: Optional[Chain] =None,
+                                rulenum: Optional[int] =None) -> None:
         """Zero the packet and byte counters for the specified chain
-        in the kernel. If no chain is specified, all chain counters are
-        zero'd.
+        or chain rule in the kernel. If no chain is specified, all chain
+        counters are zero'd.
 
         Note that this method does not affect the counters of :class:`Chain`
-        objects which will maintain the values they had from the last time
-        the system configuration was read.
+        or :class:`ChainRule` objects which will maintain the values they
+        had from the last time the system configuration was read.
         """
         cmd = ['-Z']
         if chain is not None:
             if chain.get_pft() is not self:
                 raise IptablesError(
                     'attempt to zero chain counters of '
                     'chain owned by another table')
             cmd.append(chain.get_real_name())
+            if rulenum is not None:
+                cmd.append(str(rulenum))
         _ = self.iptables_run(cmd, check=True)
 
 # pylint: enable=too-many-instance-attributes, too-many-public-methods
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/__init__.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/connmarktarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/connmarktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/logtarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/logtarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/marktarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/marktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/masqueradetarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/masqueradetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/nattarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/nattarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/notracktarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/notracktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/rejecttarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/rejecttarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/target.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/target.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/tracetarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/tracetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet/iptables/targets/ttltarget.py` & `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/ttltarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/PKG-INFO` & `linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.4.0
+Version: 6.1.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-5.4.0/linuxnet_iptables.egg-info/SOURCES.txt` & `linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/setup.py` & `linuxnet-iptables-6.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.4.0/tests/iptables_test.py` & `linuxnet-iptables-6.1.0/tests/iptables_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,105 +211,110 @@
     pkts      bytes target     prot opt in     out     source               destination
        0        0 DROP         all  -f  *      *       127.0.0.0/8          0.0.0.0/0
       29     9862 ACCEPT     udp  --  *      *       0.0.0.0/0            10.10.0.0/16
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rules = input_chain.get_rules()
-        self.assertEqual(len(rules), 2)
-        match_list = rules[0].get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[0]
-        self.assertTrue(match.fragment().is_positive())
-        src = match.source_address()
-        self.assertTrue(src.is_positive() and
-                src.get_value() == IPv4Network('127.0.0.0/8'))
-        match_list = rules[1].get_match_list()
-        match = match_list[0]
-        prot = match.protocol()
-        self.assertTrue(prot.is_positive() and
-                prot.get_value() == 'udp')
-        dest = match.dest_address()
-        self.assertTrue(dest.is_positive() and
-                dest.get_value() == IPv4Network('10.10.0.0/16'))
+        self.assertEqual(input_chain.get_rule_count(), 2)
+        for rule in input_chain:
+            if rule.get_rulenum() == 1:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                self.assertTrue(match.fragment().is_positive())
+                src = match.source_address()
+                self.assertTrue(src.is_positive() and
+                    src.get_value() == IPv4Network('127.0.0.0/8'))
+            elif rule.get_rulenum() == 2:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                prot = match.protocol()
+                self.assertTrue(prot.is_positive() and
+                    prot.get_value() == 'udp')
+                dest = match.dest_address()
+                self.assertTrue(dest.is_positive() and
+                    dest.get_value() == IPv4Network('10.10.0.0/16'))
 
     def test_parsing_packet_type_match(self):
         """Parse output with packet type match
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
       29     9862 DROP       all  --  *      *       0.0.0.0              0.0.0.0/0           PKTTYPE = broadcast
       29     9862 ACCEPT     udp  --  *      *       0.0.0.0/0            10.10.0.0/16
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rules = input_chain.get_rules()
-        match_list = rules[0].get_match_list()
+        first_rule = next(iter(input_chain))
+        match_list = first_rule.get_match_list()
         self.assertEqual(len(match_list), 2)
         match = match_list[1]
         self.assertTrue(isinstance(match, PacketTypeMatch))
         ptype = match.packet_type()
         self.assertTrue(ptype.is_positive() and
                         ptype.get_value() == 'broadcast')
 
     def test_parsing_tcp_match(self):
         """Parse output with match related to TCP (port, flags, MSS)
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
        8      524 DROP  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcpmss match 1:500
-    2182   251300 DROP  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp flags:!0x17/0x02
-      17      732 ACCEPT  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp dpt:22
+    2182   251300 DROP  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp flags:!0x17/0x02 option=10
+      17      732 ACCEPT  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp dpt:22 option=!10
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rules = input_chain.get_rules()
-        self.assertEqual(len(rules), 3)
-        for rule in rules:
+        self.assertEqual(input_chain.get_rule_count(), 3)
+        for rule in input_chain:
             rulenum = rule.get_rulenum()
             match_list = rule.get_match_list()
-            # There is a PacketMatch matching prot
+            # There is a PacketMatch matching the packet protocol
             self.assertEqual(len(match_list), 2)
             match = match_list[-1]
             if rulenum == 1:
                 self.assertTrue(isinstance(match, TcpmssMatch))
                 mss = match.mss()
                 self.assertTrue(mss.is_positive() and
                                         mss.get_value() == (1, 500))
             elif rulenum == 2:
                 self.assertTrue(isinstance(match, TcpMatch))
                 flags = match.tcp_flags()
                 self.assertTrue(flags.is_syn_only() and
                                         not flags.is_positive())
+                tcp_option = match.tcp_option()
+                self.assertTrue(tcp_option.get_value() == 10 and
+                                tcp_option.is_positive())
             elif rulenum == 3:
                 self.assertTrue(isinstance(match, TcpMatch))
                 dport = match.dest_port()
                 self.assertTrue(dport.is_positive() and
                         dport.get_value()[0] == 22)
+                tcp_option = match.tcp_option()
+                self.assertTrue(tcp_option.get_value() == 10 and
+                                not tcp_option.is_positive())
 
     def test_parsing_udp_match(self):
         """Parse output with match related to UDP
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
-      17      732 ACCEPT  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           udp dpt:53
+      17      732 ACCEPT  udp  --  *      *       0.0.0.0/0            0.0.0.0/0           udp dpt:53
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rules = input_chain.get_rules()
-        self.assertEqual(len(rules), 1)
-        rule = rules[0]
-        match_list = rule.get_match_list()
+        self.assertEqual(input_chain.get_rule_count(), 1)
+        first_rule = next(iter(input_chain))
+        match_list = first_rule.get_match_list()
         # There is a PacketMatch matching prot
         self.assertEqual(len(match_list), 2)
         match = match_list[-1]
         self.assertTrue(isinstance(match, UdpMatch))
         dport = match.dest_port()
         self.assertTrue(dport.is_positive() and
                         dport.get_value()[0] == 53)
@@ -324,68 +329,56 @@
   143588 11622518 DROP         icmp --  *      *       0.0.0.0/0            0.0.0.0/0           icmp !any
   143588 11622518 DROP         icmp --  *      *       0.0.0.0/0            0.0.0.0/0           icmp type 3 icmp !type 3 code 1
   143588 11622518 DROP         icmp --  *      *       0.0.0.0/0            0.0.0.0/0           icmptype 3
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rules = input_chain.get_rules()
-        self.assertEqual(len(rules), 4)
-        #
-        # Verify first rule
-        #
-        rule = rules[0]
-        match_list = rule.get_match_list()
-        # There is a PacketMatch matching prot
-        self.assertEqual(len(match_list), 2)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, IcmpMatch))
-        icmp_type = match.icmp_type()
-        self.assertTrue(icmp_type.is_positive() and
-                        icmp_type.get_type_name() == 'echo-request' and
-                        icmp_type.get_type_value() == 8)
-        #
-        # Verify second rule
-        #
-        rule = rules[1]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 2)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, IcmpMatch))
-        icmp_type = match.icmp_type()
-        self.assertTrue(not icmp_type.is_positive() and
-                        icmp_type.get_type_name() == 'any')
-        #
-        # Verify third rule
-        #
-        rule = rules[2]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 3)
-        match = match_list[-2]
-        self.assertTrue(isinstance(match, IcmpMatch))
-        icmp_type = match.icmp_type()
-        self.assertTrue(icmp_type.is_positive() and
-                        icmp_type.get_type_value() == 3)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, IcmpMatch))
-        icmp_type = match.icmp_type()
-        self.assertTrue(not icmp_type.is_positive() and
-                        icmp_type.get_type_value() == 3 and
-                        icmp_type.get_code() == 1)
-        #
-        # Verify fourth rule
-        #
-        rule = rules[3]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 2)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, IcmpMatch))
-        icmp_type = match.icmp_type()
-        self.assertTrue(icmp_type.is_positive() and
-                        icmp_type.get_type_value() == 3)
+        self.assertEqual(input_chain.get_rule_count(), 4)
+        for rule in input_chain:
+            if rule.get_rulenum() == 1:
+                match_list = rule.get_match_list()
+                # There is a PacketMatch matching prot
+                self.assertEqual(len(match_list), 2)
+                match = match_list[-1]
+                self.assertTrue(isinstance(match, IcmpMatch))
+                icmp_type = match.icmp_type()
+                self.assertTrue(icmp_type.is_positive() and
+                    icmp_type.get_type_name() == 'echo-request' and
+                    icmp_type.get_type_value() == 8)
+            elif rule.get_rulenum() == 2:
+                match_list = rule.get_match_list()
+                self.assertEqual(len(match_list), 2)
+                match = match_list[-1]
+                self.assertTrue(isinstance(match, IcmpMatch))
+                icmp_type = match.icmp_type()
+                self.assertTrue(not icmp_type.is_positive() and
+                                icmp_type.get_type_name() == 'any')
+            elif rule.get_rulenum() == 3:
+                match_list = rule.get_match_list()
+                self.assertEqual(len(match_list), 3)
+                match = match_list[-2]
+                self.assertTrue(isinstance(match, IcmpMatch))
+                icmp_type = match.icmp_type()
+                self.assertTrue(icmp_type.is_positive() and
+                                icmp_type.get_type_value() == 3)
+                match = match_list[-1]
+                self.assertTrue(isinstance(match, IcmpMatch))
+                icmp_type = match.icmp_type()
+                self.assertTrue(not icmp_type.is_positive() and
+                                icmp_type.get_type_value() == 3 and
+                                icmp_type.get_code() == 1)
+            elif rule.get_rulenum() == 4:
+                match_list = rule.get_match_list()
+                self.assertEqual(len(match_list), 2)
+                match = match_list[-1]
+                self.assertTrue(isinstance(match, IcmpMatch))
+                icmp_type = match.icmp_type()
+                self.assertTrue(icmp_type.is_positive() and
+                                icmp_type.get_type_value() == 3)
 
     def test_parsing_owner_match(self):
         """Parse output with match related to UID/GID
         """
         output = self.EMPTY_INPUT + '\n' + self.EMPTY_FORWARD + '\n' + \
 """\
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
@@ -395,94 +388,75 @@
        8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner UID match 100-300 ! owner UID match 200
        8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner socket exists 
        8      524   DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           owner GID match 100 ! owner socket exists 
 """
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         output_chain = pft.get_builtin_chain('OUTPUT')
-        rules = output_chain.get_rules()
-        self.assertEqual(len(rules), 5)
-        #
-        # Verify first rule
-        #
-        rule = rules[0]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, OwnerMatch))
-        uid = match.uid()
-        self.assertTrue(uid.is_positive() and uid.get_value() == (100, None))
-        #
-        # Verify second rule
-        #
-        rule = rules[1]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, OwnerMatch))
-        gid = match.gid()
-        self.assertTrue(not gid.is_positive() and gid.get_value() == (100, None))
-        #
-        # Verify third rule
-        #
-        rule = rules[2]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 2)
-        match = match_list[-2]
-        self.assertTrue(isinstance(match, OwnerMatch))
-        uid = match.uid()
-        self.assertTrue(uid.is_positive() and uid.get_value() == (100, 300))
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, OwnerMatch))
-        uid = match.uid()
-        self.assertTrue(not uid.is_positive() and uid.get_value() == (200, None))
-        #
-        # Verify fourth rule
-        #
-        rule = rules[3]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, OwnerMatch))
-        socket_exists = match.socket_exists()
-        self.assertTrue(socket_exists.is_positive())
-        #
-        # Verify fifth rule
-        # Note that a single match is expected because the owner
-        # match criteria are different.
-        #
-        rule = rules[4]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[-1]
-        self.assertTrue(isinstance(match, OwnerMatch))
-        gid = match.gid()
-        socket_exists = match.socket_exists()
-        self.assertTrue(
-                gid.is_positive() and gid.get_value() == (100, None) and
-                not socket_exists.is_positive())
+        self.assertEqual(output_chain.get_rule_count(), 5)
+        for rule in output_chain:
+            if rule.get_rulenum() == 1:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, OwnerMatch))
+                uid = match.uid()
+                self.assertTrue(uid.is_positive() and uid.get_value() == (100, None))
+            elif rule.get_rulenum() == 2:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, OwnerMatch))
+                gid = match.gid()
+                self.assertTrue(not gid.is_positive() and gid.get_value() == (100, None))
+            elif rule.get_rulenum() == 3:
+                match_list = rule.get_match_list()
+                self.assertEqual(len(match_list), 2)
+                match = match_list[-2]
+                self.assertTrue(isinstance(match, OwnerMatch))
+                uid = match.uid()
+                self.assertTrue(uid.is_positive() and uid.get_value() == (100, 300))
+                match = match_list[-1]
+                self.assertTrue(isinstance(match, OwnerMatch))
+                uid = match.uid()
+                self.assertTrue(not uid.is_positive() and uid.get_value() == (200, None))
+            elif rule.get_rulenum() == 4:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, OwnerMatch))
+                socket_exists = match.socket_exists()
+                self.assertTrue(socket_exists.is_positive())
+            elif rule.get_rulenum() == 5:
+                #
+                # Note that a single match is expected because the owner
+                # match criteria are different.
+                #
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, OwnerMatch))
+                gid = match.gid()
+                socket_exists = match.socket_exists()
+                self.assertTrue(
+                        gid.is_positive() and gid.get_value() == (100, None) and
+                        not socket_exists.is_positive())
 
     def test_parsing_connmark_match(self):
         """Parse output with connmark match
         """
         output = ("""\
 Chain PREROUTING (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
   558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK set 0x11 
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT + '\n' +
                 self.EMPTY_INPUT + '\n' + self.EMPTY_POSTROUTING)
         pft = IptablesPacketFilterTable('mangle')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('PREROUTING')
-        rules = input_chain.get_rules()
-        self.assertEqual(len(rules), 1)
-        rule = rules[0]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[-1]
+        self.assertEqual(input_chain.get_rule_count(), 1)
+        rule = next(iter(input_chain))
+        self.assertEqual(rule.get_match_count(), 1)
+        match = next(iter(rule))
         self.assertTrue(isinstance(match, ConnmarkMatch))
         cmark = match.mark()
         self.assertTrue(cmark.is_positive() and cmark.get_value() == (0, None))
 
     def test_parsing_limit_match(self):
         """Parse output with limit match
         """
@@ -491,18 +465,17 @@
     pkts      bytes target     prot opt in     out     source               destination
   487148 21609270 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           limit: avg 15/min burst 5 LOG flags 0 level 6 prefix `DROP-INPUT: '
   520139 23069461 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rule = input_chain.get_rules()[0]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[0]
+        rule = next(iter(input_chain))
+        self.assertEqual(rule.get_match_count(), 1)
+        match = next(iter(rule))
         limit = match.limit()
         self.assertTrue(limit.is_positive() and
                 limit.get_value() == LimitMatch.Rate(15, LimitMatch.Rate.PER_MIN))
         burst = match.burst()
         self.assertTrue(burst.is_positive() and
                 burst.get_value() == 5)
 
@@ -515,31 +488,31 @@
        0        0 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* my comment */ 
        0        0 REJECT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* another comment */ state NEW reject-with icmp-port-unreachable 
        0        0 REJECT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           /* another comment */ state NEW /* foo bar */ reject-with icmp-port-unreachable 
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        for rule in input_chain.get_rules():
+        for rule in input_chain:
             rulenum = rule.get_rulenum()
             if rulenum == 1:
-                for match in rule.get_match_list():
+                for match in rule:
                     if isinstance(match, CommentMatch):
                         comment = match.comment().get_value()
                         self.assertEqual(comment, 'my comment')
                         break
             elif rulenum == 2:
-                for match in rule.get_match_list():
+                for match in rule:
                     if isinstance(match, CommentMatch):
                         comment = match.comment().get_value()
                         self.assertEqual(comment, 'another comment')
                         break
             elif rulenum == 3:
                 cit = iter(['another comment', 'foo bar'])
-                for match in rule.get_match_list():
+                for match in rule:
                     if isinstance(match, CommentMatch):
                         comment = match.comment().get_value()
                         self.assertEqual(comment, next(cit))
 
     def test_parsing_addrtype_match(self):
         """Parse output with ADDRTYPE match
         """
@@ -550,63 +523,49 @@
        0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           ADDRTYPE match src-type !BLACKHOLE dst-type !UNICAST limit-in LOG flags 0 level 4 prefix `ADDR '
        0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           ADDRTYPE match src-type MULTICAST limit-out LOG flags 0 level 4 prefix `MCAST '
        0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           ADDRTYPE match src-type PROHIBIT /* PROHIBIT */ LOG flags 0 level 4 prefix `PROH '
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rule_list = input_chain.get_rules()
-        #
-        # Check 1st rule
-        #
-        rule = rule_list[0]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[0]
-        src_addr_type = match.src_addr_type()
-        self.assertTrue(src_addr_type.is_positive() and
-                        src_addr_type.get_value() == 'UNICAST')
-        dst_addr_type = match.dst_addr_type()
-        self.assertTrue(not dst_addr_type.is_positive() and
-                        dst_addr_type.get_value() == 'UNICAST')
-        #
-        # Check 2nd rule
-        #
-        rule = rule_list[1]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[0]
-        src_addr_type = match.src_addr_type()
-        self.assertTrue(not src_addr_type.is_positive() and
-                        src_addr_type.get_value() == 'BLACKHOLE')
-        dst_addr_type = match.dst_addr_type()
-        self.assertTrue(not dst_addr_type.is_positive() and
-                        dst_addr_type.get_value() == 'UNICAST')
-        self.assertTrue(match.limit_iface_in().is_positive())
-        #
-        # Check 3rd rule
-        #
-        rule = rule_list[2]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 1)
-        match = match_list[0]
-        src_addr_type = match.src_addr_type()
-        self.assertTrue(src_addr_type.is_positive() and
-                        src_addr_type.get_value() == 'MULTICAST')
-        self.assertTrue(match.limit_iface_out().is_positive())
-        #
-        # Check 4th rule
-        #
-        rule = rule_list[3]
-        match_list = rule.get_match_list()
-        self.assertEqual(len(match_list), 2)
-        match = match_list[0]
-        src_addr_type = match.src_addr_type()
-        self.assertTrue(src_addr_type.is_positive() and
-                        src_addr_type.get_value() == 'PROHIBIT')
+        for rule in input_chain:
+            rulenum = rule.get_rulenum()
+            if rulenum == 1:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                src_addr_type = match.src_addr_type()
+                self.assertTrue(src_addr_type.is_positive() and
+                                src_addr_type.get_value() == 'UNICAST')
+                dst_addr_type = match.dst_addr_type()
+                self.assertTrue(not dst_addr_type.is_positive() and
+                                dst_addr_type.get_value() == 'UNICAST')
+            elif rulenum == 2:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                src_addr_type = match.src_addr_type()
+                self.assertTrue(not src_addr_type.is_positive() and
+                                src_addr_type.get_value() == 'BLACKHOLE')
+                dst_addr_type = match.dst_addr_type()
+                self.assertTrue(not dst_addr_type.is_positive() and
+                                dst_addr_type.get_value() == 'UNICAST')
+                self.assertTrue(match.limit_iface_in().is_positive())
+            elif rulenum == 3:
+                self.assertEqual(rule.get_match_count(), 1)
+                match = next(iter(rule))
+                src_addr_type = match.src_addr_type()
+                self.assertTrue(src_addr_type.is_positive() and
+                                src_addr_type.get_value() == 'MULTICAST')
+                self.assertTrue(match.limit_iface_out().is_positive())
+            elif rulenum == 4:
+                match_list = rule.get_match_list()
+                self.assertEqual(len(match_list), 2)
+                match = match_list[0]
+                src_addr_type = match.src_addr_type()
+                self.assertTrue(src_addr_type.is_positive() and
+                                src_addr_type.get_value() == 'PROHIBIT')
 
     def test_parsing_unknown_match(self):
         """Parse output with unknown match
         """
         output = """\
 Chain INPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
@@ -655,15 +614,15 @@
     pkts      bytes target     prot opt in     out     source               destination
   487148 21609270 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           limit: avg 15/min burst 5 LOG flags 12 level 6 prefix `DROP-INPUT: '
   520139 23069461 DROP       all  --  *      *       0.0.0.0/0            0.0.0.0/0
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rule = input_chain.get_rules()[0]
+        rule = next(iter(input_chain))
         target = rule.get_target()
         self.assertEqual(target.get_log_prefix(), 'DROP-INPUT: ')
         self.assertEqual(target.get_log_level(), '6')
         self.assertTrue(target.is_logging_uid())
         self.assertTrue(target.is_logging_ip_options())
         self.assertFalse(target.is_logging_tcp_options())
         self.assertFalse(target.is_logging_tcp_sequence())
@@ -676,15 +635,15 @@
     pkts      bytes target     prot opt in     out     source               destination
      144    57620 REJECT     all  --  *      *       0.0.0.0/0            0.0.0.0/0           reject-with icmp-host-unreachable
   520139 23069461 ACCEPT     all  --  *      *       0.0.0.0/0            0.0.0.0/0
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        rule = input_chain.get_rules()[0]
+        rule = next(iter(input_chain))
         target = rule.get_target()
         self.assertTrue(isinstance(target, RejectTarget))
         self.assertEqual(target.get_rejection_message(),
                                 'icmp-host-unreachable')
 
     def test_parsing_mark_target(self):
         """Parse output with MARK target
@@ -697,45 +656,47 @@
     0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK xor 0xf 
     0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK or 0xf 
     0     0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           MARK and 0xff 
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
         pft = IptablesPacketFilterTable('filter')
         self.assertTrue(pft.init_from_output(output))
         input_chain = pft.get_builtin_chain('INPUT')
-        # Verify SET
-        rule = input_chain.get_rules()[0]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MarkTarget))
-        self.assertEqual(target.get_op(), MarkTarget.SET)
-        self.assertEqual(target.get_mark(), 0xf)
-        # Verify XSET
-        rule = input_chain.get_rules()[1]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MarkTarget))
-        self.assertEqual(target.get_op(), MarkTarget.XSET)
-        self.assertEqual(target.get_mark(), 0x11)
-        self.assertEqual(target.get_mask(), 0xffff0011)
-        # Verify XOR
-        rule = input_chain.get_rules()[2]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MarkTarget))
-        self.assertEqual(target.get_op(), MarkTarget.XOR)
-        self.assertEqual(target.get_mask(), 0xf)
-        # Verify OR
-        rule = input_chain.get_rules()[3]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MarkTarget))
-        self.assertEqual(target.get_op(), MarkTarget.OR)
-        self.assertEqual(target.get_mask(), 0xf)
-        # Verify AND
-        rule = input_chain.get_rules()[4]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MarkTarget))
-        self.assertEqual(target.get_op(), MarkTarget.AND)
-        self.assertEqual(target.get_mask(), 0xff)
+        for rule in input_chain:
+            rulenum = rule.get_rulenum()
+            if rulenum == 1:
+                # Verify SET
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, MarkTarget))
+                self.assertEqual(target.get_op(), MarkTarget.SET)
+                self.assertEqual(target.get_mark(), 0xf)
+            elif rulenum == 2:
+                # Verify XSET
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, MarkTarget))
+                self.assertEqual(target.get_op(), MarkTarget.XSET)
+                self.assertEqual(target.get_mark(), 0x11)
+                self.assertEqual(target.get_mask(), 0xffff0011)
+            elif rulenum == 3:
+                # Verify XOR
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, MarkTarget))
+                self.assertEqual(target.get_op(), MarkTarget.XOR)
+                self.assertEqual(target.get_mask(), 0xf)
+            elif rulenum == 4:
+                # Verify OR
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, MarkTarget))
+                self.assertEqual(target.get_op(), MarkTarget.OR)
+                self.assertEqual(target.get_mask(), 0xf)
+            elif rulenum == 5:
+                # Verify AND
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, MarkTarget))
+                self.assertEqual(target.get_op(), MarkTarget.AND)
+                self.assertEqual(target.get_mask(), 0xff)
 
     def test_parsing_connmark_target(self):
         """Parse output with CONNMARK target
         """
         output = ("""\
 Chain PREROUTING (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
@@ -743,30 +704,33 @@
   558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK save nfmask 0xfffff ctmask ~0x1f
   558864 28503489 CONNMARK   all  --  *      *       0.0.0.0/0            0.0.0.0/0           connmark match 0x0 CONNMARK restore ctmask 0x1f nfmask ~0xfffff
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT + '\n' +
                 self.EMPTY_INPUT + '\n' + self.EMPTY_POSTROUTING)
         pft = IptablesPacketFilterTable('mangle')
         self.assertTrue(pft.init_from_output(output))
         prerouting_chain = pft.get_builtin_chain('PREROUTING')
-        rule = prerouting_chain.get_rules()[0]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, ConnmarkTarget))
-        self.assertEqual(target.get_mark(), 0x11)
-        rule = prerouting_chain.get_rules()[1]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, ConnmarkTarget) and
+        self.assertEqual(prerouting_chain.get_rule_count(), 3)
+        for rule in prerouting_chain:
+            rulenum = rule.get_rulenum()
+            if rulenum == 1:
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, ConnmarkTarget))
+                self.assertEqual(target.get_mark(), 0x11)
+            elif rulenum == 2:
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, ConnmarkTarget) and
                                 target.is_saving_mark())
-        self.assertEqual(target.get_nfmask(), 0xfffff)
-        self.assertEqual(target.get_ctmask(), 0x1f)
-        rule = prerouting_chain.get_rules()[2]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, ConnmarkTarget) and
+                self.assertEqual(target.get_nfmask(), 0xfffff)
+                self.assertEqual(target.get_ctmask(), 0x1f)
+            elif rulenum == 3:
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, ConnmarkTarget) and
                                 target.is_restoring_mark())
-        self.assertEqual(target.get_nfmask(), 0xfffff)
-        self.assertEqual(target.get_ctmask(), 0x1f)
+                self.assertEqual(target.get_nfmask(), 0xfffff)
+                self.assertEqual(target.get_ctmask(), 0x1f)
 
     def test_parsing_ttl_target(self):
         """Parse output with TTL target
         """
         output = ("""\
 Chain PREROUTING (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
@@ -774,39 +738,40 @@
        0        0 TTL        tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL increment by 1 
        0        0 TTL        udp  --  *      *       0.0.0.0/0            0.0.0.0/0           TTL decrement by 2 
 """ + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT + '\n' +
                 self.EMPTY_INPUT + '\n' + self.EMPTY_POSTROUTING)
         pft = IptablesPacketFilterTable('mangle')
         self.assertTrue(pft.init_from_output(output))
         prerouting_chain = pft.get_builtin_chain('PREROUTING')
-        rule = prerouting_chain.get_rules()[0]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, TtlTarget) and
+        for rule in prerouting_chain:
+            rulenum = rule.get_rulenum()
+            target = rule.get_target()
+            if rulenum == 1:
+                self.assertTrue(isinstance(target, TtlTarget) and
                                 target.get_ttl_value() == 10)
-        rule = prerouting_chain.get_rules()[1]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, TtlTarget) and
+            elif rulenum == 2:
+                self.assertTrue(isinstance(target, TtlTarget) and
                                 target.get_ttl_inc() == 1)
-        rule = prerouting_chain.get_rules()[2]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, TtlTarget) and
+            elif rulenum == 3:
+                target = rule.get_target()
+                self.assertTrue(isinstance(target, TtlTarget) and
                                 target.get_ttl_dec() == 2)
 
     def test_parsing_snat_target(self):
         """Parse output with SNAT target
         """
         output = (self.EMPTY_PREROUTING + '\n' + """\
 Chain POSTROUTING (1 references)
     pkts      bytes target     prot opt in     out     source               destination         
   466007 51946882 SNAT       all  --  *      eth1    0.0.0.0/0            0.0.0.0/0           to:10.10.10.18 
 """ + '\n' + self.EMPTY_OUTPUT)
         pft = IptablesPacketFilterTable('nat')
         self.assertTrue(pft.init_from_output(output))
         postrouting_chain = pft.get_builtin_chain('POSTROUTING')
-        rule = postrouting_chain.get_rules()[0]
+        rule = next(iter(postrouting_chain))
         target = rule.get_target()
         self.assertEqual(target.get_target_name(), 'SNAT')
         self.assertEqual(target.get_address(), IPv4Address('10.10.10.18'))
 
     def test_parsing_masquerade_target(self):
         """Parse output with MASQUERADE target
         """
@@ -818,62 +783,61 @@
        0        0 MASQUERADE  tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           masq ports: 2000 
        0        0 MASQUERADE  udp  --  *      *       0.0.0.0/0            0.0.0.0/0           udp spts:1000:2000 masq ports: 2000 random 
        0        0 MASQUERADE  udp  --  *      *       0.0.0.0/0            0.0.0.0/0           udp spts:1000:2000 masq ports: 20000-30000
 """ + '\n' + self.EMPTY_OUTPUT)
         pft = IptablesPacketFilterTable('nat')
         self.assertTrue(pft.init_from_output(output))
         postrouting_chain = pft.get_builtin_chain('POSTROUTING')
-        rule = postrouting_chain.get_rules()[0]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MasqueradeTarget))
-        rule = postrouting_chain.get_rules()[1]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MasqueradeTarget) and
+        self.assertEqual(postrouting_chain.get_rule_count(), 5)
+        for rule in postrouting_chain:
+            rulenum = rule.get_rulenum()
+            target = rule.get_target()
+            if rulenum == 1:
+                self.assertTrue(isinstance(target, MasqueradeTarget))
+            elif rulenum == 2:
+                self.assertTrue(isinstance(target, MasqueradeTarget) and
                                 target.uses_random_port_mapping())
-        rule = postrouting_chain.get_rules()[2]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MasqueradeTarget) and
+            elif rulenum == 3:
+                self.assertTrue(isinstance(target, MasqueradeTarget) and
                                 target.get_ports() == (2000, None))
-        rule = postrouting_chain.get_rules()[3]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MasqueradeTarget) and
+            elif rulenum == 4:
+                self.assertTrue(isinstance(target, MasqueradeTarget) and
                             target.get_ports() == (2000, None) and
                                 target.uses_random_port_mapping())
-        rule = postrouting_chain.get_rules()[4]
-        target = rule.get_target()
-        self.assertTrue(isinstance(target, MasqueradeTarget) and
+            elif rulenum == 5:
+                self.assertTrue(isinstance(target, MasqueradeTarget) and
                                 target.get_ports() == (20000, 30000))
 
     def test_parsing_notrack_target(self):
         """Parse output with NOTRACK target
         """
         output = (self.EMPTY_PREROUTING + '\n' + """\
 Chain OUTPUT (policy ACCEPT 12 packets, 1845 bytes)
  pkts bytes target     prot opt in     out     source               destination
     0     0 NOTRACK    tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp dpt:55555
 """)
         pft = IptablesPacketFilterTable('raw')
         self.assertTrue(pft.init_from_output(output))
         output_chain = pft.get_builtin_chain('OUTPUT')
-        rule = output_chain.get_rules()[0]
+        rule = next(iter(output_chain))
         target = rule.get_target()
         self.assertTrue(isinstance(target, NoTrackTarget))
 
     def test_parsing_trace_target(self):
         """Parse output with TRACE target
         """
         output = (self.EMPTY_PREROUTING + '\n' + """\
 Chain OUTPUT (policy ACCEPT 12 packets, 1845 bytes)
  pkts bytes target     prot opt in     out     source               destination
     0     0 TRACE      tcp  --  *      *       0.0.0.0/0            0.0.0.0/0           tcp dpt:55555
 """)
         pft = IptablesPacketFilterTable('raw')
         self.assertTrue(pft.init_from_output(output))
         output_chain = pft.get_builtin_chain('OUTPUT')
-        rule = output_chain.get_rules()[0]
+        rule = next(iter(output_chain))
         target = rule.get_target()
         self.assertTrue(isinstance(target, TraceTarget))
 
     def test_parsing_unknown_target(self):
         """Parse output with unknown target
         """
         output = """\
@@ -1025,18 +989,28 @@
     def test_zero_counters(self):
         """Test that the correct command is issued to zero counters
         """
         runner = SimulatedIptablesRun(0, None)
         pft = IptablesPacketFilterTable('filter', runner=runner)
         init_ok = pft.init_from_output(self.GOOD_OUTPUT)
         self.assertTrue(init_ok)
-        chain = pft.get_builtin_chain('OUTPUT')
         #
         # Zero the counters of a specific chain
         #
+        chain = pft.get_builtin_chain('FORWARD')
+        rule = next(iter(chain))
+        rule.zero_counters()
+        expected_cmd = ['iptables', '-t', 'filter', '-Z', 'FORWARD', '1']
+        commands = runner.get_run()
+        self.assertEqual(commands[0].cmd, expected_cmd)
+        #
+        # Zero the counters of a specific chain
+        #
+        runner.clear_run()
+        chain = pft.get_builtin_chain('OUTPUT')
         chain.zero_counters()
         expected_cmd = ['iptables', '-t', 'filter', '-Z', 'OUTPUT']
         commands = runner.get_run()
         self.assertEqual(commands[0].cmd, expected_cmd)
         #
         # Zero the counters of all chains
         #
@@ -1102,15 +1076,15 @@
         expected_cmd = ['iptables', '-t', 'filter', '-P', 'OUTPUT',
                                         Targets.DROP.get_target_name()]
         commands = runner.get_run()
         self.assertEqual(commands[0].cmd, expected_cmd)
 
 
 class TestChainOperations(unittest.TestCase):
-    """Test chain operations. The runner is a no-op
+    """Test chain operations.
     """
 
     @staticmethod
     def _runner(*args, **kwargs):
         """Runner that logs the arguments without invoking iptables(8)
         """
         root_logger.info("Executing: args=%s kwargs=%s", args, kwargs)
@@ -1200,14 +1174,88 @@
         self.assertEqual(commands[2].cmd,
                         ['iptables', '-t', 'filter', '-F', 'test_chain_1'])
         self.assertEqual(commands[3].cmd,
                         ['iptables', '-t', 'filter', '-X', 'test_chain_1'])
         self.assertEqual(len(chain2.get_rules()), 0)
         self.assertEqual(len(chain3.get_rules()), 0)
 
+    def test_rule_enumeration(self):
+        """Rule enumeration
+        """
+        runner = SimulatedIptablesRun(0, None)
+        pft = IptablesPacketFilterTable('filter', runner=runner)
+        #
+        # We create the following structure:
+        #
+        #  jump_target:
+        #  goto_target:
+        #  caller_chain:
+        #       -m owner --uid-owner 10 --gid-owner 1 -j RETURN (1 match)
+        #       -p tcp --dport 22 -j jump_target                (2 matches, chain-target)
+        #       -p tcp -j DROP                                  (1 match)
+        #       -p udp -g goto_target                           (1 match, chain-target-goto)
+        #       -j jump_target                                  (0 matches, chain-target)
+        #
+        jump_target = pft.create_chain('jump_target')
+        goto_target = pft.create_chain('goto_target')
+        chain = pft.create_chain('caller_chain')
+        chain.append_rule(ChainRule(
+                match=OwnerMatch().uid().equals(10).gid().equals(1),
+                target=Targets.RETURN))
+        chain.append_rule(ChainRule(
+                match_list=[
+                        PacketMatch().protocol().equals('tcp'),
+                        TcpMatch().dest_port().equals(22),
+                        ],
+                target=ChainTarget(chain=jump_target)))
+        chain.append_rule(ChainRule(
+                match=PacketMatch().protocol().equals('tcp'),
+                target=Targets.DROP))
+        chain.append_rule(ChainRule(
+                match=PacketMatch().protocol().equals('udp')
+                        ).go_to(chain=goto_target))
+        chain.append_rule(ChainRule(
+                target=ChainTarget(chain=jump_target)))
+        #
+        # 3 rules target chains
+        #
+        rules_to_chains = list(chain.iter_rules(chain_target=True))
+        self.assertEqual(len(rules_to_chains), 3)
+        #
+        # 1 rule uses goto
+        #
+        rules_go_to_chains = list(chain.iter_rules(uses_goto=True))
+        self.assertEqual(len(rules_go_to_chains), 1)
+        #
+        # 3 rules with a single match
+        #
+        single_match_rules = list(chain.iter_rules(match_count=1))
+        self.assertEqual(len(single_match_rules), 3)
+        #
+        # 1 rule with a single match and a chain target
+        #
+        single_match_rules_to_chains = list(
+                chain.iter_rules(chain_target=True, match_count=1))
+        self.assertEqual(len(single_match_rules_to_chains), 1)
+        #
+        # 1 rule with a match for TCP dest port 22
+        #
+        port22_rules = list(chain.iter_rules(match=TcpMatch().dest_port().equals(22)))
+        self.assertEqual(len(port22_rules), 1)
+        #
+        # 1 rule with a PacketMatch that uses goto
+        #
+        packet_goto_rules = list(chain.iter_rules(match=PacketMatch(), uses_goto=True))
+        self.assertEqual(len(packet_goto_rules), 1)
+        #
+        # 1 rule with a match with 2 criteria
+        #
+        rules = list(chain.iter_rules(match=OwnerMatch().uid().any().gid().equals(1)))
+        self.assertEqual(len(rules), 1)
+
     def test_rule_operations(self):
         """Rule search, deletion
         """
         runner = SimulatedIptablesRun(0, None)
         pft = IptablesPacketFilterTable('filter', runner=runner)
         #
         # We create the following structure:
```

