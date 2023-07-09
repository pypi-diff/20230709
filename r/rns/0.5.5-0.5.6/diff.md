# Comparing `tmp/rns-0.5.5.tar.gz` & `tmp/rns-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rns-0.5.5.tar", last modified: Tue Jun 13 17:22:49 2023, max compression
+gzip compressed data, was "rns-0.5.6.tar", last modified: Sun Jul  9 14:47:38 2023, max compression
```

## Comparing `rns-0.5.5.tar` & `rns-0.5.6.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rns-0.5.5/LICENSE
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-06-13 17:22:49.632865 rns-0.5.5/PKG-INFO
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rns-0.5.5/README.md
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10926 2023-05-18 23:54:43.000000 rns-0.5.5/RNS/Buffer.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24736 2023-05-18 23:37:50.000000 rns-0.5.5/RNS/Channel.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/Cryptography/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/AES.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Fernet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rns-0.5.5/RNS/Cryptography/HKDF.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/HMAC.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Hashes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/PKCS7.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Provider.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/Proxies.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/SHA256.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/SHA512.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/X25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/Cryptography/aes/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/aes/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/aes/aes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/aes/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.626198 rns-0.5.5/RNS/Cryptography/pure25519/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/_ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/basic.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/ed25519_oop.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Cryptography/pure25519/eddsa.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rns-0.5.5/RNS/Destination.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24048 2023-05-31 13:38:00.000000 rns-0.5.5/RNS/Identity.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/Interfaces/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/AX25KISSInterface.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/Interfaces/Android/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rns-0.5.5/RNS/Interfaces/Android/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49069 2023-06-13 14:11:28.000000 rns-0.5.5/RNS/Interfaces/Android/RNodeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rns-0.5.5/RNS/Interfaces/Android/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rns-0.5.5/RNS/Interfaces/Android/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20327 2023-05-11 17:33:15.000000 rns-0.5.5/RNS/Interfaces/AutoInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rns-0.5.5/RNS/Interfaces/I2PInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/Interface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-10 13:51:28.000000 rns-0.5.5/RNS/Interfaces/LocalInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/PipeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30665 2023-06-13 14:11:28.000000 rns-0.5.5/RNS/Interfaces/RNodeInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Interfaces/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rns-0.5.5/RNS/Interfaces/TCPInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rns-0.5.5/RNS/Interfaces/UDPInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rns-0.5.5/RNS/Interfaces/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    53726 2023-06-13 17:05:12.000000 rns-0.5.5/RNS/Link.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22263 2023-05-18 14:48:32.000000 rns-0.5.5/RNS/Packet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45887 2023-05-10 13:26:58.000000 rns-0.5.5/RNS/Resource.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rns-0.5.5/RNS/Reticulum.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   130124 2023-06-13 17:09:12.000000 rns-0.5.5/RNS/Transport.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/Utilities/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Utilities/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    15089 2023-05-31 13:39:02.000000 rns-0.5.5/RNS/Utilities/rncp.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-05-09 18:30:37.000000 rns-0.5.5/RNS/Utilities/rnid.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)   208368 2023-05-31 19:25:17.000000 rns-0.5.5/RNS/Utilities/rnodeconf.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Utilities/rnpath.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/Utilities/rnprobe.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rns-0.5.5/RNS/Utilities/rnsd.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rns-0.5.5/RNS/Utilities/rnstatus.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rns-0.5.5/RNS/Utilities/rnx.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rns-0.5.5/RNS/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-06-13 12:55:02.000000 rns-0.5.5/RNS/_version.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.629532 rns-0.5.5/RNS/vendor/
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/__init__.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/configobj.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/RNS/vendor/i2plib/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/__version__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/aiosam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/exceptions.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/log.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/sam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/tunnel.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/i2plib/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/RNS/vendor/ifaddr/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rns-0.5.5/RNS/vendor/ifaddr/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rns-0.5.5/RNS/vendor/ifaddr/_posix.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rns-0.5.5/RNS/vendor/ifaddr/_shared.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rns-0.5.5/RNS/vendor/ifaddr/_win32.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rns-0.5.5/RNS/vendor/ifaddr/niwrapper.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rns-0.5.5/RNS/vendor/platformutils.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/six.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rns-0.5.5/RNS/vendor/umsgpack.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-06-13 17:22:49.632865 rns-0.5.5/rns.egg-info/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/PKG-INFO
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2237 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/SOURCES.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/dependency_links.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/entry_points.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       34 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/requires.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-06-13 17:22:49.000000 rns-0.5.5/rns.egg-info/top_level.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-06-13 17:22:49.632865 rns-0.5.5/setup.cfg
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rns-0.5.5/setup.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.173252 rns-0.5.6/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rns-0.5.6/LICENSE
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-07-09 14:47:38.173252 rns-0.5.6/PKG-INFO
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rns-0.5.6/README.md
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.166585 rns-0.5.6/RNS/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10926 2023-05-18 23:54:43.000000 rns-0.5.6/RNS/Buffer.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24736 2023-05-18 23:37:50.000000 rns-0.5.6/RNS/Channel.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.166585 rns-0.5.6/RNS/Cryptography/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/AES.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/Ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/Fernet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rns-0.5.6/RNS/Cryptography/HKDF.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/HMAC.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/Hashes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/PKCS7.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/Provider.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/Proxies.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/SHA256.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/SHA512.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/X25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.166585 rns-0.5.6/RNS/Cryptography/aes/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/aes/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/aes/aes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/aes/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.166585 rns-0.5.6/RNS/Cryptography/pure25519/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/pure25519/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/pure25519/_ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/pure25519/basic.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/pure25519/ed25519_oop.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Cryptography/pure25519/eddsa.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rns-0.5.6/RNS/Destination.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24048 2023-05-31 13:38:00.000000 rns-0.5.6/RNS/Identity.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.169918 rns-0.5.6/RNS/Interfaces/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Interfaces/AX25KISSInterface.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.169918 rns-0.5.6/RNS/Interfaces/Android/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rns-0.5.6/RNS/Interfaces/Android/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49069 2023-06-13 14:11:28.000000 rns-0.5.6/RNS/Interfaces/Android/RNodeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rns-0.5.6/RNS/Interfaces/Android/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rns-0.5.6/RNS/Interfaces/Android/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20327 2023-05-11 17:33:15.000000 rns-0.5.6/RNS/Interfaces/AutoInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rns-0.5.6/RNS/Interfaces/I2PInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Interfaces/Interface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Interfaces/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-10 13:51:28.000000 rns-0.5.6/RNS/Interfaces/LocalInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Interfaces/PipeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30665 2023-06-13 14:11:28.000000 rns-0.5.6/RNS/Interfaces/RNodeInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Interfaces/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rns-0.5.6/RNS/Interfaces/TCPInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rns-0.5.6/RNS/Interfaces/UDPInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rns-0.5.6/RNS/Interfaces/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    53726 2023-06-13 17:05:12.000000 rns-0.5.6/RNS/Link.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22263 2023-05-18 14:48:32.000000 rns-0.5.6/RNS/Packet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45887 2023-05-10 13:26:58.000000 rns-0.5.6/RNS/Resource.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rns-0.5.6/RNS/Reticulum.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   130124 2023-06-13 17:09:12.000000 rns-0.5.6/RNS/Transport.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.169918 rns-0.5.6/RNS/Utilities/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Utilities/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    15089 2023-05-31 13:39:02.000000 rns-0.5.6/RNS/Utilities/rncp.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-07-09 14:05:37.000000 rns-0.5.6/RNS/Utilities/rnid.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)   208368 2023-06-29 20:12:30.000000 rns-0.5.6/RNS/Utilities/rnodeconf.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Utilities/rnpath.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/Utilities/rnprobe.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rns-0.5.6/RNS/Utilities/rnsd.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rns-0.5.6/RNS/Utilities/rnstatus.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rns-0.5.6/RNS/Utilities/rnx.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7103 2023-06-29 20:12:30.000000 rns-0.5.6/RNS/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-07-09 14:45:38.000000 rns-0.5.6/RNS/_version.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.169918 rns-0.5.6/RNS/vendor/
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/__init__.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/configobj.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.173252 rns-0.5.6/RNS/vendor/i2plib/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/__version__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/aiosam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/exceptions.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/log.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/sam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/tunnel.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/i2plib/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.173252 rns-0.5.6/RNS/vendor/ifaddr/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rns-0.5.6/RNS/vendor/ifaddr/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rns-0.5.6/RNS/vendor/ifaddr/_posix.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rns-0.5.6/RNS/vendor/ifaddr/_shared.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rns-0.5.6/RNS/vendor/ifaddr/_win32.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rns-0.5.6/RNS/vendor/ifaddr/niwrapper.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rns-0.5.6/RNS/vendor/platformutils.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/six.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rns-0.5.6/RNS/vendor/umsgpack.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-07-09 14:47:38.173252 rns-0.5.6/rns.egg-info/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18454 2023-07-09 14:47:38.000000 rns-0.5.6/rns.egg-info/PKG-INFO
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2237 2023-07-09 14:47:38.000000 rns-0.5.6/rns.egg-info/SOURCES.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-07-09 14:47:38.000000 rns-0.5.6/rns.egg-info/dependency_links.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-07-09 14:47:38.000000 rns-0.5.6/rns.egg-info/entry_points.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       34 2023-07-09 14:47:38.000000 rns-0.5.6/rns.egg-info/requires.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-07-09 14:47:38.000000 rns-0.5.6/rns.egg-info/top_level.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-07-09 14:47:38.173252 rns-0.5.6/setup.cfg
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rns-0.5.6/setup.py
```

### Comparing `rns-0.5.5/LICENSE` & `rns-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/PKG-INFO` & `rns-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rns
-Version: 0.5.5
+Version: 0.5.6
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rns-0.5.5/README.md` & `rns-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Buffer.py` & `rns-0.5.6/RNS/Buffer.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Channel.py` & `rns-0.5.6/RNS/Channel.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/AES.py` & `rns-0.5.6/RNS/Cryptography/AES.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/Ed25519.py` & `rns-0.5.6/RNS/Cryptography/Ed25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/Fernet.py` & `rns-0.5.6/RNS/Cryptography/Fernet.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/HKDF.py` & `rns-0.5.6/RNS/Cryptography/HKDF.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/HMAC.py` & `rns-0.5.6/RNS/Cryptography/HMAC.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/Hashes.py` & `rns-0.5.6/RNS/Cryptography/Hashes.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/PKCS7.py` & `rns-0.5.6/RNS/Cryptography/PKCS7.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/Provider.py` & `rns-0.5.6/RNS/Cryptography/Provider.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/Proxies.py` & `rns-0.5.6/RNS/Cryptography/Proxies.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/SHA256.py` & `rns-0.5.6/RNS/Cryptography/SHA256.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/SHA512.py` & `rns-0.5.6/RNS/Cryptography/SHA512.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/X25519.py` & `rns-0.5.6/RNS/Cryptography/X25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/__init__.py` & `rns-0.5.6/RNS/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/aes/aes.py` & `rns-0.5.6/RNS/Cryptography/aes/aes.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/aes/utils.py` & `rns-0.5.6/RNS/Cryptography/aes/utils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/pure25519/_ed25519.py` & `rns-0.5.6/RNS/Cryptography/pure25519/_ed25519.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/pure25519/basic.py` & `rns-0.5.6/RNS/Cryptography/pure25519/basic.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/pure25519/ed25519_oop.py` & `rns-0.5.6/RNS/Cryptography/pure25519/ed25519_oop.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Cryptography/pure25519/eddsa.py` & `rns-0.5.6/RNS/Cryptography/pure25519/eddsa.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Destination.py` & `rns-0.5.6/RNS/Destination.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Identity.py` & `rns-0.5.6/RNS/Identity.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/AX25KISSInterface.py` & `rns-0.5.6/RNS/Interfaces/AX25KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/Android/KISSInterface.py` & `rns-0.5.6/RNS/Interfaces/Android/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/Android/RNodeInterface.py` & `rns-0.5.6/RNS/Interfaces/Android/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/Android/SerialInterface.py` & `rns-0.5.6/RNS/Interfaces/Android/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/Android/__init__.py` & `rns-0.5.6/RNS/Interfaces/Android/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/AutoInterface.py` & `rns-0.5.6/RNS/Interfaces/AutoInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/I2PInterface.py` & `rns-0.5.6/RNS/Interfaces/I2PInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/Interface.py` & `rns-0.5.6/RNS/Interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/KISSInterface.py` & `rns-0.5.6/RNS/Interfaces/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/LocalInterface.py` & `rns-0.5.6/RNS/Interfaces/LocalInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/PipeInterface.py` & `rns-0.5.6/RNS/Interfaces/PipeInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/RNodeInterface.py` & `rns-0.5.6/RNS/Interfaces/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/SerialInterface.py` & `rns-0.5.6/RNS/Interfaces/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/TCPInterface.py` & `rns-0.5.6/RNS/Interfaces/TCPInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/UDPInterface.py` & `rns-0.5.6/RNS/Interfaces/UDPInterface.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Interfaces/__init__.py` & `rns-0.5.6/RNS/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Link.py` & `rns-0.5.6/RNS/Link.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Packet.py` & `rns-0.5.6/RNS/Packet.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Resource.py` & `rns-0.5.6/RNS/Resource.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Reticulum.py` & `rns-0.5.6/RNS/Reticulum.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Transport.py` & `rns-0.5.6/RNS/Transport.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Utilities/__init__.py` & `rns-0.5.6/RNS/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Utilities/rncp.py` & `rns-0.5.6/RNS/Utilities/rncp.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Utilities/rnid.py` & `rns-0.5.6/RNS/Utilities/rnid.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         parser.add_argument("--config", metavar="path", action="store", default=None, help="path to alternative Reticulum config directory", type=str)
         parser.add_argument("-i", "--identity", metavar="identity", action="store", default=None, help="hexadecimal Reticulum Destination hash or path to Identity file", type=str)
         parser.add_argument("-g", "--generate", metavar="path", action="store", default=None, help="generate a new Identity")
         parser.add_argument("-v", "--verbose", action="count", default=0, help="increase verbosity")
         parser.add_argument("-q", "--quiet", action="count", default=0, help="decrease verbosity")
 
         parser.add_argument("-a", "--announce", metavar="aspects", action="store", default=None, help="announce a destination based on this Identity")
