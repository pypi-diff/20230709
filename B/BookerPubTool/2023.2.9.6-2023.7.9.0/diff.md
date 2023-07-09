# Comparing `tmp/BookerPubTool-2023.2.9.6.tar.gz` & `tmp/BookerPubTool-2023.7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BookerPubTool-2023.2.9.6.tar", last modified: Fri Mar 10 08:18:27 2023, max compression
+gzip compressed data, was "BookerPubTool-2023.7.9.0.tar", last modified: Sun Jul  9 14:00:16 2023, max compression
```

## Comparing `BookerPubTool-2023.2.9.6.tar` & `BookerPubTool-2023.7.9.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool/
--rw-rw-rw-   0        0        0      236 2023-03-10 08:18:22.000000 BookerPubTool-2023.2.9.6/BookerPubTool/__init__.py
--rw-rw-rw-   0        0        0     5082 2023-02-17 18:33:54.000000 BookerPubTool-2023.2.9.6/BookerPubTool/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/
--rw-rw-rw-   0        0        0        0 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/__init__.py
--rw-rw-rw-   0        0        0      214 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/__init__.tmpl
--rw-rw-rw-   0        0        0   383911 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/epubjs-reader.zip
--rw-rw-rw-   0        0        0      420 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/package.tmpl
--rw-rw-rw-   0        0        0      150 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/pdf.html
--rw-rw-rw-   0        0        0      424 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/readme.tmpl
--rw-rw-rw-   0        0        0     3252 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/server.js
--rw-rw-rw-   0        0        0      635 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/server.py
--rw-rw-rw-   0        0        0     1778 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/asset/setup.tmpl
--rw-rw-rw-   0        0        0     3170 2023-02-10 15:22:15.000000 BookerPubTool-2023.2.9.6/BookerPubTool/docker.py
--rw-rw-rw-   0        0        0     2088 2023-02-07 14:17:19.000000 BookerPubTool-2023.2.9.6/BookerPubTool/ebook2site.py
--rw-rw-rw-   0        0        0     6155 2023-02-17 19:00:41.000000 BookerPubTool-2023.2.9.6/BookerPubTool/git.py
--rw-rw-rw-   0        0        0     5928 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/BookerPubTool/libgen.py
--rw-rw-rw-   0        0        0     3917 2023-02-07 14:15:17.000000 BookerPubTool-2023.2.9.6/BookerPubTool/npm.py
--rw-rw-rw-   0        0        0     4817 2023-02-07 15:01:12.000000 BookerPubTool-2023.2.9.6/BookerPubTool/pypi.py
--rw-rw-rw-   0        0        0     2870 2023-02-18 05:42:26.000000 BookerPubTool-2023.2.9.6/BookerPubTool/util.py
--rw-rw-rw-   0        0        0     5690 2023-01-31 02:30:15.000000 BookerPubTool-2023.2.9.6/BookerPubTool/zhihu_msger.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/
--rw-rw-rw-   0        0        0     1233 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1233 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/README.md
--rw-rw-rw-   0        0        0       42 2023-03-10 08:18:27.000000 BookerPubTool-2023.2.9.6/setup.cfg
--rw-rw-rw-   0        0        0     2042 2023-01-31 02:03:47.000000 BookerPubTool-2023.2.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:00:16.611151 BookerPubTool-2023.7.9.0/
+drwxrwxrwx   0        0        0        0 2023-07-09 14:00:16.598151 BookerPubTool-2023.7.9.0/BookerPubTool/
+-rw-rw-rw-   0        0        0      239 2023-07-09 13:59:39.000000 BookerPubTool-2023.7.9.0/BookerPubTool/__init__.py
+-rw-rw-rw-   0        0        0     5163 2023-04-29 06:24:24.000000 BookerPubTool-2023.7.9.0/BookerPubTool/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:00:16.610153 BookerPubTool-2023.7.9.0/BookerPubTool/asset/
+-rw-rw-rw-   0        0        0        0 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/__init__.tmpl
+-rw-rw-rw-   0        0        0   383911 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/epubjs-reader.zip
+-rw-rw-rw-   0        0        0      420 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/package.tmpl
+-rw-rw-rw-   0        0        0      150 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/pdf.html
+-rw-rw-rw-   0        0        0      424 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/readme.tmpl
+-rw-rw-rw-   0        0        0     3252 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/server.js
+-rw-rw-rw-   0        0        0      635 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/server.py
+-rw-rw-rw-   0        0        0     1778 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/BookerPubTool/asset/setup.tmpl
+-rw-rw-rw-   0        0        0     3170 2023-02-10 15:22:15.000000 BookerPubTool-2023.7.9.0/BookerPubTool/docker.py
+-rw-rw-rw-   0        0        0     2199 2023-04-29 06:25:10.000000 BookerPubTool-2023.7.9.0/BookerPubTool/ebook2site.py
+-rw-rw-rw-   0        0        0     5714 2023-07-02 10:52:53.000000 BookerPubTool-2023.7.9.0/BookerPubTool/git.py
+-rw-rw-rw-   0        0        0     6228 2023-04-27 16:31:36.000000 BookerPubTool-2023.7.9.0/BookerPubTool/libgen.py
+-rw-rw-rw-   0        0        0     3917 2023-02-07 14:15:17.000000 BookerPubTool-2023.7.9.0/BookerPubTool/npm.py
+-rw-rw-rw-   0        0        0     4817 2023-02-07 15:01:12.000000 BookerPubTool-2023.7.9.0/BookerPubTool/pypi.py
+-rw-rw-rw-   0        0        0     2870 2023-02-18 05:42:26.000000 BookerPubTool-2023.7.9.0/BookerPubTool/util.py
+-rw-rw-rw-   0        0        0     5690 2023-01-31 02:30:15.000000 BookerPubTool-2023.7.9.0/BookerPubTool/zhihu_msger.py
+drwxrwxrwx   0        0        0        0 2023-07-09 14:00:16.600151 BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/
+-rw-rw-rw-   0        0        0     1195 2023-07-09 14:00:16.000000 BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-07-09 14:00:16.000000 BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 14:00:16.000000 BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-07-09 14:00:16.000000 BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-09 14:00:16.000000 BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1844 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/LICENSE
+-rw-rw-rw-   0        0        0     1195 2023-07-09 14:00:16.611151 BookerPubTool-2023.7.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 14:00:16.611151 BookerPubTool-2023.7.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2042 2023-01-31 02:03:47.000000 BookerPubTool-2023.7.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/__main__.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     npm_config_parser.add_argument("token", help="token")
     npm_config_parser.set_defaults(func=config_npm)
     
     ebook2site_parser = subparsers.add_parser("ebook2site", help="convert an ebook to a site")
     ebook2site_parser.add_argument("file", help="file")
     ebook2site_parser.add_argument("-n", "--name", help="name")
     ebook2site_parser.add_argument("-d", "--dir", help="dir", default='.')
