# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.8.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.9.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.8.tar` & `nonebot_plugin_l4d2_server-0.5.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-27 14:50:54.855206 nonebot_plugin_l4d2_server-0.5.8/LICENSE
--rw-r--r--   0        0        0     5683 2023-06-27 14:50:54.855206 nonebot_plugin_l4d2_server-0.5.8/README.md
--rw-r--r--   0        0        0    19839 2023-06-27 14:50:54.859206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-27 14:50:54.859206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-27 14:50:54.859206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1714 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1879 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-27 14:50:54.863206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3736 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10952 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     8989 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5960 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     9675 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    15320 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1604 2023-06-27 14:50:54.867206 nonebot_plugin_l4d2_server-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-09 15:23:29.852550 nonebot_plugin_l4d2_server-0.5.9/LICENSE
+-rw-r--r--   0        0        0     5683 2023-07-09 15:23:29.852550 nonebot_plugin_l4d2_server-0.5.9/README.md
+-rw-r--r--   0        0        0    18107 2023-07-09 15:23:29.856550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-07-09 15:23:29.856550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-07-09 15:23:29.856550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     9076 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1607 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3364 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1344 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4034 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1868 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1832 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     3074 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4211 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4174 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0      665 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9493 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1091 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     4018 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1421 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7222 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3854 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1030 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    11828 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4067 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1185 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9199 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6197 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1631 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0     1243 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2149 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     9994 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8469 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14982 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1604 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.9/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/LICENSE` & `nonebot_plugin_l4d2_server-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/README.md` & `nonebot_plugin_l4d2_server-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,490 +11,497 @@
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License
 * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 from nonebot import require
-require('nonebot_plugin_apscheduler')
-require('nonebot_plugin_htmlrender')
-require('nonebot_plugin_txt2img')
-from .l4d2_web import web,webUI
 
-from typing import Tuple,Union,List
+require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_htmlrender")
+require("nonebot_plugin_txt2img")
+from .l4d2_web import web, webUI
+
+from typing import Tuple, Union, List
 from time import sleep
 import time
 
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
-from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg
+from nonebot.params import CommandArg, ArgPlainText, RegexGroup, Arg
 from nonebot import get_driver, require
 from typing import Annotated
 from nonebot.params import Keyword
 
 from .l4d2_utils.config import *
 from .l4d2_utils.utils import *
 from .l4d2_utils.command import *
-from .l4d2_image.steam import url_to_byte,url_to_byte_name
+from .l4d2_image.steam import url_to_byte, url_to_byte_name
 
 from .l4d2_data import sq_L4D2
 from .l4d2_push import *
 from .l4d2_image.vtfs import img_to_vtf
-from .l4d2_file import updown_l4d2_vpk,all_zip_to_one
+from .l4d2_file import updown_l4d2_vpk, all_zip_to_one
 from .l4d2_file.input_json import *
 from .l4d2_utils.txt_to_img import mode_txt_to_img
+
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 from nonebot.plugin import PluginMetadata
 
 driver = get_driver()
-logo ="""
-    ......                  ` .]]@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
-    ......                ,/@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
-    ......            /O@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
-    `.....           ,@^=.OOO\/\@@@@@@@@@@@@@@@@@@@@OO//@@@@@/OO\]]]OO\]
-    ``....          ,@@/=^OOOOOOOO@@@@@@@@@@@\]OOOOOOO^^=@@@@OOOOOOOOOOO
-    `.....          O@O^==OOOOOOOO@@@/.,@@@OOOOOOOOOOO\O,@@@@OOOOOOOOO@@
-    ......    ,    .@@@^=`OOOOOOOOO/  ,O@@OOOOOOOOOOOOOO.O@@@OO/[[[[[[[.
-    ......    =..,//@@@^=`OOOOOOOOO@.*=@@@OOOOOOOOOOOOOO]@@@OOO.     ,/`
-    ......    =.\O]`,@O^\=OOOO@@@@@@O`=@@@@@@@OOOOOOOO*O,OO^....[[``]./]
-    ......    ,^.oOoO@O^=,OO@@@@@OoO`\O\OO@@@@OOOOOOOOO]@@^.]]]/OOOo.,OO
-    ......     =.=OOOO@@@@/[[=/.^,/....*.=^,[O@@@@OOOO.@@OOOOOOOOO/..OOO
-    ......      \.\OO`.,....*`.=.^.......=....=@O[\@@O@@[^ ,`.=Oo*.,OOO/
-    ......       ,@,`...  ....=^/......../....=/O^....\..O]/[\O[*]/OOO. 
-    ......       ]@^.,....*..=O\^........^..*.O.\O.^..=^\..,\/\@OOO[.   
-    ......    ,,`O^.,..../.,O`//........=..=`=^.=O`O..=^..OOO*/OOO.     
-    ......   .=.=@..^...=^/O`*OO.]...o**\.,/=^...O^@^..^...OO^=`OOO`    
-    ......  `=.,O^./.*.,OO`,.,/@/.*,O`,O*/@/`....\O\^......Oo^.^,OOO.   
-    ...... .,`.o=^=^.../`...]/`***/O^/@oO@`..[[[[\/=\......O^^...=OO^   
-    ......  ^.=`O^O.*.=\],]]]/\O/\@O[=O/`        =.=O....=^O^*....OOO.  
-    ...... =../=OO^.*.=@@[[,@@@\ .. ..    ,\@@@@@] =O...`=^@`.....=OO^  
-    ...... `..^=OO^.^,@`  ^ =oO\          .O\O@\.,\@@..,^OoO......=OOO. 
-    ...... ^...=OO^.^.@^ =^*=^,O          \..Ooo^  ,@..=OOOO..*....OOO. 
-    ...... ^...=o@^.`.O@. .  ... .. ....  ^.*`.*^  =^..o@oO@*.=....OOO^ 
-    ...... ^...=oOO.*.\O   ... .......... .\   ` ,=^*.,OOOO@^.=`^..=OO\ 
-    ...... ^...*`OO.*.=O ........          ......,`*^.=OOOo@^.=^^..=OOO.
-    ...... \....*oO^..*O^ ....... @OO[[[`  ......../.,@OOOo@^..OO...OOO`
-    ...... =.....*.=`..,O`       .O.....=   ... ^.=..OOOOO=O@..=O^..OOO^
-    ...... .^...**.O@...\O^ .     \.....`   .^ /.,^.=O@OO`=O@^..OO`.=OO\
-    ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
-    ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
-    @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
-    OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
-    @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
-    """
 
-
-__version__ = "0.5.7"
+__version__ = "0.5.9"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
-    description='群内对有关求生之路的查询和操作',
-    usage=logo,
+    description="群内对有关求生之路的查询和操作",
+    usage="群内对有关求生之路的查询和操作",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 
 """相当于启动就检查数据库"""
 
+
 @up.handle()
-async def _(matcher:Matcher,event: NoticeEvent):
+async def _(matcher: Matcher, event: NoticeEvent):
     args = event.dict()
-    if args['notice_type'] != 'offline_file':
-        matcher.set_arg('txt',args)
+    if args["notice_type"] != "offline_file":
+        matcher.set_arg("txt", args)  # type: ignore
         return
-    l4_file_path = l4_config.l4_ipall[l4_config.l4_number]['location']
-    map_path = Path(l4_file_path, vpk_path)
+    l4_file_path = l4_config.l4_ipall[l4_config.l4_number]["location"]
+    map_path = Path(l4_file_path, vpk_path)  # type: ignore
     # 检查下载路径是否存在
-    if not Path(l4_file_path).exists():
+    if not Path(l4_file_path).exists():  # type: ignore
         await matcher.finish("你填写的路径不存在辣")
     if not Path(map_path).exists():
         await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
-    url:str = args['file']['url']
-    name: str = args['file']['name']
+    url: str = args["file"]["url"]
+    name: str = args["file"]["name"]
     # 如果不符合格式则忽略
-    await up.send('已收到文件，开始下载')
-    sleep(1)   # 等待一秒防止因为文件名获取出现BUG
-    vpk_files = await updown_l4d2_vpk(map_path,name,url)
+    await up.send("已收到文件，开始下载")
+    sleep(1)  # 等待一秒防止因为文件名获取出现BUG
+    vpk_files = await updown_l4d2_vpk(map_path, name, url)
     if vpk_files:
         mes = "解压成功，新增以下几个vpk文件"
-        await matcher.finish(mes_list(mes,vpk_files))
+        await matcher.finish(mes_list(mes, vpk_files))
     else:
         await matcher.finish("你可能上传了相同的文件，或者解压失败了捏")
 
-path_list:str = '请选择上传位置（输入阿拉伯数字)'
+
+path_list: str = "请选择上传位置（输入阿拉伯数字)"
 times = 0
 for one_path in l4_config.l4_ipall:
     times += 1
-    path_msg = one_path['location']
-    path_list += f'\n {str(times)} | {path_msg}'
-    
-@up.got("is_sure", prompt=path_list)    
+    path_msg = one_path["location"]
+    path_list += f"\n {str(times)} | {path_msg}"
+
+
+@up.got("is_sure", prompt=path_list)
 async def _(matcher: Matcher):
-    args = matcher.get_arg('txt')
+    args = matcher.get_arg("txt")
     l4_file = l4_config.l4_ipall
     if not args:
-        await matcher.finish('获取文件出错辣，再试一次吧')
+        await matcher.finish("获取文件出错辣，再试一次吧")
 
-    is_sure = str(matcher.get_arg('is_sure')).strip()
+    is_sure = str(matcher.get_arg("is_sure")).strip()
     if not is_sure.isdigit():
-        await matcher.finish('已取消上传')
-    
-    file_path:str = ''
+        await matcher.finish("已取消上传")
+
+    file_path: str = ""
     for one_server in l4_file:
-        if one_server['id_rank'] == is_sure:
-            file_path = one_server['location']
+        if one_server["id_rank"] == is_sure:
+            file_path = one_server["location"]
     if not file_path:
         await matcher.finish("没有这个序号拉baka")
 
-
     map_path = Path(file_path, vpk_path)
 
     # 检查下载路径是否存在
     if not Path(file_path).exists():
         await matcher.finish("你填写的路径不存在辣")
     if not map_path.exists():
         await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
 
-    url = args['file']['url']
-    name = args['file']['name']
+    url = args["file"]["url"]
+    name = args["file"]["name"]
     # 如果不符合格式则忽略
-    if not name.endswith(file_format):
+    if not name.endswith(file_format):  # type: ignore
         return
 
-    await matcher.send('已收到文件，开始下载')
-    sleep(1)   # 等待一秒防止因为文件名获取出现BUG
-    vpk_files = await updown_l4d2_vpk(map_path, name, url)
+    await matcher.send("已收到文件，开始下载")
+    sleep(1)  # 等待一秒防止因为文件名获取出现BUG
+    vpk_files = await updown_l4d2_vpk(map_path, name, url)  # type: ignore
 
     if vpk_files:
-        logger.info('检查到新增文件')
+        logger.info("检查到新增文件")
         mes = "解压成功，新增以下几个vpk文件"
     elif vpk_files is None:
-        await matcher.finish('文件错误')
+        await matcher.finish("文件错误")
     else:
         mes = "你可能上传了相同的文件，或者解压失败了捏"
 
     await matcher.finish(mes_list(mes, vpk_files))
 
-    
+
 @find_vpk.handle()
-async def _(bot:Bot,event: MessageEvent,matcher: Matcher):
-    name_vpk = []
-    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],vpk_path)
-    name_vpk = get_vpk(name_vpk,map_path)
+async def _(bot: Bot, event: MessageEvent, matcher: Matcher):
+    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]["location"], vpk_path)
+    name_vpk = get_vpk(map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
-    msg = ''
-    msg = mes_list(msg,name_vpk).replace(" ","")
-    
-    await matcher.finish(mode_txt_to_img(mes,msg))
+    msg = ""
+    msg = mes_list(msg, name_vpk).replace(" ", "")
+
+    await matcher.finish(mode_txt_to_img(mes, msg))
+
 
 @del_vpk.handle()
-async def _(matcher:Matcher,args:Message = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     num1 = args.extract_plain_text()
     if num1:
-        matcher.set_arg("num",args)
+        matcher.set_arg("num", args)
+
+
+@del_vpk.got("num", prompt="你要删除第几个序号的地图(阿拉伯数字)")
+async def _(matcher: Matcher, tag: str = ArgPlainText("num")):
+    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]["location"], vpk_path)
+    vpk_name = del_map(int(tag), map_path)
+    await matcher.finish("已删除地图：" + vpk_name)
+
 
-@del_vpk.got("num",prompt="你要删除第几个序号的地图(阿拉伯数字)")
-async def _(matcher: Matcher,tag:int = ArgPlainText("num")):
-    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],vpk_path)
-    vpk_name = del_map(tag,map_path)
-    await matcher.finish('已删除地图：' + vpk_name)
-    
 @rename_vpk.handle()
-async def _(matcher:Matcher,matched: Tuple[int,str, str] = RegexGroup(),):
-    num,useless,rename = matched
-    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],vpk_path)
-    logger.info('检查是否名字是.vpk后缀')
-    if not rename.endswith('.vpk'):
-        rename = rename + '.vpk'
-    logger.info('尝试改名')
+async def _(
+    matcher: Matcher,
+    matched: Tuple[int, str, str] = RegexGroup(),
+):
+    num, useless, rename = matched
+    map_path = Path(l4_config.l4_ipall[l4_config.l4_number]["location"], vpk_path)
+    logger.info("检查是否名字是.vpk后缀")
+    if not rename.endswith(".vpk"):
+        rename = rename + ".vpk"
+    logger.info("尝试改名")
     try:
-        map_name = rename_map(num,rename,map_path)
+        map_name = rename_map(num, rename, map_path)
         if map_name:
-            await matcher.finish('改名成功\n原名:'+ map_name +'\n新名称:' + rename)
+            await matcher.finish("改名成功\n原名:" + map_name + "\n新名称:" + rename)
     except ValueError:
-        await matcher.finish('参数错误,请输入格式如【求生地图 5 改名 map.vpk】,或者输入【求生地图】获取全部名称')
-        
+        await matcher.finish("参数错误,请输入格式如【求生地图 5 改名 map.vpk】,或者输入【求生地图】获取全部名称")
+
+
 @anne_player.handle()
-async def _(matcher:Matcher,event:MessageEvent,args:Message = CommandArg()):
+async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
     name = args.extract_plain_text()
     name = name.strip()
     at = await get_message_at(event.json())
     usr_id = at_to_usrid(at)
-    if usr_id == None:
+    if not usr_id:
         usr_id = event.user_id
     # 没有参数则从db里找数据
-    msg = await search_anne(name,usr_id)
-    if type(msg)==str:
+    msg = await search_anne(name, str(usr_id))
+    if isinstance(msg, str):
         await matcher.finish(msg)
-    else:
-        await matcher.finish(MessageSegment.image(msg)) 
-    
+    elif isinstance(msg, bytes):
+        await matcher.finish(MessageSegment.image(msg))
+
+
 @anne_bind.handle()
-async def _(matcher:Matcher,event:MessageEvent,args:Message = CommandArg()):
+async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
     tag = args.extract_plain_text()
     tag = tag.strip()
-    if tag=="" or tag.isspace():
+    if tag == "" or tag.isspace():
         await matcher.finish("虚空绑定?")
     usr_id = str(event.user_id)
     nickname = event.sender.card or event.sender.nickname
-    msg = await bind_steam(usr_id,tag,nickname)
+    if not nickname:
+        nickname = "宁宁"
+    msg = await bind_steam(usr_id, tag, nickname)
     await matcher.finish(msg)
 
+
 @del_bind.handle()
-async def _(matcher:Matcher,event:MessageEvent):
+async def _(matcher: Matcher, event: MessageEvent):
     usr_id = event.user_id
-    await matcher.finish(name_exist(usr_id))
+    await matcher.finish(name_exist(str(usr_id)))
+
 
 @rcon_to_server.handle()
