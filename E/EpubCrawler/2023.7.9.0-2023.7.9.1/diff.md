# Comparing `tmp/EpubCrawler-2023.7.9.0.tar.gz` & `tmp/EpubCrawler-2023.7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EpubCrawler-2023.7.9.0.tar", last modified: Sun Jul  9 13:52:31 2023, max compression
+gzip compressed data, was "EpubCrawler-2023.7.9.1.tar", last modified: Sun Jul  9 17:19:58 2023, max compression
```

## Comparing `EpubCrawler-2023.7.9.0.tar` & `EpubCrawler-2023.7.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:31.944634 EpubCrawler-2023.7.9.0/
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:31.940635 EpubCrawler-2023.7.9.0/EpubCrawler/
--rw-rw-rw-   0        0        0      267 2023-07-09 13:49:30.000000 EpubCrawler-2023.7.9.0/EpubCrawler/__init__.py
--rw-rw-rw-   0        0        0     5990 2023-07-02 15:28:27.000000 EpubCrawler-2023.7.9.0/EpubCrawler/__main__.py
--rw-rw-rw-   0        0        0      959 2022-08-20 13:22:25.000000 EpubCrawler-2023.7.9.0/EpubCrawler/common.py
--rw-rw-rw-   0        0        0      841 2023-07-02 15:52:09.000000 EpubCrawler-2023.7.9.0/EpubCrawler/config.py
--rw-rw-rw-   0        0        0     3049 2023-02-14 05:10:37.000000 EpubCrawler-2023.7.9.0/EpubCrawler/img.py
--rw-rw-rw-   0        0        0     5670 2023-07-02 15:34:35.000000 EpubCrawler-2023.7.9.0/EpubCrawler/sele_crawler.py
--rw-rw-rw-   0        0        0     4046 2023-07-03 14:42:15.000000 EpubCrawler-2023.7.9.0/EpubCrawler/util.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:31.943634 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/
--rw-rw-rw-   0        0        0     5370 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1838 2022-03-15 14:47:20.000000 EpubCrawler-2023.7.9.0/LICENSE
--rw-rw-rw-   0        0        0     5370 2023-07-09 13:52:31.943634 EpubCrawler-2023.7.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4279 2023-02-14 05:16:13.000000 EpubCrawler-2023.7.9.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 13:52:31.944634 EpubCrawler-2023.7.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1763 2022-03-15 14:47:20.000000 EpubCrawler-2023.7.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:19:58.306899 EpubCrawler-2023.7.9.1/
+drwxrwxrwx   0        0        0        0 2023-07-09 17:19:58.302904 EpubCrawler-2023.7.9.1/EpubCrawler/
+-rw-rw-rw-   0        0        0      267 2023-07-09 17:19:38.000000 EpubCrawler-2023.7.9.1/EpubCrawler/__init__.py
+-rw-rw-rw-   0        0        0     6233 2023-07-09 17:16:05.000000 EpubCrawler-2023.7.9.1/EpubCrawler/__main__.py
+-rw-rw-rw-   0        0        0      959 2022-08-20 13:22:25.000000 EpubCrawler-2023.7.9.1/EpubCrawler/common.py
+-rw-rw-rw-   0        0        0      878 2023-07-09 16:52:44.000000 EpubCrawler-2023.7.9.1/EpubCrawler/config.py
+-rw-rw-rw-   0        0        0     3250 2023-07-09 17:16:17.000000 EpubCrawler-2023.7.9.1/EpubCrawler/img.py
+-rw-rw-rw-   0        0        0     5670 2023-07-02 15:34:35.000000 EpubCrawler-2023.7.9.1/EpubCrawler/sele_crawler.py
+-rw-rw-rw-   0        0        0     4141 2023-07-09 17:15:16.000000 EpubCrawler-2023.7.9.1/EpubCrawler/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:19:58.305900 EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/
+-rw-rw-rw-   0        0        0     5370 2023-07-09 17:19:58.000000 EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-07-09 17:19:58.000000 EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 17:19:58.000000 EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-09 17:19:58.000000 EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-09 17:19:58.000000 EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 17:19:58.000000 EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1838 2022-03-15 14:47:20.000000 EpubCrawler-2023.7.9.1/LICENSE
+-rw-rw-rw-   0        0        0     5370 2023-07-09 17:19:58.306899 EpubCrawler-2023.7.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4279 2023-02-14 05:16:13.000000 EpubCrawler-2023.7.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 17:19:58.306899 EpubCrawler-2023.7.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1763 2022-03-15 14:47:20.000000 EpubCrawler-2023.7.9.1/setup.py
```

### Comparing `EpubCrawler-2023.7.9.0/EpubCrawler/__main__.py` & `EpubCrawler-2023.7.9.1/EpubCrawler/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import json
 import yaml
 import warnings
 from pyquery import PyQuery as pq
 import time
 from os import path
 import re
