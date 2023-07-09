# Comparing `tmp/BookerDownloadTool-2023.4.27.0.tar.gz` & `tmp/BookerDownloadTool-2023.7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BookerDownloadTool-2023.4.27.0.tar", last modified: Thu Apr 27 01:52:11 2023, max compression
+gzip compressed data, was "BookerDownloadTool-2023.7.9.0.tar", last modified: Sun Jul  9 13:55:28 2023, max compression
```

## Comparing `BookerDownloadTool-2023.4.27.0.tar` & `BookerDownloadTool-2023.7.9.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/
-drwxrwxrwx   0        0        0        0 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/
--rw-rw-rw-   0        0        0      234 2023-04-27 01:49:50.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/__init__.py
--rw-rw-rw-   0        0        0     8945 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/__main__.py
--rw-rw-rw-   0        0        0     3408 2023-04-20 02:11:02.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/bili.py
--rw-rw-rw-   0        0        0     8003 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/discuz.py
--rw-rw-rw-   0        0        0     1273 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/dl_gh_book.py
--rw-rw-rw-   0        0        0     5202 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/dmzj.py
--rw-rw-rw-   0        0        0     4649 2022-08-20 12:53:30.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/lightnovel.py
--rw-rw-rw-   0        0        0     3875 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/nhentai.py
--rw-rw-rw-   0        0        0   166307 2022-03-28 16:27:49.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/stealth.min.js
--rw-rw-rw-   0        0        0     2784 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/util.py
--rw-rw-rw-   0        0        0     2326 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/zhihu_ques.py
--rw-rw-rw-   0        0        0     4640 2023-04-27 01:49:25.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool/zhihu_ques_sele.py
-drwxrwxrwx   0        0        0        0 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/
--rw-rw-rw-   0        0        0     1192 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      604 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-27 01:52:10.000000 BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1192 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/PKG-INFO
--rw-rw-rw-   0        0        0       20 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.4.27.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 01:52:11.000000 BookerDownloadTool-2023.4.27.0/setup.cfg
--rw-rw-rw-   0        0        0     2095 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.4.27.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/
+drwxrwxrwx   0        0        0        0 2023-07-09 13:55:28.271549 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/
+-rw-rw-rw-   0        0        0      236 2023-07-09 13:54:54.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/__init__.py
+-rw-rw-rw-   0        0        0    11165 2023-07-07 20:03:27.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/__main__.py
+-rw-rw-rw-   0        0        0     4982 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/bili.py
+-rw-rw-rw-   0        0        0     8003 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/discuz.py
+-rw-rw-rw-   0        0        0     1273 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dl_gh_book.py
+-rw-rw-rw-   0        0        0     5202 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dmzj.py
+-rw-rw-rw-   0        0        0     4778 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/lightnovel.py
+-rw-rw-rw-   0        0        0     3875 2023-06-10 03:19:57.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/nhentai.py
+-rw-rw-rw-   0        0        0   166307 2022-03-28 16:27:49.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/stealth.min.js
+-rw-rw-rw-   0        0        0     4055 2023-07-07 16:21:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/util.py
+-rw-rw-rw-   0        0        0     1644 2023-07-07 16:21:54.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/whole_site.py
+-rw-rw-rw-   0        0        0     2326 2023-07-04 14:56:41.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zhihu_old.py
+-rw-rw-rw-   0        0        0     8636 2023-07-08 12:22:50.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zhihu_sele.py
+-rw-rw-rw-   0        0        0     5699 2023-06-24 02:12:43.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zsxq.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/
+-rw-rw-rw-   0        0        0     1169 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-07-09 13:55:28.000000 BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1844 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/LICENSE
+-rw-rw-rw-   0        0        0     1169 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:55:28.274551 BookerDownloadTool-2023.7.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2022-08-20 12:28:23.000000 BookerDownloadTool-2023.7.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/__main__.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import argparse
 import sys
 from . import __version__
