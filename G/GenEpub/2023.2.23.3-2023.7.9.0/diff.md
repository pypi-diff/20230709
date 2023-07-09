# Comparing `tmp/GenEpub-2023.2.23.3.tar.gz` & `tmp/GenEpub-2023.7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\GenEpub-2023.2.23.3.tar", last modified: Fri Mar 10 08:19:38 2023, max compression
+gzip compressed data, was "GenEpub-2023.7.9.0.tar", last modified: Sun Jul  9 13:45:41 2023, max compression
```

## Comparing `GenEpub-2023.2.23.3.tar` & `GenEpub-2023.7.9.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/
-drwxrwxrwx   0        0        0        0 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub/
--rw-rw-rw-   0        0        0     2646 2023-03-10 08:19:33.000000 GenEpub-2023.2.23.3/GenEpub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub/assets/
--rw-rw-rw-   0        0        0     6073 2023-02-23 14:13:34.000000 GenEpub-2023.2.23.3/GenEpub/assets/Style.css
--rw-rw-rw-   0        0        0        0 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/GenEpub/assets/__init__.py
--rw-rw-rw-   0        0        0      373 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/GenEpub/assets/article.j2
--rw-rw-rw-   0        0        0      265 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/GenEpub/assets/container.xml
--rw-rw-rw-   0        0        0     1198 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/GenEpub/assets/content.j2
--rw-rw-rw-   0        0        0       20 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/GenEpub/assets/mimetype
--rw-rw-rw-   0        0        0      767 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/GenEpub/assets/toc.j2
-drwxrwxrwx   0        0        0        0 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub.egg-info/
--rw-rw-rw-   0        0        0     2873 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/GenEpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2873 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/PKG-INFO
--rw-rw-rw-   0        0        0     1344 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-10 08:19:38.000000 GenEpub-2023.2.23.3/setup.cfg
--rw-rw-rw-   0        0        0     1541 2021-08-21 04:17:00.000000 GenEpub-2023.2.23.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:45:41.759060 GenEpub-2023.7.9.0/
+drwxrwxrwx   0        0        0        0 2023-07-09 13:45:41.747602 GenEpub-2023.7.9.0/GenEpub/
+-rw-rw-rw-   0        0        0     3990 2023-07-09 13:44:06.000000 GenEpub-2023.7.9.0/GenEpub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:45:41.757599 GenEpub-2023.7.9.0/GenEpub/assets/
+-rw-rw-rw-   0        0        0     6073 2023-02-23 14:13:34.000000 GenEpub-2023.7.9.0/GenEpub/assets/Style.css
+-rw-rw-rw-   0        0        0        0 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/GenEpub/assets/__init__.py
+-rw-rw-rw-   0        0        0      373 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/GenEpub/assets/article.j2
+-rw-rw-rw-   0        0        0      265 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/GenEpub/assets/container.xml
+-rw-rw-rw-   0        0        0     1198 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/GenEpub/assets/content.j2
+-rw-rw-rw-   0        0        0       20 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/GenEpub/assets/mimetype
+-rw-rw-rw-   0        0        0      767 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/GenEpub/assets/toc.j2
+-rw-rw-rw-   0        0        0      986 2023-07-03 14:43:46.000000 GenEpub-2023.7.9.0/GenEpub/util.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:45:41.750600 GenEpub-2023.7.9.0/GenEpub.egg-info/
+-rw-rw-rw-   0        0        0     2344 2023-07-09 13:45:41.000000 GenEpub-2023.7.9.0/GenEpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-07-09 13:45:41.000000 GenEpub-2023.7.9.0/GenEpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:45:41.000000 GenEpub-2023.7.9.0/GenEpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-09 13:45:41.000000 GenEpub-2023.7.9.0/GenEpub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 13:45:41.000000 GenEpub-2023.7.9.0/GenEpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1834 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2344 2023-07-09 13:45:41.758600 GenEpub-2023.7.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1344 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:45:41.759599 GenEpub-2023.7.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1541 2021-08-21 04:17:00.000000 GenEpub-2023.7.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `GenEpub-2023.2.23.3/GenEpub/assets/Style.css` & `GenEpub-2023.7.9.0/GenEpub/assets/Style.css`

 * *Files identical despite different names*