+import random
+import traceback
 from concurrent.futures import ThreadPoolExecutor
 import hashlib
 from readability import Document
 from GenEpub import gen_epub
 from . import *
 from .util import *
 from .img import *
@@ -33,15 +35,15 @@
         
     html = request_retry(
         'GET', config['url'],
         retry=config['retry'],
         check_status=config['checkStatus'],
         headers=config['headers'],
         timeout=config['timeout'],
-        proxies=config['proxy'],
+        proxies=prdict(config['proxy'][0]),
         verify=False,
     ).content.decode(config['encoding'], 'ignore')
     return get_toc(html, config['url'])
     
 def get_toc(html, base):
     root = pq(html)
     
@@ -68,21 +70,21 @@
         if url in vis: continue
         vis.add(url)
         res.append(url)
         
     return res
 
     
-def tr_download_page_safe(url, art, imgs):
+def tr_download_page_safe(*args, **kw):
     try:
-        tr_download_page(url, art, imgs)
-    except Exception as ex:
-        print(f'{url} 下载失败：{ex}')
+        tr_download_page(*args, **kw)
+    except:
+        traceback.print_exc()
 
-def tr_download_page(url, art, imgs):
+def tr_download_page(url, proxy, art, imgs):
     hash = hashlib.md5(url.encode('utf-8')).hexdigest()
     cache = load_article(hash)
     if cache is not None and config['cache']:
         print(f'{url} 已存在于本地缓存中')
         art.update(cache)
         art['content'] = process_img(
             art['content'], imgs,
@@ -93,15 +95,15 @@
     for i in range(config['retry']):
         html = request_retry(
             'GET', url,
             retry=config['retry'],
             check_status=config['checkStatus'],
             headers=config['headers'],
             timeout=config['timeout'],
-            proxies=config['proxy'],
+            proxies=prdict(proxy),
             verify=False,
         ).content.decode(config['encoding'], 'ignore')
         r = get_article(html, url)
         if not config['checkBlank'] or \
            (r['title'] and r['content']):
            break
         if i == config['retry'] - 1:
@@ -109,33 +111,31 @@
     art.update(r)
     save_article(hash, art)
     art['content'] = process_img(
         art['content'], imgs,
         page_url=url,
         img_prefix='../Images/',
     )
-    print(f'{url} 下载成功')
+    print(f'{url} proxy:{proxy} 下载成功')
     time.sleep(config['wait'])
     
 
 def update_config(cfg_fname, user_cfg):
     global get_toc
     global get_article
     
     config.update(user_cfg)
     
     if not config['title']:
         config['title'] = 'title'
     
-    if config['proxy']:
-        proxies = {
-            'http': config['proxy'],
-            'https': config['proxy'],
-        }
-        config['proxy'] = proxies
+    if config['proxy'] is None or len(config['proxy']) == 0:
+        config['proxy'] = [None]
+    elif isinstance(config['proxy'], str):
+        config['proxy'] = config['proxy'].split(';')
     
     set_img_pool(ThreadPoolExecutor(config['imgThreads']))
     
     if config['external']:
         ex_fname = path.join(path.dirname(cfg_fname), config['external'])
         mod = load_module(ex_fname)
         get_toc = getattr(mod, 'get_toc', get_toc)
@@ -187,23 +187,27 @@
         articles.append({
             'title': config['name'],
             'content': f"<p>来源：<a href='{config['url']}'>{config['url']}</a></p>",
         })
     
     text_pool = ThreadPoolExecutor(config['textThreads'])
     hdls = []
-    for url in toc:
+    for i, url in enumerate(toc):
         print(f'page: {url}')
         if not re.search(r'^https?://', url):
             articles.append({'title': url, 'content': ''})
             continue
         
+        if config['proxyOrder'] == 'squential':
+            pr = config['proxy'][i % len(config['proxy'])]
+        else:
+            pr = random.choice(config['proxy'])
         art = {}
         articles.append(art)
-        hdl = text_pool.submit(tr_download_page_safe, url, art, imgs)
+        hdl = text_pool.submit(tr_download_page_safe, url, pr, art, imgs)
         hdls.append(hdl)
             
         
     for h in hdls: h.result()
     articles = [art for art in articles if art]
     gen_epub(articles, imgs, limit=config['sizeLimit'])
     print('done...')
```

### Comparing `EpubCrawler-2023.7.9.0/EpubCrawler/common.py` & `EpubCrawler-2023.7.9.1/EpubCrawler/common.py`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.7.9.0/EpubCrawler/config.py` & `EpubCrawler-2023.7.9.1/EpubCrawler/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     'list': [],
     'optiMode': 'quant',
     'colors': 8,
     'timeout': None,
     'connTimeout': 10,
     'readTimeout': 60,
 	'imgSrc': ['data-src', 'data-original-src', 'src'],
-    'proxy': '',
+    'proxy': [None],
+    'proxyOrder': 'sequential',
     'textThreads': 8,
     'imgThreads': 24,
     'external': None,
     'checkStatus': False,
     'checkBlank': True,
     'cache': True,
     'waitContent': False,
```

### Comparing `EpubCrawler-2023.7.9.0/EpubCrawler/img.py` & `EpubCrawler-2023.7.9.1/EpubCrawler/img.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from concurrent.futures import ThreadPoolExecutor
 from urllib.parse import urljoin, quote_plus
 import hashlib
 from pyquery import PyQuery as pq
 import time
 import re
 import base64
+import random
+import traceback
 from .util import *
 from .config import config
 
 img_pool = ThreadPoolExecutor(5)
 RE_DATA_URL = r'^data:image/\w+;base64,'
 
 
@@ -21,38 +23,38 @@
 def get_img_src(el_img):
     url = ''
     for prop in config['imgSrc']:
         url = el_img.attr(prop)
         if url: break
     return url
     
-def tr_download_img_safe(url, imgs, picname):
+def tr_download_img_safe(*args, **kw):
     try:
-        tr_download_img(url, imgs, picname)
-    except Exception as ex:
-        print(f'{url} 下载失败：{ex}')
+        tr_download_img(*args, **kw)
+    except:
+        traceback.print_exc()
 
-def tr_download_img(url, imgs, picname):
+def tr_download_img(url, proxy, imgs, picname):
     hash = hashlib.md5(url.encode('utf-8')).hexdigest()
     cache = load_img(hash, config['optiMode'])
     if cache is not None and config['cache']:
         print(f'{url} 已存在于本地缓存中')
         imgs[picname] = cache
         return
 
     data = request_retry(
         'GET', url,
         headers=config['headers'],
         check_status=config['checkStatus'],
         retry=config['retry'],
         timeout=config['timeout'],
-        proxies=config['proxy'],
+        proxies=prdict(proxy),
         verify=False,
     ).content
-    print(f'{url} 下载成功')
+    print(f'{url} proxy:{proxy} 下载成功')
     data = opti_img(data, config['optiMode'], config['colors']) or b''
     imgs[picname] = data
     save_img(hash, config['optiMode'], data)
     time.sleep(config['wait'])
     
 def process_img_data_url(url, el_img, imgs, **kw):
     if not re.search(RE_DATA_URL, url):
@@ -84,15 +86,19 @@
             if kw.get('page_url'):
                 url = urljoin(kw.get('page_url'), url)
             else: continue
         
         picname = hashlib.md5(url.encode('utf-8')).hexdigest() + '.png'
         print(f'pic: {url} => {picname}')
         if picname not in imgs:
-            hdl = img_pool.submit(tr_download_img_safe, url, imgs, picname)
+            if config['proxyOrder'] == 'squential':
+                pr = config['proxy'][i % len(config['proxy'])]
+            else:
+                pr = random.choice(config['proxy'])
+            hdl = img_pool.submit(tr_download_img_safe, url, pr, imgs, picname)
             hdls.append(hdl)
             
         el_img.attr('src', kw['img_prefix'] + picname)
         el_img.attr('data-original-src', url)
         
     for h in hdls: h.result()
     return root.html()
```

### Comparing `EpubCrawler-2023.7.9.0/EpubCrawler/sele_crawler.py` & `EpubCrawler-2023.7.9.1/EpubCrawler/sele_crawler.py`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.7.9.0/EpubCrawler/util.py` & `EpubCrawler-2023.7.9.1/EpubCrawler/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,7 +141,11 @@
     
     factor = factor_map[m.group(2)]
     return int(base * factor)
     
 def extname(fname):
     m = re.search(r'\.(\w+)$', fname)
     return m.group(1) if m else ''
+
+def prdict(pr):
+    return None if pr is None \
+           else {'http': pr, 'https': pr}
```

### Comparing `EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/PKG-INFO` & `EpubCrawler-2023.7.9.1/EpubCrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EpubCrawler
-Version: 2023.7.9.0
+Version: 2023.7.9.1
 Summary: EpubCrawler，用于抓取网页内容并制作 EPUB 的小工具
 Home-page: https://github.com/apachecn/epub-crawler
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Keywords: ebook,epub,crawler,爬虫,电子书
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `EpubCrawler-2023.7.9.0/LICENSE` & `EpubCrawler-2023.7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.7.9.0/PKG-INFO` & `EpubCrawler-2023.7.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EpubCrawler
-Version: 2023.7.9.0
+Version: 2023.7.9.1
 Summary: EpubCrawler，用于抓取网页内容并制作 EPUB 的小工具
 Home-page: https://github.com/apachecn/epub-crawler
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Keywords: ebook,epub,crawler,爬虫,电子书
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `EpubCrawler-2023.7.9.0/README.md` & `EpubCrawler-2023.7.9.1/README.md`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.7.9.0/setup.py` & `EpubCrawler-2023.7.9.1/setup.py`

 * *Files identical despite different names*

