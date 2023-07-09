# Comparing `tmp/mkdocs-zip-folders-1.0.2.tar.gz` & `tmp/mkdocs-zip-folders-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-zip-folders-1.0.2.tar", last modified: Fri Jul  7 10:09:13 2023, max compression
+gzip compressed data, was "mkdocs-zip-folders-1.0.3.tar", last modified: Sun Jul  9 13:34:07 2023, max compression
```

## Comparing `mkdocs-zip-folders-1.0.2.tar` & `mkdocs-zip-folders-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-07 10:09:13.103743 mkdocs-zip-folders-1.0.2/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-07-06 12:13:07.000000 mkdocs-zip-folders-1.0.2/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     2964 2023-07-07 10:09:13.103837 mkdocs-zip-folders-1.0.2/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     1895 2023-07-07 08:13:28.000000 mkdocs-zip-folders-1.0.2/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-07 10:09:13.103147 mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     2964 2023-07-07 10:09:13.000000 mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)      336 2023-07-07 10:09:13.000000 mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2023-07-07 10:09:13.000000 mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)       67 2023-07-07 10:09:13.000000 mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/entry_points.txt
--rw-r--r--   0 kuba       (501) staff       (20)      112 2023-07-07 10:09:13.000000 mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)       12 2023-07-07 10:09:13.000000 mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)     1243 2023-07-07 10:09:13.104208 mkdocs-zip-folders-1.0.2/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)      192 2023-07-06 12:15:09.000000 mkdocs-zip-folders-1.0.2/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-07 10:09:13.103415 mkdocs-zip-folders-1.0.2/zip_folders/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-07-06 12:15:31.000000 mkdocs-zip-folders-1.0.2/zip_folders/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     2822 2023-07-07 10:06:52.000000 mkdocs-zip-folders-1.0.2/zip_folders/plugin.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-09 13:34:07.820701 mkdocs-zip-folders-1.0.3/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-07-06 12:13:07.000000 mkdocs-zip-folders-1.0.3/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     2964 2023-07-09 13:34:07.820792 mkdocs-zip-folders-1.0.3/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     1895 2023-07-07 08:13:28.000000 mkdocs-zip-folders-1.0.3/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-09 13:34:07.820158 mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     2964 2023-07-09 13:34:07.000000 mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)      336 2023-07-09 13:34:07.000000 mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2023-07-09 13:34:07.000000 mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       67 2023-07-09 13:34:07.000000 mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/entry_points.txt
+-rw-r--r--   0 kuba       (501) staff       (20)      112 2023-07-09 13:34:07.000000 mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       12 2023-07-09 13:34:07.000000 mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)     1243 2023-07-09 13:34:07.821124 mkdocs-zip-folders-1.0.3/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)      192 2023-07-06 12:15:09.000000 mkdocs-zip-folders-1.0.3/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-09 13:34:07.820356 mkdocs-zip-folders-1.0.3/zip_folders/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-07-06 12:15:31.000000 mkdocs-zip-folders-1.0.3/zip_folders/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2700 2023-07-09 13:32:12.000000 mkdocs-zip-folders-1.0.3/zip_folders/plugin.py
```

### Comparing `mkdocs-zip-folders-1.0.2/LICENSE` & `mkdocs-zip-folders-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-zip-folders-1.0.2/PKG-INFO` & `mkdocs-zip-folders-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-zip-folders
-Version: 1.0.2
+Version: 1.0.3
 Summary: MkDocs plugin to zip configured folders and add them to the site.
 Home-page: https://github.com/JakubAndrysek/mkdocs-zip-folders
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/mkdocs-zip-folders
 Project-URL: Documentation, https://zip-folders.kubaandrysek.cz/
```

### Comparing `mkdocs-zip-folders-1.0.2/README.md` & `mkdocs-zip-folders-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-zip-folders-1.0.2/mkdocs_zip_folders.egg-info/PKG-INFO` & `mkdocs-zip-folders-1.0.3/mkdocs_zip_folders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-zip-folders
-Version: 1.0.2
+Version: 1.0.3
 Summary: MkDocs plugin to zip configured folders and add them to the site.
 Home-page: https://github.com/JakubAndrysek/mkdocs-zip-folders
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/mkdocs-zip-folders
 Project-URL: Documentation, https://zip-folders.kubaandrysek.cz/
```

### Comparing `mkdocs-zip-folders-1.0.2/setup.cfg` & `mkdocs-zip-folders-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-zip-folders
-version = 1.0.2
+version = 1.0.3
 description = MkDocs plugin to zip configured folders and add them to the site.
 keywords = mkdocs plugin zip folders download zip-folders
 url = https://github.com/JakubAndrysek/mkdocs-zip-folders
 author = Jakub Andrýsek
 author_email = email@kubaandrysek.cz
 project_urls = 
 	Source = https://github.com/JakubAndrysek/mkdocs-zip-folders
```

### Comparing `mkdocs-zip-folders-1.0.2/zip_folders/plugin.py` & `mkdocs-zip-folders-1.0.3/zip_folders/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,22 +53,20 @@
             with open(hash_path, 'w') as f:
                 f.write(self.hash_file(zip_path))
 
         return config
 
     @staticmethod
     def zip_folder(folder, debug=False):
-        # Use os.path.basename to include the root directory in the zip file
-        root_dir = os.path.basename(folder)
         zipf = zipfile.ZipFile(f'{folder}.zip', 'w', zipfile.ZIP_DEFLATED)
         for dirpath, dirnames, filenames in os.walk(folder):
             for filename in filenames:
                 # Create the file path relative to the root directory
-                relpath = os.path.relpath(dirpath, os.path.dirname(folder))
-                zipf.write(os.path.join(dirpath, filename), arcname=os.path.join(root_dir, relpath, filename))
+                relpath = os.path.relpath(dirpath, folder)  # remove os.path.dirname
+                zipf.write(os.path.join(dirpath, filename), arcname=os.path.join(relpath, filename))
         zipf.close()
 
         if debug:
             log.info(f"Zipped {folder} into {folder}.zip")
 
     @staticmethod
     def hash_file(filepath):
```