-from .zhihu_ques_sele import *
-from .zhihu_ques import *
+from .zhihu_sele import *
 from .lightnovel import *
 from .dl_gh_book import *
 from .bili import *
 from .dmzj import *
 from .discuz import *
+from .zsxq import *
+from .whole_site import *
 
 def main():
     parser = argparse.ArgumentParser(prog="BookerDownloadTool", formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument("-v", "--version", action="version", version=f"PYBP version: {__version__}")
     parser.set_defaults(func=lambda x: parser.print_help())
     subparsers = parser.add_subparsers()
     
@@ -46,14 +47,22 @@
     bili_home_parser.add_argument("-e", "--end", type=int, default=1_000_000, help="ending page for video list")
     bili_home_parser.add_argument("-a", "--audio", type=bool, default=False, help="whether to convert to audio")
     bili_home_parser.add_argument("--start_page", type=int, default=1, help="start page for every video")
     bili_home_parser.add_argument("--end_page", type=int, default=1_000_000, help="end page for every video")
     bili_home_parser.add_argument("-o", "--output_dir", default='.', help="output dir")
     bili_home_parser.set_defaults(func=batch_home_bili)
     
+    bili_meta_parser = subparsers.add_parser("bili-meta", help="download bilibili meta")
+    bili_meta_parser.add_argument("-s", "--start", type=int, default=1, help="starting page for video list")
+    bili_meta_parser.add_argument("-e", "--end", type=int, default=1_000_000, help="ending page for video list")
+    bili_meta_parser.add_argument("-t", "--threads", type=int, default=1, help="thread num")
+    bili_meta_parser.add_argument("-r", "--retry", type=int, default=10, help="retry times")
+    bili_meta_parser.add_argument("-w", "--wait", type=float, default=0, help="sec to wait")
+    bili_meta_parser.set_defaults(func=download_meta_bili)
+
     ln_parser = subparsers.add_parser("ln", help="download lightnovel")
     ln_parser.add_argument("id", help="id")
     ln_parser.add_argument("-s", "--save-path", default='out', help="path to save")
     ln_parser.add_argument("-c", "--cookie", default=os.environ.get('WK8_COOKIE', ''), help="wenku8.net cookie")
     ln_parser.set_defaults(func=download_ln)
 
     ln_batch_parser = subparsers.add_parser("batch-ln", help="download lightnovel in batch")
@@ -65,23 +74,35 @@
     ln_fetch_parser = subparsers.add_parser("fetch-ln", help="fetch lightnovel ids")
     ln_fetch_parser.add_argument("fname", help="file fname")
     ln_fetch_parser.add_argument("-c", "--cookie", default=os.environ.get('WK8_COOKIE', ''), help="wenku8.net cookie")
     ln_fetch_parser.add_argument("-s", "--start", required=True, help="starting date (YYYYMMDD)")
     ln_fetch_parser.add_argument("-e", "--end", required=True, help="ending date (YYYYMMDD)")
     ln_fetch_parser.set_defaults(func=fetch_ln)
     
-    zhihu_ques_parser = subparsers.add_parser("zhihu-ques", help="crawl zhihu question by requests")
+    zhihu_ques_parser = subparsers.add_parser("zhihu-ques", help="crawl zhihu answers of a question by **selenium**")
     zhihu_ques_parser.add_argument("qid", help="qid")
-    zhihu_ques_parser.add_argument("-o", "--opti-mode", default='thres', help="img optimazation mode, default 'thres'")
-    zhihu_ques_parser.set_defaults(func=zhihu_ques)
-
-    zhihu_ques_sele_parser = subparsers.add_parser("zhihu-ques-sele", help="crawl zhihu question by **selenium**")
-    zhihu_ques_sele_parser.add_argument("qid", help="qid")
-    zhihu_ques_sele_parser.set_defaults(func=zhihu_ques_sele)
+    zhihu_ques_parser.set_defaults(func=zhihu_ques_sele)
     
+    zhihu_ques_batch_parser = subparsers.add_parser("zhihu-ques-batch", help="crawl zhihu answers of a question by **selenium**")
+    zhihu_ques_batch_parser.add_argument("fname", help="fname of qids")
+    zhihu_ques_batch_parser.set_defaults(func=zhihu_ques_batch_sele)
+    
+    zhihu_topic_parser = subparsers.add_parser("zhihu-topic", help="crawl zhihu questions of a topic by **selenium**")
+    zhihu_topic_parser.add_argument("tid", help="tid")
+    zhihu_topic_parser.set_defaults(func=zhihu_topic_sele)
+
+    zhihu_topic_batch_parser = subparsers.add_parser("zhihu-topic-batch", help="crawl zhihu questions of a topic by **selenium**")
+    zhihu_topic_batch_parser.add_argument("fname", help="fname of tids")
+    zhihu_topic_batch_parser.set_defaults(func=zhihu_topic_batch_sele)
+
+    zhihu_topics_parser = subparsers.add_parser("zhihu-topics", help="crawl zhihu sub topics  by **selenium**")
+    zhihu_topics_parser.add_argument("root", help="root tid")
+    zhihu_topics_parser.add_argument("-c", "--cookie", default='', help="zhihu cookie")
+    zhihu_topics_parser.set_defaults(func=zhihu_all_topics_sele)
+
     dmzj_dl_parser = subparsers.add_parser("dmzj", help="download dmzj comic")
     dmzj_dl_parser.add_argument("id", help="id")
     dmzj_dl_parser.add_argument("-o", "--out", default="out", help="output dir")
     dmzj_dl_parser.add_argument("--img-threads", type=int, default=8, help="image threads")
     dmzj_dl_parser.add_argument("--ch-threads", type=int, default=8, help="chapter threads")
     dmzj_dl_parser.add_argument("-l", "--exi-list", default="dmzj_exi.json", help="fname for existed comic")
     dmzj_dl_parser.set_defaults(func=download_dmzj)
@@ -126,12 +147,24 @@
     batch_parser.add_argument("-e", "--end", help="ending date")
     batch_parser.add_argument("-c", "--cookie", default="", help="gn cookie")
     batch_parser.add_argument("-t", "--threads", type=int, default=8, help="num of threads")
     batch_parser.add_argument("-a", "--all", action='store_true', help="whether to crawl all replies")
     batch_parser.add_argument("-l", "--exi-list", default='exi_dz.json', help="existed fnames JSON")
     batch_parser.add_argument("-o", "--out", default='out', help="output dir")
     batch_parser.set_defaults(func=batch_dz)
+    
+    now = datetime.now()
+    zsxq_parser = subparsers.add_parser("zsxq", help="download zsxq")
+    zsxq_parser.add_argument('-s', '--start', default='00010101', help="starting date")
+    zsxq_parser.add_argument('-e', '--end', default=f'{now.year}{now.month:02d}{now.day:02d}', help="ending date")
+    zsxq_parser.add_argument('-c', '--cookie', default=os.environ.get('ZSXQ_COOKIE'), help="zsxq cookie, default as $ZSXQ_COOKIE")
+    zsxq_parser.add_argument('id', help='zsxq group id')
+    zsxq_parser.set_defaults(func=download_zsxq)
+
+    whole_site_parser = subparsers.add_parser("whole-site", help="crawl whole site urls")
+    whole_site_parser.add_argument("site", help="site url")
+    whole_site_parser.set_defaults(func=whole_site)
 
     args = parser.parse_args()
     args.func(args)
     
 if __name__ == '__main__': main()
```

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/discuz.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/discuz.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/dl_gh_book.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dl_gh_book.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/dmzj.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/dmzj.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/lightnovel.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/lightnovel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-import os
-import sys
-import shutil
-import copy
-import subprocess as subp
-from os import path
-import re
-import tempfile
-import uuid
-import json
-from concurrent.futures import ThreadPoolExecutor
-import requests
-from pyquery import PyQuery as pq
-from GenEpub import gen_epub
-from .util import *
-    
-def format_text(text):
-    # 多个换行变为一个
-    text = re.sub(r'(\r\n)+', '\r\n', text)
-    # 去掉前两行
-    text = re.sub(r'^.+?\r\n.+?\r\n', '', text)
-    # 去掉后两行
-    text = re.sub(r'\r\n.+?\r\n.+?$', '', text)
-    # 划分标题和段落
-    def rep_func(m):
-        s = m.group(1)
-        return '<p>' + s[4:] + '</p>' \
-            if s.startswith('    ') else \
-            '<!--split--><h1>' + s + '</h1>'
-    text = re.sub(r'^(.+?)$', rep_func, text, flags=re.M)
-    # 拆分章节，过滤空白章节
-    chs = filter(None, text.split('<!--split-->'))
-    # 将章节拆分为标题和内容
-    map_func = lambda x: {
-        'title': re.search(r'<h1>(.+?)</h1>', x).group(1),
-        'content': re.sub(r'<h1>.+?<\/h1>', '', x),
-    }
-    return list(map(map_func, chs))
-    
-def get_info(html):
-    root = pq(html)
-    dt = root('#content > div:nth-child(1) > table:nth-child(1) tr:nth-child(2) > td:nth-child(4)').text()[5:].replace('-', '') or 'UNKNOWN'
-    url = root('#content > div:nth-child(1) > div:nth-child(6) > div > span:nth-child(1) > fieldset > div > a').attr('href')
-    title = root('#content > div:nth-child(1) > table:nth-child(1) tr:nth-child(1) > td > table tr > td:nth-child(1) > span > b').text()
-    author = root('#content > div:nth-child(1) > table:nth-child(1) tr:nth-child(2) > td:nth-child(2)').text()[5:]
-    return {'dt': dt, 'url': url, 'title': fname_escape(title), 'author': fname_escape(author)}
-    
-def download_ln(args):
-    id = args.id
-    save_path = args.save_path
-    headers = default_hdrs.copy()
-    headers['Cookie'] = args.cookie
-    
-    url = f'https://www.wenku8.net/book/{id}.htm'
-    html = request_retry('GET', url, headers=headers).content.decode('gbk')
-    info = get_info(html)
-    print(info['title'], info['author'], info['dt'])
-    
-    ofname = f"{save_path}/{info['title']} - {info['author']} - {info['dt']}.epub"
-    if path.exists(ofname):
-        print('已存在')
-        return
-    safe_mkdir(save_path)
-    
-    articles = [{
-        'title': info['title'], 
-        'content': f"<p>作者：{info['author']}</p>",
-    }]
-    url = f'http://dl.wenku8.com/down.php?type=udefault_hdrstf8&id={id}'
-    text = request_retry('GET', url, headers=headers).content.decode('utf-8')
-    chs = format_text(text)
-    articles += chs
-    gen_epub(articles, {}, None, ofname)
-    
-def download_safe(args):
-    try: download_ln(args)
-    except Exception as ex: print(ex)
-    
-def batch_ln(args):
-    fname = args.fname
-    
-    lines = open(fname, encoding='utf-8').read().split('\n')
-    lines = filter(None, map(lambda x: x.strip(), lines))
-    pool = ThreadPoolExecutor(5)
-    hdls = []
-    for id in lines:
-        args = copy.deepcopy(args)
-        args.id = id
-        hdl = pool.submit(download_safe, args)
-        hdls.append(hdl)
-    for h in hdls: h.result()
-    
-def get_toc(html):
-    root = pq(html)
-    el_links = root('table.grid b a')
-    el_dts = root('table.grid div > div:nth-child(2) > p:nth-child(3)')
-    res = []
-    for i in range(len(el_links)):
-        id = re.search(r'/(\d+)\.htm', el_links.eq(i).attr('href')).group(1)
-        dt = el_dts.eq(i).text().split('/')[0][3:].replace('-', '')
-        res.append({'id': id, 'dt': dt})
-    for i in range(1, len(res)):
-        res[i]['dt'] = res[i]['dt'] or res[i - 1]['dt']
-    for i in range(len(res) - 2, -1, -1):
-        res[i]['dt'] = res[i]['dt'] or res[i + 1]['dt']
-    res = [r for r in res if r['dt']]
-    return res
-        
-    
-def fetch_ln(args):
-    fname = args.fname
-    st = args.start
-    ed = args.end
-    headers = default_hdrs.copy()
-    headers['Cookie'] = args.cookie
-
-    ofile = open(fname, 'a', encoding='utf-8')
-    
-    stop = False
-    i = 1
-    while True:
-        if stop: break
-        print(f'page: {i}')
-        url = f'https://www.wenku8.net/modules/article/index.php?page={i}'
-        html = request_retry('GET', url, headers=headers).content.decode('gbk')
-        toc = get_toc(html)
-        if len(toc) == 0: break
-        for bk in toc:
-            if ed and bk['dt'] > ed:
-                continue
-            if st and bk['dt'] < st:
-                stop = True
-                break
-            print(bk['id'], bk['dt'])
-            ofile.write(bk['id'] + '\n')
-        i += 1
-        
-    ofile.close()
-    
-    
-if __name__ == '__main__': main()  
+import os
+import sys
+import shutil
+import copy
+import subprocess as subp
+from os import path
+import re
+import tempfile
+import uuid
+import json
+from concurrent.futures import ThreadPoolExecutor
+import requests
+from pyquery import PyQuery as pq
+from GenEpub import gen_epub
+from .util import *
+    
+def format_text(text):
+    # 多个换行变为一个
+    text = re.sub(r'(\r\n)+', '\r\n', text)
+    # 去掉前两行
+    text = re.sub(r'^.+?\r\n.+?\r\n', '', text)
+    # 去掉后两行
+    text = re.sub(r'\r\n.+?\r\n.+?$', '', text)
+    # 划分标题和段落
+    def rep_func(m):
+        s = m.group(1)
+        return '<p>' + s[4:] + '</p>' \
+            if s.startswith('    ') else \
+            '<!--split--><h1>' + s + '</h1>'
+    text = re.sub(r'^(.+?)$', rep_func, text, flags=re.M)
+    # 拆分章节，过滤空白章节
+    chs = filter(None, text.split('<!--split-->'))
+    # 将章节拆分为标题和内容
+    map_func = lambda x: {
+        'title': re.search(r'<h1>(.+?)</h1>', x).group(1),
+        'content': re.sub(r'<h1>.+?<\/h1>', '', x),
+    }
+    return list(map(map_func, chs))
+    
+def get_info(html):
+    root = pq(html)
+    dt = root('#content > div:nth-child(1) > table:nth-child(1) tr:nth-child(2) > td:nth-child(4)').text()[5:].replace('-', '') or 'UNKNOWN'
+    url = root('#content > div:nth-child(1) > div:nth-child(6) > div > span:nth-child(1) > fieldset > div > a').attr('href')
+    title = root('#content > div:nth-child(1) > table:nth-child(1) tr:nth-child(1) > td > table tr > td:nth-child(1) > span > b').text()
+    author = root('#content > div:nth-child(1) > table:nth-child(1) tr:nth-child(2) > td:nth-child(2)').text()[5:]
+    return {'dt': dt, 'url': url, 'title': fname_escape(title), 'author': fname_escape(author)}
+    
+def download_ln(args):
+    id = args.id
+    save_path = args.save_path
+    headers = default_hdrs.copy()
+    headers['Cookie'] = args.cookie
+    
+    url = f'https://www.wenku8.net/book/{id}.htm'
+    html = request_retry('GET', url, headers=headers).content.decode('gbk')
+    info = get_info(html)
+    print(info['title'], info['author'], info['dt'])
+    
+    ofname = f"{save_path}/{info['title']} - {info['author']} - {info['dt']}.epub"
+    if path.exists(ofname):
+        print('已存在')
+        return
+    safe_mkdir(save_path)
+    
+    articles = [{
+        'title': info['title'], 
+        'content': f"<p>作者：{info['author']}</p>",
+    }]
+    url = f'http://dl.wenku8.com/down.php?type=utf8&id={id}'
+    text = request_retry('GET', url, headers=headers).content.decode('utf-8')
+    chs = format_text(text)
+    articles += chs
+    gen_epub(articles, {}, None, ofname)
+    
+def download_safe(args):
+    try: download_ln(args)
+    except Exception as ex: print(ex)
+    
+def batch_ln(args):
+    fname = args.fname
+    
+    lines = open(fname, encoding='utf-8').read().split('\n')
+    lines = filter(None, map(lambda x: x.strip(), lines))
+    pool = ThreadPoolExecutor(5)
+    hdls = []
+    for id in lines:
+        args = copy.deepcopy(args)
+        args.id = id
+        hdl = pool.submit(download_safe, args)
+        hdls.append(hdl)
+    for h in hdls: h.result()
+    
+def get_toc(html):
+    root = pq(html)
+    el_links = root('table.grid b a')
+    el_dts = root('table.grid div > div:nth-child(2) > p:nth-child(3)')
+    res = []
+    for i in range(len(el_links)):
+        id = re.search(r'/(\d+)\.htm', el_links.eq(i).attr('href')).group(1)
+        dt = el_dts.eq(i).text().split('/')[0][3:].replace('-', '')
+        res.append({'id': id, 'dt': dt})
+    for i in range(1, len(res)):
+        res[i]['dt'] = res[i]['dt'] or res[i - 1]['dt']
+    for i in range(len(res) - 2, -1, -1):
+        res[i]['dt'] = res[i]['dt'] or res[i + 1]['dt']
+    res = [r for r in res if r['dt']]
+    return res
+        
+    
+def fetch_ln(args):
+    fname = args.fname
+    st = args.start
+    ed = args.end
+    headers = default_hdrs.copy()
+    headers['Cookie'] = args.cookie
+
+    ofile = open(fname, 'a', encoding='utf-8')
+    
+    stop = False
+    i = 1
+    while True:
+        if stop: break
+        print(f'page: {i}')
+        url = f'https://www.wenku8.net/modules/article/index.php?page={i}'
+        html = request_retry('GET', url, headers=headers).content.decode('gbk')
+        toc = get_toc(html)
+        if len(toc) == 0: break
+        for bk in toc:
+            if ed and bk['dt'] > ed:
+                continue
+            if st and bk['dt'] < st:
+                stop = True
+                break
+            print(bk['id'], bk['dt'])
+            ofile.write(bk['id'] + '\n')
+        i += 1
+        
+    ofile.close()
+    
+    
+if __name__ == '__main__': main()
```

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/nhentai.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/nhentai.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/stealth.min.js` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/stealth.min.js`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/util.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import os
 import shutil
 from os import path
 import imgyaso
 import subprocess as subp
 import tempfile
 import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
 RE_INFO = r'\[(.+?)\]([^\[]+)'
 
 bili_hdrs = {
-    'User-Agent': 'PostmanRuntime/7.26.8',
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36',
     'Referer': 'https://www.bilibili.com/',
 }
 
 dmzj_hdrs = {
     'Referer': 'http://manhua.dmzj.com/',
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36',
 }
@@ -23,15 +25,15 @@
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36',
 }
 
 UA = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.84 Safari/537.36'
 
 DIR = path.dirname(path.abspath(__file__))
 
