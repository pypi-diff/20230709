# Comparing `tmp/Blockthon-7.3.6.tar.gz` & `tmp/Blockthon-7.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-7.3.6.tar", last modified: Sun Jul  9 06:56:37 2023, max compression
+gzip compressed data, was "Blockthon-7.3.9.tar", last modified: Sun Jul  9 07:06:41 2023, max compression
```

## Comparing `Blockthon-7.3.6.tar` & `Blockthon-7.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-09 06:56:37.199376 Blockthon-7.3.6/
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-09 06:56:37.198444 Blockthon-7.3.6/Blockthon/
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1620 2023-07-02 03:33:53.000000 Blockthon-7.3.6/Blockthon/Bitcoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-7.3.6/Blockthon/BitcoinGold.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-7.3.6/Blockthon/Check.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-7.3.6/Blockthon/Dash.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-7.3.6/Blockthon/Digibyte.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-7.3.6/Blockthon/Dogecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-7.3.6/Blockthon/Ethereum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1292 2023-07-02 03:35:14.000000 Blockthon-7.3.6/Blockthon/Litecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-7.3.6/Blockthon/Qtum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-7.3.6/Blockthon/Ravencoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-7.3.6/Blockthon/Tron.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-7.3.6/Blockthon/Utils.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-7.3.6/Blockthon/Wallet.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      597 2023-07-02 03:31:21.000000 Blockthon-7.3.6/Blockthon/__init__.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    18089 2023-07-02 02:20:10.000000 Blockthon-7.3.6/Blockthon/lib.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-7.3.6/Blockthon/zCash.py
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-09 06:56:37.199007 Blockthon-7.3.6/Blockthon.egg-info/
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     9743 2023-07-09 06:56:37.000000 Blockthon-7.3.6/Blockthon.egg-info/PKG-INFO
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-09 06:56:37.000000 Blockthon-7.3.6/Blockthon.egg-info/SOURCES.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-09 06:56:37.000000 Blockthon-7.3.6/Blockthon.egg-info/dependency_links.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      144 2023-07-09 06:56:37.000000 Blockthon-7.3.6/Blockthon.egg-info/requires.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-09 06:56:37.000000 Blockthon-7.3.6/Blockthon.egg-info/top_level.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     9743 2023-07-09 06:56:37.199203 Blockthon-7.3.6/PKG-INFO
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     9303 2023-07-02 03:50:16.000000 Blockthon-7.3.6/README.md
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-09 06:56:37.199411 Blockthon-7.3.6/setup.cfg
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1464 2023-07-09 06:26:40.000000 Blockthon-7.3.6/setup.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-09 07:06:41.362480 Blockthon-7.3.9/
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-09 07:06:41.361592 Blockthon-7.3.9/Blockthon/
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1620 2023-07-02 03:33:53.000000 Blockthon-7.3.9/Blockthon/Bitcoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-7.3.9/Blockthon/BitcoinGold.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-7.3.9/Blockthon/Check.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-7.3.9/Blockthon/Dash.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-7.3.9/Blockthon/Digibyte.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-7.3.9/Blockthon/Dogecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-7.3.9/Blockthon/Ethereum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1292 2023-07-02 03:35:14.000000 Blockthon-7.3.9/Blockthon/Litecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-7.3.9/Blockthon/Qtum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-7.3.9/Blockthon/Ravencoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-7.3.9/Blockthon/Tron.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-7.3.9/Blockthon/Utils.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-7.3.9/Blockthon/Wallet.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      597 2023-07-02 03:31:21.000000 Blockthon-7.3.9/Blockthon/__init__.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    18089 2023-07-02 02:20:10.000000 Blockthon-7.3.9/Blockthon/lib.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-7.3.9/Blockthon/zCash.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-09 07:06:41.362160 Blockthon-7.3.9/Blockthon.egg-info/
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     9923 2023-07-09 07:06:41.000000 Blockthon-7.3.9/Blockthon.egg-info/PKG-INFO
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-09 07:06:41.000000 Blockthon-7.3.9/Blockthon.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-09 07:06:41.000000 Blockthon-7.3.9/Blockthon.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      144 2023-07-09 07:06:41.000000 Blockthon-7.3.9/Blockthon.egg-info/requires.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-09 07:06:41.000000 Blockthon-7.3.9/Blockthon.egg-info/top_level.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     9923 2023-07-09 07:06:41.362332 Blockthon-7.3.9/PKG-INFO
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     9485 2023-07-09 07:05:52.000000 Blockthon-7.3.9/README.md
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-09 07:06:41.362522 Blockthon-7.3.9/setup.cfg
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1464 2023-07-09 07:06:06.000000 Blockthon-7.3.9/setup.py
```

### Comparing `Blockthon-7.3.6/Blockthon/Bitcoin.py` & `Blockthon-7.3.9/Blockthon/Bitcoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-7.3.6/Blockthon/Check.py` & `Blockthon-7.3.9/Blockthon/Check.py`

 * *Files identical despite different names*

### Comparing `Blockthon-7.3.6/Blockthon/Litecoin.py` & `Blockthon-7.3.9/Blockthon/Litecoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-7.3.6/Blockthon/Utils.py` & `Blockthon-7.3.9/Blockthon/Utils.py`

 * *Files identical despite different names*

### Comparing `Blockthon-7.3.6/Blockthon/Wallet.py` & `Blockthon-7.3.9/Blockthon/Wallet.py`

 * *Files identical despite different names*

### Comparing `Blockthon-7.3.6/Blockthon/__init__.py` & `Blockthon-7.3.9/Blockthon/__init__.py`

 * *Files identical despite different names*

### Comparing `Blockthon-7.3.6/Blockthon/lib.py` & `Blockthon-7.3.9/Blockthon/lib.py`

 * *Files identical despite different names*

### Comparing `Blockthon-7.3.6/Blockthon.egg-info/PKG-INFO` & `Blockthon-7.3.9/Blockthon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 7.3.6
+Version: 7.3.9
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 Project-URL: Documentation, https://blockthon.github.io/Blockthon/
 Project-URL: Personal Website, https://mmdrza.com
 Keywords: blockthon,bitcoin,ethereum,tron,dogecoin,dash,qtum,litecoin,bitcoingold,wallet,private key,mnemonic,seed,binary,hex,hunter,compress,un compress,compress address,un compress address
