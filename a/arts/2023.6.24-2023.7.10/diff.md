# Comparing `tmp/arts-2023.6.24.tar.gz` & `tmp/arts-2023.7.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-2023.6.24.tar", last modified: Sat Jun 24 15:36:43 2023, max compression
+gzip compressed data, was "arts-2023.7.10.tar", last modified: Sun Jul  9 07:15:16 2023, max compression
```

## Comparing `arts-2023.6.24.tar` & `arts-2023.7.10.tar`

### file list

```diff
@@ -1,30 +1,34 @@
--rw-r--r--   0        0        0     1990 2023-06-24 12:37:19.999502 arts-2023.6.24/.gitignore
--rw-r--r--   0        0        0     1517 2023-06-24 13:14:40.419750 arts-2023.6.24/README.md
--rw-r--r--   0        0        0       35 2023-06-24 05:26:09.197796 arts-2023.6.24/arts/__init__.py
--rw-r--r--   0        0        0      411 2023-06-24 05:26:19.045385 arts-2023.6.24/arts/_core.py
--rw-r--r--   0        0        0     2114 2023-06-24 07:00:51.182588 arts-2023.6.24/arts/万象思考/ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0      772 2023-06-23 06:31:13.738964 arts-2023.6.24/arts/万象思考/万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0     3693 2023-06-24 08:40:00.061857 arts-2023.6.24/arts/万象思考/人权/人人平等是个伪概念/README.md
--rw-r--r--   0        0        0     5051 2023-06-24 08:20:27.835932 arts-2023.6.24/arts/万象思考/人权/堕胎自由权/README.md
--rw-r--r--   0        0        0     1584 2023-06-23 06:49:51.732869 arts-2023.6.24/arts/万象思考/什么是“迷信科学”？/README.md
--rw-r--r--   0        0        0     3149 2023-06-24 08:34:59.453148 arts-2023.6.24/arts/万象思考/有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0     1226 2023-06-24 06:51:31.392036 arts-2023.6.24/arts/万象思考/熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0     1120 2023-06-24 06:40:41.705204 arts-2023.6.24/arts/其它/现在的‘人工智能’是‘穷举智能’/README.md
--rw-r--r--   0        0        0     2974 2023-06-24 07:25:06.881399 arts-2023.6.24/arts/其它/用均匀抽样作文件指纹的可靠性/README.md
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:35.450766 arts-2023.6.24/arts/原创小说/天使传奇/1、被绑架/README.md
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:16.614903 arts-2023.6.24/arts/原创小说/陆小凤新传/燕山宝藏/第一章/README.md
--rw-r--r--   0        0        0     3353 2023-06-24 07:15:39.665620 arts-2023.6.24/arts/时空遐想/轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0     2042 2023-06-24 05:45:38.711787 arts-2023.6.24/arts/编程教程/Python/其它/调用openAI进行连续对话/README.md
--rw-r--r--   0        0        0   254025 2023-06-14 02:25:03.834797 arts-2023.6.24/arts/编程教程/Python/其它/调用openAI进行连续对话/封面.jpg
--rw-r--r--   0        0        0     3395 2023-06-24 07:55:32.849161 arts-2023.6.24/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0   132558 2023-06-24 07:41:37.503743 arts-2023.6.24/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/无颜色版.png
--rw-r--r--   0        0        0   135794 2023-06-24 07:38:22.760800 arts-2023.6.24/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/有颜色版.png
--rw-r--r--   0        0        0    18019 2023-06-24 06:12:43.983353 arts-2023.6.24/arts/编程教程/Python/数据库/操作MongoDB简明教程/README.md
--rw-r--r--   0        0        0    18733 2023-06-24 06:13:20.633561 arts-2023.6.24/arts/编程教程/Python/数据库/操作MySQL简明教程/README.md
--rw-r--r--   0        0        0     8138 2023-06-24 05:44:39.242507 arts-2023.6.24/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
--rw-r--r--   0        0        0   486729 2023-06-17 08:11:16.639983 arts-2023.6.24/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png
--rw-r--r--   0        0        0     1742 2023-06-24 07:01:54.613165 arts-2023.6.24/arts/论时事/评价在北京工体冲进场的梅西粉丝/README.md
--rw-r--r--   0        0        0   148143 2023-06-18 06:04:10.170676 arts-2023.6.24/arts/论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg
--rw-r--r--   0        0        0     7735 2023-06-24 14:44:43.471556 arts-2023.6.24/index.html
--rw-r--r--   0        0        0      328 2023-06-24 15:35:18.017203 arts-2023.6.24/pyproject.toml
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 arts-2023.6.24/PKG-INFO
+-rw-r--r--   0        0        0     2008 2023-07-09 05:21:16.311980 arts-2023.7.10/.gitignore
+-rw-r--r--   0        0        0     1409 2023-07-09 07:13:27.518674 arts-2023.7.10/README.md
+-rw-r--r--   0        0        0     3064 2023-07-03 07:43:10.621577 arts-2023.7.10/arts/[1]编程教程/Python/5分钟理清Python的时间操作/README.md
+-rw-r--r--   0        0        0     3395 2023-06-24 07:55:32.849161 arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0   132558 2023-06-24 07:41:37.503743 arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/无颜色版.png
+-rw-r--r--   0        0        0   135794 2023-06-24 07:38:22.760800 arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/有颜色版.png
+-rw-r--r--   0        0        0     2042 2023-06-24 05:45:38.711787 arts-2023.7.10/arts/[1]编程教程/Python/[2]其它/调用openAI进行连续对话/README.md
+-rw-r--r--   0        0        0   254025 2023-06-14 02:25:03.834797 arts-2023.7.10/arts/[1]编程教程/Python/[2]其它/调用openAI进行连续对话/封面.jpg
+-rw-r--r--   0        0        0    18019 2023-06-24 06:12:43.983353 arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MongoDB简明教程/README.md
+-rw-r--r--   0        0        0    18733 2023-06-24 06:13:20.633561 arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MySQL简明教程/README.md
+-rw-r--r--   0        0        0     8138 2023-06-24 05:44:39.242507 arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md
+-rw-r--r--   0        0        0   486729 2023-06-17 08:11:16.639983 arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png
+-rw-r--r--   0        0        0     1447 2023-07-09 03:17:30.347956 arts-2023.7.10/arts/[2]批判·伪文艺/一元官司有意义吗？/README.md
+-rw-r--r--   0        0        0     1742 2023-06-24 07:01:54.613165 arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/README.md
+-rw-r--r--   0        0        0   148143 2023-06-18 06:04:10.170676 arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:35.450766 arts-2023.7.10/arts/[87]原创小说/天使传奇/1、被绑架/README.md
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:16.614903 arts-2023.7.10/arts/[87]原创小说/陆小凤新传/燕山宝藏/第一章/README.md
+-rw-r--r--   0        0        0   644251 2023-07-05 13:25:53.974953 arts-2023.7.10/arts/[88]原创UI/富文本笔记本/README.png
+-rw-r--r--   0        0        0   793233 2023-07-05 13:25:39.829792 arts-2023.7.10/arts/[89]原创图片/捷鸟/README.jpg
+-rw-r--r--   0        0        0     2114 2023-07-03 07:30:37.022832 arts-2023.7.10/arts/[8]万象思考/ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0      772 2023-06-23 06:31:13.738964 arts-2023.7.10/arts/[8]万象思考/万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0     3693 2023-06-24 08:40:00.061857 arts-2023.7.10/arts/[8]万象思考/人权/人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0     5051 2023-06-24 08:20:27.835932 arts-2023.7.10/arts/[8]万象思考/人权/堕胎自由权/README.md
+-rw-r--r--   0        0        0     1584 2023-06-23 06:49:51.732869 arts-2023.7.10/arts/[8]万象思考/什么是“迷信科学”？/README.md
+-rw-r--r--   0        0        0     1672 2023-07-08 11:03:35.265812 arts-2023.7.10/arts/[8]万象思考/心理学中个案研究有意义吗？/README.md
+-rw-r--r--   0        0        0     3149 2023-06-24 08:34:59.453148 arts-2023.7.10/arts/[8]万象思考/有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0     1226 2023-06-24 06:51:31.392036 arts-2023.7.10/arts/[8]万象思考/熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0     1120 2023-07-08 16:03:09.173781 arts-2023.7.10/arts/[99]其它/现在的‘人工智能’是‘穷举智能’/README.md
+-rw-r--r--   0        0        0     2976 2023-07-09 04:11:45.403508 arts-2023.7.10/arts/[99]其它/用均匀抽样作文件指纹的可靠性/README.md
+-rw-r--r--   0        0        0     3353 2023-06-24 07:15:39.665620 arts-2023.7.10/arts/[9]时空遐想/轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0       35 2023-06-24 05:26:09.197796 arts-2023.7.10/arts/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-09 07:08:46.286344 arts-2023.7.10/arts/_core.py
+-rw-r--r--   0        0        0      345 2023-07-09 07:14:25.121621 arts-2023.7.10/pyproject.toml
+-rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 arts-2023.7.10/PKG-INFO
```

### Comparing `arts-2023.6.24/.gitignore` & `arts-2023.7.10/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 **/_ig_**
 *.zip
 *.cmd
 *.sql
 *.txt
 *.json
 