-d = lambda name: path.join(path.dirname(__file__, name))
+d = lambda name: path.join(path.dirname(__file__), name)
 
     
 def is_gbk(ch):
     try: 
         ch.encode('gbk')
         return True
     except:
@@ -93,8 +95,39 @@
     open(fname, 'wb').write(img)
     subp.Popen(
         ['wiki-tool', 'anime4k-auto', fname, '-G'], 
         shell=True,
     ).communicate()
     img = open(fname, 'rb').read()
     safe_remove(fname)
-    return img
+    return img
+
+def parse_cookie(cookie):
+    # cookie.split('; ').map(x => x.split('='))
+    #     .filter(x => x.length >= 2)
+    #     .reduce((x, y) =>  {x[y[0]] = y[1]; return x}, {})
+    kvs = [kv.split('=') for kv in cookie.split('; ')]
+    res = {kv[0]:kv[1] for kv in kvs if len(kv) >= 2}
+    return res
+        
+def set_driver_cookie(driver, cookie):
+    if isinstance(cookie, str):
+        cookie = parse_cookie(cookie)
+    for k, v in cookie.items():
+        driver.add_cookie({'name': k, 'value': v})
+
+def create_driver():
+    options = Options()
+    options.add_argument('--headless')
+    options.add_argument('--disable-gpu')
+    options.add_argument('--log-level=3')
+    options.add_argument(f'--user-agent={UA}')
+    options.add_argument("--disable-blink-features=AutomationControlled")
+    driver = webdriver.Chrome(options=options)
+    driver.set_script_timeout(1000)
+    # StealthJS
+    stealth = open(d('stealth.min.js')).read()
+    driver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {
+        "source": stealth
+    })
+    return driver
+
```

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool/zhihu_ques.py` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool/zhihu_old.py`

 * *Files identical despite different names*

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/PKG-INFO` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: BookerDownloadTool
-Version: 2023.4.27.0
+Version: 2023.7.9.0
 Summary: book download tool for ApacheCN
 Home-page: https://github.com/apachecn/BookerDownloadTool