@@ -13,27 +13,29 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Blockthon
 Blockthon Python Package for Generate and Converting Wallet Private Key and Mnemonic for Address Bitcoin
 
+![](https://raw.githubusercontent.com/Blockthon/Blockthon/main/media/Header.png)
+
 ```bash
 # on windows
 pip install Blockthon
 
 # on Linux
 pip3 install Blockthon
 ```
 
-or for download manual:
+linux first install:
 ```bash
-git clone https://github.com/Blockthon/Blockthon
-cd Blockthon
-make
+sudo apt-get update&&sudo apt-get upgrade -y
+sudo apt-get install -y autoconf automake build-essential libffi-dev libtool pkg-config python3-dev
+pip3 install blockthon
 ```
 ---
 
 ### Private Key
 
 generated random private key without repeat :
```

### Comparing `Blockthon-7.3.6/PKG-INFO` & `Blockthon-7.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 7.3.6
+Version: 7.3.9
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 Project-URL: Documentation, https://blockthon.github.io/Blockthon/
 Project-URL: Personal Website, https://mmdrza.com
 Keywords: blockthon,bitcoin,ethereum,tron,dogecoin,dash,qtum,litecoin,bitcoingold,wallet,private key,mnemonic,seed,binary,hex,hunter,compress,un compress,compress address,un compress address
@@ -13,27 +13,29 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Blockthon
 Blockthon Python Package for Generate and Converting Wallet Private Key and Mnemonic for Address Bitcoin
 
+![](https://raw.githubusercontent.com/Blockthon/Blockthon/main/media/Header.png)
+
 ```bash
 # on windows
 pip install Blockthon
 
 # on Linux
 pip3 install Blockthon
 ```
 
-or for download manual:
+linux first install:
 ```bash
-git clone https://github.com/Blockthon/Blockthon
-cd Blockthon
-make
+sudo apt-get update&&sudo apt-get upgrade -y
+sudo apt-get install -y autoconf automake build-essential libffi-dev libtool pkg-config python3-dev
+pip3 install blockthon
 ```
 ---
 
 ### Private Key
 
 generated random private key without repeat :
```

### Comparing `Blockthon-7.3.6/README.md` & `Blockthon-7.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Blockthon
 Blockthon Python Package for Generate and Converting Wallet Private Key and Mnemonic for Address Bitcoin
 
+![](https://raw.githubusercontent.com/Blockthon/Blockthon/main/media/Header.png)
+
 ```bash
 # on windows
 pip install Blockthon
 
 # on Linux
 pip3 install Blockthon
 ```
 
-or for download manual:
+linux first install:
 ```bash
-git clone https://github.com/Blockthon/Blockthon
-cd Blockthon
-make
+sudo apt-get update&&sudo apt-get upgrade -y
+sudo apt-get install -y autoconf automake build-essential libffi-dev libtool pkg-config python3-dev
+pip3 install blockthon
 ```
 ---
 
 ### Private Key
 
 generated random private key without repeat :
```

### Comparing `Blockthon-7.3.6/setup.py` & `Blockthon-7.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Blockthon",
-    version="7.3.6",
+    version="7.3.9",
     author="Pymmdrza",
     author_email="Pymmdrza@gmail.com",
     description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, "
                 "and Decimal.",
     keywords=['blockthon','bitcoin', 'ethereum', 'tron', 'dogecoin', 'dash', 'qtum', 'litecoin', 'bitcoingold', 'wallet', 'private key', 'mnemonic', 'seed', 'binary', 'hex', 'hunter', 'compress', 'un compress', 'compress address', 'un compress address'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

