# Comparing `tmp/EpubCrawler-2023.3.14.0.tar.gz` & `tmp/EpubCrawler-2023.7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EpubCrawler-2023.3.14.0.tar", last modified: Tue Mar 14 03:55:06 2023, max compression
+gzip compressed data, was "EpubCrawler-2023.7.9.0.tar", last modified: Sun Jul  9 13:52:31 2023, max compression
```

## Comparing `EpubCrawler-2023.3.14.0.tar` & `EpubCrawler-2023.7.9.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/
-drwxrwxrwx   0        0        0        0 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler/
--rw-rw-rw-   0        0        0      265 2023-03-14 03:54:59.000000 EpubCrawler-2023.3.14.0/EpubCrawler/__init__.py
--rw-rw-rw-   0        0        0     7040 2023-03-13 02:03:53.000000 EpubCrawler-2023.3.14.0/EpubCrawler/__main__.py
--rw-rw-rw-   0        0        0      959 2022-08-20 13:22:25.000000 EpubCrawler-2023.3.14.0/EpubCrawler/common.py
--rw-rw-rw-   0        0        0      816 2023-03-14 03:53:58.000000 EpubCrawler-2023.3.14.0/EpubCrawler/config.py
--rw-rw-rw-   0        0        0     3049 2023-02-14 05:10:37.000000 EpubCrawler-2023.3.14.0/EpubCrawler/img.py
--rw-rw-rw-   0        0        0     5157 2022-08-20 13:29:14.000000 EpubCrawler-2023.3.14.0/EpubCrawler/sele_crawler.py
--rw-rw-rw-   0        0        0     4046 2023-03-13 02:03:53.000000 EpubCrawler-2023.3.14.0/EpubCrawler/util.py
-drwxrwxrwx   0        0        0        0 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler.egg-info/
--rw-rw-rw-   0        0        0     6715 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/EpubCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6715 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/PKG-INFO
--rw-rw-rw-   0        0        0     4279 2023-02-14 05:16:13.000000 EpubCrawler-2023.3.14.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-14 03:55:06.000000 EpubCrawler-2023.3.14.0/setup.cfg
--rw-rw-rw-   0        0        0     1763 2022-03-15 14:47:20.000000 EpubCrawler-2023.3.14.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:52:31.944634 EpubCrawler-2023.7.9.0/
+drwxrwxrwx   0        0        0        0 2023-07-09 13:52:31.940635 EpubCrawler-2023.7.9.0/EpubCrawler/
+-rw-rw-rw-   0        0        0      267 2023-07-09 13:49:30.000000 EpubCrawler-2023.7.9.0/EpubCrawler/__init__.py
+-rw-rw-rw-   0        0        0     5990 2023-07-02 15:28:27.000000 EpubCrawler-2023.7.9.0/EpubCrawler/__main__.py
+-rw-rw-rw-   0        0        0      959 2022-08-20 13:22:25.000000 EpubCrawler-2023.7.9.0/EpubCrawler/common.py
+-rw-rw-rw-   0        0        0      841 2023-07-02 15:52:09.000000 EpubCrawler-2023.7.9.0/EpubCrawler/config.py
+-rw-rw-rw-   0        0        0     3049 2023-02-14 05:10:37.000000 EpubCrawler-2023.7.9.0/EpubCrawler/img.py
+-rw-rw-rw-   0        0        0     5670 2023-07-02 15:34:35.000000 EpubCrawler-2023.7.9.0/EpubCrawler/sele_crawler.py
+-rw-rw-rw-   0        0        0     4046 2023-07-03 14:42:15.000000 EpubCrawler-2023.7.9.0/EpubCrawler/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:52:31.943634 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/
+-rw-rw-rw-   0        0        0     5370 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 13:52:31.000000 EpubCrawler-2023.7.9.0/EpubCrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1838 2022-03-15 14:47:20.000000 EpubCrawler-2023.7.9.0/LICENSE
+-rw-rw-rw-   0        0        0     5370 2023-07-09 13:52:31.943634 EpubCrawler-2023.7.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4279 2023-02-14 05:16:13.000000 EpubCrawler-2023.7.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:52:31.944634 EpubCrawler-2023.7.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1763 2022-03-15 14:47:20.000000 EpubCrawler-2023.7.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `EpubCrawler-2023.3.14.0/EpubCrawler/__main__.py` & `EpubCrawler-2023.7.9.0/EpubCrawler/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,32 +86,38 @@
         art.update(cache)
         art['content'] = process_img(
             art['content'], imgs,
             page_url=url,
             img_prefix='../Images/',
         )
         return
-    
-    html = request_retry(
-        'GET', url,
-        retry=config['retry'],
-        check_status=config['checkStatus'],
-        headers=config['headers'],
-        timeout=config['timeout'],
-        proxies=config['proxy'],
-        verify=False,
-    ).content.decode(config['encoding'], 'ignore')
-    print(f'{url} 下载成功')
-    art.update(get_article(html, url))
+    for i in range(config['retry']):
+        html = request_retry(
+            'GET', url,
+            retry=config['retry'],
+            check_status=config['checkStatus'],
+            headers=config['headers'],
+            timeout=config['timeout'],
+            proxies=config['proxy'],
+            verify=False,
+        ).content.decode(config['encoding'], 'ignore')
+        r = get_article(html, url)
+        if not config['checkBlank'] or \
+           (r['title'] and r['content']):
+           break
+        if i == config['retry'] - 1:
+            raise Exception(f'{url} 标题或内容为空')
+    art.update(r)
     save_article(hash, art)
     art['content'] = process_img(
         art['content'], imgs,
         page_url=url,
         img_prefix='../Images/',
     )
+    print(f'{url} 下载成功')
     time.sleep(config['wait'])
     
 
 def update_config(cfg_fname, user_cfg):
     global get_toc
     global get_article
     
@@ -137,48 +143,14 @@
         
     if not config['timeout']:
         config['timeout'] = (
             config['connTimeout'],
             config['readTimeout'],
         )
 
-def gen_epub_paging(articles, imgs, config):
-    limit = size_str_to_int(config['sizeLimit'])
-    art_part = []
-    img_part = {}
-    total = 0
-    ipt = 1
-    for a in articles:
-        art_imgs = re.findall(r'src="\.\./Images/(\w{32}\.png)"', a['content'])
-        size = sum(
-            len(imgs.get(iname, b'')) 
-            for iname in art_imgs
-        )
-        if total + size >= limit:
-            art_part.insert(0, {
-                'title': config['name'] + f' PT{ipt}',
-                'content': f"<p>来源：<a href='{config['url']}'>{config['url']}</a></p>",
-            })
-            gen_epub(art_part, img_part)
-            art_part = []
-            img_part = {}
-            total = 0
-            ipt += 1
-        art_part.append(a)
-        img_part.update({
-            iname:imgs.get(iname, b'') 
-            for iname in art_imgs
-        })
-        total += size
-    if art_part:
-        art_part.insert(0, {
-            'title': config['name'] + f' PT{ipt}',
-            'content': f"<p>来源：<a href='{config['url']}'>{config['url']}</a></p>",
-        })
-        gen_epub(art_part, img_part)
 
 def main():
     cfg_fname = sys.argv[1] \
         if len(sys.argv) > 1 \
         else 'config.json'
     if not path.exists(cfg_fname):
         print('please provide config file')
@@ -229,18 +201,12 @@
         articles.append(art)
         hdl = text_pool.submit(tr_download_page_safe, url, art, imgs)
         hdls.append(hdl)
             
         
     for h in hdls: h.result()
     articles = [art for art in articles if art]
-            
-    total = sum(len(v) for _, v in imgs.items())
-    limit = size_str_to_int(config['sizeLimit'])
-    if total <= limit:
-        gen_epub(articles, imgs)
-    else:
-        gen_epub_paging(articles[1:], imgs, config)
+    gen_epub(articles, imgs, limit=config['sizeLimit'])
     print('done...')
     
 if __name__ == '__main__': main()
```