-Author: ApacheCN
-Author-email: apachecn@163.com
-License: UNKNOWN
-Description: # BookerDownloadTool
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
@@ -23,7 +20,10 @@
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Documentation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# BookerDownloadTool
```

### Comparing `BookerDownloadTool-2023.4.27.0/BookerDownloadTool.egg-info/SOURCES.txt` & `BookerDownloadTool-2023.7.9.0/BookerDownloadTool.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+LICENSE
 README.md
 setup.py
 BookerDownloadTool/__init__.py
 BookerDownloadTool/__main__.py
 BookerDownloadTool/bili.py
 BookerDownloadTool/discuz.py
 BookerDownloadTool/dl_gh_book.py
 BookerDownloadTool/dmzj.py
 BookerDownloadTool/lightnovel.py
 BookerDownloadTool/nhentai.py
 BookerDownloadTool/stealth.min.js
 BookerDownloadTool/util.py
-BookerDownloadTool/zhihu_ques.py
-BookerDownloadTool/zhihu_ques_sele.py
+BookerDownloadTool/whole_site.py
+BookerDownloadTool/zhihu_old.py
+BookerDownloadTool/zhihu_sele.py
+BookerDownloadTool/zsxq.py
 BookerDownloadTool.egg-info/PKG-INFO
 BookerDownloadTool.egg-info/SOURCES.txt
 BookerDownloadTool.egg-info/dependency_links.txt
 BookerDownloadTool.egg-info/entry_points.txt
 BookerDownloadTool.egg-info/top_level.txt
```

### Comparing `BookerDownloadTool-2023.4.27.0/PKG-INFO` & `BookerDownloadTool-2023.7.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: BookerDownloadTool
-Version: 2023.4.27.0
+Version: 2023.7.9.0
 Summary: book download tool for ApacheCN
 Home-page: https://github.com/apachecn/BookerDownloadTool
-Author: ApacheCN
-Author-email: apachecn@163.com
-License: UNKNOWN
-Description: # BookerDownloadTool
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
@@ -23,7 +20,10 @@
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Documentation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# BookerDownloadTool
```

### Comparing `BookerDownloadTool-2023.4.27.0/setup.py` & `BookerDownloadTool-2023.7.9.0/setup.py`

 * *Files identical despite different names*