### Comparing `GenEpub-2023.2.23.3/GenEpub/assets/content.j2` & `GenEpub-2023.7.9.0/GenEpub/assets/content.j2`

 * *Files identical despite different names*

### Comparing `GenEpub-2023.2.23.3/GenEpub/assets/toc.j2` & `GenEpub-2023.7.9.0/GenEpub/assets/toc.j2`

 * *Files identical despite different names*

### Comparing `GenEpub-2023.2.23.3/GenEpub.egg-info/PKG-INFO` & `GenEpub-2023.7.9.0/GenEpub.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,15 @@
 Metadata-Version: 2.1
 Name: GenEpub
-Version: 2023.2.23.3
+Version: 2023.7.9.0
 Summary: GenEpub，用于生成 EPUB 的小工具
 Home-page: https://github.com/apachecn/gen-epub
-Author: ApacheCN
-Author-email: apachecn@163.com
-License: UNKNOWN
-Description: # gen-epub
-        
-        用于生成 EPUB 的小工具。
-        
-        ## 安装
-        
-        通过 pypi（推荐）：
-        
-        ```
-        pip install GenEpub
-        ```
-        
-        从源码安装：
-        
-        ```
-        pip install git+https://github.com/apachecn/gen-epub
-        ```
-        
-        ## 导入
-        
-        ```js
-        from GenEpub import gen_epub
-        ```
-        
-        ## 函数参考
-        
-        ```js
-        gen_epub(articles, imgs, name, path)
-        ```
-        
-        +   `articles: [{title: String, content: String}]`
-            
-            文章列表，每个文章以对象表示，`title`属性为标题（纯文本），`content`属性为正文（HTML）。
-            
-            在正文中引用图片时，将`<img>`的`src`属性设为`../Images/{文件名}`。
-            
-        +   `imgs: Map{String: Buffer}`
-        
-            图片字典，键为文件名，值为图片二进制数据。
-            
-        +   `name: String`
-        
-            在书籍元信息中显示的书名，默认为`articles[0].title`。
-            
-        +   `path: String`
-        
-            保存文件的路径名，默认为当前工作目录下的`name + '.epub'`。
-        
-        ## 协议
-        
-        本项目基于 SATA 协议发布。
-        
-        您有义务为此开源项目点赞，并考虑额外给予作者适当的奖励。
-        
-        ## 赞助我们
-        
-        ![](https://home.apachecn.org/img/about/donate.jpg)
-        
-        ## 另见
-        
-        +   [ApacheCN 学习资源](https://docs.apachecn.org/)
-        +   [计算机电子书](http://it-ebooks.flygon.net)
-        +   [布客新知](http://flygon.net/ixinzhi/)
-        
+Author: wizardforcel
+Author-email: wizard.z@qq.com
 Keywords: epub,ebook,电子书
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
@@ -84,7 +18,72 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# gen-epub
+
+用于生成 EPUB 的小工具。
+
+## 安装
+
+通过 pypi（推荐）：
+
+```
+pip install GenEpub
+```
+
+从源码安装：
+
+```
+pip install git+https://github.com/apachecn/gen-epub
+```
+
+## 导入
+
+```js
+from GenEpub import gen_epub
+```
+
+## 函数参考
+
+```js
+gen_epub(articles, imgs, name, path)
+```
+
++   `articles: [{title: String, content: String}]`
+    
+    文章列表，每个文章以对象表示，`title`属性为标题（纯文本），`content`属性为正文（HTML）。
+    
+    在正文中引用图片时，将`<img>`的`src`属性设为`../Images/{文件名}`。
+    
++   `imgs: Map{String: Buffer}`
+
+    图片字典，键为文件名，值为图片二进制数据。
+    
++   `name: String`
+
+    在书籍元信息中显示的书名，默认为`articles[0].title`。
+    
++   `path: String`
+
+    保存文件的路径名，默认为当前工作目录下的`name + '.epub'`。
+
+## 协议
+
+本项目基于 SATA 协议发布。
+
+您有义务为此开源项目点赞，并考虑额外给予作者适当的奖励。
+
+## 赞助我们
+
+![](https://home.apachecn.org/img/about/donate.jpg)
+
+## 另见
+
++   [ApacheCN 学习资源](https://docs.apachecn.org/)
++   [计算机电子书](http://it-ebooks.flygon.net)
++   [布客新知](http://flygon.net/ixinzhi/)
```

### Comparing `GenEpub-2023.2.23.3/PKG-INFO` & `GenEpub-2023.7.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,15 @@
 Metadata-Version: 2.1
 Name: GenEpub
-Version: 2023.2.23.3
+Version: 2023.7.9.0
 Summary: GenEpub，用于生成 EPUB 的小工具
 Home-page: https://github.com/apachecn/gen-epub
-Author: ApacheCN
-Author-email: apachecn@163.com
-License: UNKNOWN
-Description: # gen-epub
-        
-        用于生成 EPUB 的小工具。
-        
-        ## 安装
-        
-        通过 pypi（推荐）：
-        
-        ```
-        pip install GenEpub
-        ```
-        
-        从源码安装：
-        
-        ```
-        pip install git+https://github.com/apachecn/gen-epub
-        ```
-        
-        ## 导入
-        
-        ```js
-        from GenEpub import gen_epub
-        ```
-        
-        ## 函数参考
-        
-        ```js
-        gen_epub(articles, imgs, name, path)
-        ```
-        
-        +   `articles: [{title: String, content: String}]`
-            
-            文章列表，每个文章以对象表示，`title`属性为标题（纯文本），`content`属性为正文（HTML）。
-            
-            在正文中引用图片时，将`<img>`的`src`属性设为`../Images/{文件名}`。
-            
-        +   `imgs: Map{String: Buffer}`
-        
-            图片字典，键为文件名，值为图片二进制数据。
-            
-        +   `name: String`
-        
-            在书籍元信息中显示的书名，默认为`articles[0].title`。
-            
-        +   `path: String`
-        
-            保存文件的路径名，默认为当前工作目录下的`name + '.epub'`。
-        
-        ## 协议
-        
-        本项目基于 SATA 协议发布。
-        
-        您有义务为此开源项目点赞，并考虑额外给予作者适当的奖励。
-        
-        ## 赞助我们
-        
-        ![](https://home.apachecn.org/img/about/donate.jpg)
-        
-        ## 另见
-        
-        +   [ApacheCN 学习资源](https://docs.apachecn.org/)
-        +   [计算机电子书](http://it-ebooks.flygon.net)
-        +   [布客新知](http://flygon.net/ixinzhi/)
-        
+Author: wizardforcel
+Author-email: wizard.z@qq.com
 Keywords: epub,ebook,电子书
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
@@ -84,7 +18,72 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# gen-epub
+
+用于生成 EPUB 的小工具。
+
+## 安装
+
+通过 pypi（推荐）：
+
+```
+pip install GenEpub
+```
+
+从源码安装：
+
+```
+pip install git+https://github.com/apachecn/gen-epub
+```
+
+## 导入
+
+```js
+from GenEpub import gen_epub
+```
+
+## 函数参考
+
+```js
+gen_epub(articles, imgs, name, path)
+```
+
++   `articles: [{title: String, content: String}]`
+    
+    文章列表，每个文章以对象表示，`title`属性为标题（纯文本），`content`属性为正文（HTML）。
+    
+    在正文中引用图片时，将`<img>`的`src`属性设为`../Images/{文件名}`。
+    
++   `imgs: Map{String: Buffer}`
+
+    图片字典，键为文件名，值为图片二进制数据。
+    
++   `name: String`
+
+    在书籍元信息中显示的书名，默认为`articles[0].title`。
+    
++   `path: String`
+
+    保存文件的路径名，默认为当前工作目录下的`name + '.epub'`。
+
+## 协议
+
+本项目基于 SATA 协议发布。
+
+您有义务为此开源项目点赞，并考虑额外给予作者适当的奖励。
+
+## 赞助我们
+
+![](https://home.apachecn.org/img/about/donate.jpg)
+
+## 另见
+
++   [ApacheCN 学习资源](https://docs.apachecn.org/)
++   [计算机电子书](http://it-ebooks.flygon.net)
++   [布客新知](http://flygon.net/ixinzhi/)
```

### Comparing `GenEpub-2023.2.23.3/README.md` & `GenEpub-2023.7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `GenEpub-2023.2.23.3/setup.py` & `GenEpub-2023.7.9.0/setup.py`

 * *Files identical despite different names*

