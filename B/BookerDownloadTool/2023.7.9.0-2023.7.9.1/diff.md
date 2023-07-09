# Comparing `tmp/BookerDownloadTool-2023.7.9.0.tar.gz` & `tmp/BookerDownloadTool-2023.7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BookerDownloadTool-2023.7.9.0.tar", last modified: Sun Jul  9 13:55:28 2023, max compression
+gzip compressed data, was "BookerDownloadTool-2023.7.9.1.tar", last modified: Sun Jul  9 15:35:03 2023, max compression
```

## Comparing `BookerDownloadTool-2023.7.9.0.tar` & `BookerDownloadTool-2023.7.9.1.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/
-drwxrwxrwx   0        0        0        0 2023-07-09 13:55:28.271549 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/
--rw-rw-rw-   0        0        0      236 2023-07-09 13:54:54.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/__init__.py
--rw-rw-rw-   0        0        0    11165 2023-07-07 20:03:27.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/__main__.py
--rw-rw-rw-   0        0        0     4982 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/bili.py
--rw-rw-rw-   0        0        0     8003 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/discuz.py
--rw-rw-rw-   0        0        0     1273 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dl_gh_book.py
--rw-rw-rw-   0        0        0     5202 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dmzj.py
--rw-rw-rw-   0        0        0     4778 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/lightnovel.py
--rw-rw-rw-   0        0        0     3875 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/nhentai.py
--rw-rw-rw-   0        0        0   166307 2022-03-28 16:27:49.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/stealth.min.js
--rw-rw-rw-   0        0        0     4055 2023-07-07 16:21:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/util.py
--rw-rw-rw-   0        0        0     1644 2023-07-07 16:21:54.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/whole_site.py
--rw-rw-rw-   0        0        0     2326 2023-07-04 14:56:41.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zhihu_old.py
--rw-rw-rw-   0        0        0     8636 2023-07-08 12:22:50.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zhihu_sele.py
--rw-rw-rw-   0        0        0     5699 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zsxq.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/
--rw-rw-rw-   0        0        0     1169 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1844 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/LICENSE
--rw-rw-rw-   0        0        0     1169 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       20 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2095 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:35:03.167334 BookerDownloadTool-2023.7.9.1/
+drwxrwxrwx   0        0        0        0 2023-07-09 15:35:03.163334 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/
+-rw-rw-rw-   0        0        0      236 2023-07-09 15:34:12.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/__init__.py
+-rw-rw-rw-   0        0        0    15300 2023-07-09 15:31:34.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/__main__.py
+-rw-rw-rw-   0        0        0     4982 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/bili.py
+-rw-rw-rw-   0        0        0     8003 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/discuz.py
+-rw-rw-rw-   0        0        0     1273 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/dl_gh_book.py
+-rw-rw-rw-   0        0        0     5202 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/dmzj.py
+-rw-rw-rw-   0        0        0     4778 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/lightnovel.py
+-rw-rw-rw-   0        0        0     4565 2023-07-09 15:22:11.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/links.py
+-rw-rw-rw-   0        0        0     1287 2023-07-09 15:17:22.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/medium.py
+-rw-rw-rw-   0        0        0     3875 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/nhentai.py
+-rw-rw-rw-   0        0        0   166307 2022-03-28 16:27:49.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/stealth.min.js
+-rw-rw-rw-   0        0        0     4055 2023-07-07 16:21:28.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/util.py
+-rw-rw-rw-   0        0        0     1511 2023-07-09 15:19:40.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/webarchive.py
+-rw-rw-rw-   0        0        0     1644 2023-07-07 16:21:54.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/whole_site.py
+-rw-rw-rw-   0        0        0     1925 2023-04-12 12:54:44.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/wx.py
+-rw-rw-rw-   0        0        0      998 2023-03-02 07:04:12.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/wx_external.py
+-rw-rw-rw-   0        0        0     2326 2023-07-04 14:56:41.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/zhihu_old.py
+-rw-rw-rw-   0        0        0     8636 2023-07-08 12:22:50.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/zhihu_sele.py
+-rw-rw-rw-   0        0        0     5699 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool/zsxq.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:35:03.166334 BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/
+-rw-rw-rw-   0        0        0     1169 2023-07-09 15:35:03.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2023-07-09 15:35:03.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:35:03.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-07-09 15:35:03.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-07-09 15:35:03.000000 BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1844 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1169 2023-07-09 15:35:03.166334 BookerDownloadTool-2023.7.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:35:03.167334 BookerDownloadTool-2023.7.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.1/setup.py
```

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/__main__.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from .lightnovel import *
 from .dl_gh_book import *
 from .bili import *
 from .dmzj import *
 from .discuz import *
 from .zsxq import *
 from .whole_site import *
+from .medium import *
+from .webarchive import *
+from .links import *
+from .wx import *
 
 def main():
     parser = argparse.ArgumentParser(prog="BookerDownloadTool", formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("-v", "--version", action="version", version=f"PYBP version: {__version__}")
     parser.set_defaults(func=lambda x: parser.print_help())
     subparsers = parser.add_subparsers()
     
@@ -159,12 +163,68 @@
     zsxq_parser.add_argument('-c', '--cookie', default=os.environ.get('ZSXQ_COOKIE'), help="zsxq cookie, default as $ZSXQ_COOKIE")
     zsxq_parser.add_argument('id', help='zsxq group id')
     zsxq_parser.set_defaults(func=download_zsxq)
 
     whole_site_parser = subparsers.add_parser("whole-site", help="crawl whole site urls")
     whole_site_parser.add_argument("site", help="site url")
     whole_site_parser.set_defaults(func=whole_site)
+    
+    med_parser = subparsers.add_parser("medium", help="fetch medium toc")
+    med_parser.add_argument("host", help="medium blog host: xxx.medium.com or medium.com/xxx")
+    med_parser.add_argument('-s', '--start', default='20150101', help="starting date")
+    med_parser.add_argument('-e', '--end', default='99991231', help="ending date")
+    med_parser.add_argument('-p', '--proxy', help="proxy")
+    med_parser.set_defaults(func=fetch_medium)
+
+    war_parser = subparsers.add_parser("web-archive", help="fetch web archive")
+    war_parser.add_argument("host", help="host")
+    war_parser.add_argument("-s", "--start", type=int, default=1, help="starting page")
+    war_parser.add_argument("-e", "--end", type=int, default=1_000_000_000, help="ending page")
+    war_parser.add_argument("-r", "--regex", default='.', help="regex to match urls")
+    war_parser.add_argument("-q", "--query", action='store_true', help="whether to deduplicate with query")
+    war_parser.add_argument("-f", "--fragment", action='store_true', help="whether to deduplicate with fragment")
+    war_parser.add_argument("-p", "--proxy", help="proxy")
+    war_parser.set_defaults(vis=set())
+    war_parser.set_defaults(func=fetch_webarchive)
+
+    links_parser = subparsers.add_parser("links", help="fetch links in pages")
+    links_parser.add_argument("url", help="url with {i} as page num")
+    links_parser.add_argument("link", help="link selector")
+    links_parser.add_argument("ofname", help="output file name")
+    links_parser.add_argument("-s", "--start", type=int, default=1, help="starting page")
+    links_parser.add_argument("-e", "--end", type=int, default=10000000, help="ending page")
+    links_parser.add_argument("-t", "--time", help="time selector")
+    links_parser.add_argument("-r", "--time-regex", default=r"\d+-\d+-\d+", help="time regex")
+    links_parser.add_argument("-p", "--proxy", help="proxy")
+    links_parser.add_argument("-H", "--headers", help="headers in JSON")
+    links_parser.add_argument("-J", "--json", action='store_true', help="treat output as JSON not HTML")
+    links_parser.set_defaults(func=fetch_links)
+
+    sitemap_parser = subparsers.add_parser("sitemap", help="fetch links in sitemap")
+    sitemap_parser.add_argument("url", help="sitemap url")
+    sitemap_parser.add_argument("-r", "--regex", default="/blog/", help="link regex")
+    sitemap_parser.add_argument("-o", "--ofname", help="output file name")
+    sitemap_parser.set_defaults(func=fetch_sitemap_handle)
+
+    links_epub_parser = subparsers.add_parser("links-epub", help="batch download links to epub")
+    links_epub_parser.add_argument("links", help="name of file storing links")
+    links_epub_parser.add_argument("--name", help="epub name")
+    links_epub_parser.add_argument("-t", "--title", default="", help="title selector")
+    links_epub_parser.add_argument("-c", "--content", default="", help="content selector")
+    links_epub_parser.add_argument("-r", "--remove", default="", help="remove elems selector")
+    links_epub_parser.add_argument("-n", "--num", default=500, type=int, help="num of articles in one epub")
+    links_epub_parser.add_argument("-m", "--opti-mode", default='quant', help="img optimization mode")
+    links_epub_parser.add_argument("-l", "--size-limit", default='100m', help="epub size limit")
+    links_epub_parser.add_argument("-g", "--time-regex", default=r'(\d+)-(\d+)-(\d+)', help="time regex")
+    links_epub_parser.add_argument("-E", "--exec", action='store_true', help="whether to execute EpubCrawler on config files")
+    links_epub_parser.set_defaults(func=batch_links)
+
+    wx_parser = subparsers.add_parser("wx", help="crawler weixin articles")
+    wx_parser.add_argument("fname", help="XLSX fname")
+    wx_parser.add_argument("-n", "--size", type=int, default=500, help="num of articles per ebook")
+    wx_parser.add_argument("-o", "--opti-mode", default='thres', help="img optimization mode, default 'thres'")
+    wx_parser.set_defaults(func=crawl_wx)
 
     args = parser.parse_args()
     args.func(args)
     
 if __name__ == '__main__': main()
```

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/bili.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/bili.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/discuz.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/discuz.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dl_gh_book.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/dl_gh_book.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dmzj.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/dmzj.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/lightnovel.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/lightnovel.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/nhentai.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/nhentai.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/stealth.min.js` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/stealth.min.js`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/util.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/util.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/whole_site.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/whole_site.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zhihu_old.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/zhihu_old.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zhihu_sele.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/zhihu_sele.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zsxq.py` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool/zsxq.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/PKG-INFO` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerDownloadTool
-Version: 2023.7.9.0
+Version: 2023.7.9.1
 Summary: book download tool for ApacheCN
 Home-page: https://github.com/apachecn/BookerDownloadTool
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/SOURCES.txt` & `BookerDownloadTool-2023.7.9.1/BookerDownloadTool.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,18 +4,23 @@
 BookerDownloadTool/__init__.py
 BookerDownloadTool/__main__.py
 BookerDownloadTool/bili.py
 BookerDownloadTool/discuz.py
 BookerDownloadTool/dl_gh_book.py
 BookerDownloadTool/dmzj.py
 BookerDownloadTool/lightnovel.py