+    ebook2site_parser.add_argument("-s", "--suffix", help="suffix", default='')
     ebook2site_parser.set_defaults(func=ebook2site_handle)
     
     libgen_parser = subparsers.add_parser("libgen", help="upload to libgen")
     libgen_parser.add_argument("series", help="series")
     libgen_parser.add_argument("fname", help="file name")
     libgen_parser.add_argument("-t", "--threads", type=int, default=3, help="thread count")
     libgen_parser.add_argument("-p", "--proxy", help="proxy")
```

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/asset/epubjs-reader.zip` & `BookerPubTool-2023.7.9.0/BookerPubTool/asset/epubjs-reader.zip`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/asset/server.js` & `BookerPubTool-2023.7.9.0/BookerPubTool/asset/server.js`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/asset/server.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/asset/server.py`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/asset/setup.tmpl` & `BookerPubTool-2023.7.9.0/BookerPubTool/asset/setup.tmpl`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/docker.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/docker.py`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/ebook2site.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/ebook2site.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,17 +48,21 @@
         .replace('{npm_name}', npm_name)
     open(path.join(odir, 'README.md'), 'w', encoding='utf8').write(README_MD)
 
 def ebook2site_handle(args):
     name = args.name
     fname = args.file
     dir = args.dir
+    suff = args.suffix
         
     if not fname.endswith('.pdf') and \
        not fname.endswith('.epub'):
         print('请提供 PDF 或 EPUB')
         return 
     
     if not name: name = gen_proj_name(path.basename(fname))
+    if suff:
+        suff = gen_proj_name(suff)
+        if suff: name += '-' + suff
     proj_dir = path.join(dir, name)
     ebook2site(fname, proj_dir)
```

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/git.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,37 +156,27 @@
             
     # 检查远程库是否有该分支
     subp.Popen(
         ['git', 'remote', 'update', remote],
         shell=True, cwd=dir,
     ).communicate()
     branches = get_all_branches(dir)
-    remote_exi =  f'remotes/{remote}/{work_branch}' in branches
-    if not remote_exi:
+    remote_branch = f'remotes/{remote}/{work_branch}'
+    if remote_branch not in branches:
         # 如果远程分支不存在，推送本地分支所有提交
         cids = get_branch_cids(dir, work_branch)
     else:
-        # 拉取远程分支，并重命名
-        remote_branch = f'{remote}-{work_branch}-{uuid.uuid4().hex}'
-        subp.Popen(
-            ['git', 'fetch', remote, f'{work_branch}:{remote_branch}'],
-            shell=True, cwd=dir,
-        ).communicate()
         # 查看远程库是否有新提交
         cids = get_branch_cids(dir, remote_branch, '^' + work_branch)
         if cids:
             print('远程仓库有新的提交，需要手动 git pull')
             print('\n'.join(cids))
             return
         # 查看本地库的新提交
         cids = get_branch_cids(dir, work_branch, '^' + remote_branch)
     for cid in cids[::-1]:
-        cid_branch = 'cid-' + cid
-        cmds = [
-            # 切换分支
-            ['git', 'checkout', cid, '-f'], 
-            ['git', 'branch', cid_branch],
-            # 提交改动
-            ['git', 'push', remote, f'{cid_branch}:{work_branch}'],
-        ]
-        for cmd in cmds:
-            subp.Popen(cmd, shell=True, cwd=dir).communicate()
+        # 提交改动
+        subp.Popen(
+            ['git', 'push', remote, f'{cid}:refs/heads/{work_branch}'], 
+            shell=True, cwd=dir
+        ).communicate()
+
```

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/libgen.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/libgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     hash = hashlib.md5()
     hash.update(bts)
     return hash.hexdigest()
 
 def proc_info(fname, info):
     hdlrs = {
         'lightnovel': proc_ln_info,
+        'biquge': proc_bqg_info,
         'giantessnight': proc_gn_info,
         'it-ebooks': proc_itebooks_info,
         'dmzj': proc_dmzj_info,
         'nhentai': proc_nh_info,
         'ixinzhi': proc_ixinzhi_info,
     }
     if series in hdlrs:
@@ -54,14 +55,20 @@
         info['year'] = year
         info['series'] = f'it-ebooks-{year}'
     else:
         info['series'] = 'it-ebooks-extra'
     info['authors'] = 'it-ebooks'
     info['publisher'] = 'iBooker it-ebooks'
     
+def proc_bqg_info(fname, info):
+    ori_info = path.basename(fname) \
+        .replace('.epub', '').split(' - ')
+    info['authors'] = ori_info[1]
+    info['edition'] = ori_info[2]
+    info['publisher'] = 'BiQuGe'
 
 def proc_ln_info(fname, info):
     ori_info = path.basename(fname) \
         .replace('.epub', '').split(' - ')
     info['authors'] = ori_info[1]
     info['edition'] = ori_info[2]
     info['year'] = ori_info[2][:-4]
@@ -206,15 +213,19 @@
     if args.proxy:
         proxy = {
             'http': args.proxy,
             'https': args.proxy,
         }
     
     cate = series
-    if series in ['lightnovel', 'dmzj', 'nhentai', 'giantessnight']:
+    if series in [
+        'lightnovel', 'biquge', 
+        'dmzj', 'nhentai', 
+        'giantessnight'
+    ]:
         cate = 'fiction'
     elif series in ['it-ebooks', 'ixinzhi']:
         cate = 'main'
     for k, v in urls.items():
         urls[k] = v.replace('{cate}', cate)
     if path.isdir(fname):
         process_dir(args)
```

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/npm.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/npm.py`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/pypi.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/pypi.py`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/util.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/util.py`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool/zhihu_msger.py` & `BookerPubTool-2023.7.9.0/BookerPubTool/zhihu_msger.py`

 * *Files identical despite different names*

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/PKG-INFO` & `BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Metadata-Version: 2.1
 Name: BookerPubTool
-Version: 2023.2.9.6
+Version: 2023.7.9.0
 Summary: PYPI book publisher for ApacheCN
 Home-page: https://github.com/apachecn/BookerPubTool
-Author: ApacheCN
-Author-email: apachecn@163.com
-License: UNKNOWN
-Description: # PypiBookPublisher
-        
-        PYPI book publisher for ApacheCN
-Platform: UNKNOWN
+Author: wizardforcel
+Author-email: wizard.z@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
@@ -25,7 +20,12 @@
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Documentation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PypiBookPublisher
+
+PYPI book publisher for ApacheCN
```

### Comparing `BookerPubTool-2023.2.9.6/BookerPubTool.egg-info/SOURCES.txt` & `BookerPubTool-2023.7.9.0/BookerPubTool.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 BookerPubTool/__init__.py
 BookerPubTool/__main__.py
 BookerPubTool/docker.py
 BookerPubTool/ebook2site.py
 BookerPubTool/git.py
```

### Comparing `BookerPubTool-2023.2.9.6/PKG-INFO` & `BookerPubTool-2023.7.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Metadata-Version: 2.1
 Name: BookerPubTool
-Version: 2023.2.9.6
+Version: 2023.7.9.0
 Summary: PYPI book publisher for ApacheCN
 Home-page: https://github.com/apachecn/BookerPubTool
-Author: ApacheCN
-Author-email: apachecn@163.com
-License: UNKNOWN
-Description: # PypiBookPublisher
-        
-        PYPI book publisher for ApacheCN
-Platform: UNKNOWN
+Author: wizardforcel
+Author-email: wizard.z@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
@@ -25,7 +20,12 @@
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Documentation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PypiBookPublisher
+
+PYPI book publisher for ApacheCN
```

### Comparing `BookerPubTool-2023.2.9.6/setup.py` & `BookerPubTool-2023.7.9.0/setup.py`

 * *Files identical despite different names*