-async def _(matcher:Matcher,args:Message = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
-        matcher.set_arg("command",args)
+        matcher.set_arg("command", args)
+
 
-@rcon_to_server.got("command",prompt="请输入向服务器发送的指令")
-async def _(matcher:Matcher,tag:str = ArgPlainText("command")):
+@rcon_to_server.got("command", prompt="请输入向服务器发送的指令")
+async def _(matcher: Matcher, tag: str = ArgPlainText("command")):
     tag = tag.strip()
     msg = await command_server(tag)
     try:
-        await matcher.finish(mode_txt_to_img('服务器返回',msg))
+        await matcher.finish(mode_txt_to_img("服务器返回", msg))
     except:
-        await matcher.finish(msg,reply_message = True)
-        
+        await matcher.finish(msg, reply_message=True)
+
 
-        
 @check_path.handle()
-async def _(matcher:Matcher,args:Message = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
-    if msg.startswith('切换'):
-        msg_number = int(''.join(msg.replace('切换', ' ').split()))
+    if msg.startswith("切换"):
+        msg_number = int("".join(msg.replace("切换", " ").split()))
         if msg_number > len(l4_config.l4_ipall) or msg_number < 0:
-            await matcher.send('没有这个序号的路径呐')
+            await matcher.send("没有这个序号的路径呐")
         else:
             l4_config.l4_number = msg_number - 1
-            now_path = l4_config.l4_ipall[l4_config.l4_number]['location']
-            await matcher.send(f'已经切换路径为\n{str(l4_config.l4_number+1)}、{now_path}')
+            now_path = l4_config.l4_ipall[l4_config.l4_number]["location"]
+            await matcher.send(f"已经切换路径为\n{str(l4_config.l4_number+1)}、{now_path}")
             config_manager.save()
-    else: 
-        now_path = l4_config.l4_ipall[l4_config.l4_number]['location']
-        await matcher.send(f'当前的路径为\n{str(l4_config.l4_number+1)}、{now_path}')
-        
-        
+    else:
+        now_path = l4_config.l4_ipall[l4_config.l4_number]["location"]
+        await matcher.send(f"当前的路径为\n{str(l4_config.l4_number+1)}、{now_path}")
+
+
 @queries_comm.handle()
-async def _(matcher:Matcher,event:MessageEvent,keyword:str = Keyword()):
+async def _(matcher: Matcher, event: MessageEvent, keyword: str = Keyword()):
     msg = event.get_plaintext()
- 
+
     if not msg:
-        await matcher.finish('ip格式如中括号内【127.0.0.1】【114.51.49.19:1810】')
-    ip = msg.split(keyword)[-1].split('\r')[0].split('\n')[0].split(' ')
-    for one_msg in ip:
-        if one_msg and one_msg[-1].isdigit():
+        await matcher.finish("ip格式如中括号内【127.0.0.1】【114.51.49.19:1810】")
+    ip = msg.split(keyword)[-1].split("\r")[0].split("\n")[0].split(" ")
+    one_msg = None
+    for one in ip:
+        if one and one[-1].isdigit():
+            one_msg = one
             break
     if not one_msg:
         await matcher.finish()
     ip_list = split_maohao(one_msg)
     msg = await queries_server(ip_list)
-    await str_to_picstr(msg,matcher,keyword)
-    
+    await str_to_picstr(msg, matcher, keyword)
+
 
 @add_queries.handle()
-async def _(matcher:Matcher,event:GroupMessageEvent,args:Message = CommandArg()):
+async def _(matcher: Matcher, event: GroupMessageEvent, args: Message = CommandArg()):
     msg = args.extract_plain_text()
-    if len(msg)==0:
-        await matcher.finish('请在该指令后加入参数，例如【114.51.49.19:1810】')
-    [host,port] = split_maohao(msg)
+    if len(msg) == 0:
+        await matcher.finish("请在该指令后加入参数，例如【114.51.49.19:1810】")
+    [host, port] = split_maohao(msg)
     group_id = event.group_id
-    msg = await add_ip(group_id,host,port)
+    msg = await add_ip(group_id, host, port)
     await matcher.finish(msg)
 
+
 @del_queries.handle()
-async def _(event:GroupMessageEvent,matcher:Matcher,args:Message = CommandArg()):
+async def _(event: GroupMessageEvent, matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if not msg.isdigit():
-        await matcher.finish('请输入正确的序号数字')
+        await matcher.finish("请输入正确的序号数字")
     group_id = event.group_id
-    msg = await del_ip(group_id,msg)
+    msg = await del_ip(group_id, msg)
     await matcher.finish(msg)
-   
+
+
 @show_queries.handle()
-async def _(matcher:Matcher,event:GroupMessageEvent):
+async def _(matcher: Matcher, event: GroupMessageEvent):
     group_id = event.group_id
     msg = await show_ip(group_id)
     if not msg:
         await matcher.finish("当前没有启动的服务器捏")
-    if type(msg) == str:
+    if isinstance(msg, str):
         await matcher.finish(msg)
     else:
         await matcher.finish(MessageSegment.image(msg))
 
+
 @join_server.handle()
-async def _(args:Message = CommandArg()):
+async def _(args: Message = CommandArg()):
     msg = args.extract_plain_text()
     url = await get_number_url(msg)
     await join_server.finish(url)
-    
-        
+
+
 @up_workshop.handle()
-async def _(matcher:Matcher,args:Message = CommandArg()):
+async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
-        matcher.set_arg("ip",args)
-    
-@up_workshop.got("ip",prompt="请输入创意工坊网址或者物品id")
-async def _(matcher:Matcher,state:T_State,tag:str = ArgPlainText("ip")):
+        matcher.set_arg("ip", args)
+
+
+@up_workshop.got("ip", prompt="请输入创意工坊网址或者物品id")
+async def _(matcher: Matcher, state: T_State, tag: str = ArgPlainText("ip")):
     msg = await workshop_msg(tag)
     if not msg:
-        await matcher.finish('没有这个物品捏')
-    elif type(msg) == dict:
-        pic = await url_to_byte(msg['图片地址'])
-        message = ''
-        for item,value in msg.items():
-            if item in ['图片地址','下载地址','细节']:
+        await matcher.finish("没有这个物品捏")
+    elif isinstance(msg, dict):
+        pic = await url_to_byte(msg["图片地址"])
+        if not pic:
+            return
+        message = ""
+        for item, value in msg.items():
+            if item in ["图片地址", "下载地址", "细节"]:
                 continue
-            message += item + ':' + value + '\n'
-        state['dic'] = msg
+            message += item + ":" + value + "\n"
+        state["dic"] = msg
         await up_workshop.send(MessageSegment.image(pic) + Message(message))
-    elif type(msg) == list:
+    elif isinstance(msg, list):
         lenge = len(msg)
-        pic = await url_to_byte(msg[0]['图片地址'])
-        message = f'有{lenge}个文件\n'
+        pic = await url_to_byte(msg[0]["图片地址"])
+        message = f"有{lenge}个文件\n"
+        ones = []
         for one in msg:
-            ones = []
-            for item,value in one.items():
-                if item in ['图片地址','下载地址','细节']:
+            for item, value in one.items():
+                if item in ["图片地址", "下载地址", "细节"]:
                     continue
-                message += item + ':' + value + '\n'
+                message += item + ":" + value + "\n"
             ones.append(one)
-        state['dic'] = ones
-    
-@up_workshop.got("is_sure",prompt='如果需要上传，请发送 "yes"')    
-async def _(matcher: Matcher,bot:Bot,event:GroupMessageEvent,state:T_State):
+        state["dic"] = ones
+
+
+@up_workshop.got("is_sure", prompt='如果需要上传，请发送 "yes"')
+async def _(matcher: Matcher, bot: Bot, event: GroupMessageEvent, state: T_State):
     is_sure = str(state["is_sure"])
-    if is_sure == 'yes':
-        data_dict:Union[dict,List[dict]] = state['dic']
-        if type(data_dict) == dict:
-            logger.info('开始上传')
-            data_file = await url_to_byte(data_dict['下载地址'])
-            file_name = data_dict['名字']+ '.vpk'
-            await matcher.send('获取地址成功，尝试上传')
+    if is_sure == "yes":
+        data_dict: Union[dict, List[dict]] = state["dic"]
+        logger.info("开始上传")
+        if isinstance(data_dict, dict):
+            data_file = await url_to_byte(data_dict["下载地址"])
+            if not data_file:
+                return
+            file_name = data_dict["名字"] + ".vpk"
+            await matcher.send("获取地址成功，尝试上传")
             await upload_file(bot, event, data_file, file_name)
         else:
-            logger.info('开始上传')
+            data_file_list = []
             for data_one in data_dict:
-                data_file = await url_to_byte(data_one['下载地址'])
-                await all_zip_to_one
-            file_name = data_one['名字']+ '.vpk'
-            await upload_file(bot, event, data_file, file_name)
+                data_file = await url_to_byte(data_one["下载地址"])
+                data_file_list.append(data_file)
+                if not data_file:
+                    return
+                file_name = data_one["名字"] + ".vpk"
+                await all_zip_to_one(data_file_list)
+                await upload_file(bot, event, data_file, file_name)
     else:
-        await matcher.finish('已取消上传')
-    
+        await matcher.finish("已取消上传")
 
 
 # @updata.handle()
 # async def _(matcher:Matcher,args:Message = CommandArg()):
 #     """更新"""
 #     msg = args.extract_plain_text()
 #     if not msg:
 #         load_josn()
 #         reload_ip()
 #         await matcher.finish('已更新缓存数据')
 #     else:
 #         message = await write_json(msg)
 #         await matcher.finish(message)
-  
 
-            
+
 @vtf_make.handle()
-async def _(matcher:Matcher,state:T_State,args:Message = CommandArg()):
-    msg:str = args.extract_plain_text()
-    if msg not in ['拉伸','填充','覆盖','']:
-        await matcher.finish('错误的图片处理方式')
-    if msg == '':
-        msg = '拉伸'
-    state['way'] = msg
-    logger.info('方式',msg)
-    
-@vtf_make.got("image",prompt="请发送喷漆图片")
-async def _(bot:Bot,event:MessageEvent,state:T_State,tag = Arg("image")):
-    pic_msg:MessageSegment =  state["image"][0]
+async def _(matcher: Matcher, state: T_State, args: Message = CommandArg()):
+    msg: str = args.extract_plain_text()
+    if msg not in ["拉伸", "填充", "覆盖", ""]:
+        await matcher.finish("错误的图片处理方式")
+    if msg == "":
+        msg = "拉伸"
+    state["way"] = msg
+    logger.info("方式", msg)
+
+
+@vtf_make.got("image", prompt="请发送喷漆图片")
+async def _(bot: Bot, event: MessageEvent, state: T_State, tag=Arg("image")):
+    pic_msg: MessageSegment = state["image"][0]
     pic_url = pic_msg.data["url"]
     logger.info(pic_url)
     logger.info(type(pic_url))
-    tag = state['way']
+    tag = state["way"]
     pic_bytes = await url_to_byte(pic_url)
-    img_io = await img_to_vtf(pic_bytes,tag)
+    if not pic_bytes:
+        return
+    img_io = await img_to_vtf(pic_bytes, tag)
     img_bytes = img_io.getbuffer()
     usr_id = event.user_id
-    file_name:str = str(usr_id) + '.vtf'
+    file_name: str = str(usr_id) + ".vtf"
     await upload_file(bot, event, img_bytes, file_name)
 
 
-
 @smx_file.handle()
-async def _(matcher:Matcher,):
-    smx_path = Path(l4_config.l4_ipall[l4_config.l4_number]['location'],"left4dead2/addons/sourcemod/plugins")
-    smx_list = []
-    name_smx = get_vpk(smx_list,smx_path,file_=".smx")
+async def _(
+    matcher: Matcher,
+):
+    smx_path = Path(
+        l4_config.l4_ipall[l4_config.l4_number]["location"],
+        "left4dead2/addons/sourcemod/plugins",
+    )
+    name_smx = get_vpk(smx_path, file_=".smx")
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下smx文件"
-    msg = ''
-    msg = mes_list(msg,name_smx).replace(" ","")
-    await matcher.finish(mode_txt_to_img(mes,msg))
-    
+    msg = ""
+    msg = mes_list(msg, name_smx).replace(" ", "")
+    await matcher.finish(mode_txt_to_img(mes, msg))
+
+
 # @search_api.handle()
 # async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
 #     msg:str = args.extract_plain_text()
 #     # if msg.startswith('代码'):
 #         # 建图代码返回三方图信息
 #     data = await seach_map(msg,l4_config.l4_master[0],l4_config.l4_key)
 #     # else:
 #     if type(data) == str:
 #         await matcher.finish(data)
 #     else:
 #         state['maps'] = data
 #         await matcher.send(await map_dict_to_str(data))
-        
-@search_api.got("is_sure",prompt='如果需要上传，请发送 "yes"')    
-async def _(matcher:Matcher,bot:Bot,event:GroupMessageEvent,state:T_State):
+
+
+@search_api.got("is_sure", prompt='如果需要上传，请发送 "yes"')
+async def _(matcher: Matcher, bot: Bot, event: GroupMessageEvent, state: T_State):
     is_sure = str(state["is_sure"])
-    if is_sure == 'yes':
-        data_dict:dict = state['maps'][0]
-        if type(data_dict) == dict:
-            logger.info('开始上传')
+    if is_sure == "yes":
+        data_dict: dict = state["maps"][0]
+        if isinstance(data_dict, dict):
+            logger.info("开始上传")
             if l4_config.l4_only:
-                data_file,file_name = await url_to_byte_name(data_dict['url'],'htp')
+                reu = await url_to_byte_name(data_dict["url"], "htp")
             else:
-                data_file,file_name = await url_to_byte_name(data_dict['url'])
+                reu = await url_to_byte_name(data_dict["url"])
+            if not reu:
+                return
+            data_file, file_name = reu
             if data_file:
-                await matcher.send('获取地址成功，尝试上传')
+                await matcher.send("获取地址成功，尝试上传")
                 await upload_file(bot, event, data_file, file_name)
             else:
-                await search_api.send('出错了，原因是下载链接不存在')
+                await search_api.send("出错了，原因是下载链接不存在")
         else:
-            logger.info('开始上传')
-            for data_one in data_dict:
-                data_file,file_name = await url_to_byte_name(data_one['url'])
-                await all_zip_to_one
-                await upload_file(bot, event, data_file, file_name)
+            ...
+            # logger.info("开始上传")
+            # for data_one in data_dict:
+            #     reu = await url_to_byte_name(data_one["url"])
+            #     if not reu:
+            #         return
+            #     data_file, file_name = reu
+            #     await all_zip_to_one()
+            #     await upload_file(bot, event, data_file, file_name)
     else:
-        await matcher.finish('已取消上传')
-        
+        await matcher.finish("已取消上传")
+
+
 # @reload_ip.handle()
 # async def _(matcher:Matcher):
 #     global matchers
 #     await matcher.send('正在重载ip，可能需要一点时间')
 #     for _, l4_matchers in matchers.items():
 #         for l4_matcher in l4_matchers:
 #             l4_matcher.destroy()
 #     await get_des_ip()
 #     await matcher.finish('已重载ip')
-    
+
 
 @driver.on_shutdown
 async def close_db():
     """关闭数据库"""
     sq_L4D2._close()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,252 +1,261 @@
-
 from nonebot.log import logger
 
 import pandas as pd
 from typing import List
 
 from .analysis import df_to_guoguanlv
 from ..l4d2_utils.seach import *
 from ..l4d2_data.players import L4D2Player
 from ..l4d2_image import out_png
+
 # from .anne_telecom import ANNE_API
 
 
 s = L4D2Player()
 
-    
-async def anne_html(name:str):
-    """搜索里提取玩家信息，返回列表字典""" 
+
+async def anne_html(name: str):
+    """搜索里提取玩家信息，返回列表字典"""
     data_title = anne_search(name)
+    if not data_title:
+        return
     data = data_title[0]
     title = data_title[1]
-    if len(data) ==0 or data[0] == "No Player found.":
-        return {}
-    data_list:list = []
+    if len(data) == 0 or data[0] == "No Player found.":
+        return []
+    data_list: list = []
     logger.info(data)
     for i in data:
-        i:BeautifulSoup
+        i: BeautifulSoup
         try:
-            Rank = i.find('td', {'data-title': 'Rank:'}).text.strip()
-            player = i.find('td', {'data-title': 'Player:'}).text.strip()
-            points = i.find('td', {'data-title': 'Points:'}).text.strip()
+            Rank = i.find("td", {"data-title": "Rank:"}).text.strip()  # type: ignore
+            player = i.find("td", {"data-title": "Player:"}).text.strip()  # type: ignore
+            points = i.find("td", {"data-title": "Points:"}).text.strip()  # type: ignore
             # country = i.find('img')['alt']
-            playtime = i.find('td', {'data-title': 'Playtime:'}).text.strip()
-            last_online = i.find('td', {'data-title': 'Last Online:'}).text.strip()
+            playtime = i.find("td", {"data-title": "Playtime:"}).text.strip()  # type: ignore
+            last_online = i.find("td", {"data-title": "Last Online:"}).text.strip()  # type: ignore
         except AttributeError:
-            Rank = i.find('td', {'data-title': '排名:'}).text.strip()
-            player = i.find('td', {'data-title': '玩家:'}).text.strip()
-            points = i.find('td', {'data-title': '分数:'}).text.strip()
-            playtime = i.find('td', {'data-title': '游玩时间:'}).text.strip()
-            last_online = i.find('td', {'data-title': '最后上线时间:'}).text.strip()
-        onclick = i['onclick']
-        steamid = onclick.split('=')[2].strip("'")
-        play_json ={
-            title[0]:Rank,
-            title[1]:player,
-            title[2]:points,
+            Rank = i.find("td", {"data-title": "排名:"}).text.strip()  # type: ignore
+            player = i.find("td", {"data-title": "玩家:"}).text.strip()  # type: ignore
+            points = i.find("td", {"data-title": "分数:"}).text.strip()  # type: ignore
+            playtime = i.find("td", {"data-title": "游玩时间:"}).text.strip()  # type: ignore
+            last_online = i.find("td", {"data-title": "最后上线时间:"}).text.strip()  # type: ignore
+        onclick = i["onclick"]
+        steamid = onclick.split("=")[2].strip("'")  # type: ignore
+        play_json = {
+            title[0]: Rank,
+            title[1]: player,
+            title[2]: points,
             # title[3]:country,
-            title[3]:playtime,
-            title[4]:last_online,
-            title[5]:steamid
+            title[3]: playtime,
+            title[4]: last_online,
+            title[5]: steamid,
         }
         data_list.append(play_json)
     logger.info("搜寻数据")
     return data_list
 
-def anne_html_msg(data_list:list):
+
+def anne_html_msg(data_list: list):
     """从搜索结果的字典列表中，返回发送信息"""
-    mes = '搜索到以下玩家信息'
+    mes = "搜索到以下玩家信息"
     ns = 0
-    
+
     for one in data_list:
-        one:dict
+        one: dict
         ns += 1
         x = 6
 
         titles = list(one.keys())
         for i in range(x):
-            mes += '\n' + titles[i] + ':' + str(one[titles[i]])
-        mes += '\n--------------------'
-        if ns>4:
+            mes += "\n" + titles[i] + ":" + str(one[titles[i]])
+        mes += "\n--------------------"
+        if ns > 4:
             break
     return mes
 
 
-  
-   
-async def write_player(id,msg:str,nickname:str):
+async def write_player(id, msg: str, nickname: str):
     """绑定用户"""
     # 判断是steam
-    print(msg)
-    if msg.startswith('STEAM'):
+    if msg.startswith("STEAM"):
         # try:
         data_tuple = s._query_player_qq(id)
         if data_tuple != None:
-            qq , nicknam , steamid = data_tuple
+            qq, nicknam, steamid = data_tuple
         else:
             nicknam = None
-        await s._add_player_all(id , nicknam , msg)
+        await s._add_player_all(id, nicknam, msg)
         # except TypeError:
-            # await s._add_player_steamid(id , msg)
-        mes = '绑定成功喵~\nQQ:' + nickname +'\n' + 'steamid:'+msg
+        # await s._add_player_steamid(id , msg)
+        mes = "绑定成功喵~\nQQ:" + nickname + "\n" + "steamid:" + msg
         return mes
     else:
         # try:
         data_tuple = s._query_player_qq(id)
         if data_tuple != None:
-            id , nicknam , steamid = data_tuple
+            id, nicknam, steamid = data_tuple
         else:
             steamid = None
-        await s._add_player_all(id , msg , steamid)
+        await s._add_player_all(id, msg, steamid)
         # except TypeError:
-        #     await s._add_player_nickname(id , msg ) 
-        mes = '绑定成功喵~\nQQ:' + nickname +'\n' + 'steam昵称:'+msg
+        #     await s._add_player_nickname(id , msg )
+        mes = "绑定成功喵~\nQQ:" + nickname + "\n" + "steam昵称:" + msg
         return mes
 
-        
 
-        
-def del_player(id:str):
+def del_player(id: str):
     """删除绑定信息,返回消息"""
     if not s._query_player_qq(id):
-        return '你还没有绑定过，请使用[求生绑定+昵称/steamid]'
+        return "你还没有绑定过，请使用[求生绑定+昵称/steamid]"
     if s._delete_player:
-        return '删除成功喵~'
-        
+        return "删除成功喵~"
+
 
-    
-async def id_to_mes(name:str):
+async def id_to_mes(name: str):
     """根据name从数据库,返回steamid、或者空白"""
-    data_tuple = await s.search_data(None,name,None)
-    print(data_tuple)
+    data_tuple = await s.search_data(None, name, None)
     if data_tuple:
         steamid = data_tuple[2]
         return steamid
     return None
-    
 
-def anne_rank_dict(name:str):
+
+def anne_rank_dict(name: str):
     """用steamid,查详情,输出字典"""
     data_dict = {}
-    url =f'https://sb.trygek.com/l4d_stats/ranking/player.php?steamid={name}'
+    url = f"https://sb.trygek.com/l4d_stats/ranking/player.php?steamid={name}"
     headers = {
-        'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
     }
-    data = httpx.get(url=url,headers=headers,timeout=5)
+    data = httpx.get(url=url, headers=headers, timeout=5)
     if data.status_code != 200:
         return [f"查询错误，状态码{data.status_code}"]
-    data = data.content.decode('utf-8')
-    data = BeautifulSoup(data, 'html.parser')
-    detail = data.find_all('table')
+    data = data.content.decode("utf-8")
+    data = BeautifulSoup(data, "html.parser")
+    detail = data.find_all("table")
     n = 0
+    data_list: List[dict] = []
     while n < 2:
-        data_list:List[dict] = []
         detail2 = detail[n]
-        tr = detail2.find_all('tr')
+        tr = detail2.find_all("tr")
         for i in tr:
-            title = i.find('td', {'class': 'w-50'})
-            value = title.find_next_sibling('td')
-            new_dict = {title.text:value.text}
+            title = i.find("td", {"class": "w-50"})
+            value = title.find_next_sibling("td")
+            new_dict = {title.text: value.text}
             data_dict.update(new_dict)
         data_list.append(data_dict)
         n += 1
     # 获取头像
-    element:str = data.find_all(attrs={"style": "cursor:pointer"})[0].get("onclick")
+    element: str = data.find_all(attrs={"style": "cursor:pointer"})[0].get("onclick")
     player_url = element.split("'")[1]
-    data_list[0].update({"个人资料":player_url})
+    data_list[0].update({"个人资料": player_url})
     # 获取一言
-    message = data.select("html body div.content.text-center.text-md-left div.container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.justify-content-center.text-center span")
+    message = data.select(
+        "html body div.content.text-center.text-md-left div.container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.justify-content-center.text-center span"
+    )
     msg_list = []
     for i in message:
         msg_list.append(i.text)
-    data_list[0].update({"一言":msg_list})
+    data_list[0].update({"一言": msg_list})
     return data_list
 
+
 def anne_rank_dict_msg(data_list):
     """字典转msg"""
-    msg = ''
+    msg = ""
     for data_dict in data_list:
-        mes = ''
+        mes = ""
         for i in data_dict:
-            mes +='\n'+ i + data_dict[i]
-        mes += '\n--------------------'
+            mes += "\n" + i + data_dict[i]
+        mes += "\n--------------------"
         msg += mes
     return msg
 
 
-async def anne_messgae(name:str,usr_id:str):
+async def anne_message(name: str, usr_id: str):
     """获取anne信息可输出信息"""
     if name:
         logger.info("关键词查询" + name)
-        if not name.startswith('STEAM'):
+        if not name.startswith("STEAM"):
             steamid = await id_to_mes(name)
             if not steamid:
                 logger.info("没有找到qq，使用默认头像")
                 message = await anne_html(name)
+                if not message:
+                    return
                 usr_id = "1145149191810"
                 if len(message) == 0:
-                    return '没有叫这个名字的...\n'
+                    return "没有叫这个名字的...\n"
                 if len(message) > 1:
                     return anne_html_msg(message)
-                name = message[0]['steamid']
+                name = message[0]["steamid"]
             else:
                 name = steamid
+
         # steamid
         msg = anne_rank_dict(name)[0]
-        if type(msg) == dict:
+        if isinstance(msg, dict):
             msg.update(await df_to_guoguanlv(await anne_map_msg(name)))
-            logger.info('使用图片')
-            msg = await out_png(usr_id,msg)
+            logger.info("使用图片")
+            msg = await out_png(usr_id, msg)
         return msg
     else:
         """
         1、qq>数据>没有数据，返回
         2、qq>数据>steamid>查询
         3、qq>数据>昵称>查询
         """
         logger.info("qq信息查询")
         data_tuple = s._query_player_qq(usr_id)
         logger.info(data_tuple)
-        if data_tuple== None:
+        if not data_tuple:
             return f"没有绑定信息...请使用【求生绑定 xxx】\n"
         # 只有名字，先查询数据在判断
         elif data_tuple[2]:
             name = data_tuple[2]
         elif data_tuple[1]:
-            name = await id_to_mes(data_tuple[1])
+            name = await id_to_mes(data_tuple[1])  # type: ignore
             logger.info(name)
             if not name:
                 message = await anne_html(data_tuple[1])
+                if not message:
+                    return
                 usr_id = "1145149191810"
                 if len(message) == 0:
-                    return '没有叫这个名字的...\n'
+                    return "没有叫这个名字的...\n"
                 if len(message) > 1:
                     return anne_html_msg(message)
-                name = message[0]['steamid']
+                name = message[0]["steamid"]
+
         # name是steamid
         msg = anne_rank_dict(name)[0]
-        if type(msg) == dict:
+        if isinstance(msg, dict):
             msg.update(await df_to_guoguanlv(await anne_map_msg(name)))
-            logger.info('使用图片')
-            msg = await out_png(usr_id,msg)
+            logger.info("使用图片")
+            msg = await out_png(usr_id, msg)
         return msg
-    
-async def anne_map_msg(steamid:str):
+
+
+async def anne_map_msg(steamid: str):
     """steamid->地图信息"""
     url = f"https://sb.trygek.com/l4d_stats/ranking/timedmaps.php?steamid={steamid}"
     headers = {
-        'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
     }
-    data = httpx.get(url,headers=headers,timeout=5).content.decode('utf-8')
-    soup = BeautifulSoup(data, 'html.parser')
+    data = httpx.get(url, headers=headers, timeout=5).content.decode("utf-8")
+    soup = BeautifulSoup(data, "html.parser")
     data_list = []
-    cards = soup.select('div.card.rounded-0')
+    cards = soup.select("div.card.rounded-0")
     for card in cards:
-        tbodies = card.select('tbody')
+        tbodies = card.select("tbody")
         for tbody in tbodies:
-            rows = [td.text.strip() for td in tbody.find_all('td')]
+            rows = [td.text.strip() for td in tbody.find_all("td")]
             for i in range(0, len(rows), 9):
-                row = rows[i:i+9]
+                row = rows[i : i + 9]
                 data_list.append(row)
-    df = pd.DataFrame(data_list, columns=['游戏模式', '地图', '难度', '完成时间', '特感数量', '刷新间隔', 'B数使用', '刷特模式', 'Anne版本'])
-    return df
+    df = pd.DataFrame(
+        data_list,
+        columns=["游戏模式", "地图", "难度", "完成时间", "特感数量", "刷新间隔", "B数使用", "刷特模式", "Anne版本"],
+    )
+    return df
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-from .startand import SAVE_MAP,NUMBER_MAP
+from .startand import SAVE_MAP, NUMBER_MAP
 import pandas as pd
 
-async def df_to_guoguanlv(df:pd.DataFrame):
+
+async def df_to_guoguanlv(df: pd.DataFrame):
     """分析救援关过图率"""
-    data = df[df['游戏模式'] == 'AnneHappy药役']
-    other = df[df['游戏模式'].isin(['牛牛冲刺', '单人装逼'])]
-    all_map = len(data['地图'])
-    other_map = len(other['地图'])
+    data = df[df["游戏模式"] == "AnneHappy药役"]
+    other = df[df["游戏模式"].isin(["牛牛冲刺", "单人装逼"])]
+    all_map = len(data["地图"])
+    other_map = len(other["地图"])
     resen = 0
     last_maps = {}
     for m in SAVE_MAP:
-        prefix = m.split('m')[0]
+        prefix = m.split("m")[0]
         if prefix in last_maps:
             last_maps[prefix] = max(last_maps[prefix], m)
         else:
             last_maps[prefix] = m
 
     map_counts = {}
 
     n = 0
     for key in last_maps:
-        count = len(data[data['地图'].str.startswith(key)])
+        count = len(data[data["地图"].str.startswith(key)])
         if count == 0:
             continue
         last_map = last_maps[key]
-        map_count = len(data[data['地图'] == last_map])
-        map_counts[key] = map_count*NUMBER_MAP[n] / count
-        quan = count/all_map
+        map_count = len(data[data["地图"] == last_map])
+        map_counts[key] = map_count * NUMBER_MAP[n] / count
+        quan = count / all_map
         resen += quan * map_counts[key]
         n += 1
 
     # result = []
     # for i in range(1, 15):
     #     key = 'c{}'.format(i)
     #     if key in map_counts:
     #         result.append('{}:{}%'.format(key, round(map_counts[key] * 100)))
-            
+
     # print(result)
     # result = '救援图过关率: {:.2%}'.format(resen)
-    
+
     # 加上特殊关卡
     try:
         resen += other_map / (all_map + other_map)
-        result = {"救援关":str('{:.2%}'.format(resen))}
-    except (TypeError,KeyError):
-        result = {"救援关":"错误"}
+        result = {"救援关": str("{:.2%}".format(resen))}
+    except (TypeError, KeyError):
+        result = {"救援关": "错误"}
     except ZeroDivisionError:
-        result = {"救援关":"0.00%"}
+        result = {"救援关": "0.00%"}
     except:
-        result = {"救援关":"错误"}
-    return result
+        result = {"救援关": "错误"}
+    return result
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 from ..l4d2_utils.config import DATASQLITE
 import sqlite3
-from typing import Union,Tuple
+from typing import Union, Tuple, Optional, List
 
 
 class L4D2Player:
-    """数据库L4D2_Player表的操作""" 
+    """数据库L4D2_Player表的操作"""
+
     def __init__(self):
+
         """连接数据库"""
         self.datasqlite_path = DATASQLITE
-        self.conn = sqlite3.connect(self.datasqlite_path / 'L4D2.db')
+        self.conn = sqlite3.connect(self.datasqlite_path / "L4D2.db")
         self.c = self.conn.cursor()
-        
+
     async def _add_player_nickname(self, qq, nickname):
         """绑定昵称"""
         # try:
-        self.c.execute("INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,NULL)", (qq, nickname))
+        self.c.execute(
+            "INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,NULL)",
+            (qq, nickname),
+        )
         self.conn.commit()
         #     return True
         # except sqlite3.IntegrityError:
         #     return False
 
     async def _add_player_steamid(self, qq, steamid):
         """绑定steamid"""
-        self.c.execute("INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,NULL,?)", (qq, steamid))
+        self.c.execute(
+            "INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,NULL,?)",
+            (qq, steamid),
+        )
         self.conn.commit()
 
-              
-    async def _add_player_all(self, qq, nickname,steamid):
+    async def _add_player_all(self, qq, nickname, steamid):
         """用新数据覆盖旧数据"""
         # try:
-        self.c.execute("INSERT OR REPLACE INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,?)", (qq, nickname,steamid))
+        self.c.execute(
+            "INSERT OR REPLACE INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,?)",
+            (qq, nickname, steamid),
+        )
         self.conn.commit()
         return True
         # except sqlite3.IntegrityError:
         #     return False
-        
+
     def _delete_player(self, qq):
         """解除绑定"""
         self.c.execute(f"DELETE FROM L4d2_players WHERE qq = {qq}")
         self.conn.commit()
         return True
-        
-    def _query_player_qq(self, qq) -> Union[tuple,None]:
+
+    def _query_player_qq(self, qq) -> Union[tuple, None]:
         """通过qq获取数据"""
         self.c.execute(f"SELECT * FROM L4d2_players WHERE qq = '{qq}'")
         return self.c.fetchone()
-    
-    async def _query_player_nickname(self, nickname:str) -> Union[tuple,None]:
+
+    async def _query_player_nickname(self, nickname: str) -> Union[tuple, None]:
         """通过nickname获取数据"""
         self.c.execute(f"SELECT * FROM L4d2_players WHERE nickname = '{nickname}'")
         return self.c.fetchone()
 
-    async def _query_player_steamid(self, steamid:str):
+    async def _query_player_steamid(self, steamid: str):
         """通过steamid获取数据"""
         self.c.execute(f"SELECT * FROM L4d2_players WHERE steamid = '{steamid}'")
         data_tuple = self.c.fetchone()
         return data_tuple
-    
-    async def search_data(self, qq, nickname, steamid) -> Union[tuple,None]:
+
+    async def search_data(
+        self, qq: Optional[str], nickname: Optional[str], steamid: Optional[str]
+    ) -> Union[tuple, None]:
         """
         输入元组查询，优先qq其次steamid最后nickname，不需要值可以为None
         输出为元组，如果为空输出None
         data = (qq , nickname , steamid )
         """
         if qq:
             self.c.execute("SELECT * FROM L4d2_players WHERE qq=?", (qq,))
@@ -75,13 +87,12 @@
                 return result
         if nickname:
             self.c.execute("SELECT * FROM L4d2_players WHERE nickname=?", (nickname,))
             result = self.c.fetchone()
             if result:
                 return result
         return None
-    
-    def _query_all_player(self) -> Tuple[tuple]:
+
+    def _query_all_player(self) -> List[Tuple]:
         """获取所有玩家信息"""
         self.c.execute("SELECT * FROM L4d2_players")
         return self.c.fetchall()
-
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from ..l4d2_utils.config import DATASQLITE
 import sqlite3
 
 
-class L4D2Server():
-    """数据库L4D2_server表的操作""" 
+class L4D2Server:
+    """数据库L4D2_server表的操作"""
+
     def __init__(self):
         """连接数据库"""
         self.datasqlite_path = DATASQLITE
-        self.conn = sqlite3.connect(self.datasqlite_path / 'L4D2.db')
-        self.c = self.conn.cursor() 
-        
-    async def bind_server_ip(self,qqgroup,host,port):
+        self.conn = sqlite3.connect(self.datasqlite_path / "L4D2.db")
+        self.c = self.conn.cursor()
+
+    async def bind_server_ip(self, qqgroup, host, port):
         """绑定群订阅ip"""
-        self.c.execute("INSERT OR REPLACE INTO L4D2_server (qqgroup, host, port) VALUES (?,?,?)", (qqgroup, host,port))
+        self.c.execute(
+            "INSERT OR REPLACE INTO L4D2_server (qqgroup, host, port) VALUES (?,?,?)",
+            (qqgroup, host, port),
+        )
         self.conn.commit()
-        
-    async def query_server_ip(self,qqgroup) :
+
+    async def query_server_ip(self, qqgroup):
         """输入群号，返回数据库里订阅ip元组列表"""
-        self.c.execute(f"SELECT  number, qqgroup ,host ,port FROM L4D2_server WHERE qqgroup = {qqgroup}")        
+        self.c.execute(
+            f"SELECT  number, qqgroup ,host ,port FROM L4D2_server WHERE qqgroup = {qqgroup}"
+        )
         msg_list = self.c.fetchall()
         return msg_list
-    
-    async def del_server_ip(self,id:int):
+
+    async def del_server_ip(self, id: int):
         """删除指定id的ip"""
         self.c.execute(f"DELETE FROM L4D2_server WHERE number = {id}")
         self.conn.commit()
-        
-    async def query_number(self,number:int):
+
+    async def query_number(self, number: int):
         """通过序号找服务器"""
-        self.c.execute(f"SELECT qqgroup , host ,port FROM L4D2_server WHERE number = {number}")
+        self.c.execute(
+            f"SELECT qqgroup , host ,port FROM L4D2_server WHERE number = {number}"
+        )
         msg_list = self.c.fetchone()
-        return msg_list
+        return msg_list
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,121 +2,121 @@
 from zipfile import ZipFile
 from time import sleep
 import sys
 import os
 import io
 from typing import List
 
-from ..l4d2_utils.utils import get_file,get_vpk
+from ..l4d2_utils.utils import get_file, get_vpk
 from ..l4d2_utils.config import systems
 from nonebot.log import logger
 from rarfile import RarFile
 import rarfile
 from pyunpack import Archive
 
 
-
-async def updown_l4d2_vpk(map_paths,name,url):
+async def updown_l4d2_vpk(map_paths: Path, name: str, url: str):
     """从url下载压缩包并解压到位置"""
-    original_vpk_files = []
-    original_vpk_files = get_vpk(original_vpk_files,map_paths)
-    down_file = Path(map_paths,name)
-    if await get_file(url,down_file) == None:
+    original_vpk_files = get_vpk(map_paths)
+    down_file = Path(map_paths, name)
+    if await get_file(url, down_file) == None:
         return None
     sleep(1)
-    msg = open_packet(name,down_file)
+    msg = open_packet(name, down_file)
     logger.info(msg)
-    
+
     sleep(1)
-    extracted_vpk_files = []
-    extracted_vpk_files = get_vpk(extracted_vpk_files,map_paths)
+    extracted_vpk_files = get_vpk(map_paths)
     # 获取新增vpk文件的list
     vpk_files = list(set(extracted_vpk_files) - set(original_vpk_files))
-    return  vpk_files
+    return vpk_files
 
-def open_packet(name:str,down_file:Path):
+
+def open_packet(name: str, down_file: Path):
     """解压压缩包"""
     down_path = os.path.dirname(down_file)
-    logger.info('文件名为：' + name)
-    logger.info(f'系统为{systems}')
-    if systems == 'win':
-        if name.endswith('.zip'):
-            mes = 'zip文件已下载,正在解压'
+    logger.info("文件名为：" + name)
+    logger.info(f"系统为{systems}")
+    mes = ""
+    if systems == "win":
+        if name.endswith(".zip"):
+            mes = "zip文件已下载,正在解压"
             try:
-                with support_gbk(ZipFile(down_file, 'r')) as z:
+                with support_gbk(ZipFile(down_file, "r")) as z:
                     z.extractall(down_path)
             except UnicodeEncodeError:
-                with ZipFile(down_file, 'r') as z:
-                    z.extractall(down_path)                
+                with ZipFile(down_file, "r") as z:
+                    z.extractall(down_path)
             os.remove(down_file)
-        elif name.endswith('.7z'):
-            mes ='7z文件已下载,正在解压'
-            Archive(down_file).extractall(down_path)
+        elif name.endswith(".7z"):
+            mes = "7z文件已下载,正在解压"
+            Archive(str(down_file)).extractall(down_path)
             # with SevenZipFile(down_file, 'r') as z:
             #     z.extractall(down_path)
             os.remove(down_file)
-        elif name.endswith('rar'):
-            mes = 'rar文件已下载,正在解压'
-            with RarFile(down_file,'r') as z:
+        elif name.endswith("rar"):
+            mes = "rar文件已下载,正在解压"
+            with RarFile(down_file, "r") as z:
                 z.extractall(down_path)
             os.remove(down_file)
-        elif name.endswith('.vpk'):
-            mes ='vpk文件已下载'
+        elif name.endswith(".vpk"):
+            mes = "vpk文件已下载"
     else:
-        if name.endswith('.zip'):
-            mes = 'zip文件已下载,正在解压'
-            with support_gbk(ZipFile(down_file, 'r')) as z:
+        if name.endswith(".zip"):
+            mes = "zip文件已下载,正在解压"
+            with support_gbk(ZipFile(down_file, "r")) as z:
                 z.extractall(down_path)
             os.remove(down_file)
-        elif name.endswith('.7z'):
-            mes ='7z文件已下载,正在解压'
-            Archive(down_file).extractall(down_path)
+        elif name.endswith(".7z"):
+            mes = "7z文件已下载,正在解压"
+            Archive(str(down_file)).extractall(down_path)
             # with SevenZipFile(down_file, 'r') as z:
             #     z.extractall(down_path)
             os.remove(down_file)
-        elif name.endswith('rar'):
-            mes = 'rar文件已下载,正在解压'
-            with rarfile.RarFile(down_file,'r') as z:
+        elif name.endswith("rar"):
+            mes = "rar文件已下载,正在解压"
+            with rarfile.RarFile(down_file, "r") as z:
                 z.extractall(down_path)
             os.remove(down_file)
         else:
-            mes ='vpk文件已下载'        
+            mes = "vpk文件已下载"
     return mes
 
-def support_gbk(zip_file:ZipFile):
-    '''
+
+def support_gbk(zip_file: ZipFile):
+    """
     压缩包中文恢复
-    '''
+    """
     if type(zip_file) == ZipFile:
         name_to_info = zip_file.NameToInfo
         # copy map first
         for name, info in name_to_info.copy().items():
-            real_name = name.encode('cp437').decode('gbk')
+            real_name = name.encode("cp437").decode("gbk")
             if real_name != name:
                 info.filename = real_name
                 del name_to_info[name]
                 name_to_info[real_name] = info
     return zip_file
 
 
-
-
-async def all_zip_to_one(data_list:List[bytes]):
+async def all_zip_to_one(
+    data_list: List[bytes],
+):
     """多压缩包文件合并"""
     file_list = []
     for data in data_list:
         # 将每个bytes对象解压缩成文件对象
         # 将文件对象存储在一个列表中
         file_list.append(io.BytesIO(data))
 
     # 创建一个新的BytesIO对象
     data_file = io.BytesIO()
 
     # 使用zipfile将列表中的文件对象添加到zipfile中
-    with ZipFile(data_file, mode='w') as zf:
+    with ZipFile(data_file, mode="w") as zf:
         for i, file in enumerate(file_list):
             # 将文件名设置为"file{i}.zip"，i为文件在列表中的索引
             filename = f"file{i}.zip"
             zf.writestr(filename, file.getvalue())
 
     # 获取zipfile的bytes对象
     return data_file.getvalue()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 from nonebot import on_notice
 from nonebot.adapters.onebot.v11 import NoticeEvent
 from pathlib import Path
 import httpx
-try:
-    import ujson as json
-except:
-    import json
+
+import json
 
 
 upload = on_notice(priority=1)
+
+
 @upload.handle()
-async def _(event:NoticeEvent):
+async def _(event: NoticeEvent):
     try:
         arg = event.dict()
-        files:dict = arg['file']
-        name:str = files['name']
-        if arg['notice_type'] == 'offline_file' and name.endswith('.json'):
+        files: dict = arg["file"]
+        name: str = files["name"]
+        if arg["notice_type"] == "offline_file" and name.endswith(".json"):
             try:
-                jsons = json.loads(httpx.get(files['url']).content.decode('utf-8'))
+                jsons = json.loads(httpx.get(files["url"]).content.decode("utf-8"))
             except json.decoder:
                 await upload.finish("求生json格式不正确")
             if not validate_json(jsons):
                 await upload.finish("求生json格式不正确")
-            key = await up_date(jsons,name)
+            key = await up_date(jsons, name)
             if key:
-                msg ='输入成功\n'
+                msg = "输入成功\n"
                 for key, value in jsons.items():
                     msg += f"当前你的{key}指令：{len(value)}个\n"
                 await upload.send(msg)
     except KeyError:
         pass
-    
+
+
 async def validate_json(json_data):
     try:
         data = json.loads(json_data)
         if not isinstance(data, dict):
             return False
 
         for key, value in data.items():
             if not isinstance(value, list):
                 return False
             for item in value:
                 if not isinstance(item, dict):
                     return False
-                if not all(key in item for key in ['id', 'version', 'ip']):
+                if not all(key in item for key in ["id", "version", "ip"]):
                     return False
 
         return True
 
     except json.JSONDecodeError:
         return False
-    
+
 
 async def up_date(data, name):
     directory = Path("data/L4D2/l4d2")
     directory.mkdir(parents=True, exist_ok=True)
-    
+
     file_path = directory / name
-    with open(file_path, 'w') as json_file:
-        json.dump(data, json_file,ensure_ascii=False)
-    
-    return True
+    with open(file_path, "w") as json_file:
+        json.dump(data, json_file, ensure_ascii=False)
+
+    return True
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,65 @@
-import asyncio
-import paramiko
+# import asyncio
+# import paramiko
+
+
+# class SSHClient:
+#     def __init__(self, hostname, port, username, password):
+#         self._hostname = hostname
+#         self._port = port
+#         self._username = username
+#         self._password = password
+#         self._ssh = None
+
+#     async def connect(self):
+#         self._ssh = paramiko.SSHClient()
+#         self._ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+#         await asyncio.get_event_loop().run_in_executor(
+#             None,
+#             self._ssh.connect,
+#             self._hostname,
+#             self._port,
+#             self._username,
+#             self._password,
+#         )
+
+#     async def upload(self, local_file_path, remote_file_path):
+#         with paramiko.Transport((self._hostname, self._port)) as transport:
+#             await asyncio.get_event_loop().run_in_executor(
+#                 None, transport.connect, None, self._username, self._password
+#             )
+#             sftp = paramiko.SFTPClient.from_transport(transport)
+#             await asyncio.get_event_loop().run_in_executor(
+#                 None, sftp.put, local_file_path, remote_file_path
+#             )
+
+#     async def delete(self, remote_file_path):
+#         with paramiko.Transport((self._hostname, self._port)) as transport:
+#             await asyncio.get_event_loop().run_in_executor(
+#                 None, transport.connect, None, self._username, self._password
+#             )
+#             sftp = paramiko.SFTPClient.from_transport(transport)
+#             await asyncio.get_event_loop().run_in_executor(
+#                 None, sftp.remove, remote_file_path
+#             )
+
+#     async def read(self, remote_dir_path):
+#         with paramiko.Transport((self._hostname, self._port)) as transport:
+#             await asyncio.get_event_loop().run_in_executor(
+#                 None, transport.connect, None, self._username, self._password
+#             )
+#             sftp = paramiko.SFTPClient.from_transport(transport)
+#             return await asyncio.get_event_loop().run_in_executor(
+#                 None, sftp.listdir, remote_dir_path
+#             )
+
+#     async def close(self):
+#         if self._ssh is not None:
+# self._ssh.close()
 
-class SSHClient:
-    def __init__(self, hostname, port, username, password):
-        self._hostname = hostname
-        self._port = port
-        self._username = username
-        self._password = password
-        self._ssh = None
-
-    async def connect(self):
-        self._ssh = paramiko.SSHClient()
-        self._ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-        await asyncio.get_event_loop().run_in_executor(None, self._ssh.connect, self._hostname, self._port, self._username, self._password)
-
-    async def upload(self, local_file_path, remote_file_path):
-        with paramiko.Transport((self._hostname, self._port)) as transport:
-            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
-            await asyncio.get_event_loop().run_in_executor(None, sftp.put, local_file_path, remote_file_path)
-
-
-    async def delete(self, remote_file_path):
-        with paramiko.Transport((self._hostname, self._port)) as transport:
-            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
-            await asyncio.get_event_loop().run_in_executor(None, sftp.remove, remote_file_path)
-
-    async def read(self, remote_dir_path):
-        with paramiko.Transport((self._hostname, self._port)) as transport:
-            await asyncio.get_event_loop().run_in_executor(None, transport.connect, None, self._username, self._password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
-            return await asyncio.get_event_loop().run_in_executor(None, sftp.listdir, remote_dir_path)
-
-    async def close(self):
-        if self._ssh is not None:
-            self._ssh.close()
 
 # async def main():
 #     ssh = SSHClient("example.com", 22, "username", "password")
 #     await ssh.connect()
 
 #     await ssh.upload("/path/to/local/file", "/path/to/remote/file")
 #     await ssh.delete("/path/to/remote/file")
@@ -47,17 +67,20 @@
 #     print(files)
 
 #     await ssh.close()
 
 # if __name__ == '__main__':
 #     asyncio.run(main())
 
-async def remote(mode:str,host,user,password,local_path = '',port=22, remote_path = ''):
-    """mode:upload、read、del"""
-    client = SSHClient(host, port,user, password)
-    if mode == 'upload':
-        await client.upload(local_path, remote_path)
-    elif mode == 'read':
-        file = await client.read(remote_path)
-        return file
-    elif mode == 'del':
-        await client.delete(remote_path)
+
+# async def remote(
+#     mode: str, host, user, password, local_path="", port=22, remote_path=""
+# ):
+#     """mode:upload、read、del"""
+#     client = SSHClient(host, port, user, password)
+#     if mode == "upload":
+#         await client.upload(local_path, remote_path)
+#     elif mode == "read":
+#         file = await client.read(remote_path)
+#         return file
+#     elif mode == "del":
+#         await client.delete(remote_path)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,110 @@
-
 from bs4 import BeautifulSoup
 import jinja2
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic
-from typing import List,Optional
+from typing import List, Optional
 
 
 # from .htmlimg import dict_to_dict_img
 # from ..l4d2_anne.anne_telecom import ANNE_API
 from ..l4d2_utils.config import TEXT_PATH
 from .download import get_head_by_user_id_and_save
 from .send_image_tool import convert_img
 
 from ..l4d2_utils.config import l4_config
-template_path = TEXT_PATH/"template"
+
+template_path = TEXT_PATH / "template"
 
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 
-async def out_png(usr_id,data_dict:dict):
+
+async def out_png(usr_id, data_dict: dict):
     """使用html来生成图片"""
-    
-    with open((template_path/"anne.html"),"r", encoding="utf-8") as file:
+
+    with open((template_path / "anne.html"), "r", encoding="utf-8") as file:
         data_html = file.read()
     # content = template.render_async()
-    soup = BeautifulSoup(data_html, 'html.parser')
-    msg_dict = await dict_to_html(usr_id,data_dict,soup)
-    template = env.get_template('anne.html')
+    soup = BeautifulSoup(data_html, "html.parser")
+    msg_dict = await dict_to_html(usr_id, data_dict, soup)
+    template = env.get_template("anne.html")
     html = await template.render_async(data=msg_dict)
     pic = await html_to_pic(
-                html,
-                wait=0,
-                viewport={"width": 1100, "height": 800},
-                template_path=f"file://{template_path.absolute()}",)
+        html,
+        wait=0,
+        viewport={"width": 1100, "height": 800},
+        template_path=f"file://{template_path.absolute()}",
+    )
     return pic
 
 
-async def dict_to_html(usr_id,DETAIL_MAP:dict,soup:BeautifulSoup):
+async def dict_to_html(usr_id, DETAIL_MAP: dict, soup: BeautifulSoup):
     """输入qq、字典，获取新的msg替换html"""
     DETAIL_right = {}
-    DETAIL_right['name'] = DETAIL_MAP['Steam 名字:']
-    DETAIL_right['Steam_ID'] = DETAIL_MAP['Steam ID:']
-    DETAIL_right['play_time'] = DETAIL_MAP['游玩时间:']
-    DETAIL_right['last_online'] = DETAIL_MAP['最后上线:']
-    DETAIL_right['rank'] = DETAIL_MAP['排行:']
-    DETAIL_right['points'] = DETAIL_MAP['分数:']
-    DETAIL_right['point_min'] = DETAIL_MAP['每分钟获取分数:']
-    DETAIL_right['killed'] = DETAIL_MAP['感染者消灭:']
-    DETAIL_right['shut'] = DETAIL_MAP['爆头:']        
-    DETAIL_right['out'] = DETAIL_MAP['爆头率:']
-    DETAIL_right['playtimes'] = DETAIL_MAP['游玩地图数量:']
-    DETAIL_right['url'] = DETAIL_MAP['个人资料']
-    DETAIL_right['one_msg'] = DETAIL_MAP['一言']
-    DETAIL_right['last_one'] = DETAIL_MAP['救援关']
+    DETAIL_right["name"] = DETAIL_MAP["Steam 名字:"]
+    DETAIL_right["Steam_ID"] = DETAIL_MAP["Steam ID:"]
+    DETAIL_right["play_time"] = DETAIL_MAP["游玩时间:"]
+    DETAIL_right["last_online"] = DETAIL_MAP["最后上线:"]
+    DETAIL_right["rank"] = DETAIL_MAP["排行:"]
+    DETAIL_right["points"] = DETAIL_MAP["分数:"]
+    DETAIL_right["point_min"] = DETAIL_MAP["每分钟获取分数:"]
+    DETAIL_right["killed"] = DETAIL_MAP["感染者消灭:"]
+    DETAIL_right["shut"] = DETAIL_MAP["爆头:"]
+    DETAIL_right["out"] = DETAIL_MAP["爆头率:"]
+    DETAIL_right["playtimes"] = DETAIL_MAP["游玩地图数量:"]
+    DETAIL_right["url"] = DETAIL_MAP["个人资料"]
+    DETAIL_right["one_msg"] = DETAIL_MAP["一言"]
+    DETAIL_right["last_one"] = DETAIL_MAP["救援关"]
     # html_text = soup.prettify()
     # for key, value in DETAIL_right.items():
     #     html_text = html_text.replace(key,value)
     # 头像
     temp = await get_head_by_user_id_and_save(usr_id)
     # temp = await get_head_steam_and_save(usr_id,DETAIL_right['url'])
-    res = await convert_img(temp,is_base64=True)
-    DETAIL_right['header'] = f"data:image/png;base64,{res}"
-    data_list:List[dict] = [DETAIL_right]
+    if not temp:
+        return
+    res = await convert_img(temp, is_base64=True)
+    DETAIL_right["header"] = f"data:image/png;base64,{res}"
+    data_list: List[dict] = [DETAIL_right]
     return data_list
 
 
-async def server_ip_pic(msg_list:List[dict]):
+async def server_ip_pic(msg_list: List[dict]):
     """
     输入一个字典列表，输出图片
     msg_dict:folder/name/map_/players/max_players/Players/[Name]
     """
     for server_info in msg_list:
-        server_info['max_players'] = f"{server_info['players']}/{server_info['max_players']}"
+        server_info[
+            "max_players"
+        ] = f"{server_info['players']}/{server_info['max_players']}"
         players_list = []
-        if 'Players' in server_info:
-            sorted_players = sorted(server_info['Players'], key=lambda x: x.get('Score', 0), reverse=True)[:4]
+        if "Players" in server_info:
+            sorted_players = sorted(
+                server_info["Players"], key=lambda x: x.get("Score", 0), reverse=True
+            )[:4]
             for player_info in sorted_players:
                 player_str = f"{player_info['name']} | {player_info['Duration']}"
                 players_list.append(player_str)
             while len(players_list) < 4:
                 players_list.append("")
-            server_info['Players'] = players_list
+            server_info["Players"] = players_list
     pic = await get_help_img(msg_list)
     if pic:
-        logger.success('正在输出图片')
+        logger.success("正在输出图片")
     else:
-        logger.warning('我的图图呢')
+        logger.warning("我的图图呢")
     return pic
 
 
 async def get_help_img(plugins: List[dict]) -> Optional[bytes]:
     try:
-        if l4_config.l4_style == 'black':
+        if l4_config.l4_style == "black":
             template = env.get_template("help_dack.html")
         else:
             template = env.get_template("help.html")
         content = await template.render_async(plugins=plugins)
         return await html_to_pic(
             content,
             wait=0,
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,98 @@
 import httpx
 from nonebot.log import logger
 import asyncio
 import hashlib
 import os
 import random
-from PIL import Image,ImageDraw
+from PIL import Image, ImageDraw
+from PIL.Image import Image as ImageS
 import io
-from ..l4d2_utils.config import PLAYERSDATA,TEXT_PATH
+from ..l4d2_utils.config import PLAYERSDATA, TEXT_PATH
+
 # from .steam import web_player
 
+
 async def download_url(url: str) -> bytes:
     async with httpx.AsyncClient() as client:
         for i in range(3):
             try:
                 resp = await client.get(url, timeout=20)
                 resp.raise_for_status()
                 return resp.content
             except Exception as e:
                 logger.warning(f"Error downloading {url}, retry {i}/3: {e}")
                 await asyncio.sleep(3)
     raise Exception(f"{url} 下载失败！")
 
+
 async def download_head(user_id: str) -> bytes:
     url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
     data = await download_url(url)
     if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
         url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
         data = await download_url(url)
     return data
 
-    
-def square_to_circle(im:Image):
+
+def square_to_circle(im: ImageS):
     """im是正方形，变圆形"""
     size = im.size
-    mask = Image.new('L', size, 0)
+    mask = Image.new("L", size, 0)
     draw = ImageDraw.Draw(mask)
     draw.ellipse((0, 0) + size, fill=255)
     # 将遮罩层应用到图像上
     im.putalpha(mask)
     return im
 
+
 async def get_head_by_user_id_and_save(user_id):
     """qq转头像"""
     user_id = str(user_id)
-    
-    USER_HEAD_PATH = PLAYERSDATA / user_id / 'HEAD.png'
+
+    USER_HEAD_PATH = PLAYERSDATA / user_id / "HEAD.png"
     DEFAULT_HEADER_PATH = TEXT_PATH / "header"
     DEFAULT_HEAD_PATH = TEXT_PATH / "head"
-    DEFAULT_HEADER = DEFAULT_HEADER_PATH /random.choice(os.listdir(DEFAULT_HEADER_PATH))
-    DEFAULT_HEAD = DEFAULT_HEAD_PATH /random.choice(os.listdir(DEFAULT_HEAD_PATH))
+    DEFAULT_HEADER = DEFAULT_HEADER_PATH / random.choice(
+        os.listdir(DEFAULT_HEADER_PATH)
+    )
+    DEFAULT_HEAD = DEFAULT_HEAD_PATH / random.choice(os.listdir(DEFAULT_HEAD_PATH))
     ## im头像 im2头像框 im3合成
     if os.path.exists(USER_HEAD_PATH):
         logger.info("使用本地头像")
         im = Image.open(USER_HEAD_PATH).resize((280, 280)).convert("RGBA")
     else:
         if user_id == "1145149191810":
             logger.info("使用默认头像")
             im = Image.open(DEFAULT_HEADER).resize((280, 280)).convert("RGBA")
         else:
             try:
                 logger.info("正在下载头像")
                 image_bytes = await download_head(user_id)
-                im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")
-                if not os.path.exists(PLAYERSDATA / user_id):#用户文件夹不存在
+                im = (
+                    Image.open(io.BytesIO(image_bytes))
+                    .resize((280, 280))
+                    .convert("RGBA")
+                )
+                if not os.path.exists(PLAYERSDATA / user_id):  # 用户文件夹不存在
                     os.makedirs(PLAYERSDATA / user_id)
                 im.save(USER_HEAD_PATH, "PNG")
             except:
                 logger.error("获取失败")
-    im2 = Image.open(DEFAULT_HEAD).resize((450,450)).convert("RGBA")
-    im3 = Image.new("RGBA", im2.size, (255,255,255,0))
+                return
+    im2 = Image.open(DEFAULT_HEAD).resize((450, 450)).convert("RGBA")
+    im3 = Image.new("RGBA", im2.size, (255, 255, 255, 0))
     r, g, b, a1 = im.split()
     r, g, b, a2 = im2.split()
     im = square_to_circle(im)
-    im3.paste(im,(75,75),mask=a1)
-    im3.paste(im2,mask=a2)
+    im3.paste(im, (75, 75), mask=a1)
+    im3.paste(im2, mask=a2)
     return im3
 
+
 # async def get_head_steam_and_save(user_id:str,urls):
 #     """保存steam头像"""
 #     USER_HEAD_PATH = PLAYERSDATA / str(user_id) / 'HEAD.png'
 #     # DEFAULT_HEAD_PATH = TEXT_PATH / "template/player.jpg"
 #     ## im头像 im2头像框 im3合成
 #     if os.path.exists(USER_HEAD_PATH):
 #         logger.info("使用本地头像")
@@ -95,8 +108,7 @@
 #                 im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")
 #                 if not os.path.exists(PLAYERSDATA / user_id):#用户文件夹不存在
 #                     os.makedirs(PLAYERSDATA / user_id)
 #                 im.save(USER_HEAD_PATH, "PNG")
 #             except TimeoutError:
 #                 logger.error("获取失败")
 #     return im
-
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-
-
 class DATA_PANDS:
-    async def __init__(
-        self,
-        data_dict:dict
-        ) -> None:
-        self.new_data = {[]}
+    def __init__(self, data_dict: dict) -> None:
+        self.new_data = {}
         self.data_dict = data_dict
-        for key,value in data_dict.items():
+        for key in data_dict:
             self.dict_pan(key)
-        
-    
-    
-    async def dict_pan(self,key):
+
+    def dict_pan(self, key):
         """dict转化为图像所需要的dict量化"""
-        # 删除不必要是数据
-        if key in ['刷特模式']:
-            for item in self.data_dict[key]:
-                if item == '固定刷特':
-                    self.data_dict.pop(item)
-        elif key in ['游戏模式']:
+        # 删除不必要的数据
+        if key == "刷特模式":
+            self.data_dict.pop(key)
+        elif key == "游戏模式" or key == "特感数量" or key == "刷新间隔":
             for item in self.data_dict[key]:
                 if item in self.new_data:
                     self.new_data[item] += 1
                 else:
                     self.new_data[item] = 1
-        elif key in ['特感数量','刷新间隔']:
-            for item in self.data_dict[key]:
-                if item in self.new_data:
-                    self.new_data[item] += 1
-                else:
-                    self.new_data[item] = 1
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 from io import BytesIO
 from pathlib import Path
 from base64 import b64encode
 from typing import Union, overload
-from typing import Union,Tuple,Optional
+from typing import Union, Tuple, Optional
 import math
 import random
 
 import aiofiles
 from PIL import Image
 from httpx import get
 import sys
 from pathlib import Path
+from typing import overload
 
-MAIN_PATH = Path() / 'data' / 'GenshinUID'
+
+MAIN_PATH = Path() / "data" / "GenshinUID"
 sys.path.append(str(MAIN_PATH))
-CONFIG_PATH = MAIN_PATH / 'config.json'
-RESOURCE_PATH = MAIN_PATH / 'resource'
-WIKI_PATH = MAIN_PATH / 'wiki'
-CU_BG_PATH = MAIN_PATH / 'bg'
-CU_CHBG_PATH = MAIN_PATH / 'chbg'
-WEAPON_PATH = RESOURCE_PATH / 'weapon'
-GACHA_IMG_PATH = RESOURCE_PATH / 'gacha_img'
-CHAR_PATH = RESOURCE_PATH / 'chars'
-CHAR_STAND_PATH = RESOURCE_PATH / 'char_stand'
-CHAR_SIDE_PATH = RESOURCE_PATH / 'char_side'
-CHAR_NAMECARD_PATH = RESOURCE_PATH / 'char_namecard'
-REL_PATH = RESOURCE_PATH / 'reliquaries'
-ICON_PATH = RESOURCE_PATH / 'icon'
-TEMP_PATH = RESOURCE_PATH / 'temp'
-CARD_PATH = RESOURCE_PATH / 'card'
-GUIDE_PATH = WIKI_PATH / 'guide'
-TEXT2D_PATH = Path(__file__).parents[2] / 'resource' / 'texture2d'
-
-PLAYER_PATH = MAIN_PATH / 'players'
-
-
-TEXT2D_PATH = Path(__file__).parents[2] / 'resource' / 'texture2d'
-FETTER_PATH = TEXT2D_PATH / 'fetter'
-TALENT_PATH = TEXT2D_PATH / 'talent'
-WEAPON_BG_PATH = TEXT2D_PATH / 'weapon'
-WEAPON_AFFIX_PATH = TEXT2D_PATH / 'weapon_affix'
-LEVEL_PATH = TEXT2D_PATH / 'level'
-
-BG_PATH = Path(__file__).parent / 'bg'
-TEXT_PATH = Path(__file__).parent / 'texture2d'
-ring_pic = Image.open(TEXT_PATH / 'ring.png')
-mask_pic = Image.open(TEXT_PATH / 'mask.png')
-NM_BG_PATH = BG_PATH / 'nm_bg'
-SP_BG_PATH = BG_PATH / 'sp_bg'@overload
+CONFIG_PATH = MAIN_PATH / "config.json"
+RESOURCE_PATH = MAIN_PATH / "resource"
+WIKI_PATH = MAIN_PATH / "wiki"
+CU_BG_PATH = MAIN_PATH / "bg"
+CU_CHBG_PATH = MAIN_PATH / "chbg"
+WEAPON_PATH = RESOURCE_PATH / "weapon"
+GACHA_IMG_PATH = RESOURCE_PATH / "gacha_img"
+CHAR_PATH = RESOURCE_PATH / "chars"
+CHAR_STAND_PATH = RESOURCE_PATH / "char_stand"
+CHAR_SIDE_PATH = RESOURCE_PATH / "char_side"
+CHAR_NAMECARD_PATH = RESOURCE_PATH / "char_namecard"
+REL_PATH = RESOURCE_PATH / "reliquaries"
+ICON_PATH = RESOURCE_PATH / "icon"
+TEMP_PATH = RESOURCE_PATH / "temp"
+CARD_PATH = RESOURCE_PATH / "card"
+GUIDE_PATH = WIKI_PATH / "guide"
+TEXT2D_PATH = Path(__file__).parents[2] / "resource" / "texture2d"
+
+PLAYER_PATH = MAIN_PATH / "players"
+
+
+TEXT2D_PATH = Path(__file__).parents[2] / "resource" / "texture2d"
+FETTER_PATH = TEXT2D_PATH / "fetter"
+TALENT_PATH = TEXT2D_PATH / "talent"
+WEAPON_BG_PATH = TEXT2D_PATH / "weapon"
+WEAPON_AFFIX_PATH = TEXT2D_PATH / "weapon_affix"
+LEVEL_PATH = TEXT2D_PATH / "level"
+
+BG_PATH = Path(__file__).parent / "bg"
+TEXT_PATH = Path(__file__).parent / "texture2d"
+ring_pic = Image.open(TEXT_PATH / "ring.png")
+mask_pic = Image.open(TEXT_PATH / "mask.png")
+NM_BG_PATH = BG_PATH / "nm_bg"
+SP_BG_PATH = BG_PATH / "sp_bg"
 
 if list(CU_BG_PATH.iterdir()) != []:
     bg_path = CU_BG_PATH
 else:
     bg_path = NM_BG_PATH
 
+
+@overload
 async def convert_img(img: Image.Image, is_base64: bool = False) -> bytes:
     ...
 
 
 @overload
 async def convert_img(img: Image.Image, is_base64: bool = True) -> str:
     ...
@@ -82,47 +86,46 @@
     :参数:
       * img (Image): 图片。
       * is_base64 (bool): 是否转换为base64格式, 不填默认转为bytes。
     :返回:
       * res: bytes对象或base64编码图片。
     """
     if isinstance(img, Image.Image):
-        img = img.convert('RGB')
+        img = img.convert("RGB")
         result_buffer = BytesIO()
-        img.save(result_buffer, format='PNG', quality=80, subsampling=0)
+        img.save(result_buffer, format="PNG", quality=80, subsampling=0)
         res = result_buffer.getvalue()
         if is_base64:
-            res = 'base64://' + b64encode(res).decode()
+            res = "base64://" + b64encode(res).decode()
         return res
     elif isinstance(img, bytes):
         pass
     else:
-        async with aiofiles.open(img, 'rb') as fp:
+        async with aiofiles.open(img, "rb") as fp:
             img = await fp.read()
-    return f'[CQ:image,file=base64://{b64encode(img).decode()}]'
+    return f"[CQ:image,file=base64://{b64encode(img).decode()}]"
 
 
 async def get_color_bg(
     based_w: int, based_h: int, bg: Optional[str] = None
 ) -> Image.Image:
-    image = ''
+    image = ""
     if bg:
-        path = SP_BG_PATH / f'{bg}.jpg'
+        path = SP_BG_PATH / f"{bg}.jpg"
         if path.exists():
             image = Image.open(path)
     CI_img = CustomizeImage(image, based_w, based_h)
     img = CI_img.bg_img
     color = CI_img.bg_color
-    color_mask = Image.new('RGBA', (based_w, based_h), color)
-    enka_mask = Image.open(TEXT2D_PATH / 'mask.png').resize((based_w, based_h))
+    color_mask = Image.new("RGBA", (based_w, based_h), color)
+    enka_mask = Image.open(TEXT2D_PATH / "mask.png").resize((based_w, based_h))
     img.paste(color_mask, (0, 0), enka_mask)
     return img
 
 
-
 class CustomizeImage:
     def __init__(
         self, image: Union[str, Image.Image], based_w: int, based_h: int
     ) -> None:
 
         self.bg_img = self.get_image(image, based_w, based_h)
         self.bg_color = self.get_bg_color(self.bg_img, is_light=True)
@@ -136,18 +139,18 @@
     def get_image(
         image: Union[str, Image.Image], based_w: int, based_h: int
     ) -> Image.Image:
         # 获取背景图片
         if isinstance(image, Image.Image):
             edit_bg = image
         elif image:
-            edit_bg = Image.open(BytesIO(get(image).content)).convert('RGBA')
+            edit_bg = Image.open(BytesIO(get(image).content)).convert("RGBA")
         else:
             path = random.choice(list(bg_path.iterdir()))
-            edit_bg = Image.open(path).convert('RGBA')
+            edit_bg = Image.open(path).convert("RGBA")
 
         # 确定图片的长宽
         bg_img = crop_center_img(edit_bg, based_w, based_h)
         return bg_img
 
     @staticmethod
     def get_dominant_color(pil_img: Image.Image) -> Tuple[int, int, int]:
@@ -204,80 +207,72 @@
             math.floor(bg_color[0] + 5 if bg_color[0] + r <= 255 else 255),
             math.floor(bg_color[1] + 5 if bg_color[1] + r <= 255 else 255),
             math.floor(bg_color[2] + 5 if bg_color[2] + r <= 255 else 255),
         )
         return char_color
 
     @staticmethod
-    def get_char_high_color(
-        bg_color: Tuple[int, int, int]
-    ) -> Tuple[int, int, int]:
+    def get_char_high_color(bg_color: Tuple[int, int, int]) -> Tuple[int, int, int]:
         r = 140
         d = 20
         if max(*bg_color) > 255 - r:
             r *= -1
         char_color = (
             math.floor(bg_color[0] + d if bg_color[0] + r <= 255 else 255),
             math.floor(bg_color[1] + d if bg_color[1] + r <= 255 else 255),
             math.floor(bg_color[2] + d if bg_color[2] + r <= 255 else 255),
         )
         return char_color
 
     @staticmethod
-    def get_bg_detail_color(
-        bg_color: Tuple[int, int, int]
-    ) -> Tuple[int, int, int]:
+    def get_bg_detail_color(bg_color: Tuple[int, int, int]) -> Tuple[int, int, int]:
         r = 140
         if max(*bg_color) > 255 - r:
             r *= -1
         bg_detail_color = (
             math.floor(bg_color[0] - 20 if bg_color[0] + r <= 255 else 255),
             math.floor(bg_color[1] - 20 if bg_color[1] + r <= 255 else 255),
             math.floor(bg_color[2] - 20 if bg_color[2] + r <= 255 else 255),
         )
         return bg_detail_color
 
     @staticmethod
-    def get_highlight_color(
-        color: Tuple[int, int, int]
-    ) -> Tuple[int, int, int]:
+    def get_highlight_color(color: Tuple[int, int, int]) -> Tuple[int, int, int]:
         red_color = color[0]
         green_color = color[1]
         blue_color = color[2]
 
         highlight_color = {
-            'red': red_color - 127 if red_color > 127 else 127,
-            'green': green_color - 127 if green_color > 127 else 127,
-            'blue': blue_color - 127 if blue_color > 127 else 127,
+            "red": red_color - 127 if red_color > 127 else 127,
+            "green": green_color - 127 if green_color > 127 else 127,
+            "blue": blue_color - 127 if blue_color > 127 else 127,
         }
 
         max_color = max(highlight_color.values())
 
-        name = ''
+        name = ""
         for _highlight_color in highlight_color:
             if highlight_color[_highlight_color] == max_color:
                 name = str(_highlight_color)
 
-        if name == 'red':
-            return red_color, highlight_color['green'], highlight_color['blue']
-        elif name == 'green':
-            return highlight_color['red'], green_color, highlight_color['blue']
-        elif name == 'blue':
-            return highlight_color['red'], highlight_color['green'], blue_color
+        if name == "red":
+            return red_color, highlight_color["green"], highlight_color["blue"]
+        elif name == "green":
+            return highlight_color["red"], green_color, highlight_color["blue"]
+        elif name == "blue":
+            return highlight_color["red"], highlight_color["green"], blue_color
         else:
             return 0, 0, 0  # Error
-        
-        
-def crop_center_img(
-    img: Image.Image, based_w: int, based_h: int
-) -> Image.Image:
+
+
+def crop_center_img(img: Image.Image, based_w: int, based_h: int) -> Image.Image:
     # 确定图片的长宽
-    based_scale = '%.3f' % (based_w / based_h)
+    based_scale = "%.3f" % (based_w / based_h)
     w, h = img.size
-    scale_f = '%.3f' % (w / h)
+    scale_f = "%.3f" % (w / h)
     new_w = math.ceil(based_h * float(scale_f))
     new_h = math.ceil(based_w / float(scale_f))
     if scale_f > based_scale:
         resize_img = img.resize((new_w, based_h), Image.ANTIALIAS)
         x1 = int(new_w / 2 - based_w / 2)
         y1 = 0
         x2 = int(new_w / 2 + based_w / 2)
@@ -285,8 +280,8 @@
     else:
         resize_img = img.resize((based_w, new_h), Image.ANTIALIAS)
         x1 = 0
         y1 = int(new_h / 2 - based_h / 2)
         x2 = based_w
         y2 = int(new_h / 2 + based_h / 2)
     crop_img = resize_img.crop((x1, y1, x2, y2))
-    return crop_img
+    return crop_img
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 from pathlib import Path
 
 # 半透明素材
 half_whitel_image_path = Path(__file__).parent.parent.joinpath("data/img/white.png")
 half_whitel_image = Image.open(half_whitel_image_path)
 
 
-async def one_server_img(msg :dict):
-    """单个服务器的dict信息变成图片"""
-    img_background = await adjust_image_size(msg['Players'])
-    img_background = await adjust_server_name(img_background , msg['name'])
-    
+# async def one_server_img(msg: dict):
+#     """单个服务器的dict信息变成图片"""
+#     img_background = await adjust_image_size(msg["Players"])
+#     img_background = await adjust_server_name(img_background, msg["name"])
 
 
 async def adjust_image_size(text_list):
     """初始化背景"""
     initial_width = 1080
     initial_height = 600
     height_increment = 100
 
-    num_players = len(text_list.get('Player', []))
+    num_players = len(text_list.get("Player", []))
     final_height = initial_height + num_players * height_increment
-    
+
     image = Image.new("RGBA", (initial_width, final_height), "white")
     return image
 
-async def adjust_server_name(image:Image ,name :str):
+
+async def adjust_server_name(image: Image.Image, name: str):
     """写标题"""
     pass
 
-async def adjust_ping(image:Image ,ping :str):
+
+async def adjust_ping(image: Image.Image, ping: str):
     """写ping"""
-    
-async def adjust_player(image:Image ,Player:List[dict]):
-    """写玩家"""
 
+
+async def adjust_player(image: Image.Image, Player: List[dict]):
+    """写玩家"""
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     :参数:
       * img (Image): 图片。
       * is_base64 (bool): 是否转换为base64格式, 不填默认转为bytes。
     :返回:
       * res: bytes对象或base64编码图片。
     """
     if isinstance(img, Image.Image):
-        img = img.convert('RGBA')
+        img = img.convert("RGBA")
         result_buffer = BytesIO()
-        img.save(result_buffer, format='PNG', quality=80, subsampling=0)
+        img.save(result_buffer, format="PNG", quality=80, subsampling=0)
         res = result_buffer.getvalue()
         if is_base64:
             res = b64encode(res).decode()
         return res
     elif isinstance(img, bytes):
         return b64encode(img).decode()
     else:
-        return f'[CQ:image,file=file:///{str(img)}]'
+        return f"[CQ:image,file=file:///{str(img)}]"
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # from PIL import Image
 import httpx
 import aiohttp
+
 # from bs4 import BeautifulSoup
+from typing import List, Optional
 from urllib.parse import unquote
 
-    
+
 # async def web_player(url) -> Image :
 #     """steam个人资料获取头像"""
 #     data = BeautifulSoup(await url_for_byte(url), 'html.parser')
 #     print(data)
 #     head = data.find("div", class_="playerAvatarAutoSizeInner")
 #     img_elements = head.find_all("img")
 #     if len(img_elements)== 1:
@@ -35,49 +37,55 @@
 #         print("代理不存在")
 #         data = await url_to_byte(url)
 #     headers = {
 #         'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
 #     }
 #     data = httpx.get(url,headers=headers,proxies=l4_proxies,timeout=60,verify=False).content
 #     return data
-async def url_to_byte(url:str,filename:str =''):
+async def url_to_byte(url: str, filename: str = ""):
     """获取URL数据的字节流"""
     headers = {
-    'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
     }
     async with aiohttp.ClientSession() as session:
         async with session.get(url, headers=headers, timeout=600) as response:
             if response.status == 200:
                 return await response.read()
             else:
                 return None
 
-async def url_to_byte_name(url:str,filename:str =''):
+
+async def url_to_byte_name(url: str, filename: str = ""):
     """获取URL数据的字节流"""
     headers = {
-    'User-Agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
     }
+
     if filename == "htp":
-        response = httpx.get(url,headers=headers,timeout=600)
-        content_disposition:str = response.headers.get("Content-Disposition")
+        response = httpx.get(url, headers=headers, timeout=600)
+        content_disposition = response.headers.get("Content-Disposition")
         if not content_disposition:
             return None
         elif "''" in content_disposition:
             file_name = content_disposition.split("''")[-1]
-        else: 
+        else:
             file_name = content_disposition
         file_name = unquote(file_name)
-        return [response.read(),file_name]
-    else:       
+        if response.content and file_name:
+            return [response.content, file_name]
+    else:
         async with aiohttp.ClientSession() as session:
             async with session.get(url, headers=headers, timeout=600) as response:
-                content_disposition:str = response.headers.get("Content-Disposition")
+                content_disposition = response.headers.get("Content-Disposition")
+                if not content_disposition:
+                    return
                 if "''" in content_disposition:
                     file_name = content_disposition.split("''")[-1]
-                else: 
+                else:
                     file_name = content_disposition
+                if not file_name:
+                    file_name = "anyone"
                 file_name = unquote(file_name)
                 if response.status == 200:
-                    return [await response.read(),file_name]
+                    return [await response.read(), file_name]
                 else:
                     return None
-
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-
 from PIL import Image
 from nonebot.log import logger
 from io import BytesIO
+
 # import sys
 # sys.modules["srctools._cy_vtf_readwrite"] = None
 from srctools.vtf import VTF, ImageFormats
 
-async def img_to_vtf(pic_byte:bytes,tag) -> BytesIO:
+
+async def img_to_vtf(pic_byte: bytes, tag) -> BytesIO:
     pic = BytesIO(pic_byte)
-    pic = Image.open(pic).convert('RGBA')
+    pic = Image.open(pic).convert("RGBA")
     vtf_io = BytesIO()
-    vtf_ = VTF(1024, 1024, fmt = ImageFormats.DXT5,thumb_fmt = ImageFormats.DXT1,version=(7,2))
-    if tag == '覆盖':
+    vtf_ = VTF(
+        1024, 1024, fmt=ImageFormats.DXT5, thumb_fmt=ImageFormats.DXT1, version=(7, 2)
+    )
+    if tag == "覆盖":
         logger.info(tag)
-        img2 = Image.new('RGBA',(1024, 1024), (255, 255, 255,0))
+        img2 = Image.new("RGBA", (1024, 1024), (255, 255, 255, 0))
         r, g, b, a = pic.split()
-        img2.paste(pic,mask=a)
-        pic = pic.resize((1024,1024))
-    elif tag == '填充':
+        img2.paste(pic, mask=a)
+        pic = pic.resize((1024, 1024))
+    elif tag == "填充":
         w, h = pic.size
         if w > h:
-            ratio = 1024/w
+            ratio = 1024 / w
             new_width = 1024
             new_height = int(h * ratio)
         else:
-            ratio = 1024/h
+            ratio = 1024 / h
             new_height = 1024
             new_width = int(w * ratio)
         pic = pic.resize((new_width, new_height), Image.ANTIALIAS)
-        background = Image.new('RGBA', (1024, 1024), (255, 255, 255, 0))
-        background.paste(pic, ((1024-new_width)//2, (1024-new_height)//2))
+        background = Image.new("RGBA", (1024, 1024), (255, 255, 255, 0))
+        background.paste(pic, ((1024 - new_width) // 2, (1024 - new_height) // 2))
         pic = background
     else:
-        logger.info('拉伸')
-        pic = pic.resize((1024,1024))
-    largest_frame = vtf_.get() 
+        logger.info("拉伸")
+        pic = pic.resize((1024, 1024))
+    largest_frame = vtf_.get()
     largest_frame.copy_from(pic.tobytes(), ImageFormats.RGBA8888)
-    vtf_.save(vtf_io,version=(7,2))
+    vtf_.save(vtf_io, version=(7, 2))
     return vtf_io
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,196 +1,213 @@
 from pathlib import Path
 import re
 import a2s
-from typing import Dict,List,Union
+from typing import Dict, List, Union
+
 try:
     import ujson as json
 except:
     import json
 
 from nonebot.log import logger
-from nonebot import get_driver,on_command,get_bot
+from nonebot import get_driver, on_command, get_bot
 from nonebot import require
 from nonebot.permission import SUPERUSER
 from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import GroupMessageEvent,MessageSegment,Message
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, Message
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
 )
+
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 from ..l4d2_utils.command import get_ip_to_mes
-from ..l4d2_utils.utils import extract_last_digit,json_server_to_tag_dict,split_maohao
+from ..l4d2_utils.utils import extract_last_digit, json_server_to_tag_dict, split_maohao
 from ..l4d2_utils.config import l4_config
 from ..l4d2_queries import queries_dict
 
 driver = get_driver()
-sch_json = Path('data/L4D2/scheduler.json')
+sch_json = Path("data/L4D2/scheduler.json")
 if not sch_json.exists():
-    with sch_json.open('w') as f:
-        json.dump({}, f ,ensure_ascii=False)
-        
-add_rss = on_command('add_rss',aliases={'求生定时添加'},priority= 30,permission= SUPERUSER| GROUP_ADMIN | GROUP_OWNER)
-del_rss = on_command('del_rss',aliases={'求生定时删除'},priority= 30,permission= SUPERUSER| GROUP_ADMIN | GROUP_OWNER)
+    with sch_json.open("w") as f:
+        json.dump({}, f, ensure_ascii=False)
+
+add_rss = on_command(
+    "add_rss",
+    aliases={"求生定时添加"},
+    priority=30,
+    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+)
+del_rss = on_command(
+    "del_rss",
+    aliases={"求生定时删除"},
+    priority=30,
+    permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
+)
+
 
 @add_rss.handle()
-async def _(event:GroupMessageEvent , matcher:Matcher ,args: Message = CommandArg()):
+async def _(event: GroupMessageEvent, matcher: Matcher, args: Message = CommandArg()):
     group_id = event.group_id
     msg = args.extract_plain_text()
-    command,message = await extract_last_digit(msg)
-    push_msg =  await get_ip_to_mes(msg= message,  command= command)
-    if push_msg in ["服务器无响应" ,None] :
-        await matcher.finish('无响应的服务器，请检查')
+    command, message = await extract_last_digit(msg)
+    push_msg = await get_ip_to_mes(msg=message, command=command)
+    if not push_msg:
+        return
+    if push_msg in ["服务器无响应", None]:
+        await matcher.finish("无响应的服务器，请检查")
     else:
-        return_msg = await add_or_update_data(group_id,msg)
-        if isinstance(push_msg , bytes):
+        return_msg = await add_or_update_data(group_id, msg)
+        if isinstance(push_msg, bytes):
             await matcher.send(MessageSegment.image(push_msg))
         else:
             await matcher.send(push_msg)
-        if return_msg == 'add':
-            await matcher.send(f'已添加群定时任务【{msg}】{l4_config.l4_push_times}次')
-        elif return_msg in ['update','change']:
-            await matcher.send(f'已更新群定时任务【{msg}】{l4_config.l4_push_times}次')
+        if return_msg == "add":
+            await matcher.send(f"已添加群定时任务【{msg}】{l4_config.l4_push_times}次")
+        elif return_msg in ["update", "change"]:
+            await matcher.send(f"已更新群定时任务【{msg}】{l4_config.l4_push_times}次")
+
 
 @del_rss.handle()
-async def _(event:GroupMessageEvent , matcher:Matcher):
+async def _(event: GroupMessageEvent, matcher: Matcher):
     group_id = event.group_id
-    await add_or_update_data(group_id, '' , ad_mode= 'del')
-    await matcher.finish('已删除群定时任务')
+    await add_or_update_data(group_id, "", ad_mode="del")
+    await matcher.finish("已删除群定时任务")
 
 
-
-async def add_or_update_data(group_id:int, some_str :str = '',ad_mode :str = 'add'):
+async def add_or_update_data(group_i: int, some_str: str = "", ad_mode: str = "add"):
     """添加或者删除定时任务
     mode == [new,update,del,change]
     """
-    group_id = str(group_id)
-    sch_json = Path('data/L4D2/scheduler.json')
-    if ad_mode == 'add':
+    group_id = str(group_i)
+    sch_json = Path("data/L4D2/scheduler.json")
+    if ad_mode == "add":
         if sch_json.exists():
-            with sch_json.open(encoding='utf-8') as f:
+            with sch_json.open(encoding="utf-8") as f:
                 scheduler_data = json.load(f)
             try:
                 msg_dict = scheduler_data[group_id]
-                times = msg_dict['times'] 
-                old_msg = msg_dict['msg']
+                times = msg_dict["times"]
+                old_msg = msg_dict["msg"]
                 scheduler_data[group_id] = {
-                    'times' :l4_config.l4_push_times, 
-                    'msg' :some_str
-                    }
+                    "times": l4_config.l4_push_times,
+                    "msg": some_str,
+                }
                 if old_msg == some_str:
-                    mode = 'update' 
+                    mode = "update"
                 else:
-                    mode = 'change'
+                    mode = "change"
             except:
                 scheduler_data[group_id] = {
-                    'times' :l4_config.l4_push_times, 
-                    'msg' :some_str
-                    }
-                mode = 'new'
+                    "times": l4_config.l4_push_times,
+                    "msg": some_str,
+                }
+                mode = "new"
 
         else:
-            scheduler_data = {group_id: {
-                    'times' :l4_config.l4_push_times, 
-                    'msg' :some_str
-                    }}
-            mode = 'new'
-            
-        with sch_json.open('w',encoding='utf-8') as f:
-            json.dump(scheduler_data, f ,ensure_ascii=False)
-    
+            scheduler_data = {
+                group_id: {"times": l4_config.l4_push_times, "msg": some_str}
+            }
+            mode = "new"
+
+        with sch_json.open("w", encoding="utf-8") as f:
+            json.dump(scheduler_data, f, ensure_ascii=False)
+
     else:
         if sch_json.exists():
             with sch_json.open() as f:
-                scheduler_data:Dict[str,Dict[str,Union[str,int]]] = json.load(f)
+                scheduler_data: Dict[str, Dict[str, Union[str, int]]] = json.load(f)
             try:
                 msg_dict = scheduler_data[group_id]
-                times = msg_dict['times'] 
-                old_msg = msg_dict['msg'] 
-                scheduler_data[group_id] = {
-                    'times' :0, 
-                    'msg' :old_msg
-                    }
-            except:      
-                scheduler_data[group_id] = {
-                    'times' :0, 
-                    'msg' :some_str
-                    }
+                times = msg_dict["times"]
+                old_msg = msg_dict["msg"]
+                scheduler_data[group_id] = {"times": 0, "msg": old_msg}
+            except:
+                scheduler_data[group_id] = {"times": 0, "msg": some_str}
         else:
-            scheduler_data = {group_id: {
-                    'times' :0, 
-                    'msg' :some_str
-                    }}
-        mode = 'del'
-            
-        with sch_json.open('w',encoding='utf-8') as f:
-            json.dump(scheduler_data, f ,ensure_ascii=False)  
-            
+            scheduler_data = {group_id: {"times": 0, "msg": some_str}}
+        mode = "del"
+
+        with sch_json.open("w", encoding="utf-8") as f:
+            json.dump(scheduler_data, f, ensure_ascii=False)
+
     return mode
 
+
 async def rss_ip():
     """推送一次"""
-    sch_json = Path('data/L4D2/scheduler.json')
-    
+    sch_json = Path("data/L4D2/scheduler.json")
+
     if sch_json.exists():
-        with sch_json.open(encoding='utf-8') as f:
-            scheduler_data:Dict[str,Dict[str,Union[int,str]]] = json.load(f)
-            
+        with sch_json.open(encoding="utf-8") as f:
+            scheduler_data: Dict[str, Dict[str, Union[int, str]]] = json.load(f)
+
             for key, value in scheduler_data.items():
                 try:
                     recipient_id = int(key)
-                    count = value['times']
-                    msg = value['msg']
-        
+                    count = value["times"]
+                    msg = value["msg"]
+
                     if count > 0:
-                        msg_read = await send_message(recipient_id, msg ,value)
+                        msg_read = await send_message(recipient_id, msg, value)
                         print(msg_read)
                         if msg_read:
-                            scheduler_data[key]['ip_detail']  = msg_read
+                            scheduler_data[key]["ip_detail"] = msg_read
                         count -= 1
-                    
-                    scheduler_data[key]['times'] = count
+
+                    scheduler_data[key]["times"] = count
                 except TypeError:
                     continue
-                
-        with sch_json.open(mode='w',encoding='utf-8') as f:
-            json.dump(scheduler_data, f ,ensure_ascii=False)
-        
-async def send_message(recipient_id :int, msg :str ,value :Dict[str,Union[int,str]] = None):
+
+        with sch_json.open(mode="w", encoding="utf-8") as f:
+            json.dump(scheduler_data, f, ensure_ascii=False)
+
+
+async def send_message(
+    recipient_id: int, msg: str, value: Dict[str, Union[int, str]] = None
+):
     # 执行发送消息的操作，参数可以根据需要进行传递和使用
-    command,message = await extract_last_digit(msg)
-    push_msg =  await get_ip_to_mes(msg= message,  command= command)
-    if isinstance(push_msg ,bytes):
-        await get_bot().send_group_msg(group_id=recipient_id, message=MessageSegment.image(push_msg))
-    elif msg and isinstance(push_msg ,str):
+    command, message = await extract_last_digit(msg)
+    push_msg = await get_ip_to_mes(msg=message, command=command)
+    if isinstance(push_msg, bytes):
+        await get_bot().send_group_msg(
+            group_id=recipient_id, message=MessageSegment.image(push_msg)
+        )
+    elif msg and isinstance(push_msg, str):
         # 单服务器
-        message = await json_server_to_tag_dict(msg,command)
+        message = await json_server_to_tag_dict(msg, command)
         if len(message) == 0:
             # 关键词不匹配，忽略
             return
         try:
-            old_msg = value.get('ip_detail',{})
-            ip = str(message['ip'])
-            host,port = split_maohao(ip)
-            msg:a2s.SourceInfo = await a2s.ainfo((host,port))
-            value['map_'] = msg.map_name
-            value['rank_players'] = f'{msg.player_count}/{msg.max_players}'
-            if old_msg['map_'] == value['map_'] and old_msg['rank_players'] == value['rank_players']:
-                logger.info(f'{msg}{command}人数和地图未发生变化')
+            old_msg = value.get("ip_detail", {})
+            ip = str(message["ip"])
+            host, port = split_maohao(ip)
+            msg: a2s.SourceInfo = await a2s.ainfo((host, port))
+            value["map_"] = msg.map_name
+            value["rank_players"] = f"{msg.player_count}/{msg.max_players}"
+            if (
+                old_msg["map_"] == value["map_"]
+                and old_msg["rank_players"] == value["rank_players"]
+            ):
+                logger.info(f"{msg}{command}人数和地图未发生变化")
             else:
                 await get_bot().send_group_msg(group_id=recipient_id, message=push_msg)
         except Exception as e:
             logger.warning(e)
-            
+
         return value
-    
+
+
 async def server_is_change():
-    """检测服务器是否发生变化""" 
-    
+    """检测服务器是否发生变化"""
+
+
 @driver.on_bot_connect
-async def _():    
-    logger.success('已成功启动求生定时推送')
-    scheduler.add_job(rss_ip, "interval", minutes=l4_config.l4_push_interval, id="rss_ip")
-    
+async def _():
+    logger.success("已成功启动求生定时推送")
+    scheduler.add_job(
+        rss_ip, "interval", minutes=l4_config.l4_push_interval, id="rss_ip"
+    )
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,113 +1,122 @@
 import a2s
 from typing import List
 
-async def queries(ip:str,port:int):
+
+async def queries(ip: str, port: int):
     port = int(port)
-    msg_dict = await queries_dict(ip,port)
-    print(msg_dict['name'],type(msg_dict['name']))
+    msg_dict = await queries_dict(ip, port)
+    print(msg_dict["name"], type(msg_dict["name"]))
     message = f"名称：{msg_dict['name']}\n"
     message += f"地图：{msg_dict['map_']}\n"
     message += f"延迟：{msg_dict['ping']}\n"
     message += f"玩家：{msg_dict['players']} / {msg_dict['max_players']}\n"
     return message
 
-async def queries_dict(ip:str,port:int) -> dict:
+
+async def queries_dict(ip: str, port: int) -> dict:
     port = int(port)
     ip = str(ip)
     msg_dict = {}
     # message_dict = await l4d(ip,port)
-    msg:a2s.SourceInfo = await a2s.ainfo((ip,port))
-    msg_dict['folder'] =  msg.folder
-    msg_dict['name'] =  msg.server_name
-    msg_dict['map_'] =  msg.map_name
-    msg_dict['players'] =  msg.player_count
-    msg_dict['max_players'] =  msg.max_players
-    msg_dict['rank_players'] =  f'{msg.player_count}/{msg.max_players}'
-    msg_dict['ip'] = str(ip) + ':' +str(port)
-    msg_dict['ping'] = f"{msg.ping*1000:.0f}ms"
-    msg_dict['system'] =  f"{msg.platform}.svg"
-    if msg_dict['players'] < msg_dict['max_players']:
-        msg_dict['enabled'] = True
+    msg: a2s.SourceInfo = await a2s.ainfo((ip, port))  # type: ignore
+    msg_dict["folder"] = msg.folder
+    msg_dict["name"] = msg.server_name
+    msg_dict["map_"] = msg.map_name
+    msg_dict["players"] = msg.player_count
+    msg_dict["max_players"] = msg.max_players
+    msg_dict["rank_players"] = f"{msg.player_count}/{msg.max_players}"
+    msg_dict["ip"] = str(ip) + ":" + str(port)
+    msg_dict["ping"] = f"{msg.ping*1000:.0f}ms"
+    msg_dict["system"] = f"{msg.platform}.svg"
+    if msg_dict["players"] < msg_dict["max_players"]:
+        msg_dict["enabled"] = True
     else:
-        msg_dict['enabled'] = False
+        msg_dict["enabled"] = False
     return msg_dict
-    
-async def player_queries_anne_dict(ip:str,port:int): 
+
+
+async def player_queries_anne_dict(ip: str, port: int):
     """anne算法返回玩家"""
     port = int(port)
     # message_dic = await l4d2.APlayer(ip,port,times=5)
-    message_list:List[a2s.Player] = await a2s.aplayers((ip,port))
+    message_list: List[a2s.Player] = await a2s.aplayers((ip, port))  # type: ignore
     msg_list = []
     if message_list != []:
         for i in message_list:
-            msg_list.append({
-                'name':i.name,
-                'Score':i.score,
-                'Duration':await convert_duration(i.duration)
-            })
+            msg_list.append(
+                {
+                    "name": i.name,
+                    "Score": i.score,
+                    "Duration": await convert_duration(i.duration),
+                }
+            )
     return msg_list
 
-# async def player_queries_dict(ip:str,port:int): 
+
+# async def player_queries_dict(ip:str,port:int):
 #     """一般算法返回玩家"""
 #     port = int(port)
 #     new_dict = {}
 #     message_dic = await l4d2.APlayer(ip,port,times=5)
 #     if message_dic == {}:
 #         new_dict['header'] = 0
 #     else:
 #         pass
 #         new_list = []
 #         for i in message_dic['Players']:
 #             new_list.append(i['Name'])
 #         new_dict.update({'Players':new_list})
 #     return new_dict
 
-async def player_queries(ip:str,port:int): 
+
+async def player_queries(ip: str, port: int):
     port = int(port)
-    message_list = await player_queries_anne_dict(ip,port)
+    message_list = await player_queries_anne_dict(ip, port)
     return await msg_ip_to_list(message_list)
 
-async def msg_ip_to_list(message_list:list):
-    message = ''
+
+async def msg_ip_to_list(message_list: list):
+    message = ""
     n = 0
     if message_list == []:
-        message += '服务器里，是空空的呢\n'
+        message += "服务器里，是空空的呢\n"
     else:
-        max_duration_len = max([len(str(i['Duration'])) for i in message_list])
-        max_score_len = max([len(str(i['Score'])) for i in message_list])
+        max_duration_len = max([len(str(i["Duration"])) for i in message_list])
+        max_score_len = max([len(str(i["Score"])) for i in message_list])
         for i in message_list:
             print(i)
-            n += 1 
-            name = i['name']
-            Score = i['Score']
-            if Score == '0':
-                Score = '摸'
-            Duration = i['Duration']
-            soc = "[{:>{}}]".format(Score,max_score_len)
+            n += 1
+            name = i["name"]
+            Score = i["Score"]
+            if Score == "0":
+                Score = "摸"
+            Duration = i["Duration"]
+            soc = "[{:>{}}]".format(Score, max_score_len)
             dur = "{:^{}}".format(Duration, max_duration_len)
-            message += f'{soc} | {dur} | {name} \n'
+            message += f"{soc} | {dur} | {name} \n"
     return message
 
-async def convert_duration(duration: int) -> str:
+
+async def convert_duration(duration: float) -> str:
     minutes, seconds = divmod(duration, 60)
     hours, minutes = divmod(minutes, 60)
     time_str = ""
     if hours > 0:
         time_str += f"{int(hours)}h "
     if minutes > 0 or hours > 0:
         time_str += f"{int(minutes)}m "
     time_str += f"{int(seconds)}s"
     return time_str.strip()
 
-async def server_rule_dict(ip:str,port:int): 
+
+async def server_rule_dict(ip: str, port: int):
     port = int(port)
     ip = str(ip)
     msg_dict = {}
     # message_dict = await l4d(ip,port)
     try:
-        msg:dict = await a2s.arules((ip,port))
-        msg_dict['tick'] = msg['l4d2_tickrate_enabler'] + "tick"
+        msg: dict = await a2s.arules((ip, port))  # type: ignore
+        msg_dict["tick"] = msg["l4d2_tickrate_enabler"] + "tick"
     except:
-        msg_dict['tick'] = ''
+        msg_dict["tick"] = ""
     return msg_dict
-
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 #         except:
 #             pass
 #         print(file.json())
 #         return file.json()
 #     elif mode == 'first':
 #         ip_tag:list = file.json()
 #         return ip_tag
-        
+
 
 # async def map_dict_to_str(data:List[dict]):
 #     msg = ""
 #     for key,value in data[0].items():
 #         if key == "url":
 #             continue
 #         msg += f"{key}:{value}\n"
 #     return msg
-
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 try:
-        import ujson as json
+    import ujson as json
 except:
-        import json
+    import json
 from pathlib import Path
-from typing import Dict,List
+from typing import Dict, List
 import os
 
 BOT_DIR = os.path.dirname(os.path.abspath(__file__))
-filename = 'data/L4D2/l4d2.json'
-global_file = Path(Path(__file__).parent.parent,filename)
+filename = "data/L4D2/l4d2.json"
+global_file = Path(Path(__file__).parent.parent, filename)
+
+
 def load_josn():
-        # 本地模块
-        try:
-                LOCAL_HOST:dict = json.load(open(
-                filename, "r", encoding="utf8"))
-        except IOError or FileNotFoundError:
-                os.makedirs(os.path.dirname(filename), exist_ok=True)
-                data = {}
-                with open(filename, "w") as f:
-                        json.dump(data, f)
-                LOCAL_HOST:dict = {}
-        try:
-                # 获取所有json文件的路径
-                json_files = Path('data/L4D2/l4d2').glob('*.json')
-
-                # 将所有json文件中的字典对象合并为一个字典
-                for file_path in json_files:
-                        with open(file_path, 'r', encoding='utf-8') as f:
-                                LOCAL_HOST.update(json.load(f))
-        except:
-                pass
-        return LOCAL_HOST
+    # 本地模块
+    try:
+        LOCAL_HOST: dict = json.load(open(filename, "r", encoding="utf8"))
+    except IOError or FileNotFoundError:
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+        data = {}
+        with open(filename, "w") as f:
+            json.dump(data, f)
+        LOCAL_HOST: dict = {}
+    try:
+        # 获取所有json文件的路径
+        json_files = Path("data/L4D2/l4d2").glob("*.json")
+
+        # 将所有json文件中的字典对象合并为一个字典
+        for file_path in json_files:
+            with open(file_path, "r", encoding="utf-8") as f:
+                LOCAL_HOST.update(json.load(f))
+    except:
+        pass
+    return LOCAL_HOST
+
 
-ALL_HOST:Dict[str, List[dict]] = load_josn()
+ALL_HOST: Dict[str, List[dict]] = load_josn()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,295 +1,346 @@
 from ..l4d2_data.serverip import L4D2Server
 from ..l4d2_image import server_ip_pic
-from . import queries,player_queries,queries_dict,player_queries_anne_dict,msg_ip_to_list,server_rule_dict
+from . import (
+    queries,
+    player_queries,
+    queries_dict,
+    player_queries_anne_dict,
+    msg_ip_to_list,
+    server_rule_dict,
+)
 from nonebot.log import logger
 import random
 import asyncio
-import re
-from ..l4d2_utils.message import PRISON,QUEREN,KAILAO
+from ..l4d2_utils.message import PRISON, QUEREN, KAILAO
 from .ohter import ALL_HOST
-from typing import List,Dict
+from typing import List, Dict, Any
+
 try:
     import ujson as json
 except:
     import json
 si = L4D2Server()
-errors = (ConnectionRefusedError,ConnectionResetError,asyncio.exceptions.TimeoutError,OSError)
+errors = (
+    ConnectionRefusedError,
+    ConnectionResetError,
+    asyncio.exceptions.TimeoutError,
+    OSError,
+)
 # errors = (TypeError,KeyError,ValueError,ConnectionResetError,TimeoutError)
 
+
 async def get_qqgroup_ip_msg(qqgroup):
     """首先，获取qq群订阅数据，再依次queries返回ip原标"""
     ip_list = await si.query_server_ip(qqgroup)
     return ip_list
-    
-async def bind_group_ip(group:int,host:str,port:int):
+
+
+async def bind_group_ip(group: int, host: str, port: int):
     ip_list = await si.query_server_ip(group)
-    if (host,port) in ip_list:
+    if (host, port) in ip_list:
         return "本群已添加过该ip辣"
-    await si.bind_server_ip(group,host,port)
+    await si.bind_server_ip(group, host, port)
     return "绑定成功喵，新增ip" + host
 
-async def del_group_ip(group:int,number:int):
+
+async def del_group_ip(group: int, number: int):
     number = int(number)
     logger.info(number)
     try:
-        groups,host,port = await si.query_number(number)
+        groups, host, port = await si.query_number(number)
     except TypeError:
-        return '没有这个序号哦'
+        return "没有这个序号哦"
     if groups != group:
         return "本群可没有订阅过这个ip"
     await si.del_server_ip(number)
     return "取消成功喵，已删除序号" + str(number)
-        
-async def qq_ip_queries(msg:List[tuple]):
+
+
+async def qq_ip_queries(msg: List[tuple]):
     """输入一个ip的二元元组组成的列表，返回一个输出消息的列表
     未来作图这里重置"""
     messsage = ""
     for i in msg:
-        number,qqgroup,host,port = i
-        msg2 = await player_queries(host,port)
-        msg1 = await queries(host,port)
-        messsage += '序号、'+ str(number) + '\n' + msg1 + msg2 + '--------------------\n'
+        number, qqgroup, host, port = i
+        msg2 = await player_queries(host, port)
+        msg1 = await queries(host, port)
+        messsage += "序号、" + str(number) + "\n" + msg1 + msg2 + "--------------------\n"
     return messsage
-            
-            
-async def qq_ip_querie(msg: list,igr:bool = True):
+
+
+async def qq_ip_querie(msg: list, igr: bool = True):
     msg_list = []
     tasks = []  # 用来保存异步任务
     if msg != []:
         for i in msg:
             try:
-                number, host, port = i
-                qqgroup = ''
-            except ValueError:
-                number, qqgroup, host, port = i
-            finally:
+                number: str
+                host: str
+                port: int
+                qqgroup: str = ""  # 初始化为""
+                if len(i) == 3:
+                    number, host, port = i
+                else:
+                    number, qqgroup, host, port = i
                 # 将异步任务添加到任务列表中
-                tasks.append(asyncio.create_task(process_message(number, host, port, msg_list,qqgroup,igr)))
+                tasks.append(
+                    asyncio.create_task(
+                        process_message(
+                            number,
+                            host,
+                            port,
+                            msg_list,
+                            igr,
+                            qqgroup,
+                        )
+                    )
+                )
+            except ValueError:
+                continue  # 处理异常情况
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
-        msg_list.sort(key=lambda x: x['number'])
+        msg_list.sort(key=lambda x: x["number"])
         for i in msg_list:
             print(i)
             break
-        result = {'msg_list': msg_list}
+        result = {"msg_list": msg_list}
 
     else:
         result = {}
     return result
 
 
-async def qq_ip_queries_pic(msg: list,igr = False):
-    result = await qq_ip_querie(msg,igr)
+async def qq_ip_queries_pic(msg: list, igr=False):
+    result = await qq_ip_querie(msg, igr)
     print(result)
-    if 'msg_list' in result:
-        pic = await server_ip_pic(result['msg_list'])
+    if "msg_list" in result:
+        pic = await server_ip_pic(result["msg_list"])
     else:
         pic = None
     return pic
-            
 
 
-
-async def process_message(number, host, port, msg_list:list,igr:bool,qqgroup = ''):
+async def process_message(
+    number: str,
+    host: str,
+    port: int,
+    msg_list: List[Dict[str, Any]],
+    igr: bool,
+    qqgroup: str = "",
+):
     try:
         msg2 = await player_queries_anne_dict(host, port)
         msg1 = await queries_dict(host, port)
         msg3 = await server_rule_dict(host, port)
-        msg1.update({'Players':msg2,'number':number,})
+        msg1.update(
+            {
+                "Players": msg2,
+                "number": number,
+            }
+        )
         msg1.update(msg3)
         if qqgroup:
-            msg1.update({'tag':qqgroup})
+            msg1.update({"tag": qqgroup})
         msg_list.append(msg1)
     except errors:
         if igr:
             pass
         else:
             # 空白字典
-            null_dict = {key: 'null' for key in ['name', 'map_', 'players', 'max_players', 'rank_players', 'ping']}
-            null_dict.update({'number':number,'ip':f'{host}:{port}','Players':[]})
-            msg_list.append(null_dict)  
+            null_dict = {
+                key: "null"
+                for key in [
+                    "name",
+                    "map_",
+                    "players",
+                    "max_players",
+                    "rank_players",
+                    "ping",
+                ]
+            }
+            null_dict.update({"number": number, "ip": f"{host}:{port}", "Players": []})  # type: ignore
+            msg_list.append(null_dict)
 
 
-    
-async def get_tan_jian(msg:List[tuple],mode:int):
+async def get_tan_jian(msg: List[tuple], mode: int):
     """获取anne列表抽一个"""
     msg_list = []
     random.shuffle(msg)
     for i in msg:
-        number,host,port = i
+        number, host, port = i
         try:
             if mode == 1:
                 # 探监
-                msg2 = await player_queries_anne_dict(host,port)
+                msg2 = await player_queries_anne_dict(host, port)
                 point = 0
                 for i in msg2:
-                    point += int(i['Score'])
+                    point += int(i["Score"])
                 logger.info(point)
-                msg1 = await queries_dict(host,port)
-                sp:str = msg1['name']
-                if '特' not in sp:
+                msg1 = await queries_dict(host, port)
+                sp: str = msg1["name"]
+                if "特" not in sp:
                     continue
-                sp = int(sp.split('特')[0].split('[')[-1])
-                points = point/4
-                if points/sp <10:
+                sps = int(sp.split("特")[0].split("[")[-1])
+                points = point / 4
+                if points / sps < 10:
                     continue
-                if 'HT' in msg1['name']:
+                if "HT" in msg1["name"]:
                     continue
-                msg1.update({'Players':msg2})
-                msg1.update({'ranks':point})
-                ips = f'{host}:{str(port)}'
-                msg1.update({'ips':ips})
+                msg1.update({"Players": msg2})
+                msg1.update({"ranks": point})
+                ips = f"{host}:{str(port)}"
+                msg1.update({"ips": ips})
                 # msg1是一行数据完整的字典
                 msg_list.append(msg1)
             if mode == 2:
                 # 坐牢
                 # try:
-                msg1 = await queries_dict(host,port)
-                if '普通药役' in msg1['name']:
-                    if '缺人' in msg1['name']:
-                        msg2 = await player_queries_anne_dict(host,port)
-                        msg1.update({'Players':msg2})
-                        ips = f'{host}:{str(port)}'
-                        msg1.update({'ips':ips})
+                msg1 = await queries_dict(host, port)
+                if "普通药役" in msg1["name"]:
+                    if "缺人" in msg1["name"]:
+                        msg2 = await player_queries_anne_dict(host, port)
+                        msg1.update({"Players": msg2})
+                        ips = f"{host}:{str(port)}"
+                        msg1.update({"ips": ips})
                         # msg1是一行数据完整的字典
                     else:
                         continue
                 else:
                     continue
                 msg_list.append(msg1)
             if mode == 3:
                 # 开牢
-                msg1 = await queries_dict(host,port)
-                if '[' not in msg1['name']:
-                    msg2 = await player_queries_anne_dict(host,port)
-                    msg1.update({'Players':msg2})
-                    ips = f'{host}:{str(port)}'
-                    msg1.update({'ips':ips})
+                msg1 = await queries_dict(host, port)
+                if "[" not in msg1["name"]:
+                    msg2 = await player_queries_anne_dict(host, port)
+                    msg1.update({"Players": msg2})
+                    ips = f"{host}:{str(port)}"
+                    msg1.update({"ips": ips})
                     # msg1是一行数据完整的字典
                     msg_list.append(msg1)
         except errors:
             continue
         if msg_list != []:
             break
     # 随机选一个牢房
     logger.info(msg_list)
     if len(msg_list) == 0:
-        return '暂时没有这种牢房捏'
+        return "暂时没有这种牢房捏"
     logger.info(len(msg_list))
     mse = msg_list[0]
-    message:str = ''
+    message: str = ""
     if mode == 1:
-        ranks = mse['ranks']
-        if ranks <= 300 :
+        ranks = mse["ranks"]
+        if ranks <= 300:
             message = random.choice(PRISON[1])
-        if 300 < ranks <= 450 :
+        if 300 < ranks <= 450:
             message = random.choice(PRISON[2])
-        if ranks > 450 :
-            message = random.choice(PRISON[3]) 
+        if ranks > 450:
+            message = random.choice(PRISON[3])
     if mode == 2:
-        player_point = mse['players']
-        if player_point == '1':
+        player_point = mse["players"]
+        if player_point == "1":
             message = random.choice(QUEREN[1])
-        elif player_point == '2':
+        elif player_point == "2":
             message = random.choice(QUEREN[2])
-        elif player_point == '3':
+        elif player_point == "3":
             message = random.choice(QUEREN[3])
         else:
             message = random.choice(QUEREN[4])
     if mode == 3:
         message = random.choice(KAILAO)
-    message += '\n' + '名称：' + mse['name'] + '\n'
-    message += '地图：' + mse['map_'] + '\n'
+    message += "\n" + "名称：" + mse["name"] + "\n"
+    message += "地图：" + mse["map_"] + "\n"
     message += f"玩家：{mse['players']} / {mse['max_players']}\n"
-    print(mse['Players'])
+    print(mse["Players"])
     try:
-        message += await msg_ip_to_list(mse['Players'])
+        message += await msg_ip_to_list(mse["Players"])
     except (KeyError):
-        message += '服务器里，是空空的呢\n'
+        message += "服务器里，是空空的呢\n"
     return message
 
 
-
 async def get_server_ip(number):
-    group,host,port = await si.query_number(number)
+    group, host, port = await si.query_number(number)
     try:
-        return str(host) + ':' + str(port)
+        return str(host) + ":" + str(port)
     except TypeError:
         return None
 
-def split_maohao(msg:str) -> list:
+
+def split_maohao(msg: str) -> list:
     """分割大小写冒号"""
-    if ':' in msg:
-        msg:list = msg.split(':')
-    elif '：' in msg:
-        msg:list = msg.split('：')
-    elif msg.replace('.','').isdigit():
-        msg:List[str] = [msg,'20715']
+    if ":" in msg:
+        msgs: List[str] = msg.split(":")
+    elif "：" in msg:
+        msgs: List[str] = msg.split("：")
+    elif msg.replace(".", "").isdigit():
+        msgs: List[str] = [msg, "20715"]
     else:
-        pass  
-    mse = [msg[0],msg[-1]]
+        msgs = []
+    mse = [msgs[0], msgs[-1]]
     return mse
 
+
 async def write_json(data_str: str):
     """
     添加数据或者删除数据
      - 【求生更新 添加 腐竹 ip 模式 序号】
      - 【求生更新 添加 腐竹 ip 模式】
      - 【求生更新 删除 腐竹 序号】
     """
     data_list = data_str.split()
     logger.info(data_list)
     if data_list[0] == "添加":
         add_server = {}
         server_dict = ALL_HOST.get(data_list[1], {})
         if not server_dict:
-            logger.info('新建分支')
+            logger.info("新建分支")
             ALL_HOST[data_list[1]] = []
         for key, value in ALL_HOST.items():
             if data_list[1] == key:
-                ids = [server['id'] for server in value]
+                ids = [server["id"] for server in value]
                 # 序号
                 if len(data_list) == 4:
                     data_num = max(ids, default=0) + 1
-                    add_server.update({'id': data_num})
+                    add_server.update({"id": data_num})
                 elif len(data_list) == 5:
                     if not data_list[4].isdigit():
-                        return '序号应该为大于0的正整数，请输入【求生更新 添加 腐竹 ip 模式 序号】'
+                        return "序号应该为大于0的正整数，请输入【求生更新 添加 腐竹 ip 模式 序号】"
                     data_num = int(data_list[4])
                     if data_num in ids:
-                        return '该序号已存在，请尝试删除原序号【求生更新 删除 腐竹 序号】'
-                    add_server.update({'id': data_num})
+                        return "该序号已存在，请尝试删除原序号【求生更新 删除 腐竹 序号】"
+                    add_server.update({"id": data_num})
                 else:
-                    return '输入参数错误，请输入【求生更新 添加 腐竹 ip 模式 序号】或【求生更新 添加 腐竹 ip 模式】'
+                    return "输入参数错误，请输入【求生更新 添加 腐竹 ip 模式 序号】或【求生更新 添加 腐竹 ip 模式】"
                 # 模式，ip
                 try:
                     host, port = split_maohao(data_list[2])
-                    add_server.update({'host': host, 'port': port})
+                    add_server.update({"host": host, "port": port})
                 except KeyError:
-                    return 'ip格式不正确【114.11.4.514:9191】'
-                add_server.update({'version': data_list[3]})
+                    return "ip格式不正确【114.11.4.514:9191】"
+                add_server.update({"version": data_list[3]})
                 value.append(add_server)
                 ALL_HOST[key] = value
-                with open('data/L4D2/l4d2.json', 'w', encoding='utf8') as f_new:
+                with open("data/L4D2/l4d2.json", "w", encoding="utf8") as f_new:
                     json.dump(ALL_HOST, f_new, ensure_ascii=False, indent=4)
-                return f'添加成功，指令为{key}{data_num}'
-            
+                return f"添加成功，指令为{key}{data_num}"
+
     elif data_list[0] == "删除":
         for key, value in ALL_HOST.items():
             if data_list[1] == key:
                 try:
                     data_num = int(data_list[2])
                 except ValueError:
-                    return '序号应该为大于0的正整数，请输入【求生更新 删除 腐竹 序号】'
+                    return "序号应该为大于0的正整数，请输入【求生更新 删除 腐竹 序号】"
                 for i, server in enumerate(value):
-                    if data_num == server['id']:
+                    if data_num == server["id"]:
                         value.pop(i)
                         if not value:
                             ALL_HOST.pop(key)
-                        with open('data/L4D2/l4d2.json', 'w', encoding='utf8') as f_new:
+                        with open("data/L4D2/l4d2.json", "w", encoding="utf8") as f_new:
                             json.dump(ALL_HOST, f_new, ensure_ascii=False, indent=4)
-                        return '删除成功喵'
-                return '序号不正确，请输入【求生更新 删除 腐竹 序号】'
-        return '腐竹名不存在，请输入【求生更新 删除 腐竹 序号】'   
-
+                        return "删除成功喵"
+                return "序号不正确，请输入【求生更新 删除 腐竹 序号】"
+        return "腐竹名不存在，请输入【求生更新 删除 腐竹 序号】"
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,136 +8,130 @@
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, MessageSegment
 
 from ..l4d2_utils.utils import register_menu
 from ..l4d2_utils.rule import FullCommand
 from .draw_update_log import draw_update_log_img
 from .restart import restart_message, restart_genshinuid
 
-l4d_restart = on_command('l4重启', rule=FullCommand())
-get_update_log = on_command('l4更新记录', rule=FullCommand())
+l4d_restart = on_command("l4重启", rule=FullCommand())
+get_update_log = on_command("l4更新记录", rule=FullCommand())
 l4d_update = on_regex(
-    r'^(l4)(强行)?(强制)?(更新)$',
+    r"^(l4)(强行)?(强制)?(更新)$",
     block=True,
 )
 
 
 driver = get_driver()
 
 
 @driver.on_bot_connect
 async def _():
-    logger.info('检查遗留信息...')
+    logger.info("检查遗留信息...")
     bot = get_bot()
     update_log = await restart_message()
     if update_log == {}:
         return
-    if update_log['send_type'] == 'group':
+    if update_log["send_type"] == "group":
         await bot.call_api(
-            api='send_group_msg',
-            group_id=update_log['send_to'],
-            message=update_log['msg'],
+            api="send_group_msg",
+            group_id=update_log["send_to"],
+            message=update_log["msg"],
         )
     else:
         await bot.call_api(
-            api='send_private_msg',
-            user_id=update_log['send_to'],
-            message=update_log['msg'],
+            api="send_private_msg",
+            user_id=update_log["send_to"],
+            message=update_log["msg"],
         )
-    logger.info('遗留信息检查完毕!')
+    logger.info("遗留信息检查完毕!")
 
 
 @get_update_log.handle()
 @register_menu(
-    '更新记录',
-    '更新记录',
-    '查看插件最近的更新记录',
+    "更新记录",
+    "更新记录",
+    "查看插件最近的更新记录",
     detail_des=(
-        '介绍：\n'
-        '查看插件最近的有效Git更新记录\n'
-        ' \n'
-        '指令：\n'
-        '- <ft color=(238,120,0)>更新记录</ft>'
+        "介绍：\n" "查看插件最近的有效Git更新记录\n" " \n" "指令：\n" "- <ft color=(238,120,0)>更新记录</ft>"
     ),
 )
 async def send_updatelog_msg(
     matcher: Matcher,
 ):
     im = await draw_update_log_img(is_update=False)
-    logger.info('正在执行[更新记录]...')
+    logger.info("正在执行[更新记录]...")
     if isinstance(im, str):
         await matcher.finish(im)
     elif isinstance(im, bytes):
         await matcher.finish(MessageSegment.image(im))
     else:
-        await matcher.finish('发生了未知错误,请联系管理员检查后台输出!')
+        await matcher.finish("发生了未知错误,请联系管理员检查后台输出!")
 
 
 @l4d_restart.handle()
 @register_menu(
-    '重启Bot',
-    'l4重启',
-    '重启Bot框架',
-    trigger_method='超级用户指令',
-    detail_des=(
-        '介绍：\n' '重启Bot框架\n' ' \n' '指令：\n' '- <ft color=(238,120,0)>l4重启</ft>'
-    ),
+    "重启Bot",
+    "l4重启",
+    "重启Bot框架",
+    trigger_method="超级用户指令",
+    detail_des=("介绍：\n" "重启Bot框架\n" " \n" "指令：\n" "- <ft color=(238,120,0)>l4重启</ft>"),
 )
 async def send_restart_msg(
     bot: Bot,
     event: MessageEvent,
     matcher: Matcher,
 ):
     if not await SUPERUSER(bot, event):
         return
-    logger.warning('开始执行[重启]')
+    logger.warning("开始执行[重启]")
     qid = event.user_id
-    if len(event.get_session_id().split('_')) == 3:
-        send_id = event.get_session_id().split('_')[1]
-        send_type = 'group'
+    if len(event.get_session_id().split("_")) == 3:
+        send_id = event.get_session_id().split("_")[1]
+        send_type = "group"
     else:
         send_id = qid
-        send_type = 'private'
-    await matcher.send('正在执行[l4重启]...')
+        send_type = "private"
+    await matcher.send("正在执行[l4重启]...")
     await restart_genshinuid(send_type, str(send_id))
 
 
 @l4d_update.handle()
 @register_menu(
-    '更新插件',
-    'l4更新',
-    '手动更新插件',
+    "更新插件",
+    "l4更新",
+    "手动更新插件",
     detail_des=(
-        '介绍：\n'
-        '手动更新插件（执行 git pull）\n'
-        '每加上一个可选参数，执行等级加1\n'
-        '当执行等级≥1时会还原上次更改，等级≥2时会清空暂存\n'
-        ' \n'
-        '指令：\n'
-        '- <ft color=(238,120,0)>l4d</ft>'
-        '<ft color=(125,125,125)>(强行)(强制)</ft>'
-        '<ft color=(238,120,0)>更新</ft>'
+        "介绍：\n"
+        "手动更新插件（执行 git pull）\n"
+        "每加上一个可选参数，执行等级加1\n"
+        "当执行等级≥1时会还原上次更改，等级≥2时会清空暂存\n"
+        " \n"
+        "指令：\n"
+        "- <ft color=(238,120,0)>l4d</ft>"
+        "<ft color=(125,125,125)>(强行)(强制)</ft>"
+        "<ft color=(238,120,0)>更新</ft>"
     ),
 )
 async def send_update_msg(
     bot: Bot,
     event: MessageEvent,
     matcher: Matcher,
     args: Tuple[Any, ...] = RegexGroup(),
 ):
     if not await SUPERUSER(bot, event):
         return
 
-    logger.info('[l4更新] 正在执行 ...')
+    logger.info("[l4更新] 正在执行 ...")
     level = 2
     if args[1] is None:
         level -= 1
     if args[2] is None:
         level -= 1
-    logger.info(f'[l4更新] 更新等级为{level}')
-    await matcher.send(f'开始执行[l4更新], 执行等级为{level}')
+    logger.info(f"[l4更新] 更新等级为{level}")
+    await matcher.send(f"开始执行[l4更新], 执行等级为{level}")
     im = await draw_update_log_img(level)
     if isinstance(im, str):
         await matcher.finish(im)
     elif isinstance(im, bytes):
         await matcher.finish(MessageSegment.image(im))
     else:
-        await matcher.finish('发生了未知错误,请联系管理员检查后台输出!')
+        await matcher.finish("发生了未知错误,请联系管理员检查后台输出!")
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from pathlib import Path
 from typing import Union
 
 # from PIL import Image, ImageDraw
 
 from .update import update_from_git
+
 # from ..l4d2_image.image import convert_img
 # from ..l4d2_image.image import get_color_bg
 # from ..utils.genshin_fonts.genshin_fonts import genshin_font_origin
 
 R_PATH = Path(__file__).parent
-TEXT_PATH = R_PATH / 'texture2d'
+TEXT_PATH = R_PATH / "texture2d"
 
 # gs_font_30 = genshin_font_origin(30)
 black_color = (24, 24, 24)
 
 log_config = {
-    'key': '✨🐛🎨⚡🍱♻️',
-    'num': 18,
+    "key": "✨🐛🎨⚡🍱♻️",
+    "num": 18,
 }
 
-log_map = {'✨': 'feat', '🐛': 'bug', '🍱': 'bento', '⚡️': 'zap', '🎨': 'art'}
+log_map = {"✨": "feat", "🐛": "bug", "🍱": "bento", "⚡️": "zap", "🎨": "art"}
 
 
 async def draw_update_log_img(
     level: int = 0,
     repo_path: Union[str, Path, None] = None,
     is_update: bool = True,
 ) -> Union[bytes, str]:
     log_list = await update_from_git(level, repo_path, log_config, is_update)
     if len(log_list) == 0:
-        return '更新失败!更多错误信息请查看控制台...\n' \
-               '>> 可以尝试使用\n' \
-               '>> [l4强制更新](危险)\n' \
-               '>> [l4强行强制更新](超级危险)!'
+        return (
+            "更新失败!更多错误信息请查看控制台...\n"
+            ">> 可以尝试使用\n"
+            ">> [l4强制更新](危险)\n"
+            ">> [l4强行强制更新](超级危险)!"
+        )
 
-    result = 'L4D2Bot 更新记录\n\n'
+    result = "L4D2Bot 更新记录\n\n"
     for log in log_list:
-        result += f'- {log}\n'
+        result += f"- {log}\n"
 
     return result
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,64 +4,64 @@
 import time
 import platform
 import subprocess
 from pathlib import Path
 
 # from ..utils.db_operation.db_operation import config_check
 
-bot_start = Path().cwd() / 'bot.py'
-restart_sh_path = Path().cwd() / 'gs_restart.sh'
-update_log_path = Path(__file__).parent / 'update_log.json'
+bot_start = Path().cwd() / "bot.py"
+restart_sh_path = Path().cwd() / "gs_restart.sh"
+update_log_path = Path(__file__).parent / "update_log.json"
 
-_restart_sh = '''#!/bin/bash
+_restart_sh = """#!/bin/bash
 kill -9 {}
-{} &'''
+{} &"""
 
 
 async def get_restart_sh(extra: str) -> str:
-    args = f'{extra} {str(bot_start.absolute())}'
+    args = f"{extra} {str(bot_start.absolute())}"
     return _restart_sh.format(str(bot_start.absolute()), args)
 
 
 async def restart_genshinuid(send_type: str, send_id: str) -> None:
     # extra = ''
     # if await config_check('UsePoetry'):
     #     extra = 'poetry run '
     extra = sys.executable
     restart_sh = await get_restart_sh(extra)
     if not restart_sh_path.exists():
         with open(restart_sh_path, "w", encoding="utf8") as f:
             f.write(restart_sh)
-        if platform.system() == 'Linux':
-            os.system(f'chmod +x {str(restart_sh_path)}')
-            os.system(f'chmod +x {str(bot_start)}')
-    now_time = time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(time.time()))
+        if platform.system() == "Linux":
+            os.system(f"chmod +x {str(restart_sh_path)}")
+            os.system(f"chmod +x {str(bot_start)}")
+    now_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(time.time()))
     update_log = {
-        'type': 'restart',
-        'msg': '重启完成!',
-        'send_type': send_type,
-        'send_to': send_id,
-        'time': now_time,
+        "type": "restart",
+        "msg": "重启完成!",
+        "send_type": send_type,
+        "send_to": send_id,
+        "time": now_time,
     }
-    with open(str(update_log_path), 'w', encoding='utf-8') as f:
+    with open(str(update_log_path), "w", encoding="utf-8") as f:
         json.dump(update_log, f)
-    if platform.system() == 'Linux':
-        os.execl(str(restart_sh_path), ' ')
+    if platform.system() == "Linux":
+        os.execl(str(restart_sh_path), " ")
     else:
         pid = os.getpid()
         subprocess.Popen(
-            f'taskkill /F /PID {pid} & {extra} {bot_start}',
+            f"taskkill /F /PID {pid} & {extra} {bot_start}",
             shell=True,
         )
 
 
 async def restart_message() -> dict:
     if update_log_path.exists():
-        with open(update_log_path, 'r', encoding='utf-8') as f:
+        with open(update_log_path, "r", encoding="utf-8") as f:
             update_log = json.load(f)
         msg = f'{update_log["msg"]}\n重启时间:{update_log["time"]}'
-        update_log['msg'] = msg
+        update_log["msg"] = msg
         os.remove(update_log_path)
         os.remove(restart_sh_path)
         return update_log
     else:
         return {}
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,44 +6,44 @@
 from git.exc import GitCommandError
 
 
 async def update_from_git(
     level: int = 0,
     repo_path: Union[str, Path, None] = None,
     log_config: dict = {
-        'key': '✨🐛🎨⚡🍱♻️',
-        'num': 7,
+        "key": "✨🐛🎨⚡🍱♻️",
+        "num": 7,
     },
     is_update: bool = True,
 ) -> List[str]:
     if repo_path is None:
         repo_path = Path(__file__).parents[2]
     repo = git.Repo(repo_path)  # type: ignore
     o = repo.remotes.origin
 
     if is_update:
         # 清空暂存
         if level >= 2:
-            logger.warning('[l4更新] 正在执行 git clean --xdf')
-            repo.git.clean('-xdf')
+            logger.warning("[l4更新] 正在执行 git clean --xdf")
+            repo.git.clean("-xdf")
         # 还原上次更改
         if level >= 1:
-            logger.warning('[l4更新] 正在执行 git reset --hard')
-            repo.git.reset('--hard')
+            logger.warning("[l4更新] 正在执行 git reset --hard")
+            repo.git.reset("--hard")
 
         try:
             pull_log = o.pull()
-            logger.info(f'[l4更新] {pull_log}')
+            logger.info(f"[l4更新] {pull_log}")
         except GitCommandError as e:
             logger.warning(e)
             return []
 
     commits = list(repo.iter_commits(max_count=40))
     log_list = []
     for commit in commits:
         if isinstance(commit.message, str):
-            for key in log_config['key']:
+            for key in log_config["key"]:
                 if key in commit.message:
-                    log_list.append(commit.message.replace('\n', ''))
-                    if len(log_list) >= log_config['num']:
+                    log_list.append(commit.message.replace("\n", ""))
+                    if len(log_list) >= log_config["num"]:
                         break
     return log_list
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,249 +1,281 @@
 import re
 import asyncio
 from typing import Type
 from time import sleep
 
-from nonebot import on_notice,on_command,on_regex,on_keyword
-from nonebot.params import CommandArg,RawCommand,CommandStart
+from nonebot import on_notice, on_command, on_regex, on_keyword
+from nonebot.params import CommandArg, RawCommand, CommandStart
 from nonebot.matcher import Matcher
 import nonebot
 from nonebot.adapters.onebot.v11 import (
     GroupUploadNoticeEvent,
     NoticeEvent,
     MessageEvent,
     Message,
     MessageSegment,
     GroupMessageEvent,
-    )
+)
 
-from ..l4d2_anne.server import server_key,ANNE_IP
+from ..l4d2_anne.server import server_key, ANNE_IP
 from .config import *
 from ..l4d2_queries.qqgroup import split_maohao
+
 # from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
 from .utils import *
 from .txt_to_img import mode_txt_to_img
 from ..l4d2_image.one import one_server_img
 
-help_ = on_command('l4_help',aliases={'求生帮助'},priority=20,block=True)
+help_ = on_command("l4_help", aliases={"求生帮助"}, priority=20, block=True)
 
 # 服务器
 # last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
 
 
-
-def wenjian(
-event:NoticeEvent):
+def wenjian(event: NoticeEvent):
     args = event.dict()
     try:
-        name: str = args['file']['name']
-        usr_id = str(args['user_id'])
+        name: str = args["file"]["name"]
+        usr_id = str(args["user_id"])
     except KeyError:
         return False
-    if args['notice_type'] == 'offline_file':
+    if args["notice_type"] == "offline_file":
         if l4_config.l4_master:
             return name.endswith(file_format) and usr_id in l4_config.l4_master
         else:
             return name.endswith(file_format)
-    elif args['notice_type'] == 'group_upload':
+    elif args["notice_type"] == "group_upload":
         if l4_config.l4_master:
             return usr_id in l4_config.l4_master and name.endswith(file_format)
         else:
             return False
 
-up = on_notice(rule=wenjian)
 
+up = on_notice(rule=wenjian)
 
 
 rename_vpk = on_regex(
-        r"^求生地图\s*(\S+.*?)\s*(改|改名)?\s*(\S+.*?)\s*$",
-    flags=  re.S,
-    block= True,
-    priority= 20,
-    permission= Master,
+    r"^求生地图\s*(\S+.*?)\s*(改|改名)?\s*(\S+.*?)\s*$",
+    flags=re.S,
+    block=True,
+    priority=20,
+    permission=Master,
 )
 
-find_vpk = on_command("l4_map",aliases={"求生地图","查看求生地图"},priority=25,block=True)
-del_vpk = on_command("l4_del_map",aliases={"求生地图删除","地图删除"},priority=20,block=True,permission= Master)
-rcon_to_server = on_command('rcon',aliases={"求生服务器指令","服务器指令","求生服务器控制台"},block=True,permission= Master)
-check_path = on_command('l4_check',aliases={'求生路径'},priority=20,block=True,permission= Master)
-smx_file = on_command('l4_smx',aliases={'求生插件'},priority=20,block=True,permission= Master)
+find_vpk = on_command("l4_map", aliases={"求生地图", "查看求生地图"}, priority=25, block=True)
+del_vpk = on_command(
+    "l4_del_map", aliases={"求生地图删除", "地图删除"}, priority=20, block=True, permission=Master
+)
+rcon_to_server = on_command(
+    "rcon", aliases={"求生服务器指令", "服务器指令", "求生服务器控制台"}, block=True, permission=Master
+)
+check_path = on_command(
+    "l4_check", aliases={"求生路径"}, priority=20, block=True, permission=Master
+)
+smx_file = on_command(
+    "l4_smx", aliases={"求生插件"}, priority=20, block=True, permission=Master
+)
 
 # anne
-anne_player = on_command('Ranne',aliases={"求生anne"},priority=25,block=True)
-anne_bind = on_command('Rbind',aliases={'steam绑定','求生绑定','anne绑定'},priority=20,block=True)
-del_bind = on_command('del_bind',aliases={'steam解绑','求生解绑','anne解绑'},priority=20,block=True)
-prison = on_command('zl',aliases={'坐牢'},priority=20,block=True)
-open_prison = on_command('kl',aliases={'开牢'},priority=20,block=True)
+anne_player = on_command("Ranne", aliases={"求生anne"}, priority=25, block=True)
+anne_bind = on_command(
+    "Rbind", aliases={"steam绑定", "求生绑定", "anne绑定"}, priority=20, block=True
+)
+del_bind = on_command(
+    "del_bind", aliases={"steam解绑", "求生解绑", "anne解绑"}, priority=20, block=True
+)
+prison = on_command("zl", aliases={"坐牢"}, priority=20, block=True)
+open_prison = on_command("kl", aliases={"开牢"}, priority=20, block=True)
 
 # updata = on_command('updata',aliases={'求生更新'},priority=20,block=True,permission= Master)
-tan_jian = on_command('tj',aliases={'探监'},priority=20,block=True)
+tan_jian = on_command("tj", aliases={"探监"}, priority=20, block=True)
 
 # 查询
-queries_comm = on_keyword(keywords={'queries','求生ip','求生IP','connect'},priority=20,block=True)
-add_queries = on_command('addq',aliases={"求生添加订阅"},priority=20,block=True,permission= Master)
-del_queries = on_command('delq',aliases={"求生取消订阅"},priority=20,block=True,permission= Master)
-show_queries = on_command('showq',aliases={"求生订阅"},priority=20,block=True)
-join_server = on_command('ld_jr',aliases={"求生加入"},priority=20,block=True)
-connect_rcon = on_command("Rrcon", aliases={"求生连接", '求生链接','求生rcon'}, priority=50, block=False)
-end_connect = ['stop', '结束', '连接结束', '结束连接']
-search_api = on_command('search',aliases={'求生三方'}, priority=20, block=True,permission= Master)
-which_map = on_keyword(("是什么图"),priority=20, block=False)
-reload_ip = on_command('l4_reload',aliases={'重载ip'},priority=30,permission=Master)
+queries_comm = on_keyword(
+    keywords={"queries", "求生ip", "求生IP", "connect"}, priority=20, block=True
+)
+add_queries = on_command(
+    "addq", aliases={"求生添加订阅"}, priority=20, block=True, permission=Master
+)
+del_queries = on_command(
+    "delq", aliases={"求生取消订阅"}, priority=20, block=True, permission=Master
+)
+show_queries = on_command("showq", aliases={"求生订阅"}, priority=20, block=True)
+join_server = on_command("ld_jr", aliases={"求生加入"}, priority=20, block=True)
+connect_rcon = on_command(
+    "Rrcon", aliases={"求生连接", "求生链接", "求生rcon"}, priority=50, block=False
+)
+end_connect = ["stop", "结束", "连接结束", "结束连接"]
+search_api = on_command(
+    "search", aliases={"求生三方"}, priority=20, block=True, permission=Master
+)
+# which_map = on_keyword("是什么图"), priority=20, block=False)
+reload_ip = on_command("l4_reload", aliases={"重载ip"}, priority=30, permission=Master)
 
 # 下载内容
-up_workshop = on_command('workshop',aliases={'创意工坊下载','求生创意工坊'},priority=20,block=True)
-vtf_make = on_command('vtf_make',aliases={'求生喷漆'},priority=20,block=True)
+up_workshop = on_command(
+    "workshop", aliases={"创意工坊下载", "求生创意工坊"}, priority=20, block=True
+)
+vtf_make = on_command("vtf_make", aliases={"求生喷漆"}, priority=20, block=True)
+
 
 @help_.handle()
 async def _():
     msg = [
-        '=====求生机器人帮助=====',
-        '1、电信服战绩查询【求生anne[id/steamid/@]】',
-        '2、电信服绑定【求生绑定[id/steamid]】',
-        '3、电信服状态查询【云xx】'
-        '4、创意工坊下载【创意工坊下载[物品id/链接]】',
-        '5、指定ip查询【求生ip[ip]】(可以是域名)',
-        '6、求生喷漆制作【求生喷漆】',
-        '6、本地服务器操作(略，详情看项目地址)',
+        "=====求生机器人帮助=====",
+        "1、电信服战绩查询【求生anne[id/steamid/@]】",
+        "2、电信服绑定【求生绑定[id/steamid]】",
+        "3、电信服状态查询【云xx】" "4、创意工坊下载【创意工坊下载[物品id/链接]】",
+        "5、指定ip查询【求生ip[ip]】(可以是域名)",
+        "6、求生喷漆制作【求生喷漆】",
+        "6、本地服务器操作(略，详情看项目地址)",
     ]
-    messgae = ''
+    messgae = ""
     for i in msg:
-        messgae += i + '\n'
+        messgae += i + "\n"
     await help_.finish(messgae)
 
+
 def get_session_id(event: MessageEvent) -> str:
     if isinstance(event, GroupMessageEvent):
         return f"group_{event.group_id}"
     else:
         return f"private_{event.user_id}"
 
+
 matchers: Dict[str, List[Type[Matcher]]] = {}
 
 
-    
 async def get_des_ip():
     global ALL_HOST
     global ANNE_IP
     global matchers
-    def count_ips(ip_dict:dict):
+
+    def count_ips(ip_dict: dict):
         global ANNE_IP
         for key, value in ip_dict.items():
-            if key in ['error_','success_']:
+            if key in ["error_", "success_"]:
                 ip_dict.pop(key)
                 break
             count = len(value)
-            logger.info(f'已加载：{key} | {count}个')
-            if key == '云':
-                ANNE_IP = {key:value}
+            logger.info(f"已加载：{key} | {count}个")
+            if key == "云":
+                ANNE_IP = {key: value}
         sleep(1)
+
     count_ips(ALL_HOST)
-    ip_anne_list=[] 
+    ip_anne_list = []
     try:
         for one_tag in l4_config.l4_zl_tag:
             ips = ALL_HOST[one_tag]
             ip_anne_list = []
             for one_ip in ips:
-                host,port = split_maohao(one_ip['ip'])
-                ip_anne_list.append((one_ip['id'],host,port))
+                host, port = split_maohao(one_ip["ip"])
+                ip_anne_list.append((one_ip["id"], host, port))
     except KeyError:
         pass
     await get_read_ip(ip_anne_list)
 
-        
     @tan_jian.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
-        msg = await get_tan_jian(ip_anne_list,1)
-        await str_to_picstr(push_msg=msg,matcher=matcher) 
-        
+    async def _(matcher: Matcher, event: MessageEvent):
+        msg = await get_tan_jian(ip_anne_list, 1)
+        await str_to_picstr(push_msg=msg, matcher=matcher)
+
     @prison.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
-        msg = await get_tan_jian(ip_anne_list,2)
-        await str_to_picstr(push_msg=msg,matcher=matcher)
+    async def _(matcher: Matcher, event: MessageEvent):
+        msg = await get_tan_jian(ip_anne_list, 2)
+        await str_to_picstr(push_msg=msg, matcher=matcher)
 
     @open_prison.handle()
-    async def _(matcher:Matcher,event:MessageEvent):
+    async def _(matcher: Matcher, event: MessageEvent):
+
+        msg = await get_tan_jian(ip_anne_list, 3)
+        await str_to_picstr(push_msg=msg, matcher=matcher)
+
+
+async def get_read_ip(ip_anne_list):
+    get_ip = on_command("anne", aliases=server_key(), priority=80, block=True)
 
-        msg = await get_tan_jian(ip_anne_list,3)
-        await str_to_picstr(push_msg=msg,matcher=matcher)
-        
-    
-    
-async def get_read_ip(ip_anne_list):    
-    get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
     @get_ip.handle()
-    async def _(matcher:Matcher,start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg()):
+    async def _(
+        matcher: Matcher,
+        start: str = CommandStart(),
+        command: str = RawCommand(),
+        args: Message = CommandArg(),
+    ):
         if start:
-            command = command.replace(start,'')
-        if command == 'anne':
-            command = '云'
-        msg:str = args.extract_plain_text()
+            command = command.replace(start, "")
+        if command == "anne":
+            command = "云"
+        msg: str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
-        if isinstance(push_msg ,bytes):
+        if isinstance(push_msg, bytes):
             await matcher.finish(MessageSegment.image(push_msg))
-        elif msg and isinstance(push_msg ,list):
-            await matcher.finish(MessageSegment.image(push_msg[0]) + Message(push_msg[-1]))
-        elif msg and isinstance(push_msg ,str):
-            await str_to_picstr(push_msg,matcher)
+        elif msg and isinstance(push_msg, list):
+            await matcher.finish(
+                MessageSegment.image(push_msg[0]) + Message(push_msg[-1])
+            )
+        elif msg and isinstance(push_msg, str):
+            await str_to_picstr(push_msg, matcher)
+
 
-async def get_ip_to_mes(msg:str ,command: str = ''):   
+async def get_ip_to_mes(msg: str, command: str = ""):
     if not msg:
         # 以图片输出全部当前
         igr = False
         if command in gamemode_list:
-            this_ips = [d for l in ALL_HOST.values() for d in l if d.get('version') == command]
+            this_ips = [
+                d for l in ALL_HOST.values() for d in l if d.get("version") == command
+            ]
             igr = True
         else:
-            this_ips:list = ALL_HOST[command]
+            this_ips: list = ALL_HOST[command]
             igr = False
         if not this_ips:
             return
         ip_list = []
         for one_ip in this_ips:
-            host,port = split_maohao(one_ip['ip'])
-            ip_list.append((one_ip['id'],host,port))
-        img = await qq_ip_queries_pic(ip_list,igr)
+            host, port = split_maohao(one_ip["ip"])
+            ip_list.append((one_ip["id"], host, port))
+        img = await qq_ip_queries_pic(ip_list, igr)
         if img:
             return img
         else:
             return "服务器无响应"
     else:
 
         if not msg[0].isdigit():
             if any(mode in msg for mode in gamemode_list):
                 pass
             else:
                 return
-        message = await json_server_to_tag_dict(command,msg)
+        message = await json_server_to_tag_dict(command, msg)
         if len(message) == 0:
             # 关键词不匹配，忽略
             return
-        ip = str(message['ip'])
+        ip = str(message["ip"])
         logger.info(ip)
-        
+
         try:
-        #     if l4_config.l4_image:
-        #         host,port = split_maohao(ip)
-        #         msgs = await queries_dict(host,port)
-        #         msgs['Players'] += await player_queries_anne_dict(host,port)
-        #         imgs = await one_server_img()
+            #     if l4_config.l4_image:
+            #         host,port = split_maohao(ip)
+            #         msgs = await queries_dict(host,port)
+            #         msgs['Players'] += await player_queries_anne_dict(host,port)
+            #         imgs = await one_server_img()
             # else:
             msgs = await get_anne_server_ip(ip)
-            return  msgs
-        except (OSError,asyncio.exceptions.TimeoutError):
-            return '服务器无响应'
-    
-           
+            return msgs
+        except (OSError, asyncio.exceptions.TimeoutError):
+            return "服务器无响应"
+
 
-    
-    
 async def init():
     global matchers
     # print('启动辣')
-    from ..l4d2_update import l4d_restart,l4d_update,get_update_log,driver
+    from ..l4d2_update import l4d_restart, l4d_update, get_update_log, driver
+
     await get_des_ip()
-    
-   
-    
+
+
 @driver.on_startup
 async def _():
-    await init()
+    await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
-from typing import List,Dict,Union
+from typing import List, Dict, Union, Any
 import ast
 import platform
 import os
 from ruamel import yaml
-from pydantic import Extra,BaseModel,Field
+from pydantic import Extra, BaseModel, Field
+
 try:
     import ujson as json
 except:
     import json
 
 from nonebot.permission import SUPERUSER
 from nonebot import get_driver
@@ -16,193 +17,200 @@
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
     PRIVATE_FRIEND,
 )
 
 from ..l4d2_queries.ohter import ALL_HOST
-file_format = (".vpk",".zip",".7z",'rar')
+
+file_format = (".vpk", ".zip", ".7z", "rar")
 # 权限
 
 driver = get_driver()
-COMMAND_START = list[driver.config.command_start]
+COMMAND_START = list(driver.config.command_start)
+
 try:
     NICKNAME: str = list(driver.config.nickname)[0]
 except Exception:
-    NICKNAME = 'bot'
-CHECK_FILE:int = 0
+    NICKNAME = "bot"
+CHECK_FILE: int = 0
 
 
-reMaster = SUPERUSER | GROUP_OWNER 
-Master = SUPERUSER | GROUP_ADMIN | GROUP_OWNER 
+reMaster = SUPERUSER | GROUP_OWNER
+Master = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
 ADMINISTRATOR = SUPERUSER | GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND
 # file 填写求生服务器所在路径
 
 
-
-
-CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
+CONFIG_PATH = Path() / "data" / "L4D2" / "l4d2.yml"
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
+
 class L4d2GroupConfig(BaseModel):
-    enable: bool = Field(True, alias='是否启用求生功能')
-    map_master: List[str] = Field([], alias='分群地图管理员')
+    enable: bool = Field(True, alias="是否启用求生功能")
+    map_master: List[str] = Field([], alias="分群地图管理员")
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
 
+
 class L4d2Config(BaseModel):
-    total_enable: bool = Field(True, alias='是否全局启用求生功能')
-    l4_image: bool = Field(False , alias='是否启用图片')
-    web_username: str = Field('l4d2', alias='后台管理用户名')
-    web_password: str = Field('admin', alias='后台管理密码')
-    l4_style: str = Field("standard", alias='图片风格')
-    l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
-        [{
-        'id_rank':'1',
-        'place': False,
-        'location':'C:\\l4d2',
-        'host':'127.0.0.1',
-        'port':'20715',
-        'rcon':'114514',
-        'server_id':'本地地图',
-        },{
-        'id_rank':'2',
-        'place': True,
-        'location':'/home/unbuntu/coop',
-        'host':'11.4.51.4',
-        'port':'20715',
-        'rcon':'9191810',
-        'account':'root',
-        'password':'114514',
-        'server_id':'远程地图',
-        }],
-          alias='l4服务器ip集合')
-    l4_zl_tag :List[str] = Field(['云'], alias='坐牢三指令')
-    l4_number :int = Field(1,alias='第几个地图路径')
-    web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
-                                alias='后台管理token密钥')
-    l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
+    total_enable: bool = Field(True, alias="是否全局启用求生功能")
+    l4_image: bool = Field(False, alias="是否启用图片")
+    web_username: str = Field("l4d2", alias="后台管理用户名")
+    web_password: str = Field("admin", alias="后台管理密码")
+    l4_style: str = Field("standard", alias="图片风格")
+    l4_ipall: List[Dict[str, Any]] = Field(
+        [
+            {
+                "id_rank": "1",
+                "place": False,
+                "location": "C:\\l4d2",
+                "host": "127.0.0.1",
+                "port": "20715",
+                "rcon": "114514",
+                "server_id": "本地地图",
+            },
+            {
+                "id_rank": "2",
+                "place": True,
+                "location": "/home/unbuntu/coop",
+                "host": "11.4.51.4",
+                "port": "20715",
+                "rcon": "9191810",
+                "account": "root",
+                "password": "114514",
+                "server_id": "远程地图",
+            },
+        ],
+        alias="l4服务器ip集合",
+    )
+    l4_zl_tag: List[str] = Field(["云"], alias="坐牢三指令")
+    l4_number: int = Field(1, alias="第几个地图路径")
+    web_secret_key: str = Field(
+        "49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0",
+        alias="后台管理token密钥",
+    )
+    l4_master: List[str] = Field(["114514919"], alias="求生地图全局管理员qq")
     # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
-    l4_font: str = Field('simsun.ttc', alias='字体')
-    l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
-    l4_push_interval: int = Field(3, alias='定时任务间隔')
-    l4_push_times: int = Field(10, alias='定时任务次数')
+    l4_font: str = Field("simsun.ttc", alias="字体")
+    l4_only: bool = Field(False, alias="下载地图是是否阻碍其他指令")
+    l4_push_interval: int = Field(3, alias="定时任务间隔")
+    l4_push_times: int = Field(10, alias="定时任务次数")
     l4_connect: bool = Field(True, alias="是否在查服命令后加入connect ip")
-    group_config: Dict[int, L4d2GroupConfig] = Field({}, alias='分群配置')
+    group_config: Dict[int, L4d2GroupConfig] = Field({}, alias="分群配置")
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
-                
-class L4d2ConfigManager:
 
+
+class L4d2ConfigManager:
     def __init__(self):
         self.file_path = CONFIG_PATH
         if self.file_path.exists():
             self.config = L4d2Config.parse_obj(
-                yaml.load(self.file_path.read_text(encoding='utf-8'), Loader=yaml.Loader))
+                yaml.load(
+                    self.file_path.read_text(encoding="utf-8"), Loader=yaml.Loader
+                )
+            )
         else:
-            self.config = L4d2Config()
+            self.config = L4d2Config()  # type: ignore
         self.save()
 
     def get_group_config(self, group_id: int) -> L4d2GroupConfig:
         if group_id not in self.config.group_config:
-            self.config.group_config[group_id] = L4d2GroupConfig()
+            self.config.group_config[group_id] = L4d2GroupConfig()  # type: ignore
             self.save()
         return self.config.group_config[group_id]
 
     @property
     def config_list(self) -> List[str]:
         return list(self.config.dict(by_alias=True).keys())
 
     def save(self):
-        with self.file_path.open('w', encoding='utf-8') as f:
+        with self.file_path.open("w", encoding="utf-8") as f:
             yaml.dump(
                 self.config.dict(by_alias=True),
                 f,
                 indent=2,
                 Dumper=yaml.RoundTripDumper,
-                allow_unicode=True)
+                allow_unicode=True,
+            )
+
 
 # 参数设置为全局变量
-global config_manager,l4_config            
+global config_manager, l4_config
 config_manager = L4d2ConfigManager()
 l4_config = config_manager.config
 
+
 class UserModel(BaseModel):
     username: str
     password: str
 
-     
-'''
+
+"""
 地图路径
-'''
+"""
 vpk_path = "left4dead2/addons"
 
 
 PLAYERSDATA = Path() / "data/L4D2/image/players"
 """用户数据路径"""
-TEXT_PATH = Path(__file__).parent.parent / 'data/L4D2/image'
+TEXT_PATH = Path(__file__).parent.parent / "data/L4D2/image"
 """图片存储路径"""
-TEXT_XPATH = Path() / 'data/L4D2/image'
+TEXT_XPATH = Path() / "data/L4D2/image"
 """内置图片路径"""
 
 
-
 PLAYERSDATA = Path() / "data/L4D2/sql"
 """数据库路径"""
 DATASQLITE = Path().parent.parent / "data/L4D2/sql/L4D2.db"
-"""数据库！"""  
+"""数据库！"""
 
-table_data = ["L4d2_players","L4D2_server"]
+table_data = ["L4d2_players", "L4D2_server"]
 """数据库表"""
-L4d2_players_tag = ['qq', 'nickname', 'steamid']
+L4d2_players_tag = ["qq", "nickname", "steamid"]
 """数据库表1"""
-L4d2_server_tag = ['id','qqgroup', 'host', 'port', 'rcon']
+L4d2_server_tag = ["id", "qqgroup", "host", "port", "rcon"]
 """数据库表2"""
-L4d2_INTEGER = ['id','qq','qqgroup','port']
+L4d2_INTEGER = ["id", "qq", "qqgroup", "port"]
 """INITEGER的表头"""
-L4d2_TEXT = ['nickname','steamid','host','rcon','path']
+L4d2_TEXT = ["nickname", "steamid", "host", "rcon", "path"]
 """TEXT的表头"""
-L4d2_BOOLEAN = ['use']
+L4d2_BOOLEAN = ["use"]
 """BOOLEAN的表头"""
 
-tables_columns = {
-    table_data[0]:L4d2_players_tag,
-    table_data[1]:L4d2_server_tag
-}
+tables_columns = {table_data[0]: L4d2_players_tag, table_data[1]: L4d2_server_tag}
 
 # 求生anne服务器
 anne_url = "https://server.trygek.com/"
 
 gamemode_list = [
-    '纯净',
-    '魔改战役',
-    '多特',
-    '魔改多特',
-    '写专',
-    '对抗',
-    '魔改对抗',
-    '药役',
-    '药抗',
-    '包抗',
-    '绝境',
-    '死专',
-    'ast',
-    '清道夫',
+    "纯净",
+    "魔改战役",
+    "多特",
+    "魔改多特",
+    "写专",
+    "对抗",
+    "魔改对抗",
+    "药役",
+    "药抗",
+    "包抗",
+    "绝境",
+    "死专",
+    "ast",
+    "清道夫",
 ]
 
 # 系统
-if platform.system() == 'Windows':
-    systems:str = 'win'
-elif platform.system() == 'Linux':
-    systems:str = 'linux'
+if platform.system() == "Windows":
+    systems: str = "win"
+elif platform.system() == "Linux":
+    systems: str = "linux"
 else:
-    systems:str = 'others'
+    systems: str = "others"
 ANNE_IP = {}
-
-
-
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,64 +2,72 @@
 from PIL import Image, ImageDraw, ImageFont
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot_plugin_txt2img import Txt2Img
 from .config import l4_config
 
 l4_font = l4_config.l4_font
 """直接超的智障回复"""
+
+
 def txt_to_img(text: str, font_size=30, font_path=l4_font) -> bytes:
     text = line_break(text)
     d_font = ImageFont.truetype(font_path, font_size)
-    lines = text.count('\n')  # 计算行数
-    image = Image.new("L", (LINE_CHAR_COUNT*font_size //
-                      2 + 50, font_size*lines+50), "white")
+    lines = text.count("\n")  # 计算行数
+    image = Image.new(
+        "L", (LINE_CHAR_COUNT * font_size // 2 + 50, font_size * lines + 50), "white"
+    )
     draw_table = ImageDraw.Draw(im=image)
-    draw_table.text(xy=(25, 25), text=text, fill='#000000',
-                    font=d_font, spacing=4)  # spacing调节机制不清楚如何计算
+    draw_table.text(
+        xy=(25, 25), text=text, fill="#000000", font=d_font, spacing=4
+    )  # spacing调节机制不清楚如何计算
     new_img = image.convert("RGB")
     img_byte = BytesIO()
-    new_img.save(img_byte, format='PNG')
+    new_img.save(img_byte, format="PNG")
     binary_content = img_byte.getvalue()
     return binary_content
 
 
-LINE_CHAR_COUNT = 30*2  # 每行字符数：30个中文字符(=60英文字符)
+LINE_CHAR_COUNT = 30 * 2  # 每行字符数：30个中文字符(=60英文字符)
 CHAR_SIZE = 30
 TABLE_WIDTH = 4
 
 
 def line_break(line: str) -> str:
-    ret = ''
+    ret = ""
     width = 0
     for c in line:
-        if len(c.encode('utf8')) == 3:  # 中文
+        if len(c.encode("utf8")) == 3:  # 中文
             if LINE_CHAR_COUNT == width + 1:  # 剩余位置不够一个汉字
                 width = 2
-                ret += '\n' + c
+                ret += "\n" + c
             else:  # 中文宽度加2，注意换行边界
                 width += 2
                 ret += c
         else:
-            if c == '\t':
+            if c == "\t":
                 space_c = TABLE_WIDTH - width % TABLE_WIDTH  # 已有长度对TABLE_WIDTH取余
-                ret += ' ' * space_c
+                ret += " " * space_c
                 width += space_c
-            elif c == '\n':
+            elif c == "\n":
                 width = 0
                 ret += c
             else:
                 width += 1
                 ret += c
         if width >= LINE_CHAR_COUNT:
-            ret += '\n'
+            ret += "\n"
             width = 0
-    if ret.endswith('\n'):
+    if ret.endswith("\n"):
         return ret
-    return ret + '\n'
+    return ret + "\n"
 
 
-def mode_txt_to_img(title:str,text:str,font_size:int = 32,):
+def mode_txt_to_img(
+    title: str,
+    text: str,
+    font_size: int = 32,
+):
     txt2img = Txt2Img()
     txt2img.set_font_size(font_size)
     pic = txt2img.draw(title, text)
     msg = MessageSegment.image(pic)
-    return msg
+    return msg
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,300 +1,316 @@
-
-from nonebot.adapters.onebot.v11 import Bot,MessageEvent,GroupMessageEvent
+from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 import struct
 import httpx
 import os
 from pathlib import Path
 
-from typing import List,Dict,Union,Optional
+from typing import List, Dict, Union, Optional
 from .txt_to_img import txt_to_img
 from .config import *
-from ..l4d2_anne import write_player,del_player,anne_messgae
-from ..l4d2_server.rcon import read_server_cfg_rcon,rcon_server
-from ..l4d2_queries import queries,player_queries
+from ..l4d2_anne import write_player, del_player, anne_message
+from ..l4d2_server.rcon import read_server_cfg_rcon, rcon_server
+from ..l4d2_queries import queries, player_queries
 from ..l4d2_queries.qqgroup import *
 from ..l4d2_server.workshop import workshop_to_dict
 from ..l4d2_image.steam import url_to_byte
 from .txt_to_img import mode_txt_to_img
 import tempfile
 import random
 
 
-
 async def get_file(url: str, down_file: Path):
-    '''
+    """
     下载指定Url到指定位置
-    '''
+    """
     try:
         if l4_config.l4_only:
             maps = await url_to_byte(url)
         else:
             maps = httpx.get(url).content
-        logger.info('已获取文件，尝试新建文件并写入')
-        with open(down_file, 'wb') as mfile:
-            mfile.write(maps)
-        logger.info('下载成功')
-        return '文件已下载，正在解压'
+        logger.info("已获取文件，尝试新建文件并写入")
+        if maps:
+            with open(down_file, "wb") as mfile:
+                mfile.write(maps)
+            logger.info("下载成功")
+            return "文件已下载，正在解压"
     except Exception as e:
         logger.info(f"文件获取不到/已损坏:原因是{e}")
         return None
 
 
-def get_vpk(vpk_list: List[str], map_path: Path, file_: str = '.vpk') -> List[str]:
-    '''
+def get_vpk(map_path: Path, file_: str = ".vpk") -> List[str]:
+    """
     获取路径下所有vpk文件名，并存入vpk_list列表中
-    '''
-    vpk_list.extend([file for file in os.listdir(str(map_path)) if file.endswith(file_)])
+    """
+    vpk_list: List[str] = [str(file) for file in map_path.glob(f"*{file_}")]
     return vpk_list
 
 
-
 def mes_list(mes: str, name_list: List[str]) -> str:
     if name_list:
         for idx, name in enumerate(name_list):
-            mes += f'\n{idx+1}、{name}'
+            mes += f"\n{idx+1}、{name}"
     return mes
 
 
-
-
 def del_map(num: int, map_path: Path) -> str:
-    '''
+    """
     删除指定的地图
-    '''
+    """
     map = get_vpk(map_path)
     map_name = map[num - 1]
     del_file = map_path / map_name
     os.remove(del_file)
     return map_name
 
 
 def rename_map(num: int, rename: str, map_path: Path) -> str:
-    '''
+    """
     改名指定的地图
-    '''
+    """
     map = get_vpk(map_path)
     map_name = map[num - 1]
     old_file = map_path / map_name
     new_file = map_path / rename
     os.rename(old_file, new_file)
-    logger.info('改名成功')
+    logger.info("改名成功")
     return map_name
 
 
 def text_to_png(msg: str) -> bytes:
     """文字转png"""
     return txt_to_img(msg)
 
 
-
-def solve(msg:str):
+def solve(msg: str):
     """删除str最后一行"""
     lines = msg.splitlines()
     lines.pop()
-    return '\n'.join(lines)
+    return "\n".join(lines)
 
 
-async def search_anne(name:str,usr_id:str):
+async def search_anne(name: str, usr_id: str):
     """获取anne成绩"""
-    return await anne_messgae(name,usr_id)
-    
+    return await anne_message(name, usr_id)
 
-async def bind_steam(id:str,msg:str,nickname:str):
+
+async def bind_steam(id: str, msg: str, nickname: str):
     """绑定qq-steam"""
-    return await write_player(id,msg,nickname)
+    return await write_player(id, msg, nickname)
+
 
-def name_exist(id:str):
+def name_exist(id: str):
     """删除绑定信息"""
     return del_player(id)
 
-async def get_message_at(data: str) -> list:
-    data = json.loads(data)
-    return [int(msg['data']['qq']) for msg in data['message'] if msg['type'] == 'at']
 
-    
+async def get_message_at(datas: str) -> List[int]:
+    data: Dict[str, Any] = json.loads(datas)
+    return [int(msg["data"]["qq"]) for msg in data["message"] if msg["type"] == "at"]
 
-def at_to_usrid(at):
+
+def at_to_usrid(at: List[int]):
     return at[0] if at else None
 
 
 async def rcon_command(rcon, cmd):
     return await rcon_server(rcon, cmd.strip())
 
+
 async def command_server(msg: str):
     rcon = await read_server_cfg_rcon()
     msg = await rcon_command(rcon, msg)
     if not msg:
-        msg = '你可能发送了一个无用指令，或者换图导致服务器无响应'
-    elif msg.startswith('Unknown command'):
-        msg = '无效指令：' + msg.replace('Unknown command', '').strip()
-    return msg.strip().replace('\n', '')
+        msg = "你可能发送了一个无用指令，或者换图导致服务器无响应"
+    elif msg.startswith("Unknown command"):
+        msg = "无效指令：" + msg.replace("Unknown command", "").strip()
+    return msg.strip().replace("\n", "")
 
 
-
-
-async def queries_server(msg:list) -> str:
+async def queries_server(msg: list) -> str:
     """查询ip返回信息"""
     ip = msg[0]
     port = msg[1]
-    msgs = ''
+    msgs = ""
     try:
-        msgs = await  queries(ip,port)
-        msgs += await player_queries(ip,port)
-    except (struct.error,TimeoutError):
+        msgs = await queries(ip, port)
+        msgs += await player_queries(ip, port)
+    except (struct.error, TimeoutError):
         pass
     # except Exception:
-        # msgs = '有无法识别的用户名'
-        # return msgs
+    # msgs = '有无法识别的用户名'
+    # return msgs
     return msgs
 
-async def add_ip(group_id,host,port):
+
+async def add_ip(group_id, host, port):
     """先查找是否存在，如果不存在则创建"""
-    return await bind_group_ip(group_id,host,port)
+    return await bind_group_ip(group_id, host, port)
 
-async def del_ip(group_id,number):
+
+async def del_ip(group_id, number):
     """删除群ip"""
-    return await del_group_ip(group_id,number)
+    return await del_group_ip(group_id, number)
+
 
 async def show_ip(group_id):
     """先查找群ip，再根据群ip返回"""
     data_list = await get_qqgroup_ip_msg(group_id)
     logger.info(data_list)
-    if len(data_list) == 0 :
+    if len(data_list) == 0:
         return "本群没有订阅"
     msg = await qq_ip_queries_pic(data_list)
-    return  msg
+    return msg
+
 
 async def get_number_url(number):
-    'connect AGNES.DIGITAL.LINE.PM:40001'
+    "connect AGNES.DIGITAL.LINE.PM:40001"
     ip = await get_server_ip(number)
     if not ip:
-        return '该序号不存在'
-    url = f'connect {ip}'
+        return "该序号不存在"
+    url = f"connect {ip}"
     return url
 
-async def workshop_msg(msg:str):
+
+async def workshop_msg(msg: str):
     """url变成id，拼接post请求"""
-    if msg.startswith('https://steamcommunity.com/sharedfiles/filedetails/?id'):
+    if msg.startswith("https://steamcommunity.com/sharedfiles/filedetails/?id"):
         try:
-            msg = msg.split('&')[0]
+            msg = msg.split("&")[0]
         except:
             pass
-        msg = msg.replace('https://steamcommunity.com/sharedfiles/filedetails/?id=','')
+        msg = msg.replace("https://steamcommunity.com/sharedfiles/filedetails/?id=", "")
     if msg.isdigit():
-        data:Union[dict,List[dict]] = await workshop_to_dict(msg)
+        data: Union[dict, List[dict]] = await workshop_to_dict(msg)
         return data
     else:
         return None
-    
-async def save_file(file:bytes,path_name):
+
+
+async def save_file(file: bytes, path_name):
     """保存文件"""
-    with open(path_name,'w') as files:
+    with open(path_name, "wb") as files:
         files.write(file)
-        
-async def get_anne_server_ip(ip ,ismsg :bool = False):
+
+
+async def get_anne_server_ip(ip, ismsg: bool = False):
     """输出查询ip和ping"""
-    host,port = split_maohao(ip)
-    data = await queries_server([host,port])
+    host, port = split_maohao(ip)
+    data = await queries_server([host, port])
     lines = data.splitlines()
-    msg = '\n'.join(lines[1:])
-    msg += '\nconnect ' + ip
+    msg = "\n".join(lines[1:])
+    msg += "\nconnect " + ip
     return msg
 
+
 async def upload_file(bot: Bot, event: MessageEvent, file_data: bytes, filename: str):
     """上传临时文件"""
     if systems == "win" or "other":
         with tempfile.TemporaryDirectory() as temp_dir:
             with open(Path(temp_dir) / filename, "wb") as f:
                 f.write(file_data)
             if isinstance(event, GroupMessageEvent):
                 await bot.call_api(
-                    "upload_group_file", group_id=event.group_id, file=f.name, name=filename
+                    "upload_group_file",
+                    group_id=event.group_id,
+                    file=f.name,
+                    name=filename,
                 )
             else:
                 await bot.call_api(
-                    "upload_private_file", user_id=event.user_id, file=f.name, name=filename
+                    "upload_private_file",
+                    user_id=event.user_id,
+                    file=f.name,
+                    name=filename,
                 )
         os.remove(Path().joinpath(filename))
     elif systems == "linux":
         with tempfile.NamedTemporaryFile("wb+") as f:
             f.write(file_data)
             if isinstance(event, GroupMessageEvent):
                 await bot.call_api(
-                    "upload_group_file", group_id=event.group_id, file=f.name, name=filename
+                    "upload_group_file",
+                    group_id=event.group_id,
+                    file=f.name,
+                    name=filename,
                 )
             else:
                 await bot.call_api(
-                    "upload_private_file", user_id=event.user_id, file=f.name, name=filename
+                    "upload_private_file",
+                    user_id=event.user_id,
+                    file=f.name,
+                    name=filename,
                 )
 
 
-async def json_server_to_tag_dict(key:str,msg:str):
+async def json_server_to_tag_dict(key: str, msg: str):
     """
     l4d2字典转tag的dict结果
      - 1、先匹配腐竹
      - 2、再匹配模式、没有参数则从直接匹配最上面的
      - 3、匹配数字（几服），没有参数则从结果里随机返回一个
     """
     data_dict = {}
     data_list = []
-    msg = msg.replace(' ','')
+    msg = msg.replace(" ", "")
     # 腐竹循环
-    for tag,value in ALL_HOST.items():
-        value:List[dict]  
+    for tag, value in ALL_HOST.items():
+        value: List[dict]
         if tag == key:
-            data_dict.update({'server':tag})
+            data_dict.update({"server": tag})
             if not msg:
                 # 腐竹
                 data_dict.update(random.choice(value))
             elif msg.isdigit():
                 logger.info("腐竹 + 序号")
                 for server in value:
-                    if msg == str(server['id']):
+                    if msg == str(server["id"]):
                         data_dict.update(server)
                         break
             else:
                 logger.info("腐竹 + 模式 + 序号")
                 for server in value:
-                    if msg.startswith(server['version']):
+                    if msg.startswith(server["version"]):
                         data_list.append(server)
-                        msg_id = msg[len(server['version']):]
-                        if msg_id == str(server['id']):
+                        msg_id = msg[len(server["version"]) :]
+                        if msg_id == str(server["id"]):
                             data_dict.update(server)
                             break
                 else:
                     # 腐竹 + 模式
                     data_dict.update(random.choice(data_list))
 
     logger.info(data_dict)
     return data_dict
 
 
-
 sub_menus = []
 
+
 def register_menu_func(
     func: str,
     trigger_condition: str,
     brief_des: str,
-    trigger_method: str = '指令',
+    trigger_method: str = "指令",
     detail_des: Optional[str] = None,
 ):
     sub_menus.append(
         {
-            'func': func,
-            'trigger_method': trigger_method,
-            'trigger_condition': trigger_condition,
-            'brief_des': brief_des,
-            'detail_des': detail_des or brief_des,
+            "func": func,
+            "trigger_method": trigger_method,
+            "trigger_condition": trigger_condition,
+            "brief_des": brief_des,
+            "detail_des": detail_des or brief_des,
         }
     )
 
+
 def register_menu(*args, **kwargs):
     def decorator(f):
         register_menu_func(*args, **kwargs)
         return f
 
     return decorator
 
@@ -302,25 +318,26 @@
 async def extract_last_digit(msg: str) -> tuple[str, str]:
     "分离str和数字"
     for i in range(len(msg) - 1, -1, -1):
         if msg[i].isdigit():
             last_digit = msg[i]
             new_msg = msg[:i]
             return new_msg, last_digit
-    return msg, ''
+    return msg, ""
+
 
-async def str_to_picstr(push_msg:str,matcher:Matcher,keyword:str = None):
+async def str_to_picstr(push_msg: str, matcher: Matcher, keyword: Optional[str] = None):
     """判断图片输出还是正常输出"""
     if l4_config.l4_image:
         lines = push_msg.splitlines()
         first_str = lines[0]
         last_str = lines[-1]
-        push_msg = '\n'.join(lines[1:-1])
+        push_msg = "\n".join(lines[1:-1])
         if l4_config.l4_connect:
-            await matcher.send(mode_txt_to_img(first_str,push_msg)+last_str)
+            await matcher.send(mode_txt_to_img(first_str, push_msg) + last_str)
         else:
-            await matcher.send(mode_txt_to_img(first_str,push_msg))
+            await matcher.send(mode_txt_to_img(first_str, push_msg))
     else:
-        if l4_config.l4_connect or keyword== "connect":
+        if l4_config.l4_connect or keyword == "connect":
             await matcher.send(push_msg)
         else:
-            await matcher.send('\n'.join(push_msg.splitlines()[1:-2]))
+            await matcher.send("\n".join(push_msg.splitlines()[1:-2]))
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,226 +9,234 @@
 
 from pathlib import Path
 
 from nonebot import get_driver, logger
 from ..l4d2_utils.config import *
 from ..l4d2_utils.utils import split_maohao
 from ..l4d2_queries.qqgroup import qq_ip_querie
-CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
+
+CONFIG_PATH = Path() / "data" / "L4D2" / "l4d2.yml"
 
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 driver = get_driver()
 
 from .webUI import login_page, admin_app
 
-requestAdaptor = '''
+requestAdaptor = """
 requestAdaptor(api) {
     api.headers["token"] = localStorage.getItem("token");
     return api;
 },
-'''
-responseAdaptor = '''
+"""
+responseAdaptor = """
 responseAdaptor(api, payload, query, request, response) {
     if (response.data.detail == '登录验证失败或已失效，请重新登录') {
         window.location.href = '/l4d2/login'
         window.localStorage.clear()
         window.sessionStorage.clear()
         window.alert('登录验证失败或已失效，请重新登录')
     }
     return payload
 },
-'''
+"""
 
 
 def authentication():
     def inner(token: Optional[str] = Header(...)):
         try:
-            payload = jwt.decode(token, config_manager.config.web_secret_key, algorithms='HS256')
-            if not (username := payload.get('username')) or username != config_manager.config.web_username:
-                raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+            if not token:
+                raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
+            payload = jwt.decode(
+                token, config_manager.config.web_secret_key, algorithms="HS256"
+            )
+            if (
+                not (username := payload.get("username"))
+                or username != config_manager.config.web_username
+            ):
+                raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
         except (jwt.JWTError, jwt.ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail='登录验证失败或已失效，请重新登录')
+            raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
 
     return Depends(inner)
 
 
 COMMAND_START = driver.config.command_start.copy()
-if '' in COMMAND_START:
-    COMMAND_START.remove('')
-
-
-
+if "" in COMMAND_START:
+    COMMAND_START.remove("")
 
 
 @driver.on_startup
 async def init_web():
     if not config_manager.config.total_enable:
         return
     app: FastAPI = get_app()
-    logger.success('成功加载网页控制台')
-    @app.post('/l4d2/api/login', response_class=JSONResponse)
-    async def login(user: UserModel):
-        if user.username != config_manager.config.web_username or user.password != config_manager.config.web_password:
-            return {
-                'status': -100,
-                'msg':    '登录失败，请确认用户ID和密码无误'
-            }
-        token = jwt.encode({'username': user.username,
-                            'exp':      datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
-                                minutes=30)}, config_manager.config.web_secret_key, algorithm='HS256')
-        return {
-            'status': 0,
-            'msg':    '登录成功',
-            'data':   {
-                'token': token
-            }
-        }
+    logger.success("成功加载网页控制台")
 
-    @app.get('/l4d2/api/get_group_list', response_class=JSONResponse, dependencies=[authentication()])
+    @app.post("/l4d2/api/login", response_class=JSONResponse)
+    async def login(user: UserModel):
+        if (
+            user.username != config_manager.config.web_username
+            or user.password != config_manager.config.web_password
+        ):
+            return {"status": -100, "msg": "登录失败，请确认用户ID和密码无误"}
+        token = jwt.encode(
+            {
+                "username": user.username,
+                "exp": datetime.datetime.now(datetime.timezone.utc)
+                + datetime.timedelta(minutes=30),
+            },
+            config_manager.config.web_secret_key,
+            algorithm="HS256",
+        )
+        return {"status": 0, "msg": "登录成功", "data": {"token": token}}
+
+    @app.get(
+        "/l4d2/api/get_group_list",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def get_group_list_api():
         try:
             group_list = await get_bot().get_group_list()
-            group_list = [{'label': f'{group["group_name"]}({group["group_id"]})', 'value': group['group_id']} for group
-                          in group_list]
-            return {
-                'status': 0,
-                'msg':    'ok',
-                'data':   {
-                    'group_list': group_list
+            group_list = [
+                {
+                    "label": f'{group["group_name"]}({group["group_id"]})',
+                    "value": group["group_id"],
                 }
-            }
+                for group in group_list
+            ]
+            return {"status": 0, "msg": "ok", "data": {"group_list": group_list}}
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
-            }
+            return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
 
-    @app.post('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    @app.post(
+        "/l4d2/api/l4d2_global_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def post_l4d2_global_config(data: dict):
         config_manager.config.update(**data)
         config_manager.save()
-        return {
-            'status': 0,
-            'msg':    '保存成功'
-        }
+        return {"status": 0, "msg": "保存成功"}
 
-    @app.get('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    @app.get(
+        "/l4d2/api/l4d2_global_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def get_l4d2_global_config():
         try:
             bot = get_bot()
             groups = await bot.get_group_list()
             member_list = []
             for group in groups:
-                members = await bot.get_group_member_list(group_id=group['group_id'])
+                members = await bot.get_group_member_list(group_id=group["group_id"])
                 member_list.extend(
-                    [{'label': f'{member["nickname"] or member["card"]}({member["user_id"]})',
-                      'value': member['user_id']}
-                     for
-                     member in members])
-            config = config_manager.config.dict(exclude={'group_config'})
-            config['member_list'] = member_list
-            config['l4_styles'] = ['standard','black']
+                    [
+                        {
+                            "label": f'{member["nickname"] or member["card"]}({member["user_id"]})',
+                            "value": member["user_id"],
+                        }
+                        for member in members
+                    ]
+                )
+            config = config_manager.config.dict(exclude={"group_config"})
+            config["member_list"] = member_list
+            config["l4_styles"] = ["standard", "black"]
 
             return config
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
-            }
-            
-    @app.get('/l4d2/api/get_query_contexts', response_class=JSONResponse, dependencies=[authentication()])
+            return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
+
+    @app.get(
+        "/l4d2/api/get_query_contexts",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def get_query_context():
         try:
             from ..l4d2_utils.command import ALL_HOST
+
             this_ips = ALL_HOST
             ip_lists = []
             for ip_list, v in this_ips.items():
                 for d in v:
-                    host, port = split_maohao(d['ip'])
-                    ip_lists.append((d['id'], ip_list, host, port))
+                    host, port = split_maohao(d["ip"])
+                    ip_lists.append((d["id"], ip_list, host, port))
             data_dict = await qq_ip_querie(ip_lists)
             if not data_dict:
-                return{
-                'status': -100,
-                'msg':    '返回失败，请确保有可用的服务器ip' 
-                }
-            data_list = data_dict['msg_list']
+                return {"status": -100, "msg": "返回失败，请确保有可用的服务器ip"}
+            data_list = data_dict["msg_list"]
             return {
-                'status': 0,
-                'msg': 'ok',
-                'data': {
-                    'items': data_list,
-                    'total': len(data_list),
-                }
+                "status": 0,
+                "msg": "ok",
+                "data": {
+                    "items": data_list,
+                    "total": len(data_list),
+                },
             }
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '返回失败，请确保网络连接正常'
-            }
+            return {"status": -100, "msg": "返回失败，请确保网络连接正常"}
 
-    @app.get('/l4d2/api/get_l4d2_messages', response_class=JSONResponse, dependencies=[authentication()])
+    @app.get(
+        "/l4d2/api/get_l4d2_messages",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
     async def get_l4d2_messages():
         try:
             l4_ipall = config_manager.config.l4_ipall
-            config = [{'label': item['server_id'] , 'value': item['id_rank']}
-                for item in l4_ipall]
-            return {
-                'status': 0,
-                'msg': 'ok',
-                'data': {'server_list':config}
-            }
+            config = [
+                {"label": item["server_id"], "value": item["id_rank"]}
+                for item in l4_ipall
+            ]
+            return {"status": 0, "msg": "ok", "data": {"server_list": config}}
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '返回失败，请确保网络连接正常'
-            }
-    @app.get('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_l4d2_server_config(id_rank :str):
+            return {"status": -100, "msg": "返回失败，请确保网络连接正常"}
+
+    @app.get(
+        "/l4d2/api/l4d2_server_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def get_l4d2_server_config(id_rank: str):
         try:
             l4_ipall = config_manager.config.l4_ipall
             config = {}
             for item in l4_ipall:
-                if item['id_rank'] == id_rank :
-                    item['place'] = item['place'] == 'True' or item['place'] == True
+                if item["id_rank"] == id_rank:
+                    item["place"] = item["place"] == "True" or item["place"] == True
                     config = item
                     break
-            return {
-                'status': 0,
-                'msg': 'ok',
-                'data': config
-            }
+            return {"status": 0, "msg": "ok", "data": config}
         except ValueError:
-            return {
-                'status': -100,
-                'msg':    '返回失败，请确保网络连接正常'
-            }
-        
-    @app.post('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def post_l4d2_server_config(id_rank :str,data: dict):
+            return {"status": -100, "msg": "返回失败，请确保网络连接正常"}
+
+    @app.post(
+        "/l4d2/api/l4d2_server_config",
+        response_class=JSONResponse,
+        dependencies=[authentication()],
+    )
+    async def post_l4d2_server_config(id_rank: str, data: dict):
         for one in config_manager.config.l4_ipall:
-            if one['id_rank']==id_rank:
+            if one["id_rank"] == id_rank:
                 one.update(**data)
         config_manager.save()
-        return {
-            'status': 0,
-            'msg':    '保存成功'
-        }        
+        return {"status": 0, "msg": "保存成功"}
 
-        
-    @app.get('/l4d2', response_class=RedirectResponse)
+    @app.get("/l4d2", response_class=RedirectResponse)
     async def redirect_page():
-        return RedirectResponse('/l4d2/login')
+        return RedirectResponse("/l4d2/login")
 
-    @app.get('/l4d2/login', response_class=HTMLResponse)
+    @app.get("/l4d2/login", response_class=HTMLResponse)
     async def login_page_app():
-        return login_page.render(site_title='登录 | l4d2 后台管理',
-                                 theme='ang')
+        return login_page.render(site_title="登录 | l4d2 后台管理", theme="ang")
 
-    @app.get('/l4d2/admin', response_class=HTMLResponse)
+    @app.get("/l4d2/admin", response_class=HTMLResponse)
     async def admin_page_app():
-        return admin_app.render(site_title='l4d2-l4d2 后台管理',
-                                theme='ang',
-                                requestAdaptor=requestAdaptor,
-                                responseAdaptor=responseAdaptor)
-
+        return admin_app.render(
+            site_title="l4d2-l4d2 后台管理",
+            theme="ang",
+            requestAdaptor=requestAdaptor,
+            responseAdaptor=responseAdaptor,
+        )
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,254 +1,433 @@
-from amis import  ActionType, TableCRUD, TableColumn
-from amis import  PageSchema, Switch, InputNumber, InputTag, Action, App
-from amis import Form, InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page, AmisAPI, Wrapper
-from amis import LevelEnum, Select,  Alert, Tpl, Flex
+from amis import ActionType, TableCRUD, TableColumn
+from amis import PageSchema, Switch, InputNumber, InputTag, Action, App
+from amis import (
+    Form,
+    InputText,
+    InputPassword,
+    DisplayModeEnum,
+    Horizontal,
+    Remark,
+    Html,
+    Page,
+    AmisAPI,
+    Wrapper,
+)
+from amis import LevelEnum, Select, Alert, Tpl, Flex
 
 
 from ..l4d2_utils.config import NICKNAME
 
-logo = Html(html='''
+logo = Html(
+    html="""
 <p align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server">
         <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
          width="256" height="256" alt="l4d2-server">
     </a>
 </p>
 <h1 align="center">Nonebot-Plugin-L4d2-Server 控制台</h1>
 <div align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/" target="_blank">
     Github仓库</a>
 </div>
 <br>
 <br>
-''')
+"""
+)
 login_api = AmisAPI(
-    url='/l4d2/api/login',
-    method='post',
-    adaptor='''
+    url="/l4d2/api/login",
+    method="post",
+    adaptor="""
         if (payload.status == 0) {
             localStorage.setItem("token", payload.data.token);
         }
         return payload;
-    '''
+    """,
 )
 
-login_form = Form(api=login_api, title='', body=[
-    InputText(name='username', label='用户名',
-              labelRemark=Remark(shape='circle', content='后台管理用户名，默认为l4d2')),
-    InputPassword(name='password', label='密码',
-                  labelRemark=Remark(shape='circle', content='后台管理密码，默认为admin')),
-], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5), redirect='/l4d2/admin')
-body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
-login_page = Page(title='', body=[logo, body])
+login_form = Form(
+    api=login_api,
+    title="",
+    body=[
+        InputText(
+            name="username",
+            label="用户名",
+            labelRemark=Remark(shape="circle", content="后台管理用户名，默认为l4d2"),
+        ),
+        InputPassword(
+            name="password",
+            label="密码",
+            labelRemark=Remark(shape="circle", content="后台管理密码，默认为admin"),
+        ),
+    ],
+    mode=DisplayModeEnum.horizontal,
+    horizontal=Horizontal(left=3, right=9, offset=5),
+    redirect="/l4d2/admin",
+)
+body = Wrapper(className="w-2/5 mx-auto my-0 m:w-full", body=login_form)
+login_page = Page(title="", body=[logo, body])
 
 global_config_form = Form(
-    title='全局配置',
-    name='global_config',
-    initApi='/l4d2/api/l4d2_global_config',
-    api='post:/l4d2/api/l4d2_global_config',
+    title="全局配置",
+    name="global_config",
+    initApi="/l4d2/api/l4d2_global_config",
+    api="post:/l4d2/api/l4d2_global_config",
     body=[
-        Switch(label='控制总开关（摆设）', name='total_enable', value='${total_enable}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle',
-                                  content='关闭后，禁用网页控制台，请参考文档启动方法')),
-        InputText(label='后台管理用户名', name='web_username', value='${web_username}',
-                  labelRemark=Remark(shape='circle',
-                                     content='登录本后台管理所需要的用户名。')),
-        InputPassword(label='后台管理密码', name='web_password', value='${web_password}',
-                      labelRemark=Remark(shape='circle',
-                                         content='登录本后台管理所需要的密码。')),
-        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于本后台管理加密验证token的密钥。')),
-        InputText(label='字体', name='l4_font', value='${l4_font}',
-                  labelRemark=Remark(shape='circle',
-                                     content='机器人返回图片中文字的字体。')),
-        Select(label='图片风格', name='l4_style', value='${l4_style}',source='${l4_styles}',
-                  labelRemark=Remark(shape='circle',
-                                     content='仅仅是批量查询的风格')),
-        Switch(label='是否优先上传地图', name='l4_only', value='${l4_only}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle',
-                                  content='开启时，上传地图会保证优先级，从而阻碍其他指令')),
-        Switch(label='是否显示connect', name='l4_connect', value='${l4_connect}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle',
-                                  content='关闭后，查询服务器将不再显示connect和ip地址')),
-        InputNumber(label='定时推送间隔（min）', name='l4_push_interval', value='${l4_push_interval}',
-                  labelRemark=Remark(shape='circle',
-                                     content='设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次')),
-        InputNumber(label='定时推次数', name='l4_push_times', value='${l4_push_times}',
-                  labelRemark=Remark(shape='circle',
-                                     content='设置好后，将按照推送间隔时间推送x此')),        
-        InputNumber(label='当前路径序号', name='l4_number', value='${l4_number}',
-                  labelRemark=Remark(shape='circle',
-                                     content='如果选定了路径，则上传地图优先传这个路径')),     
-        InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
-                 enableBatchAdd=True,
-                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='在这里加入的用户，才能上传地图')),           
-
-        InputTag(label='坐牢三指令tag', name='l4_zl_tag', value='${l4_zl_tag}',
-                 enableBatchAdd=True,
-                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle',
-                                    content='在这里的指令，可以响应坐牢三指令')),
-
+        Switch(
+            label="控制总开关（摆设）",
+            name="total_enable",
+            value="${total_enable}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(shape="circle", content="关闭后，禁用网页控制台，请参考文档启动方法"),
+        ),
+        InputText(
+            label="后台管理用户名",
+            name="web_username",
+            value="${web_username}",
+            labelRemark=Remark(shape="circle", content="登录本后台管理所需要的用户名。"),
+        ),
+        InputPassword(
+            label="后台管理密码",
+            name="web_password",
+            value="${web_password}",
+            labelRemark=Remark(shape="circle", content="登录本后台管理所需要的密码。"),
+        ),
+        InputText(
+            label="后台管理token密钥",
+            name="web_secret_key",
+            value="${web_secret_key}",
+            labelRemark=Remark(shape="circle", content="用于本后台管理加密验证token的密钥。"),
+        ),
+        InputText(
+            label="字体",
+            name="l4_font",
+            value="${l4_font}",
+            labelRemark=Remark(shape="circle", content="机器人返回图片中文字的字体。"),
+        ),
+        Select(
+            label="图片风格",
+            name="l4_style",
+            value="${l4_style}",
+            source="${l4_styles}",
+            labelRemark=Remark(shape="circle", content="仅仅是批量查询的风格"),
+        ),
+        Switch(
+            label="是否优先上传地图",
+            name="l4_only",
+            value="${l4_only}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(shape="circle", content="开启时，上传地图会保证优先级，从而阻碍其他指令"),
+        ),
+        Switch(
+            label="是否显示connect",
+            name="l4_connect",
+            value="${l4_connect}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(shape="circle", content="关闭后，查询服务器将不再显示connect和ip地址"),
+        ),
+        InputNumber(
+            label="定时推送间隔（min）",
+            name="l4_push_interval",
+            value="${l4_push_interval}",
+            labelRemark=Remark(shape="circle", content="设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次"),
+        ),
+        InputNumber(
+            label="定时推次数",
+            name="l4_push_times",
+            value="${l4_push_times}",
+            labelRemark=Remark(shape="circle", content="设置好后，将按照推送间隔时间推送x此"),
+        ),
+        InputNumber(
+            label="当前路径序号",
+            name="l4_number",
+            value="${l4_number}",
+            labelRemark=Remark(shape="circle", content="如果选定了路径，则上传地图优先传这个路径"),
+        ),
+        InputTag(
+            label="求生上传地图用户",
+            name="l4_master",
+            value="${l4_master}",
+            enableBatchAdd=True,
+            placeholder="添加qq号",
+            visibleOn="${total_enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(shape="circle", content="在这里加入的用户，才能上传地图"),
+        ),
+        InputTag(
+            label="坐牢三指令tag",
+            name="l4_zl_tag",
+            value="${l4_zl_tag}",
+            enableBatchAdd=True,
+            placeholder="添加qq号",
+            visibleOn="${total_enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(shape="circle", content="在这里的指令，可以响应坐牢三指令"),
+        ),
+    ],
+    actions=[
+        Action(label="保存", level=LevelEnum.success, type="submit"),
+        Action(label="重置", level=LevelEnum.warning, type="reset"),
     ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
 
 upload_map_form = Form(
-    title='全局配置',
-    name='global_config',
-    api='post:/l4d2/api/l4d2_map_config',
+    title="全局配置",
+    name="global_config",
+    api="post:/l4d2/api/l4d2_map_config",
     body=[
-        InputText(label='服务器host', name='web_username', value='${web_username}',
-                  labelRemark=Remark(shape='circle',
-                                     content='127.0.0.1')),
-        InputPassword(label='服务器', name='web_password', value='${web_password}',
-                      labelRemark=Remark(shape='circle',
-                                         content='登录本后台管理所需要的密码。')),
-        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于本后台管理加密验证token的密钥。')),
-        InputText(label='查询key', name='l4_key', value='${l4_key}',
-                  labelRemark=Remark(shape='circle',
-                                     content='用于获取拓展功能的key。')),
-
+        InputText(
+            label="服务器host",
+            name="web_username",
+            value="${web_username}",
+            labelRemark=Remark(shape="circle", content="127.0.0.1"),
+        ),
+        InputPassword(
+            label="服务器",
+            name="web_password",
+            value="${web_password}",
+            labelRemark=Remark(shape="circle", content="登录本后台管理所需要的密码。"),
+        ),
+        InputText(
+            label="后台管理token密钥",
+            name="web_secret_key",
+            value="${web_secret_key}",
+            labelRemark=Remark(shape="circle", content="用于本后台管理加密验证token的密钥。"),
+        ),
+        InputText(
+            label="查询key",
+            name="l4_key",
+            value="${l4_key}",
+            labelRemark=Remark(shape="circle", content="用于获取拓展功能的key。"),
+        ),
+    ],
+    actions=[
+        Action(label="保存", level=LevelEnum.success, type="submit"),
+        Action(label="重置", level=LevelEnum.warning, type="reset"),
     ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
 
 
-group_select = Select(label='分群配置（暂未完成）', name='group_id', source='${group_list}',
-                      placeholder='选择群')
+group_select = Select(
+    label="分群配置（暂未完成）", name="group_id", source="${group_list}", placeholder="选择群"
+)
 group_config_form = Form(
-    title='分群配置（暂未完成）',
-    visibleOn='group_id != null',
-    initApi='/l4d2/api/l4d2_group_config?group_id=${group_id}',
-    api='post:/l4d2/api/l4d2_group_config?group_id=${group_id}',
+    title="分群配置（暂未完成）",
+    visibleOn="group_id != null",
+    initApi="/l4d2/api/l4d2_group_config?group_id=${group_id}",
+    api="post:/l4d2/api/l4d2_group_config?group_id=${group_id}",
     body=[
-        Switch(label='分群开关', name='enable', value='${enable}', onText='开启', offText='关闭',
-               labelRemark=Remark(shape='circle', content='针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。')),
-        InputNumber(label='占位符', name='answer_threshold', value='${answer_threshold}', visibleOn='${enable}',
-                    min=2,
-                    labelRemark=Remark(shape='circle', content='单文本')),
-        InputTag(label='占位符', name='ban_words', value='${ban_words}', enableBatchAdd=True,
-                 placeholder='占位符，词条', visibleOn='${enable}', joinValues=False, extractValue=True,
-                 labelRemark=Remark(shape='circle', content='占位符词条')),
-
-    ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             ActionType.Ajax(
-                 label='保存至所有群',
-                 level=LevelEnum.primary,
-                 confirmText='确认将当前配置保存至所有群？',
-                 api='post:/l4d2/api/l4d2_group_config?group_id=all'
-             ),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
-)
-
-server_control = Select(label='服务器设置', name='id_rank', source='${server_list}',
-                      placeholder='选择服务器')
-
-server_ditail= Form(
-    title='',
-    api='post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
-    initApi='/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
-    visibleOn='id_rank != null',
+        Switch(
+            label="分群开关",
+            name="enable",
+            value="${enable}",
+            onText="开启",
+            offText="关闭",
+            labelRemark=Remark(shape="circle", content="针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。"),
+        ),
+        InputNumber(
+            label="占位符",
+            name="answer_threshold",
+            value="${answer_threshold}",
+            visibleOn="${enable}",
+            min=2,
+            labelRemark=Remark(shape="circle", content="单文本"),
+        ),
+        InputTag(
+            label="占位符",
+            name="ban_words",
+            value="${ban_words}",
+            enableBatchAdd=True,
+            placeholder="占位符，词条",
+            visibleOn="${enable}",
+            joinValues=False,
+            extractValue=True,
+            labelRemark=Remark(shape="circle", content="占位符词条"),
+        ),
+    ],
+    actions=[
+        Action(label="保存", level=LevelEnum.success, type="submit"),
+        ActionType.Ajax(
+            label="保存至所有群",
+            level=LevelEnum.primary,
+            confirmText="确认将当前配置保存至所有群？",
+            api="post:/l4d2/api/l4d2_group_config?group_id=all",
+        ),
+        Action(label="重置", level=LevelEnum.warning, type="reset"),
+    ],
+)
+
+server_control = Select(
+    label="服务器设置", name="id_rank", source="${server_list}", placeholder="选择服务器"
+)
+
+server_ditail = Form(
+    title="",
+    api="post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}",
+    initApi="/l4d2/api/l4d2_server_config?id_rank=${id_rank}",
+    visibleOn="id_rank != null",
     body=[
-        Switch(label='是否是远程服务器', name='place', value='${place}', onText='是的', offText='不是',
-               labelRemark=Remark(shape='circle',
-                                  content='开启则确认为远程服务器')),
-        InputText(label='服务器名称', name='server_id', value='${server_id}',
-                  labelRemark=Remark(shape='circle',
-                                     content='服务器名字')),
-        InputText(label='服务器ip地址', name='host', value='${host}',
-                  labelRemark=Remark(shape='circle',
-                                     content='服务端所在ip地址,也可以是域名')),
-        InputText(label='所在端口', name='port', value='${port}',
-                      labelRemark=Remark(shape='circle',
-                                         content='服务端所在端口')),
-        InputPassword(label='rcon控制台密码', name='rcon', value='${rcon}',
-                      labelRemark=Remark(shape='circle',
-                                         content='服务端rcon密码')),
-        InputText(label='服务器本地文件位置', name='location', value='${location}',
-                      labelRemark=Remark(shape='circle',
-                                         content='求生服务器所在路径,该路径下有文件srcds_run')),        
-        InputText(label='远程账户', name='account', value='${account}',
-                  visibleOn='${place}',
-                  labelRemark=Remark(shape='circle',
-                                     content='远程服务器的登录账户名')),
-        InputPassword(label='远程密码', name='password', value='${password}',
-                      visibleOn='${place}',
-                  labelRemark=Remark(shape='circle',
-                                     content='远程服务器的登录密码')),
-    ],
-    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
-             Action(label='重置', level=LevelEnum.warning, type='reset')]
-)
-
-query_table = TableCRUD(mode='table',
-                          title='',
-                          syncLocation=False,
-                          api='/l4d2/api/get_query_contexts',
-                          interval=60000,
-                          footable=True,
-                          itemActions=[ActionType.Url(
-                                tooltip='加入游戏',
-                                icon='fa fa-gamepad',
-                                confirmText = "加入steam://connect/"+'${ip}',
-                                url= "steam://connect/"+'${ip}',
-                                # url= "http://"+'${ip}',
-                                blank= True
-                                 ),
-                            ],
-                          columns = [
-                                    TableColumn(label='服主', name='master', searchable=True),
-                                    TableColumn(label='名称', name='name', searchable=True),
-                                    TableColumn(label='地图', name='map_', searchable=True),
-                                    TableColumn(label='玩家', name='rank_players', searchable=True),
-                                    TableColumn(label='延迟', name='ping', searchable=True),
-                                    TableColumn(label='IP 地址', name='ip', searchable=True),
-                                    ])
-
-server_page = PageSchema(url='/messages', icon='fa fa-comment', label='本地服务器管理',
-                          schema=Page(title='本地服务器管理',
-                                      interval=120000,
-                                      initApi='/l4d2/api/get_l4d2_messages',
-                                        body=[
-                              Alert(level=LevelEnum.info,
-                                    className='white-space-pre-wrap',
-                                    body=(f'此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n'
-
-                                          f'· 功能暂未完善')),
-                              server_control,server_ditail]))
-query_page = PageSchema(url='/contexts', icon='fa fa-comments', label='远程服务器查询',
-                          schema=Page(title='远程服务器查询',
-                                      body=[Alert(level=LevelEnum.info,
-                                                  className='white-space-pre-wrap',
-                                                  body=(f'此数据库记录了{NICKNAME}所记录可查询的服务器ip。\n'
-                                                        # '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
-                                                        # '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
-                                                        f'· 功能暂未完善')),
-                                            query_table]))
-
-database_page = PageSchema(label='数据库', icon='fa fa-database',
-                           children=[server_page, query_page])
-config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='配置',
-                         schema=Page(title='配置', initApi='/l4d2/api/get_group_list',
-                                     body=[global_config_form,group_select, group_config_form]))
-l4d2_page = PageSchema(label='求生之路', icon='fa fa-wechat (alias)', children=[config_page, database_page])
-
-github_logo = Tpl(className='w-full',
-                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>')
-header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
-
-admin_app = App(brandName='L4d2-Server',
-                logo='https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png',
-                header=header,
-                pages=[{
-                    'children': [config_page, database_page]
-                }],
-                footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>')
+        Switch(
+            label="是否是远程服务器",
+            name="place",
+            value="${place}",
+            onText="是的",
+            offText="不是",
+            labelRemark=Remark(shape="circle", content="开启则确认为远程服务器"),
+        ),
+        InputText(
+            label="服务器名称",
+            name="server_id",
+            value="${server_id}",
+            labelRemark=Remark(shape="circle", content="服务器名字"),
+        ),
+        InputText(
+            label="服务器ip地址",
+            name="host",
+            value="${host}",
+            labelRemark=Remark(shape="circle", content="服务端所在ip地址,也可以是域名"),
+        ),
+        InputText(
+            label="所在端口",
+            name="port",
+            value="${port}",
+            labelRemark=Remark(shape="circle", content="服务端所在端口"),
+        ),
+        InputPassword(
+            label="rcon控制台密码",
+            name="rcon",
+            value="${rcon}",
+            labelRemark=Remark(shape="circle", content="服务端rcon密码"),
+        ),
+        InputText(
+            label="服务器本地文件位置",
+            name="location",
+            value="${location}",
+            labelRemark=Remark(shape="circle", content="求生服务器所在路径,该路径下有文件srcds_run"),
+        ),
+        InputText(
+            label="远程账户",
+            name="account",
+            value="${account}",
+            visibleOn="${place}",
+            labelRemark=Remark(shape="circle", content="远程服务器的登录账户名"),
+        ),
+        InputPassword(
+            label="远程密码",
+            name="password",
+            value="${password}",
+            visibleOn="${place}",
+            labelRemark=Remark(shape="circle", content="远程服务器的登录密码"),
+        ),
+    ],
+    actions=[
+        Action(label="保存", level=LevelEnum.success, type="submit"),
+        Action(label="重置", level=LevelEnum.warning, type="reset"),
+    ],
+)
+
+query_table = TableCRUD(
+    mode="table",
+    title="",
+    syncLocation=False,
+    api="/l4d2/api/get_query_contexts",
+    interval=60000,
+    footable=True,
+    itemActions=[
+        ActionType.Url(
+            tooltip="加入游戏",
+            icon="fa fa-gamepad",
+            confirmText="加入steam://connect/" + "${ip}",
+            url="steam://connect/" + "${ip}",
+            # url= "http://"+'${ip}',
+            blank=True,
+        ),
+    ],
+    columns=[
+        TableColumn(label="服主", name="master", searchable=True),
+        TableColumn(label="名称", name="name", searchable=True),
+        TableColumn(label="地图", name="map_", searchable=True),
+        TableColumn(label="玩家", name="rank_players", searchable=True),
+        TableColumn(label="延迟", name="ping", searchable=True),
+        TableColumn(label="IP 地址", name="ip", searchable=True),
+    ],
+)
+
+server_page = PageSchema(
+    url="/messages",
+    icon="fa fa-comment",
+    label="本地服务器管理",
+    schema=Page(
+        title="本地服务器管理",
+        interval=120000,
+        initApi="/l4d2/api/get_l4d2_messages",
+        body=[
+            Alert(
+                level=LevelEnum.info,
+                className="white-space-pre-wrap",
+                body=(f"此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n" f"· 功能暂未完善"),
+            ),
+            server_control,
+            server_ditail,
+        ],
+    ),
+)
+query_page = PageSchema(
+    url="/contexts",
+    icon="fa fa-comments",
+    label="远程服务器查询",
+    schema=Page(
+        title="远程服务器查询",
+        body=[
+            Alert(
+                level=LevelEnum.info,
+                className="white-space-pre-wrap",
+                body=(
+                    f"此数据库记录了{NICKNAME}所记录可查询的服务器ip。\n"
+                    # '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
+                    # '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
+                    f"· 功能暂未完善"
+                ),
+            ),
+            query_table,
+        ],
+    ),
+)
+
+database_page = PageSchema(
+    label="数据库", icon="fa fa-database", children=[server_page, query_page]
+)  # type: ignore
+config_page = PageSchema(
+    url="/configs",
+    isDefaultPage=True,
+    icon="fa fa-wrench",
+    label="配置",
+    schema=Page(
+        title="配置",
+        initApi="/l4d2/api/get_group_list",
+        body=[global_config_form, group_select, group_config_form],
+    ),
+)
+l4d2_page = PageSchema(
+    label="求生之路", icon="fa fa-wechat (alias)", children=[config_page, database_page]
+)  # type: ignore
+
+github_logo = Tpl(
+    className="w-full",
+    tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>',
+)
+header = Flex(
+    className="w-full", justify="flex-end", alignItems="flex-end", items=[github_logo]
+)
+
+admin_app = App(
+    brandName="L4d2-Server",
+    logo="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png",
+    header=header,
+    pages=[{"children": [config_page, database_page]}],
+    footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>',
+)
```

#### html2text {}

```diff
@@ -1,161 +1,162 @@
 from amis import ActionType, TableCRUD, TableColumn from amis import
-PageSchema, Switch, InputNumber, InputTag, Action, App from amis import Form,
+PageSchema, Switch, InputNumber, InputTag, Action, App from amis import ( Form,
 InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page,
-AmisAPI, Wrapper from amis import LevelEnum, Select, Alert, Tpl, Flex from
-..l4d2_utils.config import NICKNAME logo = Html(html='''
+AmisAPI, Wrapper, ) from amis import LevelEnum, Select, Alert, Tpl, Flex from
+..l4d2_utils.config import NICKNAME logo = Html( html="""
                                  [l4d2-server]
               ****** Nonebot-Plugin-L4d2-Server æ§å¶å° ******
                                  Githubä»åº
 
 
-''') login_api = AmisAPI( url='/l4d2/api/login', method='post', adaptor=''' if
+""" ) login_api = AmisAPI( url="/l4d2/api/login", method="post", adaptor=""" if
 (payload.status == 0) { localStorage.setItem("token", payload.data.token); }
-return payload; ''' ) login_form = Form(api=login_api, title='', body=
-[ InputText(name='username', label='ç¨æ·å', labelRemark=Remark
-(shape='circle', content='åå°ç®¡çç¨æ·åï¼é»è®¤ä¸ºl4d2')),
-InputPassword(name='password', label='å¯ç ', labelRemark=Remark
-(shape='circle', content='åå°ç®¡çå¯ç ï¼é»è®¤ä¸ºadmin')), ],
+return payload; """, ) login_form = Form( api=login_api, title="", body=
+[ InputText( name="username", label="ç¨æ·å", labelRemark=Remark
+(shape="circle", content="åå°ç®¡çç¨æ·åï¼é»è®¤ä¸ºl4d2"), ),
+InputPassword( name="password", label="å¯ç ", labelRemark=Remark
+(shape="circle", content="åå°ç®¡çå¯ç ï¼é»è®¤ä¸ºadmin"), ), ],
 mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9,
-offset=5), redirect='/l4d2/admin') body = Wrapper(className='w-2/5 mx-auto my-
-0 m:w-full', body=login_form) login_page = Page(title='', body=[logo, body])
-global_config_form = Form( title='å¨å±éç½®', name='global_config',
-initApi='/l4d2/api/l4d2_global_config', api='post:/l4d2/api/
-l4d2_global_config', body=[ Switch(label='æ§å¶æ»å¼å³ï¼æè®¾ï¼',
-name='total_enable', value='${total_enable}', onText='å¼å¯',
-offText='å³é­', labelRemark=Remark(shape='circle',
-content='å³é­åï¼ç¦ç¨ç½é¡µæ§å¶å°ï¼è¯·åèææ¡£å¯å¨æ¹æ³')),
-InputText(label='åå°ç®¡çç¨æ·å', name='web_username', value='$
-{web_username}', labelRemark=Remark(shape='circle',
-content='ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã')), InputPassword
-(label='åå°ç®¡çå¯ç ', name='web_password', value='${web_password}',
-labelRemark=Remark(shape='circle',
-content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
-(label='åå°ç®¡çtokenå¯é¥', name='web_secret_key', value='$
-{web_secret_key}', labelRemark=Remark(shape='circle',
-content='ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã')), InputText
-(label='å­ä½', name='l4_font', value='${l4_font}', labelRemark=Remark
-(shape='circle', content='æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã')), Select
-(label='å¾çé£æ ¼', name='l4_style', value='${l4_style}',source='$
-{l4_styles}', labelRemark=Remark(shape='circle',
-content='ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼')), Switch
-(label='æ¯å¦ä¼åä¸ä¼ å°å¾', name='l4_only', value='${l4_only}',
-onText='å¼å¯', offText='å³é­', labelRemark=Remark(shape='circle',
-content='å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤')),
-Switch(label='æ¯å¦æ¾ç¤ºconnect', name='l4_connect', value='${l4_connect}',
-onText='å¼å¯', offText='å³é­', labelRemark=Remark(shape='circle',
-content='å³é­åï¼æ¥è¯¢æå¡å¨å°ä¸åæ¾ç¤ºconnectåipå°å')),
-InputNumber(label='å®æ¶æ¨éé´éï¼minï¼', name='l4_push_interval',
-value='${l4_push_interval}', labelRemark=Remark(shape='circle',
-content='è®¾ç½®å¥½åï¼ä½¿ç¨æ¨éæå¡å¨å®æ¶æä»¤ï¼å°ä»¥xåéä¸ºé´éæ¨éä¸æ¬¡')),
-InputNumber(label='å®æ¶æ¨æ¬¡æ°', name='l4_push_times', value='$
-{l4_push_times}', labelRemark=Remark(shape='circle',
-content='è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤')), InputNumber
-(label='å½åè·¯å¾åºå·', name='l4_number', value='${l4_number}',
-labelRemark=Remark(shape='circle',
-content='å¦æéå®äºè·¯å¾ï¼åä¸ä¼ å°å¾ä¼åä¼ è¿ä¸ªè·¯å¾')),
-InputTag(label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='$
-{l4_master}', enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='$
-{total_enable}', joinValues=False, extractValue=True, labelRemark=Remark
-(shape='circle', content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')),
-InputTag(label='åç¢ä¸æä»¤tag', name='l4_zl_tag', value='${l4_zl_tag}',
-enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
-joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
-content='å¨è¿éçæä»¤ï¼å¯ä»¥ååºåç¢ä¸æä»¤')), ], actions=
-[Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
-(label='éç½®', level=LevelEnum.warning, type='reset')] ) upload_map_form =
-Form( title='å¨å±éç½®', name='global_config', api='post:/l4d2/api/
-l4d2_map_config', body=[ InputText(label='æå¡å¨host', name='web_username',
-value='${web_username}', labelRemark=Remark(shape='circle',
-content='127.0.0.1')), InputPassword(label='æå¡å¨', name='web_password',
-value='${web_password}', labelRemark=Remark(shape='circle',
-content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
-(label='åå°ç®¡çtokenå¯é¥', name='web_secret_key', value='$
-{web_secret_key}', labelRemark=Remark(shape='circle',
-content='ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã')), InputText
-(label='æ¥è¯¢key', name='l4_key', value='${l4_key}', labelRemark=Remark
-(shape='circle', content='ç¨äºè·åæå±åè½çkeyã')), ], actions=
-[Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
-(label='éç½®', level=LevelEnum.warning, type='reset')] ) group_select =
-Select(label='åç¾¤éç½®ï¼ææªå®æï¼', name='group_id', source='$
-{group_list}', placeholder='éæ©ç¾¤') group_config_form = Form
-( title='åç¾¤éç½®ï¼ææªå®æï¼', visibleOn='group_id != null',
-initApi='/l4d2/api/l4d2_group_config?group_id=${group_id}', api='post:/l4d2/
-api/l4d2_group_config?group_id=${group_id}', body=[ Switch
-(label='åç¾¤å¼å³', name='enable', value='${enable}', onText='å¼å¯',
-offText='å³é­', labelRemark=Remark(shape='circle',
-content='éå¯¹è¯¥ç¾¤çç¾¤èå­¦ä¹ å¼å³ï¼å³é­åï¼ä»è¯¥ç¾¤ä¸ä¼å­¦ä¹ ååå¤ã')),
-InputNumber(label='å ä½ç¬¦', name='answer_threshold', value='$
-{answer_threshold}', visibleOn='${enable}', min=2, labelRemark=Remark
-(shape='circle', content='åææ¬')), InputTag(label='å ä½ç¬¦',
-name='ban_words', value='${ban_words}', enableBatchAdd=True,
-placeholder='å ä½ç¬¦ï¼è¯æ¡', visibleOn='${enable}', joinValues=False,
-extractValue=True, labelRemark=Remark(shape='circle',
-content='å ä½ç¬¦è¯æ¡')), ], actions=[Action(label='ä¿å­',
-level=LevelEnum.success, type='submit'), ActionType.Ajax
-( label='ä¿å­è³ææç¾¤', level=LevelEnum.primary,
-confirmText='ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼', api='post:/l4d2/api/
-l4d2_group_config?group_id=all' ), Action(label='éç½®',
-level=LevelEnum.warning, type='reset')] ) server_control = Select
-(label='æå¡å¨è®¾ç½®', name='id_rank', source='${server_list}',
-placeholder='éæ©æå¡å¨') server_ditail= Form( title='', api='post:/l4d2/
-api/l4d2_server_config?id_rank=${id_rank}', initApi='/l4d2/api/
-l4d2_server_config?id_rank=${id_rank}', visibleOn='id_rank != null', body=
-[ Switch(label='æ¯å¦æ¯è¿ç¨æå¡å¨', name='place', value='${place}',
-onText='æ¯ç', offText='ä¸æ¯', labelRemark=Remark(shape='circle',
-content='å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨')), InputText
-(label='æå¡å¨åç§°', name='server_id', value='${server_id}',
-labelRemark=Remark(shape='circle', content='æå¡å¨åå­')), InputText
-(label='æå¡å¨ipå°å', name='host', value='${host}', labelRemark=Remark
-(shape='circle', content='æå¡ç«¯æå¨ipå°å,ä¹å¯ä»¥æ¯åå')),
-InputText(label='æå¨ç«¯å£', name='port', value='${port}',
-labelRemark=Remark(shape='circle', content='æå¡ç«¯æå¨ç«¯å£')),
-InputPassword(label='rconæ§å¶å°å¯ç ', name='rcon', value='${rcon}',
-labelRemark=Remark(shape='circle', content='æå¡ç«¯rconå¯ç ')), InputText
-(label='æå¡å¨æ¬å°æä»¶ä½ç½®', name='location', value='${location}',
-labelRemark=Remark(shape='circle',
-content='æ±çæå¡å¨æå¨è·¯å¾,è¯¥è·¯å¾ä¸ææä»¶srcds_run')),
-InputText(label='è¿ç¨è´¦æ·', name='account', value='${account}',
-visibleOn='${place}', labelRemark=Remark(shape='circle',
-content='è¿ç¨æå¡å¨çç»å½è´¦æ·å')), InputPassword
-(label='è¿ç¨å¯ç ', name='password', value='${password}', visibleOn='$
-{place}', labelRemark=Remark(shape='circle',
-content='è¿ç¨æå¡å¨çç»å½å¯ç ')), ], actions=[Action(label='ä¿å­',
-level=LevelEnum.success, type='submit'), Action(label='éç½®',
-level=LevelEnum.warning, type='reset')] ) query_table = TableCRUD(mode='table',
-title='', syncLocation=False, api='/l4d2/api/get_query_contexts',
-interval=60000, footable=True, itemActions=[ActionType.Url
-( tooltip='å å¥æ¸¸æ', icon='fa fa-gamepad', confirmText = "å å¥steam://
-connect/"+'${ip}', url= "steam://connect/"+'${ip}', # url= "http://"+'${ip}',
-blank= True ), ], columns = [ TableColumn(label='æä¸»', name='master',
-searchable=True), TableColumn(label='åç§°', name='name', searchable=True),
-TableColumn(label='å°å¾', name='map_', searchable=True), TableColumn
-(label='ç©å®¶', name='rank_players', searchable=True), TableColumn
-(label='å»¶è¿', name='ping', searchable=True), TableColumn(label='IP å°å',
-name='ip', searchable=True), ]) server_page = PageSchema(url='/messages',
-icon='fa fa-comment', label='æ¬å°æå¡å¨ç®¡ç', schema=Page
-(title='æ¬å°æå¡å¨ç®¡ç', interval=120000, initApi='/l4d2/api/
-get_l4d2_messages', body=[ Alert(level=LevelEnum.info, className='white-space-
-pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
-{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n' f'Â·
-åè½ææªå®å')), server_control,server_ditail])) query_page = PageSchema
-(url='/contexts', icon='fa fa-comments', label='è¿ç¨æå¡å¨æ¥è¯¢',
-schema=Page(title='è¿ç¨æå¡å¨æ¥è¯¢', body=[Alert(level=LevelEnum.info,
-className='white-space-pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
-{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n' # 'Â·
+offset=5), redirect="/l4d2/admin", ) body = Wrapper(className="w-2/5 mx-auto
+my-0 m:w-full", body=login_form) login_page = Page(title="", body=[logo, body])
+global_config_form = Form( title="å¨å±éç½®", name="global_config",
+initApi="/l4d2/api/l4d2_global_config", api="post:/l4d2/api/
+l4d2_global_config", body=[ Switch( label="æ§å¶æ»å¼å³ï¼æè®¾ï¼",
+name="total_enable", value="${total_enable}", onText="å¼å¯",
+offText="å³é­", labelRemark=Remark(shape="circle",
+content="å³é­åï¼ç¦ç¨ç½é¡µæ§å¶å°ï¼è¯·åèææ¡£å¯å¨æ¹æ³"), ),
+InputText( label="åå°ç®¡çç¨æ·å", name="web_username", value="$
+{web_username}", labelRemark=Remark(shape="circle",
+content="ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã"), ), InputPassword
+( label="åå°ç®¡çå¯ç ", name="web_password", value="${web_password}",
+labelRemark=Remark(shape="circle",
+content="ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã"), ), InputText
+( label="åå°ç®¡çtokenå¯é¥", name="web_secret_key", value="$
+{web_secret_key}", labelRemark=Remark(shape="circle",
+content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã"), ), InputText
+( label="å­ä½", name="l4_font", value="${l4_font}", labelRemark=Remark
+(shape="circle", content="æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã"), ),
+Select( label="å¾çé£æ ¼", name="l4_style", value="${l4_style}", source="$
+{l4_styles}", labelRemark=Remark(shape="circle",
+content="ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼"), ), Switch
+( label="æ¯å¦ä¼åä¸ä¼ å°å¾", name="l4_only", value="${l4_only}",
+onText="å¼å¯", offText="å³é­", labelRemark=Remark(shape="circle",
+content="å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤"),
+), Switch( label="æ¯å¦æ¾ç¤ºconnect", name="l4_connect", value="$
+{l4_connect}", onText="å¼å¯", offText="å³é­", labelRemark=Remark
+(shape="circle",
+content="å³é­åï¼æ¥è¯¢æå¡å¨å°ä¸åæ¾ç¤ºconnectåipå°å"), ),
+InputNumber( label="å®æ¶æ¨éé´éï¼minï¼", name="l4_push_interval",
+value="${l4_push_interval}", labelRemark=Remark(shape="circle",
+content="è®¾ç½®å¥½åï¼ä½¿ç¨æ¨éæå¡å¨å®æ¶æä»¤ï¼å°ä»¥xåéä¸ºé´éæ¨éä¸æ¬¡"),
+), InputNumber( label="å®æ¶æ¨æ¬¡æ°", name="l4_push_times", value="$
+{l4_push_times}", labelRemark=Remark(shape="circle",
+content="è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤"), ), InputNumber
+( label="å½åè·¯å¾åºå·", name="l4_number", value="${l4_number}",
+labelRemark=Remark(shape="circle",
+content="å¦æéå®äºè·¯å¾ï¼åä¸ä¼ å°å¾ä¼åä¼ è¿ä¸ªè·¯å¾"), ),
+InputTag( label="æ±çä¸ä¼ å°å¾ç¨æ·", name="l4_master", value="$
+{l4_master}", enableBatchAdd=True, placeholder="æ·»å qqå·", visibleOn="$
+{total_enable}", joinValues=False, extractValue=True, labelRemark=Remark
+(shape="circle", content="å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾"), ),
+InputTag( label="åç¢ä¸æä»¤tag", name="l4_zl_tag", value="${l4_zl_tag}",
+enableBatchAdd=True, placeholder="æ·»å qqå·", visibleOn="${total_enable}",
+joinValues=False, extractValue=True, labelRemark=Remark(shape="circle",
+content="å¨è¿éçæä»¤ï¼å¯ä»¥ååºåç¢ä¸æä»¤"), ), ], actions=
+[ Action(label="ä¿å­", level=LevelEnum.success, type="submit"), Action
+(label="éç½®", level=LevelEnum.warning, type="reset"), ], ) upload_map_form =
+Form( title="å¨å±éç½®", name="global_config", api="post:/l4d2/api/
+l4d2_map_config", body=[ InputText( label="æå¡å¨host", name="web_username",
+value="${web_username}", labelRemark=Remark(shape="circle",
+content="127.0.0.1"), ), InputPassword( label="æå¡å¨", name="web_password",
+value="${web_password}", labelRemark=Remark(shape="circle",
+content="ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã"), ), InputText
+( label="åå°ç®¡çtokenå¯é¥", name="web_secret_key", value="$
+{web_secret_key}", labelRemark=Remark(shape="circle",
+content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã"), ), InputText
+( label="æ¥è¯¢key", name="l4_key", value="${l4_key}", labelRemark=Remark
+(shape="circle", content="ç¨äºè·åæå±åè½çkeyã"), ), ], actions=
+[ Action(label="ä¿å­", level=LevelEnum.success, type="submit"), Action
+(label="éç½®", level=LevelEnum.warning, type="reset"), ], ) group_select =
+Select( label="åç¾¤éç½®ï¼ææªå®æï¼", name="group_id", source="$
+{group_list}", placeholder="éæ©ç¾¤" ) group_config_form = Form
+( title="åç¾¤éç½®ï¼ææªå®æï¼", visibleOn="group_id != null",
+initApi="/l4d2/api/l4d2_group_config?group_id=${group_id}", api="post:/l4d2/
+api/l4d2_group_config?group_id=${group_id}", body=[ Switch
+( label="åç¾¤å¼å³", name="enable", value="${enable}", onText="å¼å¯",
+offText="å³é­", labelRemark=Remark(shape="circle",
+content="éå¯¹è¯¥ç¾¤çç¾¤èå­¦ä¹ å¼å³ï¼å³é­åï¼ä»è¯¥ç¾¤ä¸ä¼å­¦ä¹ ååå¤ã"),
+), InputNumber( label="å ä½ç¬¦", name="answer_threshold", value="$
+{answer_threshold}", visibleOn="${enable}", min=2, labelRemark=Remark
+(shape="circle", content="åææ¬"), ), InputTag( label="å ä½ç¬¦",
+name="ban_words", value="${ban_words}", enableBatchAdd=True,
+placeholder="å ä½ç¬¦ï¼è¯æ¡", visibleOn="${enable}", joinValues=False,
+extractValue=True, labelRemark=Remark(shape="circle",
+content="å ä½ç¬¦è¯æ¡"), ), ], actions=[ Action(label="ä¿å­",
+level=LevelEnum.success, type="submit"), ActionType.Ajax
+( label="ä¿å­è³ææç¾¤", level=LevelEnum.primary,
+confirmText="ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼", api="post:/l4d2/api/
+l4d2_group_config?group_id=all", ), Action(label="éç½®",
+level=LevelEnum.warning, type="reset"), ], ) server_control = Select
+( label="æå¡å¨è®¾ç½®", name="id_rank", source="${server_list}",
+placeholder="éæ©æå¡å¨" ) server_ditail = Form( title="", api="post:/
+l4d2/api/l4d2_server_config?id_rank=${id_rank}", initApi="/l4d2/api/
+l4d2_server_config?id_rank=${id_rank}", visibleOn="id_rank != null", body=
+[ Switch( label="æ¯å¦æ¯è¿ç¨æå¡å¨", name="place", value="${place}",
+onText="æ¯ç", offText="ä¸æ¯", labelRemark=Remark(shape="circle",
+content="å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨"), ), InputText
+( label="æå¡å¨åç§°", name="server_id", value="${server_id}",
+labelRemark=Remark(shape="circle", content="æå¡å¨åå­"), ), InputText
+( label="æå¡å¨ipå°å", name="host", value="${host}", labelRemark=Remark
+(shape="circle", content="æå¡ç«¯æå¨ipå°å,ä¹å¯ä»¥æ¯åå"), ),
+InputText( label="æå¨ç«¯å£", name="port", value="${port}",
+labelRemark=Remark(shape="circle", content="æå¡ç«¯æå¨ç«¯å£"), ),
+InputPassword( label="rconæ§å¶å°å¯ç ", name="rcon", value="${rcon}",
+labelRemark=Remark(shape="circle", content="æå¡ç«¯rconå¯ç "), ), InputText
+( label="æå¡å¨æ¬å°æä»¶ä½ç½®", name="location", value="${location}",
+labelRemark=Remark(shape="circle",
+content="æ±çæå¡å¨æå¨è·¯å¾,è¯¥è·¯å¾ä¸ææä»¶srcds_run"), ),
+InputText( label="è¿ç¨è´¦æ·", name="account", value="${account}",
+visibleOn="${place}", labelRemark=Remark(shape="circle",
+content="è¿ç¨æå¡å¨çç»å½è´¦æ·å"), ), InputPassword
+( label="è¿ç¨å¯ç ", name="password", value="${password}", visibleOn="$
+{place}", labelRemark=Remark(shape="circle",
+content="è¿ç¨æå¡å¨çç»å½å¯ç "), ), ], actions=[ Action
+(label="ä¿å­", level=LevelEnum.success, type="submit"), Action
+(label="éç½®", level=LevelEnum.warning, type="reset"), ], ) query_table =
+TableCRUD( mode="table", title="", syncLocation=False, api="/l4d2/api/
+get_query_contexts", interval=60000, footable=True, itemActions=
+[ ActionType.Url( tooltip="å å¥æ¸¸æ", icon="fa fa-gamepad",
+confirmText="å å¥steam://connect/" + "${ip}", url="steam://connect/" + "$
+{ip}", # url= "http://"+'${ip}', blank=True, ), ], columns=[ TableColumn
+(label="æä¸»", name="master", searchable=True), TableColumn(label="åç§°",
+name="name", searchable=True), TableColumn(label="å°å¾", name="map_",
+searchable=True), TableColumn(label="ç©å®¶", name="rank_players",
+searchable=True), TableColumn(label="å»¶è¿", name="ping", searchable=True),
+TableColumn(label="IP å°å", name="ip", searchable=True), ], ) server_page =
+PageSchema( url="/messages", icon="fa fa-comment",
+label="æ¬å°æå¡å¨ç®¡ç", schema=Page( title="æ¬å°æå¡å¨ç®¡ç",
+interval=120000, initApi="/l4d2/api/get_l4d2_messages", body=[ Alert
+( level=LevelEnum.info, className="white-space-pre-wrap", body=
+(f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n"
+f"Â· åè½ææªå®å"), ), server_control, server_ditail, ], ), ) query_page
+= PageSchema( url="/contexts", icon="fa fa-comments",
+label="è¿ç¨æå¡å¨æ¥è¯¢", schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢",
+body=[ Alert( level=LevelEnum.info, className="white-space-pre-wrap", body=
+( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
-f'Â· åè½ææªå®å')), query_table])) database_page = PageSchema
-(label='æ°æ®åº', icon='fa fa-database', children=[server_page, query_page])
-config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-
-wrench', label='éç½®', schema=Page(title='éç½®', initApi='/l4d2/api/
-get_group_list', body=[global_config_form,group_select, group_config_form]))
-l4d2_page = PageSchema(label='æ±çä¹è·¯', icon='fa fa-wechat (alias)',
-children=[config_page, database_page]) github_logo = Tpl(className='w-full',
-tpl='
-') header = Flex(className='w-full', justify='flex-end', alignItems='flex-end',
-items=[github_logo]) admin_app = App(brandName='L4d2-Server', logo='https://
-raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/
-logo.png', header=header, pages=[{ 'children': [config_page, database_page] }],
-footer='
+f"Â· åè½ææªå®å" ), ), query_table, ], ), ) database_page = PageSchema
+( label="æ°æ®åº", icon="fa fa-database", children=[server_page, query_page]
+) # type: ignore config_page = PageSchema( url="/configs", isDefaultPage=True,
+icon="fa fa-wrench", label="éç½®", schema=Page( title="éç½®", initApi="/
+l4d2/api/get_group_list", body=[global_config_form, group_select,
+group_config_form], ), ) l4d2_page = PageSchema( label="æ±çä¹è·¯", icon="fa
+fa-wechat (alias)", children=[config_page, database_page] ) # type: ignore
+github_logo = Tpl( className="w-full", tpl='
+', ) header = Flex( className="w-full", justify="flex-end", alignItems="flex-
+end", items=[github_logo] ) admin_app = App( brandName="L4d2-Server",
+logo="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/
+main/image/logo.png", header=header, pages=[{"children": [config_page,
+database_page]}], footer='
 Copyright Â© 2022 - 2023 AGNES_DIGIAL Xamis_v2.2.0
-')
+', )
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.8"
+version = "0.5.9"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.8/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.8
+Version: 0.5.9
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.9 Summary:
 L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