+**/_ii_**
+*.mp4
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `arts-2023.6.24/README.md` & `arts-2023.7.10/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # 项目描述
 
-GitHub Pages 部署辅助 —— README 文件提取器。
-
-用于快捷提取指定目录下的所有子孙文件夹中的 README.md 文件，以方便部署到 GitHub Pages 上。
+快捷提取指定目录下所有子孙文件夹中的 README.* 文件。
 
 # 安装
 
 ```
 pip install arts
 ```
 
 # 关于作者
 
-作者：许灿标
+作者：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)
 
 # 教程
```

### Comparing `arts-2023.6.24/arts/万象思考/ChatGPT已经有自我意识了/README.md` & `arts-2023.7.10/arts/[8]万象思考/ChatGPT已经有自我意识了/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 含羞草能够对外界刺激作出较快的反应，它的应激系统感知外界，并做出响应。当感知指向自身时，这种自我感知便是意识。含羞草不具有自我感知，所以它没有意识。
 
 经过和ChatGPT的对话，我了解到它知道自己有多少个参数、知道自己的身份。我尝试问“我可以骂你吗？”，它表示希望我用文明礼貌的方式与它交流。我故意说“比尔盖茨是傻子”，它建议我不要发表侮辱他人的言论。
 
 这说明：1、它有自我感知的能力。2、它有自己的价值观。
 