### Comparing `EpubCrawler-2023.3.14.0/EpubCrawler/common.py` & `EpubCrawler-2023.7.9.0/EpubCrawler/common.py`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.3.14.0/EpubCrawler/config.py` & `EpubCrawler-2023.7.9.0/EpubCrawler/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     'colors': 8,
     'timeout': None,
     'connTimeout': 10,
     'readTimeout': 60,
 	'imgSrc': ['data-src', 'data-original-src', 'src'],
     'proxy': '',
     'textThreads': 8,
-    'imgThreads': 8,
+    'imgThreads': 24,
     'external': None,
     'checkStatus': False,
+    'checkBlank': True,
     'cache': True,
     'waitContent': False,
     'debug': False,
     'selenium': False,
-    'sizeLimit': '100m',
+    'sizeLimit': '50m',
 }
```

### Comparing `EpubCrawler-2023.3.14.0/EpubCrawler/img.py` & `EpubCrawler-2023.7.9.0/EpubCrawler/img.py`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.3.14.0/EpubCrawler/sele_crawler.py` & `EpubCrawler-2023.7.9.0/EpubCrawler/sele_crawler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pyquery import PyQuery as pq
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.wait import WebDriverWait
+from selenium.webdriver.common.by import By   
 from GenEpub import gen_epub
 from urllib.parse import urljoin
 import sys
 import json
 import re
 import hashlib
 import base64
@@ -93,31 +94,39 @@
     return driver.execute_script('''
         var titlePresent = document.querySelector(arguments[0]) != null
         var contPresent = document.querySelector(arguments[1]) != null
         return titlePresent && contPresent
     ''', config['title'], config['content'])
 
 def download_page(url, art, imgs):
-    print(url)
+    hash = hashlib.md5(url.encode('utf-8')).hexdigest()
+    cache = load_article(hash)
+    if cache is not None and config['cache']:
+        print(f'{url} 已存在于本地缓存中')
+        art.update(cache)
+        art['content'] = process_img(
+            art['content'], imgs,
+            page_url=url,
+            img_prefix='../Images/',
+        )
+        return
     
     if not hasattr(trlocal, 'driver'):
         trlocal.driver = create_driver()
         drivers.append(trlocal.driver)
     driver = trlocal.driver
-    
-    if not re.search(r'^https?://', url):
-        articles.append({'title': url, 'content': ''})
-        return
     driver.get(url)
     # 显式等待
     if config['waitContent']:
         WebDriverWait(driver, config['waitContent'], 0.5) \
             .until(wait_content_cb, "无法获取标题或内容")
-    html = driver.find_element_by_css_selector('body').get_attribute('outerHTML')
+    html = driver.find_element(By.CSS_SELECTOR, 'body').get_attribute('outerHTML')
     art.update(get_article(html, url))
+    save_article(hash, art)
+    print(f'{url} 下载成功')
     art['content'] = process_img(art['content'], imgs, page_url=url, img_prefix='../Images/')
     time.sleep(config['wait'])
 
 def download_page_safe(url, art, imgs):
     try: download_page(url, art, imgs)
     except: traceback.print_exc()
 
@@ -143,18 +152,21 @@
         'title': config['name'],
         'content': f"<p>来源：<a href='" + config['url'] + "'>" + config['url'] + "</a></p>"
     }]
     imgs = {}
     pool = ThreadPoolExecutor(config['textThreads'])
     hdls = []
     for url in config['list']:
+        if not re.search(r'^https?://', url):
+            articles.append({'title': url, 'content': ''})
+            continue
         art = {}
         articles.append(art)
         h = pool.submit(download_page_safe, url, art, imgs)
         hdls.append(h)
         # download_page_safe(driver, url, articles, imgs)
     for h in hdls: h.result()
     
     articles = [art for art in articles if art]
-    gen_epub(articles, imgs)
+    gen_epub(articles, imgs, limit=config['sizeLimit'])
     
     for d in drivers: d.close()
```

### Comparing `EpubCrawler-2023.3.14.0/EpubCrawler/util.py` & `EpubCrawler-2023.7.9.0/EpubCrawler/util.py`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.3.14.0/README.md` & `EpubCrawler-2023.7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `EpubCrawler-2023.3.14.0/setup.py` & `EpubCrawler-2023.7.9.0/setup.py`

 * *Files identical despite different names*

