# Comparing `tmp/AshCrypt-1.3.3.tar.gz` & `tmp/AshCrypt-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.3.3.tar", last modified: Fri Jul  7 14:06:15 2023, max compression
+gzip compressed data, was "AshCrypt-1.3.4.tar", last modified: Sun Jul  9 12:40:53 2023, max compression
```

## Comparing `AshCrypt-1.3.3.tar` & `AshCrypt-1.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.587549 AshCrypt-1.3.3/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.523386 AshCrypt-1.3.3/AshCrypt/
--rw-rw-rw-   0        0        0     4985 2023-07-02 19:28:38.000000 AshCrypt-1.3.3/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    37331 2023-07-07 14:05:56.000000 AshCrypt-1.3.3/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.3.3/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.3.3/AshCrypt/Database.py
--rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.3.3/AshCrypt/FileCrypt.py
--rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.3.3/AshCrypt/README.md
--rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.3.3/AshCrypt/TextCrypt.py
--rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.3/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.565834 AshCrypt-1.3.3/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
--rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/Database.cpython-39.pyc
--rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.3.3/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.3.3/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.573752 AshCrypt-1.3.3/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.3/AshCrypt/unittests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.581571 AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
--rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.3.3/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:06:15.544791 AshCrypt-1.3.3/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19466 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 14:06:15.000000 AshCrypt-1.3.3/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.3/LICENSE
--rw-rw-rw-   0        0        0    19466 2023-07-07 14:06:15.585649 AshCrypt-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    21853 2023-07-02 19:31:35.000000 AshCrypt-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 14:06:15.587549 AshCrypt-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-07 14:05:56.000000 AshCrypt-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.070354 AshCrypt-1.3.4/
+drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.015336 AshCrypt-1.3.4/AshCrypt/
+-rw-rw-rw-   0        0        0     4985 2023-07-07 17:08:02.000000 AshCrypt-1.3.4/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    37332 2023-07-07 18:14:16.000000 AshCrypt-1.3.4/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6654 2023-07-01 17:13:11.000000 AshCrypt-1.3.4/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8450 2023-07-03 21:05:38.000000 AshCrypt-1.3.4/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     3849 2023-07-01 02:35:10.000000 AshCrypt-1.3.4/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0    18439 2023-07-02 19:28:42.000000 AshCrypt-1.3.4/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1852 2023-07-01 02:35:10.000000 AshCrypt-1.3.4/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.4/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.053665 AshCrypt-1.3.4/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6336 2023-07-03 12:24:42.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7285 2023-07-03 21:09:38.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3236 2023-07-01 17:13:25.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2409 2023-07-01 17:13:25.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2023-07-07 12:45:40.000000 AshCrypt-1.3.4/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      536 2023-07-07 12:45:35.000000 AshCrypt-1.3.4/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.059756 AshCrypt-1.3.4/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.4/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.066348 AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5782 2023-07-03 12:24:42.000000 AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3395 2023-07-03 12:52:55.000000 AshCrypt-1.3.4/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-09 12:40:53.031857 AshCrypt-1.3.4/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19466 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 12:40:52.000000 AshCrypt-1.3.4/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0    19466 2023-07-09 12:40:53.069349 AshCrypt-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21819 2023-07-07 14:29:17.000000 AshCrypt-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 12:40:53.070354 AshCrypt-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-07 14:06:29.000000 AshCrypt-1.3.4/setup.py
```

### Comparing `AshCrypt-1.3.3/AshCrypt/Ash.py` & `AshCrypt-1.3.4/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.3.4/AshCrypt/AshCryptGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,29 +105,29 @@
                             eBuffer = {}
                             for e in conn.content_by_id(int(idd)):
                                 eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {'Content': e[2].__str__()},
                                                                    {'KeyRef': e[3]}]
                             eJSON = json.dumps(eBuffer, indent=2)
                             f.write(eJSON)
                         db_display_text.insert(tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
-                                                       f"chosen path :\n\n'{usable_real_path}'")
+                                                       f" chosen path :\n\n'{usable_real_path}'")
                     if int(idd) == last_id:
                         db_display_text.delete('1.0', tk.END)
                         db_display_text.insert(tk.END, 'Chosen last ID\n\n')
                         to_json_path = os.path.join(usable_real_path,'output.json')
                         try:
                             with open(to_json_path, 'w') as f:
                                 eBuffer = {}
                                 for e in conn.content_by_id(int(idd)):
                                     eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {'Content': e[2].__str__()},
                                                                        {'KeyRef': e[3]}]
                                 eJSON = json.dumps(eBuffer, indent=2)
                                 f.write(eJSON)
                             db_display_text.insert(tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
-                                                           f"the chosen path :\n\n'{usable_real_path}'")
+                                                           f" the chosen path :\n\n'{usable_real_path}'")
                         except:
                             db_display_text.delete('1.0', tk.END)
                             db_display_text.insert(tk.END,"ERROR \n\nCheck the validity of 'output.json' file"
                                                           "\n\nCheck if the database is faulty\n")
                     elif int(idd) > last_id:
                         db_display_text.delete('1.0', tk.END)
                         db_display_text.insert(tk.END, 'Given ID is greater than the highest available ID')