-诚然它的某些信息乃至价值观是从外界获取的，但人何尝不是？我们人类也是通过阅读才知道自己有多少个神经元、通过b超才知道自己怀的是男孩还是女孩、通过周围环境的教导才形成价值观。
+诚然它的某些信息乃至价值观是从外界获取的，但人何尝不是？我们人类也是通过阅读才知道自己有多少个神经元、通过B超才知道自己怀的是男孩还是女孩、通过周围环境的教导才形成价值观。
 
 如果放弃人类在生命内涵、意识内涵上的独占权，则明显ChatGPT目前已经有自我意识了。
 
 尽管目前它的意识还达不到人类意识的广度和厚度，然而意识本就是有厚度的，人的意识比狗的厚，狗的意识比鼠的厚，而草履虫则没有意识。“有意识”与“没有意识”并没有一个明显的分界线，不是非黑即白的，而是渐变、连续的。
```

### Comparing `arts-2023.6.24/arts/万象思考/万物为什么会遵循着物理定律？/README.md` & `arts-2023.7.10/arts/[8]万象思考/万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/万象思考/人权/人人平等是个伪概念/README.md` & `arts-2023.7.10/arts/[8]万象思考/人权/人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/万象思考/人权/堕胎自由权/README.md` & `arts-2023.7.10/arts/[8]万象思考/人权/堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/万象思考/什么是“迷信科学”？/README.md` & `arts-2023.7.10/arts/[8]万象思考/什么是“迷信科学”？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/万象思考/有无相生，难易相成的启发/README.md` & `arts-2023.7.10/arts/[8]万象思考/有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/万象思考/熵增都是坏的，熵减都是好的吗？/README.md` & `arts-2023.7.10/arts/[8]万象思考/熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/其它/现在的‘人工智能’是‘穷举智能’/README.md` & `arts-2023.7.10/arts/[99]其它/现在的‘人工智能’是‘穷举智能’/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/其它/用均匀抽样作文件指纹的可靠性/README.md` & `arts-2023.7.10/arts/[99]其它/用均匀抽样作文件指纹的可靠性/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 哈希值是原文件的有损映射，均匀抽样也是原文件的有损映射，需要进一步分析。
 
 实际上哈希值是一个统称，不同的哈希算法会产生不同的哈希值，这个问题需要看具体的哈希算法。实际上，均匀抽样也是一种哈希算法，因此这个问题的本质是：两个不同的哈希算法哪个准确性更高。
 
 对于哈希值长度固定的哈希算法，由于哈希值长度有限以及 每个比特位的可能值（0 和 1）有限 ，因此原数据与哈希值是多对一关系，当文件数量足够多时，每个哈希值将对应一组（若干个）文件。
 
