# Comparing `tmp/cloudoll-2.0.3.tar.gz` & `tmp/cloudoll-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-2.0.3.tar", last modified: Thu Jul  6 03:43:43 2023, max compression
+gzip compressed data, was "cloudoll-2.0.4.tar", last modified: Sun Jul  9 17:09:07 2023, max compression
```

## Comparing `cloudoll-2.0.3.tar` & `cloudoll-2.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.473207 cloudoll-2.0.3/
--rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.3/LICENSE
--rw-r--r--   0 xiaobei    (501) staff       (20)     7131 2023-07-06 03:43:43.472624 cloudoll-2.0.3/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)     6497 2023-07-06 01:49:11.000000 cloudoll-2.0.3/README.md
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.459141 cloudoll-2.0.3/cloudoll/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.463281 cloudoll-2.0.3/cloudoll/error/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/error/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/error/errors.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.463921 cloudoll-2.0.3/cloudoll/logging/
--rw-r--r--   0 xiaobei    (501) staff       (20)     3817 2023-04-26 01:55:04.000000 cloudoll-2.0.3/cloudoll/logging/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.465102 cloudoll-2.0.3/cloudoll/mail/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/mail/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.3/cloudoll/mail/smtp.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.465963 cloudoll-2.0.3/cloudoll/orm/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/orm/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.3/cloudoll/orm/mysql.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.468034 cloudoll-2.0.3/cloudoll/robot/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/robot/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.3/cloudoll/robot/dingtalk.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.3/cloudoll/robot/feishu.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.471761 cloudoll-2.0.3/cloudoll/web/
--rw-r--r--   0 xiaobei    (501) staff       (20)    13965 2023-07-06 01:49:11.000000 cloudoll-2.0.3/cloudoll/web/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.3/cloudoll/web/html.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.3/cloudoll/web/http.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.3/cloudoll/web/jwt.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.3/cloudoll/web/settings.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-06 03:43:43.462197 cloudoll-2.0.3/cloudoll.egg-info/
--rw-r--r--   0 xiaobei    (501) staff       (20)     7131 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)      121 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/requires.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-06 03:43:43.000000 cloudoll-2.0.3/cloudoll.egg-info/top_level.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-06 03:43:43.473381 cloudoll-2.0.3/setup.cfg
--rw-r--r--   0 xiaobei    (501) staff       (20)     4177 2023-07-06 01:49:11.000000 cloudoll-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.806840 cloudoll-2.0.4/
+-rw-rw-rw-   0        0        0     1065 2022-07-18 10:31:06.000000 cloudoll-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     7468 2023-07-09 17:09:07.804738 cloudoll-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6814 2023-07-09 17:04:34.000000 cloudoll-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.746205 cloudoll-2.0.4/cloudoll/
+-rw-rw-rw-   0        0        0        0 2022-07-19 03:42:12.000000 cloudoll-2.0.4/cloudoll/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.768068 cloudoll-2.0.4/cloudoll/error/
+-rw-rw-rw-   0        0        0        0 2022-07-01 10:11:13.000000 cloudoll-2.0.4/cloudoll/error/__init__.py
+-rw-rw-rw-   0        0        0     3549 2022-07-22 04:14:59.000000 cloudoll-2.0.4/cloudoll/error/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.770527 cloudoll-2.0.4/cloudoll/logging/
+-rw-rw-rw-   0        0        0     3942 2023-07-09 17:05:00.000000 cloudoll-2.0.4/cloudoll/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.775343 cloudoll-2.0.4/cloudoll/mail/
+-rw-rw-rw-   0        0        0        0 2022-07-18 02:25:44.000000 cloudoll-2.0.4/cloudoll/mail/__init__.py
+-rw-rw-rw-   0        0        0     5941 2023-05-16 06:40:58.000000 cloudoll-2.0.4/cloudoll/mail/smtp.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.780682 cloudoll-2.0.4/cloudoll/orm/
+-rw-rw-rw-   0        0        0        0 2022-07-01 10:09:39.000000 cloudoll-2.0.4/cloudoll/orm/__init__.py
+-rw-rw-rw-   0        0        0    28854 2023-07-09 17:04:34.000000 cloudoll-2.0.4/cloudoll/orm/mysql.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.785809 cloudoll-2.0.4/cloudoll/robot/
+-rw-rw-rw-   0        0        0        0 2022-07-23 10:06:35.000000 cloudoll-2.0.4/cloudoll/robot/__init__.py
+-rw-rw-rw-   0        0        0     6589 2023-03-26 12:01:43.000000 cloudoll-2.0.4/cloudoll/robot/dingtalk.py
+-rw-rw-rw-   0        0        0     3214 2023-03-26 12:01:43.000000 cloudoll-2.0.4/cloudoll/robot/feishu.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.802314 cloudoll-2.0.4/cloudoll/web/
+-rw-rw-rw-   0        0        0    14435 2023-07-09 17:04:34.000000 cloudoll-2.0.4/cloudoll/web/__init__.py
+-rw-rw-rw-   0        0        0     2170 2022-08-31 06:32:31.000000 cloudoll-2.0.4/cloudoll/web/html.py
+-rw-rw-rw-   0        0        0     3679 2023-05-16 06:41:49.000000 cloudoll-2.0.4/cloudoll/web/http.py
+-rw-rw-rw-   0        0        0     1137 2023-06-05 15:08:43.000000 cloudoll-2.0.4/cloudoll/web/jwt.py
+-rw-rw-rw-   0        0        0      310 2023-06-04 15:40:20.000000 cloudoll-2.0.4/cloudoll/web/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:09:07.762279 cloudoll-2.0.4/cloudoll.egg-info/
+-rw-rw-rw-   0        0        0     7468 2023-07-09 17:09:07.000000 cloudoll-2.0.4/cloudoll.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2023-07-09 17:09:07.000000 cloudoll-2.0.4/cloudoll.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 17:09:07.000000 cloudoll-2.0.4/cloudoll.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-09 17:09:07.000000 cloudoll-2.0.4/cloudoll.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 17:09:07.000000 cloudoll-2.0.4/cloudoll.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 17:09:07.807855 cloudoll-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     4326 2023-07-09 17:08:59.000000 cloudoll-2.0.4/setup.py
```

### Comparing `cloudoll-2.0.3/LICENSE` & `cloudoll-2.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright <YEAR> <COPYRIGHT HOLDER>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright <YEAR> <COPYRIGHT HOLDER>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `cloudoll-2.0.3/PKG-INFO` & `cloudoll-2.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,337 +1,337 @@
-Metadata-Version: 2.1
-Name: cloudoll
-Version: 2.0.3
-Summary: 辅助快速创建可分布的微服务。
-Home-page: https://gitee.com/chuchur/cloudoll-py
-Author: chuchur
-Author-email: chuchur@qq.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# cloudoll 云端玩具
-
-## 更新日志
-`2.0.2` 2023-07-03
-- 优化一系列问题
-- 可以热加载
-
-`2.0.0` 2023-06-09
-- 优化一系列问题
-- orm 执行更优雅
-
-`0.1.6` 2022-11-03
-- orm 允许更新为空数据
-- server 文件上传加入大小限制
-- smtp 出错异常处理
-
-`0.1.5` 2022-09-19
-- 修复logging level 错误的问题
-- 修正默认依赖
- 
-`0.1.4` 2022-09-12
-- 优化orm 超时的问题
-- 增加websocket 支持
-
-
-## Documentation
-
-
-[Docs](https://cloudoll.chuchur.com)
-
-[Docs](https://cloudoll.chuchur.com)
-
-[Structure](https://cloudoll.chuchur.com/structure)
-
-[Config](https://cloudoll.chuchur.com/config)
-
-[Middleware](https://cloudoll.chuchur.com/middleware)
-
-[Router](https://cloudoll.chuchur.com/router)
-
-[View](https://cloudoll.chuchur.com/view)
-
-[Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
-
-[Upload file](https://cloudoll.chuchur.com/file-uploads)
-
-[WebSocket](https://cloudoll.chuchur.com/websockets)
-
-[Mysql](https://cloudoll.chuchur.com/mysql)
-
-[Deployment](https://cloudoll.chuchur.com/deployment)
-
-
-## 环境准备
-
-- 操作系统：支持 macOS，Linux，Windows
-- 运行环境：最低要求 3.6.0。
-
-## 快速开始
-
-```sh
-$ mkdir cloudoll-demo && cd cloudoll-demo
-$ pip3 install cloudoll
-$ vi app.py
-```
-
-`app.py` 内容如下:
-
-```python
-## /app.py
-from cloudoll.web import app
-
-
-if __name__ == "__main__":
-    app.create().run()
-```
-
-### 编写 Controller
-
-```sh
-$ mkdir -p controllers/home
-$ touch controllers/home/__init__.py
-$ vi controllers/home/index.py
-```
-
-`controllers/home/index.py` 内容如下:
-
-```python
-# /controllers/home/index.py
-from cloudoll.web import get, jsons
-
-@get('/')
-async def home():
-    return jsons({"name": "chuchur" ,"msg": "ok"})
-```
-
-运行:
-```sh
-$ python3 app.py
-$ open http://localhost:9001
-```
-
-在浏览器打开 [http://127.0.0.1:9001/](http://127.0.0.1:9001/)
-
-就能看到:
-
-```json
-{ 
-    "name": "chuchur" ,
-    "msg": "ok" ,
-    "timestamp": 1681993906410 
-}
-```
-
-恭喜, 你已经成功的写好了一个 `Restful API`接口. 
-
-
-### 模板渲染
-
-绝大多数情况，我们都需要读取数据后渲染模板，然后呈现给用户。故我们需要引入对应的模板引擎。
-
-在本例中，我们使用 [Nunjucks](https://mozilla.github.io/nunjucks/) 来渲染
-```sh
-$ mkdir templates
-$ vi templates/index.html
-```
-
-`index.html` 内容如下:
-
-```html
-<!-- /templates/index.html -->
-
-<!DOCTYPE html>
-<html lang="zh">
-<head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>Home</title>
-</head>
-<body>
-    <p>My name is {{name} }</p>
-</body>
-</html>
-```
-
-
-修改 `/controllers/home/index.py` 内容如下:
-
-```python
-# /controllers/home/index.py
-from cloudoll.web import get, view
-
-@get('/')
-async def home():
-    data = {"name": "chuchur" ,"msg": "ok"}
-    return view("index.html",data)
-```
-
-这时 页面正常渲染 ,可以看到  `“My name is chuchur”`
-
-恭喜, 你已经成功的写好了一个视图页面.
-
-### 静态资源
-
-我们想在模版里面嵌入静态资源,如图片,js ,css , 这个时候就得用到静态资源. 我们把这些`js` ,`css` ,`image`  都放到 `static` 目录
-
-线上环境建议部署到 CDN，或者使用 `nginx` 等相关服务器
-
-```sh
-$ mkdir -p static/img
-$ mkdir -p static/js
-$ mkdir -p static/css
-```
-在 `img`目录 放入在张图 名`logo.png`
-
-在 `js` 目录新建 `index.js` ,内容如下:
-
-点击页面 弹出 "hello world"
-```js
-// /static/js/index.js
-document.addEventListener('DOMContentLoaded',function(){
-    document.body.addEventListener('click',function(){
-        alert('hello world.')
-    })
-})
-```
-在 `css` 目录新建 `index.css` ,内容如下:
-```css
- /* /static/css/index.css */
-html,body {
-    width: 100%;
-    height: 100%;
-    color: red;
-}
-```
-
-修改视图 `/templates/index.html` ,在 `head` 引入 静态资源, 内容如下:
-
-```html
-<!-- /templates/index.html -->
-<!DOCTYPE html>
-<html lang="zh">
-<head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <link rel="icon" type="image/png" href="/static/img/logo.png"/>
-    <link rel="stylesheet" href="/static/css/index.css">
-    <script src="/static/js/index.js"></script>
-    <title>Home</title>
-</head>
-<body>
-    <p>My name is {{name} }</p>
-</body>
-</html>
-```
-
-我们新建一个配置文件, 在配置文件里面配置静态 资源.
-
-```sh
-$ mkdir config
-$ vi config/conf.local.yaml
-```
-
-`/config/conf.local.yaml` 内容如下:
-
-```yaml
-server:
-  static:
-    prefix: /static
-```
-
-
-刷新页面之后, 我们所改动即可呈现.
-
-### 编写 Middleware
-
-假设有个需求：我们的新闻站点，禁止百度爬虫访问。
-
-所以可以通过 `Middleware` 判断 User-Agent，如下：
-
-```sh
-$ mkdir middlewares
-$ vi middlewares/robot.py
-```
-
-修改 `middlewares/robot.py`, 内容如下:
-
-```python
-# /middlewares/robot.py
-from cloudoll.web import middleware, render
-import re
-
-@middleware()
-def mid_robot():
-    async def robot(request, handler):
-        ua = request.headers.get('user-agent')
-        if re.match('Baiduspider', ua):
-            return render(status=403, text="Go away , robot.")
-        return await handler(request)
-
-    return robot
-```
-
-重新启动之后, 现在可以使用 `curl http://localhost:7001/news -A "Baiduspider"` 看看效果。
-
-更多参见中间件文档。
-
-### 配置文件
-写业务的时候，不可避免的需要有配置文件，使用代码管理配置，在代码中添加多个环境的配置，在启动时传入当前环境的参数即可.
-
-cloudoll 支持根据环境来加载配置，定义多个环境的配置文件
-
-```ini
-config
-|- conf.local.yaml
-|- conf.prod.yaml
-`- conf.test.yaml
-```
-
-我们创建配置文件：
-
-```sh
-$ mkdir -p config/conf.local.yaml
-$ vi config/conf.local.yaml
-```
-
-如下是 mysql 和 server 的配置：
-
-```yaml
-server:
-  host: 192.168.0.1
-  port: 9001
-  static: false
-  client_max_size: 1024000
-  static: 
-    prefix: /static
-    show_index: true
-    append_version: true
-    follow_symlinks: true
-mysql:
-  host: 127.0.0.1
-  port: 3306
-  user: root
-  password: abcd
-  db: blog
-  charset: utf8mb4
-```
-
-默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
-
-
-# 开发模式
-
-```sh
-adev runserver app.py
-```
+Metadata-Version: 2.1
+Name: cloudoll
+Version: 2.0.4
+Summary: 辅助快速创建可分布的微服务。
+Home-page: https://gitee.com/chuchur/cloudoll-py
+Author: chuchur
+Author-email: chuchur@qq.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# cloudoll 云端玩具
+
+## 更新日志
+`2.0.2` 2023-07-03
+- 优化一系列问题
+- 可以热加载
+
+`2.0.0` 2023-06-09
+- 优化一系列问题
+- orm 执行更优雅
+
+`0.1.6` 2022-11-03
+- orm 允许更新为空数据
+- server 文件上传加入大小限制
+- smtp 出错异常处理
+
+`0.1.5` 2022-09-19
+- 修复logging level 错误的问题
+- 修正默认依赖
+ 
+`0.1.4` 2022-09-12
+- 优化orm 超时的问题
+- 增加websocket 支持
+
+
+## Documentation
+
+
+[Docs](https://cloudoll.chuchur.com)
+
+[Docs](https://cloudoll.chuchur.com)
+
+[Structure](https://cloudoll.chuchur.com/structure)
+
+[Config](https://cloudoll.chuchur.com/config)
+
+[Middleware](https://cloudoll.chuchur.com/middleware)
+
+[Router](https://cloudoll.chuchur.com/router)
+
+[View](https://cloudoll.chuchur.com/view)
+
+[Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
+
+[Upload file](https://cloudoll.chuchur.com/file-uploads)
+
+[WebSocket](https://cloudoll.chuchur.com/websockets)
+
+[Mysql](https://cloudoll.chuchur.com/mysql)
+
+[Deployment](https://cloudoll.chuchur.com/deployment)
+
+
+## 环境准备
+
+- 操作系统：支持 macOS，Linux，Windows
+- 运行环境：最低要求 3.6.0。
+
+## 快速开始
+
+```sh
+$ mkdir cloudoll-demo && cd cloudoll-demo
+$ pip3 install cloudoll
+$ vi app.py
+```
+
+`app.py` 内容如下:
+
+```python
+## /app.py
+from cloudoll.web import app
+
+
+if __name__ == "__main__":
+    app.create().run()
+```
+
+### 编写 Controller
+
+```sh
+$ mkdir -p controllers/home
+$ touch controllers/home/__init__.py
+$ vi controllers/home/index.py
+```
+
+`controllers/home/index.py` 内容如下:
+
+```python
+# /controllers/home/index.py
+from cloudoll.web import get, jsons
+
+@get('/')
+async def home():
+    return jsons({"name": "chuchur" ,"msg": "ok"})
+```
+
+运行:
+```sh
+$ python3 app.py
+$ open http://localhost:9001
+```
+
+在浏览器打开 [http://127.0.0.1:9001/](http://127.0.0.1:9001/)
+
+就能看到:
+
+```json
+{ 
+    "name": "chuchur" ,
+    "msg": "ok" ,
+    "timestamp": 1681993906410 
+}
+```
+
+恭喜, 你已经成功的写好了一个 `Restful API`接口. 
+
+
+### 模板渲染
+
+绝大多数情况，我们都需要读取数据后渲染模板，然后呈现给用户。故我们需要引入对应的模板引擎。
+
+在本例中，我们使用 [Nunjucks](https://mozilla.github.io/nunjucks/) 来渲染
+```sh
+$ mkdir templates
+$ vi templates/index.html
+```
+
+`index.html` 内容如下:
+
+```html
+<!-- /templates/index.html -->
+
+<!DOCTYPE html>
+<html lang="zh">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Home</title>
+</head>
+<body>
+    <p>My name is {{name} }</p>
+</body>
+</html>
+```
+
+
+修改 `/controllers/home/index.py` 内容如下:
+
+```python
+# /controllers/home/index.py
+from cloudoll.web import get, view
+
+@get('/')
+async def home():
+    data = {"name": "chuchur" ,"msg": "ok"}
+    return view("index.html",data)
+```
+
+这时 页面正常渲染 ,可以看到  `“My name is chuchur”`
+
+恭喜, 你已经成功的写好了一个视图页面.
+
+### 静态资源
+
+我们想在模版里面嵌入静态资源,如图片,js ,css , 这个时候就得用到静态资源. 我们把这些`js` ,`css` ,`image`  都放到 `static` 目录
+
+线上环境建议部署到 CDN，或者使用 `nginx` 等相关服务器
+
+```sh
+$ mkdir -p static/img
+$ mkdir -p static/js
+$ mkdir -p static/css
+```
+在 `img`目录 放入在张图 名`logo.png`
+
+在 `js` 目录新建 `index.js` ,内容如下:
+
+点击页面 弹出 "hello world"
+```js
+// /static/js/index.js
+document.addEventListener('DOMContentLoaded',function(){
+    document.body.addEventListener('click',function(){
+        alert('hello world.')
+    })
+})
+```
+在 `css` 目录新建 `index.css` ,内容如下:
+```css
+ /* /static/css/index.css */
+html,body {
+    width: 100%;
+    height: 100%;
+    color: red;
+}
+```
+
+修改视图 `/templates/index.html` ,在 `head` 引入 静态资源, 内容如下:
+
+```html
+<!-- /templates/index.html -->
+<!DOCTYPE html>
+<html lang="zh">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <link rel="icon" type="image/png" href="/static/img/logo.png"/>
+    <link rel="stylesheet" href="/static/css/index.css">
+    <script src="/static/js/index.js"></script>
+    <title>Home</title>
+</head>
+<body>
+    <p>My name is {{name} }</p>
+</body>
+</html>
+```
+
+我们新建一个配置文件, 在配置文件里面配置静态 资源.
+
+```sh
+$ mkdir config
+$ vi config/conf.local.yaml
+```
+
+`/config/conf.local.yaml` 内容如下:
+
+```yaml
+server:
+  static:
+    prefix: /static
+```
+
+
+刷新页面之后, 我们所改动即可呈现.
+
+### 编写 Middleware
+
+假设有个需求：我们的新闻站点，禁止百度爬虫访问。
+
+所以可以通过 `Middleware` 判断 User-Agent，如下：
+
+```sh
+$ mkdir middlewares
+$ vi middlewares/robot.py
+```
+
+修改 `middlewares/robot.py`, 内容如下:
+
+```python
+# /middlewares/robot.py
+from cloudoll.web import middleware, render
+import re
+
+@middleware()
+def mid_robot():
+    async def robot(request, handler):
+        ua = request.headers.get('user-agent')
+        if re.match('Baiduspider', ua):
+            return render(status=403, text="Go away , robot.")
+        return await handler(request)
+
+    return robot
+```
+
+重新启动之后, 现在可以使用 `curl http://localhost:7001/news -A "Baiduspider"` 看看效果。
+
+更多参见中间件文档。
+
+### 配置文件
+写业务的时候，不可避免的需要有配置文件，使用代码管理配置，在代码中添加多个环境的配置，在启动时传入当前环境的参数即可.
+
+cloudoll 支持根据环境来加载配置，定义多个环境的配置文件
+
+```ini
+config
+|- conf.local.yaml
+|- conf.prod.yaml
+`- conf.test.yaml
+```
+
+我们创建配置文件：
+
+```sh
+$ mkdir -p config/conf.local.yaml
+$ vi config/conf.local.yaml
+```
+
+如下是 mysql 和 server 的配置：
+
+```yaml
+server:
+  host: 192.168.0.1
+  port: 9001
+  static: false
+  client_max_size: 1024000
+  static: 
+    prefix: /static
+    show_index: true
+    append_version: true
+    follow_symlinks: true
+mysql:
+  host: 127.0.0.1
+  port: 3306
+  user: root
+  password: abcd
+  db: blog
+  charset: utf8mb4
+```
+
+默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
+
+
+# 开发模式
+
+```sh
+adev runserver app.py
+```
```