@@ -634,15 +634,15 @@
                       text='FILE PATH',
                       font='Calibre 20 bold' ,
                       )
 filepathlabel.place(relx=0.335,rely=0.10)
 
 import platform
 if platform.system() == 'Windows':
-    resultvarfile = tk.StringVar(value='                  ..........')
+    resultvarfile = tk.StringVar(value='                 ..........')
     resultLabelfile =  tk.Label(master= frameFile1,
                              textvariable=resultvarfile,
                              font='terminal 13 bold').place(rely= 0.55)
 else:
     resultvarfile = tk.StringVar(value='                    ..........')
     resultLabelfile = tk.Label(master=frameFile1,
                                textvariable=resultvarfile,
```

### Comparing `AshCrypt-1.3.3/AshCrypt/CliCrypt.py` & `AshCrypt-1.3.4/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/Database.py` & `AshCrypt-1.3.4/AshCrypt/Database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/FileCrypt.py` & `AshCrypt-1.3.4/AshCrypt/FileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/README.md` & `AshCrypt-1.3.4/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/TextCrypt.py` & `AshCrypt-1.3.4/AshCrypt/TextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-1.3.4/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc` & `AshCrypt-1.3.4/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/__pycache__/Database.cpython-39.pyc` & `AshCrypt-1.3.4/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc` & `AshCrypt-1.3.4/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc` & `AshCrypt-1.3.4/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/__pycache__/qr.cpython-39.pyc` & `AshCrypt-1.3.4/AshCrypt/__pycache__/qr.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/qr.py` & `AshCrypt-1.3.4/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc` & `AshCrypt-1.3.4/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.3.4/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.3.4/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.3
+Version: 1.3.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.3/AshCrypt.egg-info/SOURCES.txt` & `AshCrypt-1.3.4/AshCrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/LICENSE` & `AshCrypt-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.3/PKG-INFO` & `AshCrypt-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.3
+Version: 1.3.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.3/README.md` & `AshCrypt-1.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Reason Behind It
 In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
 
 As a firm believer in **Freedom** , I have developed a set of tools in Python that leverages the AES-256 algorithm to make it easier for undividuals to safeguard their data without blindly relying on third parties to do it tor them  . 
 
 My aim here is to make these tools accessible and user-friendly, even for individuals with limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
 ## Overview ## 
-The project incorporates a library I made called **[AshCrypt](https://github.com/AshGw/AES-256/AshCrypt)** : 
+The project incorporates a library I made called **AshCrypt** : 
 
 <br>A simple, secure, and developer-oriented library for
 encryption and decryption with AES-256 (CBC) . 
 <br>The core of the library is the module `Ash`
 It offers an intuitive interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
@@ -28,15 +28,15 @@
 The project uses `Ash` module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
 view the headers for [FileCrypt](https://github.com/AshGw/AES-256#filecrypt) and [TextCrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
 
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
-<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [Database](https://github.com/AshGw#Database) header to learn more.
+<br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [Database](https://github.com/AshGw/AES-256#database-1) header to learn more.
 
 ## Installation ##
 There are many ways to go by this : 
 ### If you want to use it as a library ###
 You can simply use **pip**
 <br>First upgrade the package installer 
 ```bash
@@ -109,15 +109,15 @@
 ## Ash Module ##
 The `Ash.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
-<br>You can check the [unittesting file](AshCryt/unittests/unittestAsh.py) to verify how it works.
+<br>You can check the [unittesting file](AshCrypt/unittests/unittestAsh.py) to verify how it works.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genMainkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
```

### Comparing `AshCrypt-1.3.3/setup.py` & `AshCrypt-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.3.3',
+    version='1.3.4',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