-        parser.add_argument("-H", "--hash", metavar="aspects", action="store", default=None, help="show destination hash5s for other aspects for this Identity")
+        parser.add_argument("-H", "--hash", metavar="aspects", action="store", default=None, help="show destination hashes for other aspects for this Identity")
         parser.add_argument("-e", "--encrypt", metavar="path", action="store", default=None, help="encrypt file")
         parser.add_argument("-d", "--decrypt", metavar="path", action="store", default=None, help="decrypt file")
         parser.add_argument("-s", "--sign", metavar="path", action="store", default=None, help="sign file")
         parser.add_argument("-V", "--validate", metavar="path", action="store", default=None, help="validate signature")
 
         parser.add_argument("-r", "--read", metavar="path", action="store", default=None, help="input file path", type=str)
         parser.add_argument("-w", "--write", metavar="path", action="store", default=None, help="output file path", type=str)
```

### Comparing `rns-0.5.5/RNS/Utilities/rnodeconf.py` & `rns-0.5.6/RNS/Utilities/rnodeconf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1490,15 +1490,15 @@
             print("")
             print("---------------------------------------------------------------------------")
             print("\nEnter the number that matches your device type:\n? ", end="")
 
             selected_product = None
             try:
                 c_dev = int(input())
-                if c_dev < 1 or c_dev > 6:
+                if c_dev < 1 or c_dev > 7:
                     raise ValueError()
                 elif c_dev == 1:
                     selected_product = ROM.PRODUCT_RNODE
                 elif c_dev == 2:
                     selected_product = ROM.PRODUCT_HMBRW
                     clear()
                     print("")