### Comparing `cloudoll-2.0.3/README.md` & `cloudoll-2.0.4/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-# cloudoll 云端玩具
-
-## 更新日志
-`2.0.2` 2023-07-03
-- 优化一系列问题
-- 可以热加载
-
-`2.0.0` 2023-06-09
-- 优化一系列问题
-- orm 执行更优雅
-
-`0.1.6` 2022-11-03
-- orm 允许更新为空数据
-- server 文件上传加入大小限制
-- smtp 出错异常处理
-
-`0.1.5` 2022-09-19
-- 修复logging level 错误的问题
-- 修正默认依赖
- 
-`0.1.4` 2022-09-12
-- 优化orm 超时的问题
-- 增加websocket 支持
-
-
-## Documentation
-
-
-[Docs](https://cloudoll.chuchur.com)
-
-[Docs](https://cloudoll.chuchur.com)
-
-[Structure](https://cloudoll.chuchur.com/structure)
-
-[Config](https://cloudoll.chuchur.com/config)
-
-[Middleware](https://cloudoll.chuchur.com/middleware)
-
-[Router](https://cloudoll.chuchur.com/router)
-
-[View](https://cloudoll.chuchur.com/view)
-
-[Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
-
-[Upload file](https://cloudoll.chuchur.com/file-uploads)
-
-[WebSocket](https://cloudoll.chuchur.com/websockets)
-
-[Mysql](https://cloudoll.chuchur.com/mysql)
-
-[Deployment](https://cloudoll.chuchur.com/deployment)
-
-
-## 环境准备
-
-- 操作系统：支持 macOS，Linux，Windows
-- 运行环境：最低要求 3.6.0。
-
-## 快速开始
-
-```sh
-$ mkdir cloudoll-demo && cd cloudoll-demo
-$ pip3 install cloudoll
-$ vi app.py
-```
-
-`app.py` 内容如下:
-
-```python
-## /app.py
-from cloudoll.web import app
-
-
-if __name__ == "__main__":
-    app.create().run()
-```
-
-### 编写 Controller
-
-```sh
-$ mkdir -p controllers/home
-$ touch controllers/home/__init__.py
-$ vi controllers/home/index.py
-```
-
-`controllers/home/index.py` 内容如下:
-
-```python
-# /controllers/home/index.py
-from cloudoll.web import get, jsons
-
-@get('/')
-async def home():
-    return jsons({"name": "chuchur" ,"msg": "ok"})
-```
-
-运行:
-```sh
-$ python3 app.py
-$ open http://localhost:9001
-```
-
-在浏览器打开 [http://127.0.0.1:9001/](http://127.0.0.1:9001/)
-
-就能看到:
-
-```json
-{ 
-    "name": "chuchur" ,
-    "msg": "ok" ,
-    "timestamp": 1681993906410 
-}
-```
-
-恭喜, 你已经成功的写好了一个 `Restful API`接口. 
-
-
-### 模板渲染
-
-绝大多数情况，我们都需要读取数据后渲染模板，然后呈现给用户。故我们需要引入对应的模板引擎。
-
-在本例中，我们使用 [Nunjucks](https://mozilla.github.io/nunjucks/) 来渲染
-```sh
-$ mkdir templates
-$ vi templates/index.html
-```
-
-`index.html` 内容如下:
-
-```html
-<!-- /templates/index.html -->
-
-<!DOCTYPE html>
-<html lang="zh">
-<head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>Home</title>
-</head>
-<body>
-    <p>My name is {{name} }</p>
-</body>
-</html>
-```
-
-
-修改 `/controllers/home/index.py` 内容如下:
-
-```python
-# /controllers/home/index.py
-from cloudoll.web import get, view
-
-@get('/')
-async def home():
-    data = {"name": "chuchur" ,"msg": "ok"}
-    return view("index.html",data)
-```
-
-这时 页面正常渲染 ,可以看到  `“My name is chuchur”`
-
-恭喜, 你已经成功的写好了一个视图页面.
-
-### 静态资源
-
-我们想在模版里面嵌入静态资源,如图片,js ,css , 这个时候就得用到静态资源. 我们把这些`js` ,`css` ,`image`  都放到 `static` 目录
-
-线上环境建议部署到 CDN，或者使用 `nginx` 等相关服务器
-
-```sh
-$ mkdir -p static/img
-$ mkdir -p static/js
-$ mkdir -p static/css
-```
-在 `img`目录 放入在张图 名`logo.png`
-
-在 `js` 目录新建 `index.js` ,内容如下:
-
-点击页面 弹出 "hello world"
-```js
-// /static/js/index.js
-document.addEventListener('DOMContentLoaded',function(){
-    document.body.addEventListener('click',function(){
-        alert('hello world.')
-    })
-})
-```
-在 `css` 目录新建 `index.css` ,内容如下:
-```css
- /* /static/css/index.css */
-html,body {
-    width: 100%;
-    height: 100%;
-    color: red;
-}
-```
-
-修改视图 `/templates/index.html` ,在 `head` 引入 静态资源, 内容如下:
-
-```html
-<!-- /templates/index.html -->
-<!DOCTYPE html>
-<html lang="zh">
-<head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <link rel="icon" type="image/png" href="/static/img/logo.png"/>
-    <link rel="stylesheet" href="/static/css/index.css">
-    <script src="/static/js/index.js"></script>
-    <title>Home</title>
-</head>
-<body>
-    <p>My name is {{name} }</p>
-</body>
-</html>
-```
-
-我们新建一个配置文件, 在配置文件里面配置静态 资源.
-
-```sh
-$ mkdir config
-$ vi config/conf.local.yaml
-```
-
-`/config/conf.local.yaml` 内容如下:
-
-```yaml
-server:
-  static:
-    prefix: /static
-```
-
-
-刷新页面之后, 我们所改动即可呈现.
-
-### 编写 Middleware
-
-假设有个需求：我们的新闻站点，禁止百度爬虫访问。
-
-所以可以通过 `Middleware` 判断 User-Agent，如下：
-
-```sh
-$ mkdir middlewares
-$ vi middlewares/robot.py
-```
-
-修改 `middlewares/robot.py`, 内容如下:
-
-```python
-# /middlewares/robot.py
-from cloudoll.web import middleware, render
-import re
-
-@middleware()
-def mid_robot():
-    async def robot(request, handler):
-        ua = request.headers.get('user-agent')
-        if re.match('Baiduspider', ua):
-            return render(status=403, text="Go away , robot.")
-        return await handler(request)
-
-    return robot
-```
-
-重新启动之后, 现在可以使用 `curl http://localhost:7001/news -A "Baiduspider"` 看看效果。
-
-更多参见中间件文档。
-
-### 配置文件
-写业务的时候，不可避免的需要有配置文件，使用代码管理配置，在代码中添加多个环境的配置，在启动时传入当前环境的参数即可.
-
-cloudoll 支持根据环境来加载配置，定义多个环境的配置文件
-
-```ini
-config
-|- conf.local.yaml
-|- conf.prod.yaml
-`- conf.test.yaml
-```
-
-我们创建配置文件：
-
-```sh
-$ mkdir -p config/conf.local.yaml
-$ vi config/conf.local.yaml
-```
-
-如下是 mysql 和 server 的配置：
-
-```yaml
-server:
-  host: 192.168.0.1
-  port: 9001
-  static: false
-  client_max_size: 1024000
-  static: 
-    prefix: /static
-    show_index: true
-    append_version: true
-    follow_symlinks: true
-mysql:
-  host: 127.0.0.1
-  port: 3306
-  user: root
-  password: abcd
-  db: blog
-  charset: utf8mb4
-```
-
-默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
-
-
-# 开发模式
-
-```sh
-adev runserver app.py
+# cloudoll 云端玩具
+
+## 更新日志
+`2.0.2` 2023-07-03
+- 优化一系列问题
+- 可以热加载
+
+`2.0.0` 2023-06-09
+- 优化一系列问题
+- orm 执行更优雅
+
+`0.1.6` 2022-11-03
+- orm 允许更新为空数据
+- server 文件上传加入大小限制
+- smtp 出错异常处理
+
+`0.1.5` 2022-09-19
+- 修复logging level 错误的问题
+- 修正默认依赖
+ 
+`0.1.4` 2022-09-12
+- 优化orm 超时的问题
+- 增加websocket 支持
+
+
+## Documentation
+
+
+[Docs](https://cloudoll.chuchur.com)
+
+[Docs](https://cloudoll.chuchur.com)
+
+[Structure](https://cloudoll.chuchur.com/structure)
+
+[Config](https://cloudoll.chuchur.com/config)
+
+[Middleware](https://cloudoll.chuchur.com/middleware)
+
+[Router](https://cloudoll.chuchur.com/router)
+
+[View](https://cloudoll.chuchur.com/view)
+
+[Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
+
+[Upload file](https://cloudoll.chuchur.com/file-uploads)
+
+[WebSocket](https://cloudoll.chuchur.com/websockets)
+
+[Mysql](https://cloudoll.chuchur.com/mysql)
+
+[Deployment](https://cloudoll.chuchur.com/deployment)
+
+
+## 环境准备
+
+- 操作系统：支持 macOS，Linux，Windows
+- 运行环境：最低要求 3.6.0。
+
+## 快速开始
+
+```sh
+$ mkdir cloudoll-demo && cd cloudoll-demo
+$ pip3 install cloudoll
+$ vi app.py
+```
+
+`app.py` 内容如下:
+
+```python
+## /app.py
+from cloudoll.web import app
+
+
+if __name__ == "__main__":
+    app.create().run()
+```
+
+### 编写 Controller
+
+```sh
+$ mkdir -p controllers/home
+$ touch controllers/home/__init__.py
+$ vi controllers/home/index.py
+```
+
+`controllers/home/index.py` 内容如下:
+
+```python
+# /controllers/home/index.py
+from cloudoll.web import get, jsons
+
+@get('/')
+async def home():
+    return jsons({"name": "chuchur" ,"msg": "ok"})
+```
+
+运行:
+```sh
+$ python3 app.py
+$ open http://localhost:9001
+```
+
+在浏览器打开 [http://127.0.0.1:9001/](http://127.0.0.1:9001/)
+
+就能看到:
+
+```json
+{ 
+    "name": "chuchur" ,
+    "msg": "ok" ,
+    "timestamp": 1681993906410 
+}
+```
+
+恭喜, 你已经成功的写好了一个 `Restful API`接口. 
+
+
+### 模板渲染
+
+绝大多数情况，我们都需要读取数据后渲染模板，然后呈现给用户。故我们需要引入对应的模板引擎。
+
+在本例中，我们使用 [Nunjucks](https://mozilla.github.io/nunjucks/) 来渲染
+```sh
+$ mkdir templates
+$ vi templates/index.html
+```
+
+`index.html` 内容如下:
+
+```html
+<!-- /templates/index.html -->
+
+<!DOCTYPE html>
+<html lang="zh">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Home</title>
+</head>
+<body>
+    <p>My name is {{name} }</p>
+</body>
+</html>
+```
+
+
+修改 `/controllers/home/index.py` 内容如下:
+
+```python
+# /controllers/home/index.py
+from cloudoll.web import get, view
+
+@get('/')
+async def home():
+    data = {"name": "chuchur" ,"msg": "ok"}
+    return view("index.html",data)
+```
+
+这时 页面正常渲染 ,可以看到  `“My name is chuchur”`
+
+恭喜, 你已经成功的写好了一个视图页面.
+
+### 静态资源
+
+我们想在模版里面嵌入静态资源,如图片,js ,css , 这个时候就得用到静态资源. 我们把这些`js` ,`css` ,`image`  都放到 `static` 目录
+
+线上环境建议部署到 CDN，或者使用 `nginx` 等相关服务器
+
+```sh
+$ mkdir -p static/img
+$ mkdir -p static/js
+$ mkdir -p static/css
+```
+在 `img`目录 放入在张图 名`logo.png`
+
+在 `js` 目录新建 `index.js` ,内容如下:
+
+点击页面 弹出 "hello world"
+```js
+// /static/js/index.js
+document.addEventListener('DOMContentLoaded',function(){
+    document.body.addEventListener('click',function(){
+        alert('hello world.')
+    })
+})
+```
+在 `css` 目录新建 `index.css` ,内容如下:
+```css
+ /* /static/css/index.css */
+html,body {
+    width: 100%;
+    height: 100%;
+    color: red;
+}
+```
+
+修改视图 `/templates/index.html` ,在 `head` 引入 静态资源, 内容如下:
+
+```html
+<!-- /templates/index.html -->
+<!DOCTYPE html>
+<html lang="zh">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <link rel="icon" type="image/png" href="/static/img/logo.png"/>
+    <link rel="stylesheet" href="/static/css/index.css">
+    <script src="/static/js/index.js"></script>
+    <title>Home</title>
+</head>
+<body>
+    <p>My name is {{name} }</p>
+</body>
+</html>
+```
+
+我们新建一个配置文件, 在配置文件里面配置静态 资源.
+
+```sh
+$ mkdir config
+$ vi config/conf.local.yaml
+```
+
+`/config/conf.local.yaml` 内容如下:
+
+```yaml
+server:
+  static:
+    prefix: /static
+```
+
+
+刷新页面之后, 我们所改动即可呈现.
+
+### 编写 Middleware
+
+假设有个需求：我们的新闻站点，禁止百度爬虫访问。
+
+所以可以通过 `Middleware` 判断 User-Agent，如下：
+
+```sh
+$ mkdir middlewares
+$ vi middlewares/robot.py
+```
+
+修改 `middlewares/robot.py`, 内容如下:
+
+```python
+# /middlewares/robot.py
+from cloudoll.web import middleware, render
+import re
+
+@middleware()
+def mid_robot():
+    async def robot(request, handler):
+        ua = request.headers.get('user-agent')
+        if re.match('Baiduspider', ua):
+            return render(status=403, text="Go away , robot.")
+        return await handler(request)
+
+    return robot
+```
+
+重新启动之后, 现在可以使用 `curl http://localhost:7001/news -A "Baiduspider"` 看看效果。
+
+更多参见中间件文档。
+
+### 配置文件
+写业务的时候，不可避免的需要有配置文件，使用代码管理配置，在代码中添加多个环境的配置，在启动时传入当前环境的参数即可.
+
+cloudoll 支持根据环境来加载配置，定义多个环境的配置文件
+
+```ini
+config
+|- conf.local.yaml
+|- conf.prod.yaml
+`- conf.test.yaml
+```
+
+我们创建配置文件：
+
+```sh
+$ mkdir -p config/conf.local.yaml
+$ vi config/conf.local.yaml
+```
+
+如下是 mysql 和 server 的配置：
+
+```yaml
+server:
+  host: 192.168.0.1
+  port: 9001
+  static: false
+  client_max_size: 1024000
+  static: 
+    prefix: /static
+    show_index: true
+    append_version: true
+    follow_symlinks: true
+mysql:
+  host: 127.0.0.1
+  port: 3306
+  user: root
+  password: abcd
+  db: blog
+  charset: utf8mb4
+```
+
+默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
+
+
+# 开发模式
+
+```sh
+adev runserver app.py
 ```
```

### Comparing `cloudoll-2.0.3/cloudoll/error/errors.py` & `cloudoll-2.0.4/cloudoll/error/errors.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-ERROR = {
-    CUSTOM: {code: -1, message: "%s"},
-    HSF_ERROR: {code: -6, message: "HSF 调用失败：%s。"},
-    SYSTEM_ERROR: {code: -10, message: "系统错误。"},
-    BAD_REQUEST: {code: -400, message: "错误的 http 请求。"},
-    NOT_FOUND: {code: -404, message: "您请求的 http 资源没有找到。"},
-    INTERNAL_SERVER_ERROR: {code: -500, message: "内部服务器错误。"},
-    DB: {code: -700, message: "%s"},
-    DATA_OCCUPIED: {code: -701, message: "数据被占用。"},
-    WHAT_REQUIRE: {code: -1001, message: "缺少参数 %s。"},
-    WHAT_WRONG_RANGE: {code: -1002, message: "%s 的取值范围错误。最小 %s，最大 %s"},
-    WHAT_WRONG_FORMAT: {code: -1003, message: "%s 格式不正确。"},
-    WHAT_NOT_SAME: {code: -1004, message: "输入的 %s 值不一致。"},
-    WHAT_NOT_EXISTS: {code: -1005, message: "%s 不存在。"},
-    WHAT_TOO_MUCH: {code: -1006, message: "%s 太多了。"},
-    WHAT_TOO_LITTLE: {code: -1007, message: "%s 太少了。"},
-    WHAT_NOT_BELONGS_TO_YOU: {code: -1008, message: "%s 不属于你。"},
-    WHAT_TOO_LONG: {code: -1009, message: "%s 太长了，请不要超过 %s。"},
-    WHAT_TOO_SHORT: {code: -1010, message: "%s 太短了，请不要少于 %s。"},
-    WHAT_EXISTED: {code: -1011, message: "%s 已经存在。"},
-    WHAT_OCCUPIED: {code: -1012, message: "%s 被占用。"},
-    WHAT_TIMEOUT: {code: -1013, message: "%s 已超时。"},
-    WHAT_EXPIRED: {code: -1014, message: "%s 已过期。"},
-    WHAT_ILLEGAL: {code: -1015, message: "%s 不合法。"},
-    WHAT_NOT_FOUND: {code: -1016, message: "%s 没找到。"},
-    WHAT_WRONG_LENGTH_RANGE: {code: -1017, message: "%s 的长度错误，最短是 %s，最长 %s。"},
-    WHAT_WRONG_TYPE: {code: -1018, message: "%s 的类型错误"},
-    ACCESS_TOKEN_NOT_FOUND: {code: -2001, message: "access_token 不存在。"},
-    ACCESS_TOKEN_EXPIRED: {code: -2002, message: "access_token 已经过期。"},
-    TICKET_EXPIRED: {code: -2050, message: "票据已经过期，请重新获取。"},
-    TICKET_VERIFY_FAILED: {code: -2051, message: "票据校验失败。篡改登录信息是违法行为！"},
-    TICKET_ILLEGAL: {code: -2052, message: "非法票据。篡改登录信息是违法行为！"},
-    SIGN_VERIFY_FAILED: {code: -2053, message: "签名验证失败。"},
-    PASSWORD_NOT_STRONG: {code: -3001, message: "密码太简单。%s"},
-    CHINA_MOBILE_ILLEGAL: {code: -3002, message: "不正确的手机号码。"},
-    EMAIL_ILLEGAL: {code: -3003, message: "不正确的Email。"},
-    CAPTCHA_VALIDATE_FAIL: {code: -3004, message: "验证码校验失败。"},
-    PASSPORT_ILLEGAL: {code: -3005, message: "不正确的登录凭据，必须是手机或者 Email。"},
-    MEMBER_ONLY: {code: -3006, message: "您还没有登录，请登录。"},
-    NO_RIGHTS: {code: -3007, message: "您没有权限，请联系管理员授权。"},
-    LOGIN_ERROR: {code: -3050, message: "登录失败"},
-    LOGIN_ERROR_BECAUSE: {code: -3051, message: "登录失败。%s"},
-    MEMBER_NOT_EXISTS: {code: -3052, message: "用户不存在。"},
-    MEMBER_NOT_APPROVED: {code: -3053, message: "尚未审批通过，请耐心等待。"},
-    MEMBER_FORBIDDEN: {code: -3054, message: "您已经被系统禁止。"},
-    MEMBER_LOGIN_TOO_MUCH_FAILURE: {code: -3055, message: "您登录失败的次数太多。暂时被系统锁定"},
-    IP_LOGIN_TOO_MUCH: {code: -3056, message: "您登录失败的次数太多。暴力破解他人密码是违法行为！"},
-}
+ERROR = {
+    CUSTOM: {code: -1, message: "%s"},
+    HSF_ERROR: {code: -6, message: "HSF 调用失败：%s。"},
+    SYSTEM_ERROR: {code: -10, message: "系统错误。"},
+    BAD_REQUEST: {code: -400, message: "错误的 http 请求。"},
+    NOT_FOUND: {code: -404, message: "您请求的 http 资源没有找到。"},
+    INTERNAL_SERVER_ERROR: {code: -500, message: "内部服务器错误。"},
+    DB: {code: -700, message: "%s"},
+    DATA_OCCUPIED: {code: -701, message: "数据被占用。"},
+    WHAT_REQUIRE: {code: -1001, message: "缺少参数 %s。"},
+    WHAT_WRONG_RANGE: {code: -1002, message: "%s 的取值范围错误。最小 %s，最大 %s"},
+    WHAT_WRONG_FORMAT: {code: -1003, message: "%s 格式不正确。"},
+    WHAT_NOT_SAME: {code: -1004, message: "输入的 %s 值不一致。"},
+    WHAT_NOT_EXISTS: {code: -1005, message: "%s 不存在。"},
+    WHAT_TOO_MUCH: {code: -1006, message: "%s 太多了。"},
+    WHAT_TOO_LITTLE: {code: -1007, message: "%s 太少了。"},
+    WHAT_NOT_BELONGS_TO_YOU: {code: -1008, message: "%s 不属于你。"},
+    WHAT_TOO_LONG: {code: -1009, message: "%s 太长了，请不要超过 %s。"},
+    WHAT_TOO_SHORT: {code: -1010, message: "%s 太短了，请不要少于 %s。"},
+    WHAT_EXISTED: {code: -1011, message: "%s 已经存在。"},
+    WHAT_OCCUPIED: {code: -1012, message: "%s 被占用。"},
+    WHAT_TIMEOUT: {code: -1013, message: "%s 已超时。"},
+    WHAT_EXPIRED: {code: -1014, message: "%s 已过期。"},
+    WHAT_ILLEGAL: {code: -1015, message: "%s 不合法。"},
+    WHAT_NOT_FOUND: {code: -1016, message: "%s 没找到。"},
+    WHAT_WRONG_LENGTH_RANGE: {code: -1017, message: "%s 的长度错误，最短是 %s，最长 %s。"},
+    WHAT_WRONG_TYPE: {code: -1018, message: "%s 的类型错误"},
+    ACCESS_TOKEN_NOT_FOUND: {code: -2001, message: "access_token 不存在。"},
+    ACCESS_TOKEN_EXPIRED: {code: -2002, message: "access_token 已经过期。"},
+    TICKET_EXPIRED: {code: -2050, message: "票据已经过期，请重新获取。"},
+    TICKET_VERIFY_FAILED: {code: -2051, message: "票据校验失败。篡改登录信息是违法行为！"},
+    TICKET_ILLEGAL: {code: -2052, message: "非法票据。篡改登录信息是违法行为！"},
+    SIGN_VERIFY_FAILED: {code: -2053, message: "签名验证失败。"},
+    PASSWORD_NOT_STRONG: {code: -3001, message: "密码太简单。%s"},
+    CHINA_MOBILE_ILLEGAL: {code: -3002, message: "不正确的手机号码。"},
+    EMAIL_ILLEGAL: {code: -3003, message: "不正确的Email。"},
+    CAPTCHA_VALIDATE_FAIL: {code: -3004, message: "验证码校验失败。"},
+    PASSPORT_ILLEGAL: {code: -3005, message: "不正确的登录凭据，必须是手机或者 Email。"},
+    MEMBER_ONLY: {code: -3006, message: "您还没有登录，请登录。"},
+    NO_RIGHTS: {code: -3007, message: "您没有权限，请联系管理员授权。"},
+    LOGIN_ERROR: {code: -3050, message: "登录失败"},
+    LOGIN_ERROR_BECAUSE: {code: -3051, message: "登录失败。%s"},
+    MEMBER_NOT_EXISTS: {code: -3052, message: "用户不存在。"},
+    MEMBER_NOT_APPROVED: {code: -3053, message: "尚未审批通过，请耐心等待。"},
+    MEMBER_FORBIDDEN: {code: -3054, message: "您已经被系统禁止。"},
+    MEMBER_LOGIN_TOO_MUCH_FAILURE: {code: -3055, message: "您登录失败的次数太多。暂时被系统锁定"},
+    IP_LOGIN_TOO_MUCH: {code: -3056, message: "您登录失败的次数太多。暴力破解他人密码是违法行为！"},
+}
```

### Comparing `cloudoll-2.0.3/cloudoll/robot/dingtalk.py` & `cloudoll-2.0.4/cloudoll/robot/dingtalk.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-# docs: https://open.dingtalk.com/document/group/message-types-and-data-format
-__author__ = "chuchur/chuchur.com"
-
-import base64
-import hashlib
-import hmac
-import logging
-import requests as http
-import time
-from urllib import parse
-
-
-class Client(object):
-    def __init__(self, **kw):
-        self._webhook = kw.get("webhook")
-        self._secret = kw.get("secret")
-        self._access_token = kw.get("access_token")
-
-    def _get_sign(self):
-        secret = self._secret
-        if not secret:
-            logging.error("缺少secret")
-            return None, None
-
-        # 拼接timestamp和secret
-        timestamp = str(round(time.time() * 1000))
-        string_to_sign = "{}\n{}".format(timestamp, secret)
-        hmac_code = hmac.new(
-            secret.encode("utf-8"),
-            string_to_sign.encode("utf-8"),
-            digestmod=hashlib.sha256,
-        ).digest()
-
-        # 对结果进行base64处理
-        sign = base64.b64encode(hmac_code).decode("utf-8")
-        sign = parse.quote(sign)
-        return timestamp, sign
-
-    def upload(self, type: str, filepath: str):
-        """
-        上传媒体
-        :params access_token
-        :params type 文件类型 image|voice|video|file
-        :params filepath 要上传的文件路径
-        """
-        access_token = self._access_token
-        if not access_token:
-            logging.error("请配置access_token")
-            return False
-        url = "https://oapi.dingtalk.com/media/upload?access_token=%s" % access_token
-        with open(filepath, "rb") as f:
-            files = {"media": f}
-            result = http.post(url=url, files=files, data={"type": type})
-            res = result.json()
-            if res["errcode"] == 0:
-                return res
-            else:
-                logging.error(res["errmsg"])
-
-    def send(self, data: dict):
-        """
-        发送除签名外的自定义消息结构体 https://open.dingtalk.com/document/orgapp-server/message-types-and-data-format
-        :params data 自定义消息结构体
-        """
-        webhook = self._webhook
-        if not webhook:
-            logging.error("缺少webhook")
-            return False
-        timestamp, sign = self._get_sign()
-        if not timestamp or not sign:
-            return False
-        url = webhook + "&timestamp=%s&sign=%s" % (timestamp, sign)
-        result = http.post(
-            url=url,
-            json={**data},
-            # data=data
-            # data=json.dumps(data)
-        )
-        if result:
-            res = result.json()
-            if res["errcode"] == 0:
-                logging.info("发送成功！")
-                return True
-            else:
-                logging.info("发送失败")
-                logging.error(res["errmsg"])
-                return False
-
-    def send_text(self, text: str):
-        """
-        发送文本消息
-        :params text 消息内容
-        """
-
-        return self.send(
-            data={
-                "msgtype": "text",
-                "text": {"content": text},
-            }
-        )
-
-    def _send_media(self, type, media_id, **kw):
-        """
-        发送媒体
-        :params type 媒体类型 image|voice|video|file
-        :params media_id 媒体ID
-        """
-        data = {"msgtype": type}
-        data[type] = {"media_id": media_id}
-        if type == "voice":
-            data["voice"]["duration"] = kw.get("duration")
-        return self.send(data)
-
-    def send_markdown(self, title, text):
-        """
-        发送Markdown消息
-        :params title 标题
-        :params text markdown结构体
-        """
-        return self.send(
-            data={"msgtype": "markdown", "markdown": {"title": title, "text": text}}
-        )
-
-    def send_image(self, media_id: str):
-        """
-        发送图片消息
-        :params media_id 媒体ID
-        """
-        return self._send_media("image", media_id)
-
-    def send_voice(self, media_id: str, duration: str):
-        """
-        发送语音消息
-        :params media_id 媒体ID
-        :params duration 正整数，小于60，表示音频时长。
-        """
-        return self._send_media("voice", media_id, duration=duration)
-
-    def send_file(self, media_id: str):
-        """
-        发送文件消息
-        :params media_id 媒体ID
-        """
-        return self._send_media("file", media_id)
-
-    def send_link(self, messageUrl, picUrl, title, text):
-        """
-        发送链接消息
-        :params messageUrl 链接地址
-        :params picUrl 链接的小图
-        :params title 链接标题 100字内
-        :params text 链接副标题 500字内
-        """
-        return self.send(
-            data={
-                "msgtype": "link",
-                "link": {
-                    "picUrl": picUrl,
-                    "messageUrl": messageUrl,
-                    "title": title,
-                    "text": text,
-                },
-            }
-        )
-
-    def send_card(self, **kw):
-        """
-        发送卡片消息
-        :params title 标题
-        :params text 消息内容 必填
-        :params single_title 查看详情(按钮文字) btns 二选一
-        :params single_url 查看详情(链接) btns 二选一
-        :params btn_orientation 按钮排列顺序。0|1
-        :params btns 按钮 [{title:'',actionURL:''}]
-        """
-        title = kw.get("title", "")
-        text = kw.get("text", "")
-        single_title = kw.get("single_title", "")
-        single_url = kw.get("single_url", "")
-        btn_orientation = kw.get("btn_orientation", 0)
-        btns = kw.get("btns", []) or []
-        return self.send(
-            data={
-                "msgtype": "actionCard",
-                "actionCard": {
-                    "title": title,
-                    "text": text,
-                    "singleTitle": single_title,
-                    "singleUrl": single_url,
-                    "btnOrientation": btn_orientation,
-                    "btns": btns,
-                },
-            }
-        )
-
-    def send_freecard(self, links: list):
-        """
-        发送卡片消息
-        :params links [{ title:'',messageURL:'',picURL:''}]
-        """
-        return self.send(
-            data={
-                "msgtype": "feedCard",
-                "feedCard": {"links": links},
-            }
-        )
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+# docs: https://open.dingtalk.com/document/group/message-types-and-data-format
+__author__ = "chuchur/chuchur.com"
+
+import base64
+import hashlib
+import hmac
+import logging
+import requests as http
+import time
+from urllib import parse
+
+
+class Client(object):
+    def __init__(self, **kw):
+        self._webhook = kw.get("webhook")
+        self._secret = kw.get("secret")
+        self._access_token = kw.get("access_token")
+
+    def _get_sign(self):
+        secret = self._secret
+        if not secret:
+            logging.error("缺少secret")
+            return None, None
+
+        # 拼接timestamp和secret
+        timestamp = str(round(time.time() * 1000))
+        string_to_sign = "{}\n{}".format(timestamp, secret)
+        hmac_code = hmac.new(
+            secret.encode("utf-8"),
+            string_to_sign.encode("utf-8"),
+            digestmod=hashlib.sha256,
+        ).digest()
+
+        # 对结果进行base64处理
+        sign = base64.b64encode(hmac_code).decode("utf-8")
+        sign = parse.quote(sign)
+        return timestamp, sign
+
+    def upload(self, type: str, filepath: str):
+        """
+        上传媒体
+        :params access_token
+        :params type 文件类型 image|voice|video|file
+        :params filepath 要上传的文件路径
+        """
+        access_token = self._access_token
+        if not access_token:
+            logging.error("请配置access_token")
+            return False
+        url = "https://oapi.dingtalk.com/media/upload?access_token=%s" % access_token
+        with open(filepath, "rb") as f:
+            files = {"media": f}
+            result = http.post(url=url, files=files, data={"type": type})
+            res = result.json()
+            if res["errcode"] == 0:
+                return res
+            else:
+                logging.error(res["errmsg"])
+
+    def send(self, data: dict):
+        """
+        发送除签名外的自定义消息结构体 https://open.dingtalk.com/document/orgapp-server/message-types-and-data-format
+        :params data 自定义消息结构体
+        """
+        webhook = self._webhook
+        if not webhook:
+            logging.error("缺少webhook")
+            return False
+        timestamp, sign = self._get_sign()
+        if not timestamp or not sign:
+            return False
+        url = webhook + "&timestamp=%s&sign=%s" % (timestamp, sign)
+        result = http.post(
+            url=url,
+            json={**data},
+            # data=data
+            # data=json.dumps(data)
+        )
+        if result:
+            res = result.json()
+            if res["errcode"] == 0:
+                logging.info("发送成功！")
+                return True
+            else:
+                logging.info("发送失败")
+                logging.error(res["errmsg"])
+                return False
+
+    def send_text(self, text: str):
+        """
+        发送文本消息
+        :params text 消息内容
+        """
+
+        return self.send(
+            data={
+                "msgtype": "text",
+                "text": {"content": text},
+            }
+        )
+
+    def _send_media(self, type, media_id, **kw):
+        """
+        发送媒体
+        :params type 媒体类型 image|voice|video|file
+        :params media_id 媒体ID
+        """
+        data = {"msgtype": type}
+        data[type] = {"media_id": media_id}
+        if type == "voice":
+            data["voice"]["duration"] = kw.get("duration")
+        return self.send(data)
+
+    def send_markdown(self, title, text):
+        """
+        发送Markdown消息
+        :params title 标题
+        :params text markdown结构体
+        """
+        return self.send(
+            data={"msgtype": "markdown", "markdown": {"title": title, "text": text}}
+        )
+
+    def send_image(self, media_id: str):
+        """
+        发送图片消息
+        :params media_id 媒体ID
+        """
+        return self._send_media("image", media_id)
+
+    def send_voice(self, media_id: str, duration: str):
+        """
+        发送语音消息
+        :params media_id 媒体ID
+        :params duration 正整数，小于60，表示音频时长。
+        """
+        return self._send_media("voice", media_id, duration=duration)
+
+    def send_file(self, media_id: str):
+        """
+        发送文件消息
+        :params media_id 媒体ID
+        """
+        return self._send_media("file", media_id)
+
+    def send_link(self, messageUrl, picUrl, title, text):
+        """
+        发送链接消息
+        :params messageUrl 链接地址
+        :params picUrl 链接的小图
+        :params title 链接标题 100字内
+        :params text 链接副标题 500字内
+        """
+        return self.send(
+            data={
+                "msgtype": "link",
+                "link": {
+                    "picUrl": picUrl,
+                    "messageUrl": messageUrl,
+                    "title": title,
+                    "text": text,
+                },
+            }
+        )
+
+    def send_card(self, **kw):
+        """
+        发送卡片消息
+        :params title 标题
+        :params text 消息内容 必填
+        :params single_title 查看详情(按钮文字) btns 二选一
+        :params single_url 查看详情(链接) btns 二选一
+        :params btn_orientation 按钮排列顺序。0|1
+        :params btns 按钮 [{title:'',actionURL:''}]
+        """
+        title = kw.get("title", "")
+        text = kw.get("text", "")
+        single_title = kw.get("single_title", "")
+        single_url = kw.get("single_url", "")
+        btn_orientation = kw.get("btn_orientation", 0)
+        btns = kw.get("btns", []) or []
+        return self.send(
+            data={
+                "msgtype": "actionCard",
+                "actionCard": {
+                    "title": title,
+                    "text": text,
+                    "singleTitle": single_title,
+                    "singleUrl": single_url,
+                    "btnOrientation": btn_orientation,
+                    "btns": btns,
+                },
+            }
+        )
+
+    def send_freecard(self, links: list):
+        """
+        发送卡片消息
+        :params links [{ title:'',messageURL:'',picURL:''}]
+        """
+        return self.send(
+            data={
+                "msgtype": "feedCard",
+                "feedCard": {"links": links},
+            }
+        )
```

### Comparing `cloudoll-2.0.3/cloudoll/web/__init__.py` & `cloudoll-2.0.4/cloudoll/web/__init__.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,470 +1,470 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-__author__ = "chuchur/chuchur.com"
-
-import argparse
-import asyncio
-import hashlib
-import os, base64, datetime
-import importlib
-import inspect
-import json
-import pkgutil
-import sys
-import socket
-from urllib import parse
-import aiomcache
-import aioredis
-from aiohttp import web
-from aiohttp.web_exceptions import *
-from aiohttp.web_ws import WebSocketResponse as WebSocket, WSMsgType
-from aiohttp_session import (
-    get_session,
-    setup,
-    redis_storage,
-    memcached_storage,
-    cookie_storage,
-)
-from jinja2 import Environment, FileSystemLoader
-from setuptools import find_packages
-from .settings import get_config
-
-from ..logging import logging
-from ..orm.mysql import sa
-from . import jwt
-
-
-class _Handler(object):
-    def __init__(self, cls, fn):
-        self.cls = cls
-        self.fn = fn
-
-    async def __call__(self, request):
-        c_type = request.content_type
-        # 获取函数参数的名称和默认值
-        props = inspect.getfullargspec(self.fn)
-        if len(props.args) == 2 and c_type == "multipart/form-data":
-            await _set_session_route(request)
-            multipart = await request.multipart()
-            field = await multipart.next()
-            return await self.fn(request, field)
-        elif len(props.args) == 1:
-            await _set_session_route(request)
-            if c_type == "multipart/form-data":
-                data = await request.post()
-            elif c_type == "application/json":
-                data = await request.json()
-            else:
-                data = await request.post()
-            q_s = request.query_string
-            body = {}
-            for k in data:
-                body[k] = data[k]
-            qs = {}
-            if q_s:
-                for k, v in parse.parse_qs(q_s, True).items():
-                    qs[k] = v[0]
-            request.qs = Object(qs)
-            request.body = Object(body)
-            return await self.fn(request)
-        else:
-            return await self.fn()
-
-
-async def _set_session_route(request):
-    params = dict()
-    # match
-    rt = request.match_info
-    for k, v in rt.items():
-        params[k] = v
-    request.params = Object(params)
-    session = await get_session(request)
-    # session = await new_session(request)
-    request.session = session
-
-
-def _get_modules(fd):
-    modules = set()
-    temp = os.path.join(os.path.abspath("."), fd)
-    if not os.path.exists(temp):
-        return
-    s = find_packages(temp)
-    for pkg in s:
-        # modules.add(pkg)
-        pkg_path = temp + "/" + pkg.replace(".", "/")
-        if sys.version_info.major == 2 or (
-            sys.version_info.major == 3 and sys.version_info.minor < 6
-        ):
-            for _, name, ispkg in pkgutil.iter_modules([pkg_path]):
-                if not ispkg:
-                    modules.add(f".{pkg}.{name}")
-        else:
-            for info in pkgutil.iter_modules([pkg_path]):
-                if not info.ispkg:
-                    modules.add(f".{pkg}.{info.name}")
-    return modules
-
-
-def _check_address(host, port):
-    sk = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    try:
-        r = sk.connect_ex((host, int(port)))
-    except OSError as err:
-        raise err.strerror
-    finally:
-        sk.close()
-    if r == 0:
-        raise OSError(f"Address {host}:{port} already in use.")
-
-
-def _reg_middleware():
-    fd = "middlewares"
-    temp = os.path.join(os.path.abspath("."), fd)
-    if not os.path.exists(temp):
-        return
-    for f in os.listdir(temp):
-        if not f.startswith("__"):
-            module_name = f"{fd}.{os.path.basename(f)[:-3]}"
-            importlib.import_module(module_name, fd)
-
-
-def _int(num):
-    return eval(num) if isinstance(num, str) else num
-
-
-class Application(object):
-    def __init__(self):
-        self._loop = None
-        self.mysql = None
-        self.env = None
-        self.app = None
-        self._route_table = web.RouteTableDef()
-        self._middleware = []
-        self.config = {}
-        self._args = None
-
-    def create(self):
-        loop = asyncio.get_event_loop()
-        if loop is None:
-            loop = asyncio.new_event_loop()
-        self._loop = loop
-
-        parser = argparse.ArgumentParser(description="cloudoll app.")
-        parser.add_argument("--env", default="local")
-        parser.add_argument("--host", default=None)
-        parser.add_argument("--port", default=None)
-        parser.add_argument("--path", default=None)
-        args, extra_argv = parser.parse_known_args()
-        config = get_config(args.env)
-
-        self._args = args
-        self.config = config
-
-        # middlewares
-        _reg_middleware()
-
-        conf_server = config.get("server")
-        client_max_size = 1024**2 * 2
-        if conf_server is not None:
-            client_max_size = conf_server.get("client_max_size", client_max_size)
-        self.app = web.Application(
-            logger=None,
-            loop=loop,
-            middlewares=self._middleware,
-            client_max_size=_int(client_max_size),
-        )
-        # database
-        self.app.on_startup.append(self._init_database)
-        self.app.on_cleanup.append(self._close_database)
-        self.app.config = config
-        self.app.jwt_encode = self.jwt_encode
-        self.app.jwt_decode = self.jwt_decode
-        # session
-        self._init_session()
-        #  router:
-        self._reg_router()
-
-        # static
-        if conf_server is not None:
-            conf_st = conf_server.get("static")
-            if conf_st:
-                temp = os.path.join(os.path.abspath("."), "static")
-                self.app.router.add_static(**conf_st, path=temp)
-                logging.warning("Suggest using nginx or others instead.")
-
-        temp = os.path.join(os.path.abspath("."), "templates")
-        if os.path.exists(temp):
-            self.env = Environment(loader=FileSystemLoader(temp), autoescape=True)
-
-        return self
-
-    async def _close_database(self, apps):
-        if self.mysql:
-            await self.mysql.close()
-
-    async def _init_database(self, apps):
-        conf_mysql = self.config.get("mysql")
-        if conf_mysql is not None:
-            self.mysql = await sa.create_engine(**conf_mysql)
-            self.app.mysql = self.mysql
-            apps.mysql = self.mysql
-
-    def _init_session(self):
-        config = self.config
-        # redis
-        redis_conf = config.get("redis")
-        mcache_conf = config.get("memcached")
-        _SESSION_KEY = "CLOUDOLL_SESSION"
-
-        if redis_conf:
-            redis_url = redis_conf.get("url")
-            if not redis_url:
-                protocol = redis_conf.get("protocol", "redis:")
-                host = redis_conf.get("host")
-                port = redis_conf.get("port", 6379)
-                username = redis_conf.get("username")
-                password = redis_conf.get("password")
-                db = redis_conf.get("db", 0)
-                path = redis_conf.get("path")
-                if not path:
-                    path = f"{host}:{port}/{db}"
-                else:
-                    path = f"{path}?db={db}"
-                if password and username:
-                    path = f"{username}:{password}@{path}"
-                redis_url = f"{protocol}//{path}"
-
-            max_age = redis_conf.get("max_age")
-            secure = redis_conf.get("secure")
-            httponly = redis_conf.get("httponly")
-            cookie_name = redis_conf.get("key", _SESSION_KEY)
-
-            redis = aioredis.from_url(redis_url)
-            self.app.redis = redis
-            storage = redis_storage.RedisStorage(
-                redis,
-                cookie_name=cookie_name,
-                max_age=_int(max_age),
-                httponly=httponly,
-                secure=secure,
-            )
-            setup(self.app, storage)
-        elif mcache_conf:
-            host = mcache_conf.get("host")
-            port = mcache_conf.get("port", 11211)
-            max_age = mcache_conf.get("max_age")
-            secure = mcache_conf.get("secure")
-            httponly = mcache_conf.get("httponly")
-            cookie_name = mcache_conf.get("key", _SESSION_KEY)
-            mc = aiomcache.Client(host, port)
-            self.app.memcached = mc
-            storage = memcached_storage.MemcachedStorage(
-                mc,
-                cookie_name=cookie_name,
-                max_age=_int(max_age),
-                httponly=httponly,
-                secure=secure,
-            )
-            setup(self.app, storage)
-        else:
-            sess = config.get("session", {})
-            sess_name = sess.get("key", _SESSION_KEY)
-
-            dig = hashlib.sha256(sess_name.encode()).digest()
-            fernet_key = base64.urlsafe_b64encode(dig)
-            secret_key = base64.urlsafe_b64decode(fernet_key)
-
-            # fernet_key = fernet.Fernet.generate_key()
-            # secret_key = base64.urlsafe_b64decode(fernet_key)
-
-            max_age = sess.get("max_age")
-            httponly = sess.get("httponly")
-            storage = cookie_storage.EncryptedCookieStorage(
-                secret_key,
-                cookie_name=sess_name,
-                max_age=_int(max_age),
-                httponly=httponly,
-            )
-            setup(self.app, storage)
-
-    def _reg_router(self):
-        fd = "controllers"
-        modules = _get_modules(fd)
-        for module in modules:
-            # print(module, router)
-            importlib.import_module(module, fd)
-
-        self.app.add_routes(self._route_table)
-        # for route in self._routes:
-        #     self.app.router.add_route(**route)
-
-    def run(self, *args, **kw):
-        """
-        run app
-        :params prot default  9001
-        :params host default 127.0.0.1
-        """
-        conf = self.config.get("server", {})
-        # if conf.get('reload',False) is True:
-        # import aioreloader
-        # aioreloader.start()
-        conf.update(args)
-        args = {k: v for k, v in vars(self._args).items() if v is not None}
-        conf.update(args)
-        host = conf.get("host", "127.0.0.1")
-        port = conf.get("port", 9001)
-        path = conf.get("path")
-        _check_address(host, port)
-        # logging.info(f"Server run at http://{host}:{port}")
-        web.run_app(
-            self.app,
-            loop=self._loop,
-            host=host,
-            port=port,
-            path=path,
-            access_log=None,
-            **kw,
-        )
-        # # old
-        # if self.loop is None:
-        #     return web.run_app(self.app, host=host, port=port, **kw)
-        # else:
-        #     logging.info(f"Server run at http://{host}:{port}")
-        #     return self.loop.create_server(
-        #         self.app.make_handler(), host=host, port=port, **kw
-        #     )
-
-    def add_router(self, path, method, name):
-        def inner(handler):
-            handler = _Handler(self, handler)
-            self.app.router.add_route(method, path, handler, name=name)
-            return handler
-
-        return inner
-
-    def add_middleware(self):
-        def wrapper(func):
-            mid = func()
-            mid.__middleware_version__ = 1
-            self._middleware.append(mid)
-
-        return wrapper
-
-    def jwt_encode(self, payload):
-        jwt_conf = self.config.get("jwt", {})
-        key = jwt_conf.get("key")
-        exp = jwt_conf.get("exp")
-        if not key or not exp:
-            raise KeyError("Please set jwt key or exp...")
-        return jwt.encode(payload, key, exp)
-
-    def jwt_decode(self, token):
-        jwt_conf = self.config.get("jwt", {})
-        key = jwt_conf.get("key")
-        return jwt.decode(token, key)
-
-    @property
-    def route_table(self):
-        return self._route_table
-
-    @property
-    def on_startup(self):
-        return self.app.on_startup
-
-    @property
-    def on_shutdown(self):
-        return self.app.on_shutdown
-
-    @property
-    def on_cleanup(self):
-        return self.app.on_cleanup
-
-    @property
-    def cleanup_ctx(self):
-        return self.app.cleanup_ctx
-
-
-app = Application()
-
-
-class Object(dict):
-    def __init__(self, obj: dict):
-        super().__init__()
-        for k, v in obj.items():
-            self[k] = v
-
-    def __getattr__(self, key):
-        return self[key] if key in self else ""
-
-    def __setattr__(self, key, value):
-        self[key] = value
-
-    def __str__(self):
-        return self.key
-
-
-class JsonEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, datetime.datetime) or isinstance(obj, datetime.date):
-            return obj.__str__()
-        else:
-            return super(JsonEncoder, self).default(obj)
-
-
-def get(path, name=None):
-    return app.add_router(path, "GET", name)
-
-
-def post(path, name=None):
-    return app.add_router(path, "POST", name)
-
-
-def put(path, name=None):
-    return app.add_router(path, "PUT", name)
-
-
-def delete(path, name=None):
-    return app.add_router(path, "DELETE", name)
-
-
-def all(path):
-    #     return app._actions(path, 'GET')
-    return app.route_table.view(path)
-
-
-def jsons(data, **kw):
-    res = {}
-    if isinstance(data, list):
-        res["data"] = data
-    elif isinstance(data, dict):
-        res.update(data)
-    elif isinstance(data, tuple):
-        data = dict(data)
-        res.update(data)
-    else:
-        raise ValueError("data must be list , dict or tuple.")
-    res["timestamp"] = int(datetime.datetime.now().timestamp() * 1000)
-    text = json.dumps(res, ensure_ascii=False, cls=JsonEncoder)
-    return web.json_response(text=text, **kw)
-
-
-def middleware():
-    return app.add_middleware()
-
-
-def render(**kw):
-    return web.Response(**kw)
-
-
-def view(template=None, *args, **kw):
-    body = None
-    if app.env is not None:
-        body = app.env.get_template(template).render(*args)
-    _view = render(body=body, **kw)
-    _view.content_type = "text/html;charset=utf-8"
-    return _view
-
-
-def redirect(urlpath):
-    return web.HTTPFound(location=urlpath)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "chuchur/chuchur.com"
+
+import argparse
+import asyncio
+import hashlib
+import os, base64, datetime
+import importlib
+import inspect
+import json
+import pkgutil
+import sys
+import socket
+from urllib import parse
+import aiomcache
+import aioredis
+from aiohttp import web
+from aiohttp.web_exceptions import *
+from aiohttp.web_ws import WebSocketResponse as WebSocket, WSMsgType
+from aiohttp_session import (
+    get_session,
+    setup,
+    redis_storage,
+    memcached_storage,
+    cookie_storage,
+)
+from jinja2 import Environment, FileSystemLoader
+from setuptools import find_packages
+from .settings import get_config
+
+from ..logging import logging
+from ..orm.mysql import sa
+from . import jwt
+
+
+class _Handler(object):
+    def __init__(self, cls, fn):
+        self.cls = cls
+        self.fn = fn
+
+    async def __call__(self, request):
+        c_type = request.content_type
+        # 获取函数参数的名称和默认值
+        props = inspect.getfullargspec(self.fn)
+        if len(props.args) == 2 and c_type == "multipart/form-data":
+            await _set_session_route(request)
+            multipart = await request.multipart()
+            field = await multipart.next()
+            return await self.fn(request, field)
+        elif len(props.args) == 1:
+            await _set_session_route(request)
+            if c_type == "multipart/form-data":
+                data = await request.post()
+            elif c_type == "application/json":
+                data = await request.json()
+            else:
+                data = await request.post()
+            q_s = request.query_string
+            body = {}
+            for k in data:
+                body[k] = data[k]
+            qs = {}
+            if q_s:
+                for k, v in parse.parse_qs(q_s, True).items():
+                    qs[k] = v[0]
+            request.qs = Object(qs)
+            request.body = Object(body)
+            return await self.fn(request)
+        else:
+            return await self.fn()
+
+
+async def _set_session_route(request):
+    params = dict()
+    # match
+    rt = request.match_info
+    for k, v in rt.items():
+        params[k] = v
+    request.params = Object(params)
+    session = await get_session(request)
+    # session = await new_session(request)
+    request.session = session
+
+
+def _get_modules(fd):
+    modules = set()
+    temp = os.path.join(os.path.abspath("."), fd)
+    if not os.path.exists(temp):
+        return
+    s = find_packages(temp)
+    for pkg in s:
+        # modules.add(pkg)
+        pkg_path = temp + "/" + pkg.replace(".", "/")
+        if sys.version_info.major == 2 or (
+            sys.version_info.major == 3 and sys.version_info.minor < 6
+        ):
+            for _, name, ispkg in pkgutil.iter_modules([pkg_path]):
+                if not ispkg:
+                    modules.add(f".{pkg}.{name}")
+        else:
+            for info in pkgutil.iter_modules([pkg_path]):
+                if not info.ispkg:
+                    modules.add(f".{pkg}.{info.name}")
+    return modules
+
+
+def _check_address(host, port):
+    sk = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    try:
+        r = sk.connect_ex((host, int(port)))
+    except OSError as err:
+        raise err.strerror
+    finally:
+        sk.close()
+    if r == 0:
+        raise OSError(f"Address {host}:{port} already in use.")
+
+
+def _reg_middleware():
+    fd = "middlewares"
+    temp = os.path.join(os.path.abspath("."), fd)
+    if not os.path.exists(temp):
+        return
+    for f in os.listdir(temp):
+        if not f.startswith("__"):
+            module_name = f"{fd}.{os.path.basename(f)[:-3]}"
+            importlib.import_module(module_name, fd)
+
+
+def _int(num):
+    return eval(num) if isinstance(num, str) else num
+
+
+class Application(object):
+    def __init__(self):
+        self._loop = None
+        self.mysql = None
+        self.env = None
+        self.app = None
+        self._route_table = web.RouteTableDef()
+        self._middleware = []
+        self.config = {}
+        self._args = None
+
+    def create(self):
+        loop = asyncio.get_event_loop()
+        if loop is None:
+            loop = asyncio.new_event_loop()
+        self._loop = loop
+
+        parser = argparse.ArgumentParser(description="cloudoll app.")
+        parser.add_argument("--env", default="local")
+        parser.add_argument("--host", default=None)
+        parser.add_argument("--port", default=None)
+        parser.add_argument("--path", default=None)
+        args, extra_argv = parser.parse_known_args()
+        config = get_config(args.env)
+
+        self._args = args
+        self.config = config
+
+        # middlewares
+        _reg_middleware()
+
+        conf_server = config.get("server")
+        client_max_size = 1024**2 * 2
+        if conf_server is not None:
+            client_max_size = conf_server.get("client_max_size", client_max_size)
+        self.app = web.Application(
+            logger=None,
+            loop=loop,
+            middlewares=self._middleware,
+            client_max_size=_int(client_max_size),
+        )
+        # database
+        self.app.on_startup.append(self._init_database)
+        self.app.on_cleanup.append(self._close_database)
+        self.app.config = config
+        self.app.jwt_encode = self.jwt_encode
+        self.app.jwt_decode = self.jwt_decode
+        # session
+        self._init_session()
+        #  router:
+        self._reg_router()
+
+        # static
+        if conf_server is not None:
+            conf_st = conf_server.get("static")
+            if conf_st:
+                temp = os.path.join(os.path.abspath("."), "static")
+                self.app.router.add_static(**conf_st, path=temp)
+                logging.warning("Suggest using nginx or others instead.")
+
+        temp = os.path.join(os.path.abspath("."), "templates")
+        if os.path.exists(temp):
+            self.env = Environment(loader=FileSystemLoader(temp), autoescape=True)
+
+        return self
+
+    async def _close_database(self, apps):
+        if self.mysql:
+            await self.mysql.close()
+
+    async def _init_database(self, apps):
+        conf_mysql = self.config.get("mysql")
+        if conf_mysql is not None:
+            self.mysql = await sa.create_engine(**conf_mysql)
+            self.app.mysql = self.mysql
+            apps.mysql = self.mysql
+
+    def _init_session(self):
+        config = self.config
+        # redis
+        redis_conf = config.get("redis")
+        mcache_conf = config.get("memcached")
+        _SESSION_KEY = "CLOUDOLL_SESSION"
+
+        if redis_conf:
+            redis_url = redis_conf.get("url")
+            if not redis_url:
+                protocol = redis_conf.get("protocol", "redis:")
+                host = redis_conf.get("host")
+                port = redis_conf.get("port", 6379)
+                username = redis_conf.get("username")
+                password = redis_conf.get("password")
+                db = redis_conf.get("db", 0)
+                path = redis_conf.get("path")
+                if not path:
+                    path = f"{host}:{port}/{db}"
+                else:
+                    path = f"{path}?db={db}"
+                if password and username:
+                    path = f"{username}:{password}@{path}"
+                redis_url = f"{protocol}//{path}"
+
+            max_age = redis_conf.get("max_age")
+            secure = redis_conf.get("secure")
+            httponly = redis_conf.get("httponly")
+            cookie_name = redis_conf.get("key", _SESSION_KEY)
+
+            redis = aioredis.from_url(redis_url)
+            self.app.redis = redis
+            storage = redis_storage.RedisStorage(
+                redis,
+                cookie_name=cookie_name,
+                max_age=_int(max_age),
+                httponly=httponly,
+                secure=secure,
+            )
+            setup(self.app, storage)
+        elif mcache_conf:
+            host = mcache_conf.get("host")
+            port = mcache_conf.get("port", 11211)
+            max_age = mcache_conf.get("max_age")
+            secure = mcache_conf.get("secure")
+            httponly = mcache_conf.get("httponly")
+            cookie_name = mcache_conf.get("key", _SESSION_KEY)
+            mc = aiomcache.Client(host, port)
+            self.app.memcached = mc
+            storage = memcached_storage.MemcachedStorage(
+                mc,
+                cookie_name=cookie_name,
+                max_age=_int(max_age),
+                httponly=httponly,
+                secure=secure,
+            )
+            setup(self.app, storage)
+        else:
+            sess = config.get("session", {})
+            sess_name = sess.get("key", _SESSION_KEY)
+
+            dig = hashlib.sha256(sess_name.encode()).digest()
+            fernet_key = base64.urlsafe_b64encode(dig)
+            secret_key = base64.urlsafe_b64decode(fernet_key)
+
+            # fernet_key = fernet.Fernet.generate_key()
+            # secret_key = base64.urlsafe_b64decode(fernet_key)
+
+            max_age = sess.get("max_age")
+            httponly = sess.get("httponly")
+            storage = cookie_storage.EncryptedCookieStorage(
+                secret_key,
+                cookie_name=sess_name,
+                max_age=_int(max_age),
+                httponly=httponly,
+            )
+            setup(self.app, storage)
+
+    def _reg_router(self):
+        fd = "controllers"
+        modules = _get_modules(fd)
+        for module in modules:
+            # print(module, router)
+            importlib.import_module(module, fd)
+
+        self.app.add_routes(self._route_table)
+        # for route in self._routes:
+        #     self.app.router.add_route(**route)
+
+    def run(self, *args, **kw):
+        """
+        run app
+        :params prot default  9001
+        :params host default 127.0.0.1
+        """
+        conf = self.config.get("server", {})
+        # if conf.get('reload',False) is True:
+        # import aioreloader
+        # aioreloader.start()
+        conf.update(args)
+        args = {k: v for k, v in vars(self._args).items() if v is not None}
+        conf.update(args)
+        host = conf.get("host", "127.0.0.1")
+        port = conf.get("port", 9001)
+        path = conf.get("path")
+        _check_address(host, port)
+        # logging.info(f"Server run at http://{host}:{port}")
+        web.run_app(
+            self.app,
+            loop=self._loop,
+            host=host,
+            port=port,
+            path=path,
+            access_log=None,
+            **kw,
+        )
+        # # old
+        # if self.loop is None:
+        #     return web.run_app(self.app, host=host, port=port, **kw)
+        # else:
+        #     logging.info(f"Server run at http://{host}:{port}")
+        #     return self.loop.create_server(
+        #         self.app.make_handler(), host=host, port=port, **kw
+        #     )
+
+    def add_router(self, path, method, name):
+        def inner(handler):
+            handler = _Handler(self, handler)
+            self.app.router.add_route(method, path, handler, name=name)
+            return handler
+
+        return inner
+
+    def add_middleware(self):
+        def wrapper(func):
+            mid = func()
+            mid.__middleware_version__ = 1
+            self._middleware.append(mid)
+
+        return wrapper
+
+    def jwt_encode(self, payload):
+        jwt_conf = self.config.get("jwt", {})
+        key = jwt_conf.get("key")
+        exp = jwt_conf.get("exp")
+        if not key or not exp:
+            raise KeyError("Please set jwt key or exp...")
+        return jwt.encode(payload, key, exp)
+
+    def jwt_decode(self, token):
+        jwt_conf = self.config.get("jwt", {})
+        key = jwt_conf.get("key")
+        return jwt.decode(token, key)
+
+    @property
+    def route_table(self):
+        return self._route_table
+
+    @property
+    def on_startup(self):
+        return self.app.on_startup
+
+    @property
+    def on_shutdown(self):
+        return self.app.on_shutdown
+
+    @property
+    def on_cleanup(self):
+        return self.app.on_cleanup
+
+    @property
+    def cleanup_ctx(self):
+        return self.app.cleanup_ctx
+
+
+app = Application()
+
+
+class Object(dict):
+    def __init__(self, obj: dict):
+        super().__init__()
+        for k, v in obj.items():
+            self[k] = v
+
+    def __getattr__(self, key):
+        return self[key] if key in self else ""
+
+    def __setattr__(self, key, value):
+        self[key] = value
+
+    def __str__(self):
+        return self.key
+
+
+class JsonEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, datetime.datetime) or isinstance(obj, datetime.date):
+            return obj.__str__()
+        else:
+            return super(JsonEncoder, self).default(obj)
+
+
+def get(path, name=None):
+    return app.add_router(path, "GET", name)
+
+
+def post(path, name=None):
+    return app.add_router(path, "POST", name)
+
+
+def put(path, name=None):
+    return app.add_router(path, "PUT", name)
+
+
+def delete(path, name=None):
+    return app.add_router(path, "DELETE", name)
+
+
+def all(path):
+    #     return app._actions(path, 'GET')
+    return app.route_table.view(path)
+
+
+def jsons(data, **kw):
+    res = {}
+    if isinstance(data, list):
+        res["data"] = data
+    elif isinstance(data, dict):
+        res.update(data)
+    elif isinstance(data, tuple):
+        data = dict(data)
+        res.update(data)
+    else:
+        raise ValueError("data must be list , dict or tuple.")
+    res["timestamp"] = int(datetime.datetime.now().timestamp() * 1000)
+    text = json.dumps(res, ensure_ascii=False, cls=JsonEncoder)
+    return web.json_response(text=text, **kw)
+
+
+def middleware():
+    return app.add_middleware()
+
+
+def render(**kw):
+    return web.Response(**kw)
+
+
+def view(template=None, *args, **kw):
+    body = None
+    if app.env is not None:
+        body = app.env.get_template(template).render(*args)
+    _view = render(body=body, **kw)
+    _view.content_type = "text/html;charset=utf-8"
+    return _view
+
+
+def redirect(urlpath):
+    return web.HTTPFound(location=urlpath)
```

### Comparing `cloudoll-2.0.3/cloudoll/web/http.py` & `cloudoll-2.0.4/cloudoll/web/http.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
- 
-__author__ = "chuchur/chuchur.com"
-
-import requests
-import time
-
-from ..logging import logging
-
-PROXIES = {
-    "http": "http://127.0.0.1:7890",
-    "https": "http://127.0.0.1:7890",
-}
-
-HEADERS = {
-    "sec-ch-ua": '"Not A;Brand";v="99", "Chromium";v="102", "Google Chrome";v="102"',
-    "sec-ch-ua-mobile": "?0",
-    "sec-ch-ua-platform": "Windows",
-    "sec-fetch-dest": "empty",
-    "sec-fetch-mode": "cors",
-    "Expires": "0",
-    "Pragma": "no-cache",
-    "Cache": "no-cache",
-    "Cache-control": "no-cache",
-    "Connection": "keep-alive",
-    # "Content-Type": "application/json; charset=UTF-8",
-    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36",
-}
-
-
-class Client(object):
-    def __init__(self):
-        self.session = requests.Session()
-
-    def requests(self, method, url, **kw):
-        headers = kw.get("headers", None)
-        if headers is None:
-            headers = HEADERS
-        else:
-            headers = {**headers, **HEADERS}
-        kw["headers"] = headers
-        proxies = kw.get("proxies", False)
-        if proxies:
-            if proxies is True:
-                kw["proxies"] = PROXIES
-            else:
-                kw["proxies"] = proxies
-        trytimes = kw.get("trytimes", 2)
-        if trytimes != 2:
-            kw.pop("trytimes")
-        result = None
-        while trytimes > 0:
-            try:
-                fun = getattr(self.session, method, None)
-                result = fun(url, **kw)
-                trytimes = 0
-                head = result.headers
-                ctype = head["Content-Type"]
-                if result.status_code==200:
-                    if "application/json" in ctype:
-                        return result.json()
-                    elif "text/html" in ctype:
-                        return result.text
-                    return result
-                else:
-                    logging.error("Network error ,try gain....")
-                    trytimes += 1
-                    time.sleep(2)
-            except BaseException as e:
-                # logging.info(e)
-                logging.error("Network error ,try gain....")
-                trytimes -= 1
-                time.sleep(2)
-                # logging.info(e)
-        return result
-
-
-http = Client()
-
-
-def get(url, **kw):
-    """
-    get 请求
-    :params params=dict() 传参
-    """
-    return http.requests("get", url, **kw)
-
-
-def post(url, **kw):
-    """
-    post 请求
-    :params data=dict() or json=dict() 传参
-    """
-    return http.requests("post", url, **kw)
-
-
-def put(url, **kw):
-    """
-    post 请求
-    data=dict()传参
-    """
-    return http.requests("put", url, **kw)
-
-
-def delete(url, **kw):
-    return http.requests("delete", url, **kw)
-
-
-def head(url, **kw):
-    return http.requests("head", url, **kw)
-
-
-def option(url, **kw):
-    return http.requests("option", url, **kw)
-
-
-def download(url, savepath=None, **kw):
-    """
-    下载文件
-    :params url 文件的地址
-    :params savepath 保存路径
-    """
-    rb = http.requests("get", url, **kw)
-    if not savepath:
-        return rb.content
-    if not rb:
-        logging.error("下载出错")
-        return False
-    else:
-        try:
-            with open(savepath, "wb") as f:
-                f.write(rb.content)
-                logging.info("下载完成！")
-        except BaseException as e:
-            logging.error(e)
-            return False
-    return True
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+ 
+__author__ = "chuchur/chuchur.com"
+
+import requests
+import time
+
+from ..logging import logging
+
+PROXIES = {
+    "http": "http://127.0.0.1:7890",
+    "https": "http://127.0.0.1:7890",
+}
+
+HEADERS = {
+    "sec-ch-ua": '"Not A;Brand";v="99", "Chromium";v="102", "Google Chrome";v="102"',
+    "sec-ch-ua-mobile": "?0",
+    "sec-ch-ua-platform": "Windows",
+    "sec-fetch-dest": "empty",
+    "sec-fetch-mode": "cors",
+    "Expires": "0",
+    "Pragma": "no-cache",
+    "Cache": "no-cache",
+    "Cache-control": "no-cache",
+    "Connection": "keep-alive",
+    # "Content-Type": "application/json; charset=UTF-8",
+    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36",
+}
+
+
+class Client(object):
+    def __init__(self):
+        self.session = requests.Session()
+
+    def requests(self, method, url, **kw):
+        headers = kw.get("headers", None)
+        if headers is None:
+            headers = HEADERS
+        else:
+            headers = {**headers, **HEADERS}
+        kw["headers"] = headers
+        proxies = kw.get("proxies", False)
+        if proxies:
+            if proxies is True:
+                kw["proxies"] = PROXIES
+            else:
+                kw["proxies"] = proxies
+        trytimes = kw.get("trytimes", 2)
+        if trytimes != 2:
+            kw.pop("trytimes")
+        result = None
+        while trytimes > 0:
+            try:
+                fun = getattr(self.session, method, None)
+                result = fun(url, **kw)
+                trytimes = 0
+                head = result.headers
+                ctype = head["Content-Type"]
+                if result.status_code==200:
+                    if "application/json" in ctype:
+                        return result.json()
+                    elif "text/html" in ctype:
+                        return result.text
+                    return result
+                else:
+                    logging.error("Network error ,try gain....")
+                    trytimes += 1
+                    time.sleep(2)
+            except BaseException as e:
+                # logging.info(e)
+                logging.error("Network error ,try gain....")
+                trytimes -= 1
+                time.sleep(2)
+                # logging.info(e)
+        return result
+
+
+http = Client()
+
+
+def get(url, **kw):
+    """
+    get 请求
+    :params params=dict() 传参
+    """
+    return http.requests("get", url, **kw)
+
+
+def post(url, **kw):
+    """
+    post 请求
+    :params data=dict() or json=dict() 传参
+    """
+    return http.requests("post", url, **kw)
+
+
+def put(url, **kw):
+    """
+    post 请求
+    data=dict()传参
+    """
+    return http.requests("put", url, **kw)
+
+
+def delete(url, **kw):
+    return http.requests("delete", url, **kw)
+
+
+def head(url, **kw):
+    return http.requests("head", url, **kw)
+
+
+def option(url, **kw):
+    return http.requests("option", url, **kw)
+
+
+def download(url, savepath=None, **kw):
+    """
+    下载文件
+    :params url 文件的地址
+    :params savepath 保存路径
+    """
+    rb = http.requests("get", url, **kw)
+    if not savepath:
+        return rb.content
+    if not rb:
+        logging.error("下载出错")
+        return False
+    else:
+        try:
+            with open(savepath, "wb") as f:
+                f.write(rb.content)
+                logging.info("下载完成！")
+        except BaseException as e:
+            logging.error(e)
+            return False
+    return True
```

### Comparing `cloudoll-2.0.3/cloudoll/web/jwt.py` & `cloudoll-2.0.4/cloudoll/web/jwt.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-__author__ = "chuchur/chuchur.com"
-
-import jwt, datetime
-from ..logging import logging
-
-
-def encode(payload, key, exp: [int, str] = 3600):
-    """
-    jwt 加密
-    :params payload
-    :params key
-    :params exp 过期时间单位秒，默认1个小时
-    """
-    headers = dict(typ="jwt", alg="HS256")
-    exp = datetime.datetime.now() + datetime.timedelta(seconds=eval(exp) if isinstance(exp, str) else exp)  # 过期时间
-    payload["exp"] = exp.timestamp()
-    result = jwt.encode(payload=payload, key=key, algorithm="HS256", headers=headers)
-    return result
-
-
-def decode(token, key):
-    """
-    jwt
-    :params token
-    :params key
-    """
-    try:
-        payload = jwt.decode(token, key, algorithms=['HS256'])
-        if not payload:
-            return None
-        now = datetime.datetime.now().timestamp()  # 当前时间
-        if int(now) > int(payload["exp"]):  # 登录时间过期
-            return None
-        return payload  # 返回自定义内容
-    except Exception as e:
-        logging.error(e)
-        return None
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+__author__ = "chuchur/chuchur.com"
+
+import jwt, datetime
+from ..logging import logging
+
+
+def encode(payload, key, exp: [int, str] = 3600):
+    """
+    jwt 加密
+    :params payload
+    :params key
+    :params exp 过期时间单位秒，默认1个小时
+    """
+    headers = dict(typ="jwt", alg="HS256")
+    exp = datetime.datetime.now() + datetime.timedelta(seconds=eval(exp) if isinstance(exp, str) else exp)  # 过期时间
+    payload["exp"] = exp.timestamp()
+    result = jwt.encode(payload=payload, key=key, algorithm="HS256", headers=headers)
+    return result
+
+
+def decode(token, key):
+    """
+    jwt
+    :params token
+    :params key
+    """
+    try:
+        payload = jwt.decode(token, key, algorithms=['HS256'])
+        if not payload:
+            return None
+        now = datetime.datetime.now().timestamp()  # 当前时间
+        if int(now) > int(payload["exp"]):  # 登录时间过期
+            return None
+        return payload  # 返回自定义内容
+    except Exception as e:
+        logging.error(e)
+        return None
```

### Comparing `cloudoll-2.0.3/cloudoll.egg-info/PKG-INFO` & `cloudoll-2.0.4/cloudoll.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,337 +1,337 @@
-Metadata-Version: 2.1
-Name: cloudoll
-Version: 2.0.3
-Summary: 辅助快速创建可分布的微服务。
-Home-page: https://gitee.com/chuchur/cloudoll-py
-Author: chuchur
-Author-email: chuchur@qq.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# cloudoll 云端玩具
-
-## 更新日志
-`2.0.2` 2023-07-03
-- 优化一系列问题
-- 可以热加载
-
-`2.0.0` 2023-06-09
-- 优化一系列问题
-- orm 执行更优雅
-
-`0.1.6` 2022-11-03
-- orm 允许更新为空数据
-- server 文件上传加入大小限制
-- smtp 出错异常处理
-
-`0.1.5` 2022-09-19
-- 修复logging level 错误的问题
-- 修正默认依赖
- 
-`0.1.4` 2022-09-12
-- 优化orm 超时的问题
-- 增加websocket 支持
-
-
-## Documentation
-
-
-[Docs](https://cloudoll.chuchur.com)
-
-[Docs](https://cloudoll.chuchur.com)
-
-[Structure](https://cloudoll.chuchur.com/structure)
-
-[Config](https://cloudoll.chuchur.com/config)
-
-[Middleware](https://cloudoll.chuchur.com/middleware)
-
-[Router](https://cloudoll.chuchur.com/router)
-
-[View](https://cloudoll.chuchur.com/view)
-
-[Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
-
-[Upload file](https://cloudoll.chuchur.com/file-uploads)
-
-[WebSocket](https://cloudoll.chuchur.com/websockets)
-
-[Mysql](https://cloudoll.chuchur.com/mysql)
-
-[Deployment](https://cloudoll.chuchur.com/deployment)
-
-
-## 环境准备
-
-- 操作系统：支持 macOS，Linux，Windows
-- 运行环境：最低要求 3.6.0。
-
-## 快速开始
-
-```sh
-$ mkdir cloudoll-demo && cd cloudoll-demo
-$ pip3 install cloudoll
-$ vi app.py
-```
-
-`app.py` 内容如下:
-
-```python
-## /app.py
-from cloudoll.web import app
-
-
-if __name__ == "__main__":
-    app.create().run()
-```
-
-### 编写 Controller
-
-```sh
-$ mkdir -p controllers/home
-$ touch controllers/home/__init__.py
-$ vi controllers/home/index.py
-```
-
-`controllers/home/index.py` 内容如下:
-
-```python
-# /controllers/home/index.py
-from cloudoll.web import get, jsons
-
-@get('/')
-async def home():
-    return jsons({"name": "chuchur" ,"msg": "ok"})
-```
-
-运行:
-```sh
-$ python3 app.py
-$ open http://localhost:9001
-```
-
-在浏览器打开 [http://127.0.0.1:9001/](http://127.0.0.1:9001/)
-
-就能看到:
-
-```json
-{ 
-    "name": "chuchur" ,
-    "msg": "ok" ,
-    "timestamp": 1681993906410 
-}
-```
-
-恭喜, 你已经成功的写好了一个 `Restful API`接口. 
-
-
-### 模板渲染
-
-绝大多数情况，我们都需要读取数据后渲染模板，然后呈现给用户。故我们需要引入对应的模板引擎。
-
-在本例中，我们使用 [Nunjucks](https://mozilla.github.io/nunjucks/) 来渲染
-```sh
-$ mkdir templates
-$ vi templates/index.html
-```
-
-`index.html` 内容如下:
-
-```html
-<!-- /templates/index.html -->
-
-<!DOCTYPE html>
-<html lang="zh">
-<head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>Home</title>
-</head>
-<body>
-    <p>My name is {{name} }</p>
-</body>
-</html>
-```
-
-
-修改 `/controllers/home/index.py` 内容如下:
-
-```python
-# /controllers/home/index.py
-from cloudoll.web import get, view
-
-@get('/')
-async def home():
-    data = {"name": "chuchur" ,"msg": "ok"}
-    return view("index.html",data)
-```
-
-这时 页面正常渲染 ,可以看到  `“My name is chuchur”`
-
-恭喜, 你已经成功的写好了一个视图页面.
-
-### 静态资源
-
-我们想在模版里面嵌入静态资源,如图片,js ,css , 这个时候就得用到静态资源. 我们把这些`js` ,`css` ,`image`  都放到 `static` 目录
-
-线上环境建议部署到 CDN，或者使用 `nginx` 等相关服务器
-
-```sh
-$ mkdir -p static/img
-$ mkdir -p static/js
-$ mkdir -p static/css
-```
-在 `img`目录 放入在张图 名`logo.png`
-
-在 `js` 目录新建 `index.js` ,内容如下:
-
-点击页面 弹出 "hello world"
-```js
-// /static/js/index.js
-document.addEventListener('DOMContentLoaded',function(){
-    document.body.addEventListener('click',function(){
-        alert('hello world.')
-    })
-})
-```
-在 `css` 目录新建 `index.css` ,内容如下:
-```css
- /* /static/css/index.css */
-html,body {
-    width: 100%;
-    height: 100%;
-    color: red;
-}
-```
-
-修改视图 `/templates/index.html` ,在 `head` 引入 静态资源, 内容如下:
-
-```html
-<!-- /templates/index.html -->
-<!DOCTYPE html>
-<html lang="zh">
-<head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <link rel="icon" type="image/png" href="/static/img/logo.png"/>
-    <link rel="stylesheet" href="/static/css/index.css">
-    <script src="/static/js/index.js"></script>
-    <title>Home</title>
-</head>
-<body>
-    <p>My name is {{name} }</p>
-</body>
-</html>
-```
-
-我们新建一个配置文件, 在配置文件里面配置静态 资源.
-
-```sh
-$ mkdir config
-$ vi config/conf.local.yaml
-```
-
-`/config/conf.local.yaml` 内容如下:
-
-```yaml
-server:
-  static:
-    prefix: /static
-```
-
-
-刷新页面之后, 我们所改动即可呈现.
-
-### 编写 Middleware
-
-假设有个需求：我们的新闻站点，禁止百度爬虫访问。
-
-所以可以通过 `Middleware` 判断 User-Agent，如下：
-
-```sh
-$ mkdir middlewares
-$ vi middlewares/robot.py
-```
-
-修改 `middlewares/robot.py`, 内容如下:
-
-```python
-# /middlewares/robot.py
-from cloudoll.web import middleware, render
-import re
-
-@middleware()
-def mid_robot():
-    async def robot(request, handler):
-        ua = request.headers.get('user-agent')
-        if re.match('Baiduspider', ua):
-            return render(status=403, text="Go away , robot.")
-        return await handler(request)
-
-    return robot
-```
-
-重新启动之后, 现在可以使用 `curl http://localhost:7001/news -A "Baiduspider"` 看看效果。
-
-更多参见中间件文档。
-
-### 配置文件
-写业务的时候，不可避免的需要有配置文件，使用代码管理配置，在代码中添加多个环境的配置，在启动时传入当前环境的参数即可.
-
-cloudoll 支持根据环境来加载配置，定义多个环境的配置文件
-
-```ini
-config
-|- conf.local.yaml
-|- conf.prod.yaml
-`- conf.test.yaml
-```
-
-我们创建配置文件：
-
-```sh
-$ mkdir -p config/conf.local.yaml
-$ vi config/conf.local.yaml
-```
-
-如下是 mysql 和 server 的配置：
-
-```yaml
-server:
-  host: 192.168.0.1
-  port: 9001
-  static: false
-  client_max_size: 1024000
-  static: 
-    prefix: /static
-    show_index: true
-    append_version: true
-    follow_symlinks: true
-mysql:
-  host: 127.0.0.1
-  port: 3306
-  user: root
-  password: abcd
-  db: blog
-  charset: utf8mb4
-```
-
-默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
-
-
-# 开发模式
-
-```sh
-adev runserver app.py
-```
+Metadata-Version: 2.1
+Name: cloudoll
+Version: 2.0.4
+Summary: 辅助快速创建可分布的微服务。
+Home-page: https://gitee.com/chuchur/cloudoll-py
+Author: chuchur
+Author-email: chuchur@qq.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# cloudoll 云端玩具
+
+## 更新日志
+`2.0.2` 2023-07-03
+- 优化一系列问题
+- 可以热加载
+
+`2.0.0` 2023-06-09
+- 优化一系列问题
+- orm 执行更优雅
+
+`0.1.6` 2022-11-03
+- orm 允许更新为空数据
+- server 文件上传加入大小限制
+- smtp 出错异常处理
+
+`0.1.5` 2022-09-19
+- 修复logging level 错误的问题
+- 修正默认依赖
+ 
+`0.1.4` 2022-09-12
+- 优化orm 超时的问题
+- 增加websocket 支持
+
+
+## Documentation
+
+
+[Docs](https://cloudoll.chuchur.com)
+
+[Docs](https://cloudoll.chuchur.com)
+
+[Structure](https://cloudoll.chuchur.com/structure)
+
+[Config](https://cloudoll.chuchur.com/config)
+
+[Middleware](https://cloudoll.chuchur.com/middleware)
+
+[Router](https://cloudoll.chuchur.com/router)
+
+[View](https://cloudoll.chuchur.com/view)
+
+[Cookie and Session](https://cloudoll.chuchur.com/session-cookie)
+
+[Upload file](https://cloudoll.chuchur.com/file-uploads)
+
+[WebSocket](https://cloudoll.chuchur.com/websockets)
+
+[Mysql](https://cloudoll.chuchur.com/mysql)
+
+[Deployment](https://cloudoll.chuchur.com/deployment)
+
+
+## 环境准备
+
+- 操作系统：支持 macOS，Linux，Windows
+- 运行环境：最低要求 3.6.0。
+
+## 快速开始
+
+```sh
+$ mkdir cloudoll-demo && cd cloudoll-demo
+$ pip3 install cloudoll
+$ vi app.py
+```
+
+`app.py` 内容如下:
+
+```python
+## /app.py
+from cloudoll.web import app
+
+
+if __name__ == "__main__":
+    app.create().run()
+```
+
+### 编写 Controller
+
+```sh
+$ mkdir -p controllers/home
+$ touch controllers/home/__init__.py
+$ vi controllers/home/index.py
+```
+
+`controllers/home/index.py` 内容如下:
+
+```python
+# /controllers/home/index.py
+from cloudoll.web import get, jsons
+
+@get('/')
+async def home():
+    return jsons({"name": "chuchur" ,"msg": "ok"})
+```
+
+运行:
+```sh
+$ python3 app.py
+$ open http://localhost:9001
+```
+
+在浏览器打开 [http://127.0.0.1:9001/](http://127.0.0.1:9001/)
+
+就能看到:
+
+```json
+{ 
+    "name": "chuchur" ,
+    "msg": "ok" ,
+    "timestamp": 1681993906410 
+}
+```
+
+恭喜, 你已经成功的写好了一个 `Restful API`接口. 
+
+
+### 模板渲染
+
+绝大多数情况，我们都需要读取数据后渲染模板，然后呈现给用户。故我们需要引入对应的模板引擎。
+
+在本例中，我们使用 [Nunjucks](https://mozilla.github.io/nunjucks/) 来渲染
+```sh
+$ mkdir templates
+$ vi templates/index.html
+```
+
+`index.html` 内容如下:
+
+```html
+<!-- /templates/index.html -->
+
+<!DOCTYPE html>
+<html lang="zh">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Home</title>
+</head>
+<body>
+    <p>My name is {{name} }</p>
+</body>
+</html>
+```
+
+
+修改 `/controllers/home/index.py` 内容如下:
+
+```python
+# /controllers/home/index.py
+from cloudoll.web import get, view
+
+@get('/')
+async def home():
+    data = {"name": "chuchur" ,"msg": "ok"}
+    return view("index.html",data)
+```
+
+这时 页面正常渲染 ,可以看到  `“My name is chuchur”`
+
+恭喜, 你已经成功的写好了一个视图页面.
+
+### 静态资源
+
+我们想在模版里面嵌入静态资源,如图片,js ,css , 这个时候就得用到静态资源. 我们把这些`js` ,`css` ,`image`  都放到 `static` 目录
+
+线上环境建议部署到 CDN，或者使用 `nginx` 等相关服务器
+
+```sh
+$ mkdir -p static/img
+$ mkdir -p static/js
+$ mkdir -p static/css
+```
+在 `img`目录 放入在张图 名`logo.png`
+
+在 `js` 目录新建 `index.js` ,内容如下:
+
+点击页面 弹出 "hello world"
+```js
+// /static/js/index.js
+document.addEventListener('DOMContentLoaded',function(){
+    document.body.addEventListener('click',function(){
+        alert('hello world.')
+    })
+})
+```
+在 `css` 目录新建 `index.css` ,内容如下:
+```css
+ /* /static/css/index.css */
+html,body {
+    width: 100%;
+    height: 100%;
+    color: red;
+}
+```
+
+修改视图 `/templates/index.html` ,在 `head` 引入 静态资源, 内容如下:
+
+```html
+<!-- /templates/index.html -->
+<!DOCTYPE html>
+<html lang="zh">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <link rel="icon" type="image/png" href="/static/img/logo.png"/>
+    <link rel="stylesheet" href="/static/css/index.css">
+    <script src="/static/js/index.js"></script>
+    <title>Home</title>
+</head>
+<body>
+    <p>My name is {{name} }</p>
+</body>
+</html>
+```
+
+我们新建一个配置文件, 在配置文件里面配置静态 资源.
+
+```sh
+$ mkdir config
+$ vi config/conf.local.yaml
+```
+
+`/config/conf.local.yaml` 内容如下:
+
+```yaml
+server:
+  static:
+    prefix: /static
+```
+
+
+刷新页面之后, 我们所改动即可呈现.
+
+### 编写 Middleware
+
+假设有个需求：我们的新闻站点，禁止百度爬虫访问。
+
+所以可以通过 `Middleware` 判断 User-Agent，如下：
+
+```sh
+$ mkdir middlewares
+$ vi middlewares/robot.py
+```
+
+修改 `middlewares/robot.py`, 内容如下:
+
+```python
+# /middlewares/robot.py
+from cloudoll.web import middleware, render
+import re
+
+@middleware()
+def mid_robot():
+    async def robot(request, handler):
+        ua = request.headers.get('user-agent')
+        if re.match('Baiduspider', ua):
+            return render(status=403, text="Go away , robot.")
+        return await handler(request)
+
+    return robot
+```
+
+重新启动之后, 现在可以使用 `curl http://localhost:7001/news -A "Baiduspider"` 看看效果。
+
+更多参见中间件文档。
+
+### 配置文件
+写业务的时候，不可避免的需要有配置文件，使用代码管理配置，在代码中添加多个环境的配置，在启动时传入当前环境的参数即可.
+
+cloudoll 支持根据环境来加载配置，定义多个环境的配置文件
+
+```ini
+config
+|- conf.local.yaml
+|- conf.prod.yaml
+`- conf.test.yaml
+```
+
+我们创建配置文件：
+
+```sh
+$ mkdir -p config/conf.local.yaml
+$ vi config/conf.local.yaml
+```
+
+如下是 mysql 和 server 的配置：
+
+```yaml
+server:
+  host: 192.168.0.1
+  port: 9001
+  static: false
+  client_max_size: 1024000
+  static: 
+    prefix: /static
+    show_index: true
+    append_version: true
+    follow_symlinks: true
+mysql:
+  host: 127.0.0.1
+  port: 3306
+  user: root
+  password: abcd
+  db: blog
+  charset: utf8mb4
+```
+
+默认开发会使用默认的`local`作为配置。 启动时 通过 `env` 加载对应的配置。 如 `python3 app.py --env=prod` 会加载 `conf.prod.yaml`
+
+
+# 开发模式
+
+```sh
+adev runserver app.py
+```
```

### Comparing `cloudoll-2.0.3/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.0.4/cloudoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.3/setup.py` & `cloudoll-2.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pipenv install twine --dev # pip install --user --upgrade twine
-# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = "cloudoll"
-DESCRIPTION = "辅助快速创建可分布的微服务。"
-URL = "https://gitee.com/chuchur/cloudoll-py"
-EMAIL = "chuchur@qq.com"
-AUTHOR = "chuchur"
-REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.0.3"
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-    "requests",
-    "colorlog",
-    "aiomysql",
-    "aiopg",
-    "aiohttp",
-    "aioredis",
-    "aiomcache",
-    "aiohttp-devtools",
-    "jinja2",
-    "pyjwt",
-    "aiohttp_session[secure]",
-    "PyYAML",
-]
-
-# What packages are optional?
-EXTRAS = {
-    # 'fancy feature': ['django'],
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
-        long_description = "\n" + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, "__version__.py")) as f:
-        exec(f.read(), about)
-else:
-    about["__version__"] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = "Build and publish the package."
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print("\033[1m{0}\033[0m".format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status("Removing previous builds…")
-            rmtree(os.path.join(here, "dist"))
-        except OSError:
-            pass
-
-        self.status("Building Source and Wheel (universal) distribution…")
-        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
-
-        self.status("Uploading the package to PyPI via Twine…")
-        os.system("twine upload dist/*")
-
-        self.status("Pushing git tags…")
-        os.system("git tag v{0}".format(about["__version__"]))
-        os.system("git push --tags")
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about["__version__"],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license="MIT",
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        "upload": UploadCommand,
-    },
-)
-
-# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pipenv install twine --dev # pip install --user --upgrade twine
+# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = "cloudoll"
+DESCRIPTION = "辅助快速创建可分布的微服务。"
+URL = "https://gitee.com/chuchur/cloudoll-py"
+EMAIL = "chuchur@qq.com"
+AUTHOR = "chuchur"
+REQUIRES_PYTHON = ">=3.6.0"
+VERSION = "2.0.4"
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+    "requests",
+    "colorlog",
+    "aiomysql",
+    "aiopg",
+    "aiohttp",
+    "aioredis",
+    "aiomcache",
+    "aiohttp-devtools",
+    "jinja2",
+    "pyjwt",
+    "aiohttp_session[secure]",
+    "PyYAML",
+]
+
+# What packages are optional?
+EXTRAS = {
+    # 'fancy feature': ['django'],
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
+        exec(f.read(), about)
+else:
+    about["__version__"] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = "Build and publish the package."
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print("\033[1m{0}\033[0m".format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
+        except OSError:
+            pass
+
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
+
+        # self.status("Pushing git tags…")
+        # os.system("git tag v{0}".format(about["__version__"]))
+        # os.system("git push --tags")
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about["__version__"],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license="MIT",
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        "upload": UploadCommand,
+    },
+)
+
+# python setup.py sdist build && python setup.py bdist_wheel && python setup.py sdist upload
```