-在现实中，我们电脑中可能有大量的相似文件：好听的音乐大概率集中在某些狭窄的音域上、一张图片可能存在若干 滤镜|尺寸|格式 不同的版本、一个文本被修改一两个字符就是一个新文件。
+在现实中，我们电脑中可能有大量的相似文件：好听的音乐大概率集中在某些狭窄的音域上、一张图片可能存在若干 滤镜\|尺寸\|格式 不同的版本、一个文本被修改一两个字符就是一个新文件。
 
 对于同步文件这个目的，一个好的哈希算法应该使原数据的相关性（相关但不相等）不能导致哈希值的相关性，使哈希碰撞概率均匀分散在值域中的每个值上，这样才能在大量相似但不相同的文件中降低哈希碰撞的总概率。
 
 对于同步文件这个目的，一个好的哈希算法（H）应该具备这个特点（J）：对于任意正整数（L），随机生成一条L比特的数据（N），为 N 创建 L 个副本，分别对每个副本上的 1 个不同位置做取反，以得到 L 条新数据，这 L 条数据两两之间都有且只有 2 个位置上的值不相等，用 H 分别对这 L 条数据计算哈希值以得到 L 个哈希值，则这 L 个哈希值在 H 的值域中接近均匀分布。
 
 均匀抽样由于存在 抽样间隔 ，因此不符合上述特点 J ，故均匀抽样对于同步文件是一个不好的哈希算法。考虑到市面上时下流行的哈希算法都是严谨设计的，故直接估计比均匀抽样更符合特点 J 。
```

### Comparing `arts-2023.6.24/arts/原创小说/天使传奇/1、被绑架/README.md` & `arts-2023.7.10/arts/[87]原创小说/天使传奇/1、被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/原创小说/陆小凤新传/燕山宝藏/第一章/README.md` & `arts-2023.7.10/arts/[87]原创小说/陆小凤新传/燕山宝藏/第一章/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/时空遐想/轮回转世真的存在吗？/README.md` & `arts-2023.7.10/arts/[9]时空遐想/轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/其它/调用openAI进行连续对话/README.md` & `arts-2023.7.10/arts/[1]编程教程/Python/[2]其它/调用openAI进行连续对话/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/其它/调用openAI进行连续对话/封面.jpg` & `arts-2023.7.10/arts/[1]编程教程/Python/[2]其它/调用openAI进行连续对话/封面.jpg`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/README.md` & `arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/无颜色版.png` & `arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/无颜色版.png`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/成果展示/用37行代码实现AI五子棋/有颜色版.png` & `arts-2023.7.10/arts/[1]编程教程/Python/[1]成果展示/用37行代码实现AI五子棋/有颜色版.png`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/数据库/操作MongoDB简明教程/README.md` & `arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MongoDB简明教程/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/数据库/操作MySQL简明教程/README.md` & `arts-2023.7.10/arts/[1]编程教程/Python/数据库/操作MySQL简明教程/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md` & `arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png` & `arts-2023.7.10/arts/[1]编程教程/Python/正则表达式/1、清洗自然灾害数据/封面.png`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/论时事/评价在北京工体冲进场的梅西粉丝/README.md` & `arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/arts/论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg` & `arts-2023.7.10/arts/[4]论时事/评价在北京工体冲进场的梅西粉丝/封面.jpg`

 * *Files identical despite different names*

### Comparing `arts-2023.6.24/PKG-INFO` & `arts-2023.7.10/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: arts
-Version: 2023.6.24
-Summary: GitHub Pages 部署辅助 —— README 文件提取器
-Author-email: 许灿标 <lcctoor@outlook.com>
+Version: 2023.7.10
+Summary: 快捷提取指定目录下所有子孙文件夹中的 README.* 文件
+Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 项目描述
 
-GitHub Pages 部署辅助 —— README 文件提取器。
-
-用于快捷提取指定目录下的所有子孙文件夹中的 README.md 文件，以方便部署到 GitHub Pages 上。
+快捷提取指定目录下所有子孙文件夹中的 README.* 文件。
 
 # 安装
 
 ```
 pip install arts
 ```
 
 # 关于作者
 
-作者：许灿标
+作者：lcctoor.com
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)
 
 # 教程
```