```

### Comparing `rns-0.5.5/RNS/Utilities/rnpath.py` & `rns-0.5.6/RNS/Utilities/rnpath.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Utilities/rnprobe.py` & `rns-0.5.6/RNS/Utilities/rnprobe.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Utilities/rnsd.py` & `rns-0.5.6/RNS/Utilities/rnsd.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Utilities/rnstatus.py` & `rns-0.5.6/RNS/Utilities/rnstatus.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/Utilities/rnx.py` & `rns-0.5.6/RNS/Utilities/rnx.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/__init__.py` & `rns-0.5.6/RNS/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 def timestamp_str(time_s):
     timestamp = time.localtime(time_s)
     return time.strftime(logtimefmt, timestamp)
 
 def log(msg, level=3, _override_destination = False):
     global _always_override_destination, compact_log_fmt
-    
+    msg = str(msg)
     if loglevel >= level:
         if not compact_log_fmt:
             logstring = "["+timestamp_str(time.time())+"] ["+loglevelname(level)+"] "+msg
         else:
             logstring = "["+timestamp_str(time.time())+"] "+msg
 
         logging_lock.acquire()
@@ -234,8 +234,8 @@
     print("Link Private Key Size       : "+str(Link.KEYSIZE*8)+" bits")
 
 def panic():
     os._exit(255)
 
 def exit():
     print("")