+BookerDownloadTool/links.py
+BookerDownloadTool/medium.py
 BookerDownloadTool/nhentai.py
 BookerDownloadTool/stealth.min.js
 BookerDownloadTool/util.py
+BookerDownloadTool/webarchive.py
 BookerDownloadTool/whole_site.py
+BookerDownloadTool/wx.py
+BookerDownloadTool/wx_external.py
 BookerDownloadTool/zhihu_old.py
 BookerDownloadTool/zhihu_sele.py
 BookerDownloadTool/zsxq.py
 BookerDownloadTool.egg-info/PKG-INFO
 BookerDownloadTool.egg-info/SOURCES.txt
 BookerDownloadTool.egg-info/dependency_links.txt
 BookerDownloadTool.egg-info/entry_points.txt
```

### Comparing `BookerDownloadTool-2023.7.9.0/LICENSE` & `BookerDownloadTool-2023.7.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.7.9.0/PKG-INFO` & `BookerDownloadTool-2023.7.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BookerDownloadTool
-Version: 2023.7.9.0
+Version: 2023.7.9.1
 Summary: book download tool for ApacheCN
 Home-page: https://github.com/apachecn/BookerDownloadTool
 Author: wizardforcel
 Author-email: wizard.z@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `BookerDownloadTool-2023.7.9.0/setup.py` & `BookerDownloadTool-2023.7.9.1/setup.py`

 * *Files identical despite different names*