-    sys.exit(0)
+    sys.exit(0)
```

### Comparing `rns-0.5.5/RNS/vendor/configobj.py` & `rns-0.5.6/RNS/vendor/configobj.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/i2plib/__init__.py` & `rns-0.5.6/RNS/vendor/i2plib/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/i2plib/aiosam.py` & `rns-0.5.6/RNS/vendor/i2plib/aiosam.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/i2plib/exceptions.py` & `rns-0.5.6/RNS/vendor/i2plib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/i2plib/sam.py` & `rns-0.5.6/RNS/vendor/i2plib/sam.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/i2plib/tunnel.py` & `rns-0.5.6/RNS/vendor/i2plib/tunnel.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/i2plib/utils.py` & `rns-0.5.6/RNS/vendor/i2plib/utils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/ifaddr/__init__.py` & `rns-0.5.6/RNS/vendor/ifaddr/__init__.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/ifaddr/_posix.py` & `rns-0.5.6/RNS/vendor/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/ifaddr/_shared.py` & `rns-0.5.6/RNS/vendor/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/ifaddr/_win32.py` & `rns-0.5.6/RNS/vendor/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/ifaddr/niwrapper.py` & `rns-0.5.6/RNS/vendor/ifaddr/niwrapper.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/platformutils.py` & `rns-0.5.6/RNS/vendor/platformutils.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/six.py` & `rns-0.5.6/RNS/vendor/six.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/RNS/vendor/umsgpack.py` & `rns-0.5.6/RNS/vendor/umsgpack.py`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/rns.egg-info/PKG-INFO` & `rns-0.5.6/rns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rns
-Version: 0.5.5
+Version: 0.5.6
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rns-0.5.5/rns.egg-info/SOURCES.txt` & `rns-0.5.6/rns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rns-0.5.5/setup.py` & `rns-0.5.6/setup.py`

 * *Files identical despite different names*

