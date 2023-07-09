# Comparing `tmp/dimples-0.2.1.tar.gz` & `tmp/dimples-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.2.1.tar", last modified: Wed Jul  5 17:47:29 2023, max compression
+gzip compressed data, was "dist/dimples-0.2.2.tar", last modified: Sun Jul  9 10:01:21 2023, max compression
```

## Comparing `dimples-0.2.1.tar` & `dimples-0.2.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-05 17:47:29.000000 dimples-0.2.1/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.2.1/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7179 2023-07-05 16:12:35.000000 dimples-0.2.1/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1966 2023-07-05 17:00:59.000000 dimples-0.2.1/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2117 2023-07-05 16:57:49.000000 dimples-0.2.1/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.2.1/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.2.1/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.2.1/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.2.1/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.2.1/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.2.1/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.2.1/dimples/client/cpu/text.py
--rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.2.1/dimples/client/group.py
--rw-r--r--   0 moky       (501) staff       (20)     9952 2023-07-05 17:01:39.000000 dimples-0.2.1/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.2.1/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.2.1/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.2.1/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.2.1/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     7022 2023-07-05 17:01:13.000000 dimples-0.2.1/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.2.1/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2213 2023-07-05 16:06:45.000000 dimples-0.2.1/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5644 2023-06-19 15:11:53.000000 dimples-0.2.1/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.2.1/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.2.1/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.2.1/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.2.1/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.2.1/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.2.1/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.2.1/dimples/common/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2354 2023-07-05 16:06:45.000000 dimples-0.2.1/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.2.1/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.2.1/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.2.1/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.2.1/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.2.1/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.2.1/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.2.1/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.2.1/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.2.1/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.2.1/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.2.1/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.2.1/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.2.1/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.2.1/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.2.1/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7085 2023-06-19 07:42:03.000000 dimples-0.2.1/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.2.1/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.2.1/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.2.1/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.2.1/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.2.1/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.2.1/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.2.1/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.2.1/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.2.1/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.2.1/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.2.1/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.2.1/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.2.1/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.2.1/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.2.1/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.2.1/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.2.1/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.2.1/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.2.1/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.2.1/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5929 2023-06-19 07:20:16.000000 dimples-0.2.1/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.2.1/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.2.1/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.2.1/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2654 2023-07-05 16:58:00.000000 dimples-0.2.1/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8020 2023-06-18 10:50:18.000000 dimples-0.2.1/dimples/server/broadcast.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.2.1/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2652 2023-07-05 17:27:48.000000 dimples-0.2.1/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-19 07:56:29.000000 dimples-0.2.1/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3610 2023-07-05 17:26:22.000000 dimples-0.2.1/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4009 2023-07-05 17:20:53.000000 dimples-0.2.1/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3517 2023-07-05 17:23:20.000000 dimples-0.2.1/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13524 2023-07-05 17:00:59.000000 dimples-0.2.1/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     9473 2023-06-18 09:35:15.000000 dimples-0.2.1/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6638 2023-06-18 11:45:32.000000 dimples-0.2.1/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5615 2023-07-05 17:00:01.000000 dimples-0.2.1/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5448 2023-06-18 14:36:35.000000 dimples-0.2.1/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     7978 2023-06-16 11:57:03.000000 dimples-0.2.1/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)     9722 2023-06-26 11:02:55.000000 dimples-0.2.1/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.2.1/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.2.1/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     6424 2023-06-19 07:20:09.000000 dimples-0.2.1/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-06-18 11:31:20.000000 dimples-0.2.1/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.2.1/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6446 2023-06-18 10:21:27.000000 dimples-0.2.1/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.2.1/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.2.1/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.2.1/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3170 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-07-05 17:47:29.000000 dimples-0.2.1/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-05 17:47:29.000000 dimples-0.2.1/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-07-05 17:12:33.000000 dimples-0.2.1/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-09 10:01:21.000000 dimples-0.2.2/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.2.2/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7179 2023-07-05 16:12:35.000000 dimples-0.2.2/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1966 2023-07-05 17:00:59.000000 dimples-0.2.2/dimples/client/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2117 2023-07-05 16:57:49.000000 dimples-0.2.2/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4460 2023-07-09 09:34:27.000000 dimples-0.2.2/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4324 2023-07-09 09:34:17.000000 dimples-0.2.2/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3807 2023-07-09 09:34:07.000000 dimples-0.2.2/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3959 2023-07-09 09:34:01.000000 dimples-0.2.2/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     7077 2023-07-09 09:33:49.000000 dimples-0.2.2/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.2.2/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     3065 2023-07-09 09:15:32.000000 dimples-0.2.2/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.2.2/dimples/client/cpu/text.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.2.2/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     9952 2023-07-05 17:01:39.000000 dimples-0.2.2/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.2.2/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.2.2/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.2.2/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.2.2/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7022 2023-07-05 17:01:13.000000 dimples-0.2.2/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.2.2/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2213 2023-07-05 16:06:45.000000 dimples-0.2.2/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5644 2023-06-19 15:11:53.000000 dimples-0.2.2/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.2.2/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.2.2/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.2.2/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.2.2/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.2.2/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.2.2/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.2.2/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2354 2023-07-05 16:06:45.000000 dimples-0.2.2/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.2.2/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.2.2/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.2.2/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.2.2/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.2.2/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.2.2/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.2.2/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.2.2/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.2.2/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.2.2/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.2.2/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.2.2/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.2.2/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.2.2/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.2.2/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7085 2023-06-19 07:42:03.000000 dimples-0.2.2/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.2.2/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.2.2/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.2.2/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.2.2/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.2.2/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.2.2/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.2.2/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.2.2/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.2.2/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.2.2/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.2.2/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.2.2/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.2.2/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.2.2/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.2.2/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.2.2/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.2.2/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.2.2/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.2.2/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.2.2/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5929 2023-06-19 07:20:16.000000 dimples-0.2.2/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.2.2/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.2.2/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.2.2/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2654 2023-07-05 16:58:00.000000 dimples-0.2.2/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8020 2023-06-18 10:50:18.000000 dimples-0.2.2/dimples/server/broadcast.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.2.2/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2640 2023-07-09 09:36:32.000000 dimples-0.2.2/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-19 07:56:29.000000 dimples-0.2.2/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3622 2023-07-09 09:09:31.000000 dimples-0.2.2/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4021 2023-07-09 09:04:04.000000 dimples-0.2.2/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3369 2023-07-09 09:09:31.000000 dimples-0.2.2/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13524 2023-07-05 17:00:59.000000 dimples-0.2.2/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     9473 2023-06-18 09:35:15.000000 dimples-0.2.2/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6638 2023-06-18 11:45:32.000000 dimples-0.2.2/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5619 2023-07-09 09:40:25.000000 dimples-0.2.2/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5448 2023-06-18 14:36:35.000000 dimples-0.2.2/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     8005 2023-07-09 09:47:11.000000 dimples-0.2.2/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)     9722 2023-06-26 11:02:55.000000 dimples-0.2.2/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.2.2/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.2.2/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     6424 2023-06-19 07:20:09.000000 dimples-0.2.2/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-06-18 11:31:20.000000 dimples-0.2.2/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.2.2/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6446 2023-06-18 10:21:27.000000 dimples-0.2.2/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.2.2/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.2.2/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.2.2/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3170 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-07-09 10:01:21.000000 dimples-0.2.2/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-07-09 10:01:21.000000 dimples-0.2.2/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-07-09 09:00:39.000000 dimples-0.2.2/setup.py
```

### Comparing `dimples-0.2.1/PKG-INFO` & `dimples-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.2.1
+Version: 0.2.2
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.2.1/README.md` & `dimples-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/__init__.py` & `dimples-0.2.2/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/__init__.py` & `dimples-0.2.2/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/cpu/__init__.py` & `dimples-0.2.2/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/cpu/grp_expel.py` & `dimples-0.2.2/dimples/client/cpu/grp_query.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,78 +25,68 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Expel Group Command Processor
+    Query Group Command Processor
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-    1. remove group member(s)
-    2. only group owner or assistant can expel member
+    1. query for group members-list
+    2. any existed member or assistant can query group members-list
 """
 
 from typing import List
 
 from dimp import ID
 from dimp import ReliableMessage
 from dimp import Content
-from dimp import ExpelCommand
+from dimp import GroupCommand, QueryCommand
+
+from ...common import CommonFacebook
 
 from .history import GroupCommandProcessor
 
 
-class ExpelCommandProcessor(GroupCommandProcessor):
+class QueryCommandProcessor(GroupCommandProcessor):
 
-    STR_EXPEL_CMD_ERROR = 'Expel command error.'
-    STR_EXPEL_NOT_ALLOWED = 'Sorry, you are not allowed to expel member from this group.'
-    STR_CANNOT_EXPEL_OWNER = 'Group owner cannot be expelled.'
+    def _respond_group_members(self, owner: ID, group: ID, members: List[ID]) -> Content:
+        facebook = self.facebook
+        assert isinstance(facebook, CommonFacebook), 'facebook error: %s' % facebook
+        user = facebook.current_user
+        assert user is not None, 'current user not set'
+        if user.identifier == owner:
+            return GroupCommand.reset(group=group, members=members)
+        else:
+            return GroupCommand.invite(group=group, members=members)
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
-        assert isinstance(content, ExpelCommand), 'expel command error: %s' % content
+        assert isinstance(content, QueryCommand), 'query command error: %s' % content
         facebook = self.facebook
         group = content.group
         owner = facebook.owner(identifier=group)
         members = facebook.members(identifier=group)
         # 0. check group
         if owner is None or members is None or len(members) == 0:
-            text = self.STR_GROUP_EMPTY
-            return self._respond_text(text=text, group=group)
+            return self._respond_receipt(text='Group empty.', msg=msg, group=group, extra={
+                'template': 'Group empty: ${ID}',
+                'replacements': {
+                    'ID': str(group),
+                }
+            })
         # 1. check permission
         sender = msg.sender
-        if sender != owner:
-            # not the owner? check assistants
+        if sender not in members:
+            # not a member? check assistants
             assistants = facebook.assistants(identifier=group)
             if assistants is None or sender not in assistants:
-                text = self.STR_EXPEL_NOT_ALLOWED
-                return self._respond_text(text=text, group=group)
-        # 2. expelling members
-        expel_list = self.members(content=content)
-        if expel_list is None or len(expel_list) == 0:
-            text = self.STR_EXPEL_CMD_ERROR
-            return self._respond_text(text=text, group=group)
-        # 2.1. check owner
-        if owner in expel_list:
-            text = self.STR_CANNOT_EXPEL_OWNER
-            return self._respond_text(text=text, group=group)
-        # 2.2. build removed-list
-        remove_list = []
-        for item in expel_list:
-            if item not in members:
-                continue
-            # expelled member found
-            remove_list.append(item)
-            members.remove(item)
-        # 2.3. do expel
-        if len(remove_list) > 0:
-            man = group_manager()
-            if man.save_members(members=members, group=group):
-                content['removed'] = ID.revert(remove_list)
-        # 3. response (no need to response this group command)
-        return []
-
-
-def group_manager():
-    from ..group import GroupManager
-    return GroupManager()
+                return self._respond_receipt(text='Permission denied.', msg=msg, group=group, extra={
+                    'template': 'Not allowed to query members of group: ${ID}',
+                    'replacements': {
+                        'ID': str(group),
+                    }
+                })
+        # 2. respond
+        res = self._respond_group_members(owner=owner, group=group, members=members)
+        return [] if res is None else [res]
```

### Comparing `dimples-0.2.1/dimples/client/cpu/grp_invite.py` & `dimples-0.2.2/dimples/client/cpu/grp_invite.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,47 +44,52 @@
 from dimp import InviteCommand
 
 from .grp_reset import ResetCommandProcessor
 
 
 class InviteCommandProcessor(ResetCommandProcessor):
 
-    STR_INVITE_CMD_ERROR = 'Invite command error.'
-    STR_INVITE_NOT_ALLOWED = 'Sorry, you are not allowed to invite new members into this group.'
-
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, InviteCommand), 'invite command error: %s' % content
         facebook = self.facebook
         group = content.group
         owner = facebook.owner(identifier=group)
         members = facebook.members(identifier=group)
         # 0. check group
         if owner is None or members is None or len(members) == 0:
             # NOTICE: group membership lost?
             #         reset group members
-            return self._temporary_save(content=content, sender=msg.sender)
+            return self._temporary_save(content=content, sender=msg.sender, msg=msg)
         # 1. check permission
         sender = msg.sender
         if sender not in members:
             # not a member? check assistants
             assistants = facebook.assistants(identifier=group)
             if assistants is None or sender not in assistants:
-                text = self.STR_INVITE_NOT_ALLOWED
-                return self._respond_text(text=text, group=group)
+                return self._respond_receipt(text='Permission denied.', msg=msg, group=group, extra={
+                    'template': 'Not allowed to invite member into group: ${ID}',
+                    'replacements': {
+                        'ID': str(group),
+                    }
+                })
         # 2. inviting members
         invite_list = self.members(content=content)
         if invite_list is None or len(invite_list) == 0:
-            text = self.STR_INVITE_CMD_ERROR
-            return self._respond_text(text=text, group=group)
+            return self._respond_receipt(text='Command error.', msg=msg, group=group, extra={
+                'template': 'Invite list is empty: ${ID}',
+                'replacements': {
+                    'ID': str(group),
+                }
+            })
         # 2.1. check for reset
         if sender == owner and owner in invite_list:
             # NOTICE: owner invites owner?
             #         it means this should be a 'reset' command
-            return self._temporary_save(content=content, sender=sender)
+            return self._temporary_save(content=content, sender=sender, msg=msg)
         # 2.2. build invited-list
         add_list = []
         for item in invite_list:
             if item in members:
                 continue
             # new member found
             add_list.append(item)
```

### Comparing `dimples-0.2.1/dimples/client/cpu/grp_query.py` & `dimples-0.2.2/dimples/server/cpu/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 # -*- coding: utf-8 -*-
-#
-#   DIM-SDK : Decentralized Instant Messaging Software Development Kit
-#
-#                                Written in 2019 by Moky <albert.moky@gmail.com>
-#
 # ==============================================================================
 # MIT License
 #
 # Copyright (c) 2019 Albert Moky
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
@@ -25,62 +20,66 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 """
-    Query Group Command Processor
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    Command Processor for 'report'
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-    1. query for group members-list
-    2. any existed member or assistant can query group members-list
+    Report protocol
 """
 
 from typing import List
 
-from dimp import ID
 from dimp import ReliableMessage
 from dimp import Content
-from dimp import GroupCommand, QueryCommand
 
-from ...common import CommonFacebook
+from dimsdk.cpu import BaseCommandProcessor
 
-from .history import GroupCommandProcessor
+from ...utils import Logging
+from ...common import ReportCommand
+from ...common import CommonMessenger, Session
 
 
-class QueryCommandProcessor(GroupCommandProcessor):
+class ReportCommandProcessor(BaseCommandProcessor, Logging):
 
-    STR_QUERY_NOT_ALLOWED = 'Sorry, you are not allowed to query this group.'
-
-    def _respond_group_members(self, owner: ID, group: ID, members: List[ID]) -> Content:
-        facebook = self.facebook
-        assert isinstance(facebook, CommonFacebook), 'facebook error: %s' % facebook
-        user = facebook.current_user
-        assert user is not None, 'current user not set'
-        if user.identifier == owner:
-            return GroupCommand.reset(group=group, members=members)
-        else:
-            return GroupCommand.invite(group=group, members=members)
+    @property
+    def session(self) -> Session:
+        messenger = self.messenger
+        assert isinstance(messenger, CommonMessenger), 'messenger error: %s' % messenger
+        return messenger.session
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
-        assert isinstance(content, QueryCommand), 'query command error: %s' % content
-        facebook = self.facebook
-        group = content.group
-        owner = facebook.owner(identifier=group)
-        members = facebook.members(identifier=group)
-        # 0. check group
-        if owner is None or members is None or len(members) == 0:
-            text = self.STR_GROUP_EMPTY
-            return self._respond_text(text=text, group=group)
-        # 1. check permission
+        assert isinstance(content, ReportCommand), 'report command error: %s' % content
+        # check session sender
+        session = self.session
         sender = msg.sender
-        if sender not in members:
-            # not a member? check assistants
-            assistants = facebook.assistants(identifier=group)
-            if assistants is None or sender not in assistants:
-                text = self.STR_QUERY_NOT_ALLOWED
-                return self._respond_text(text=text, group=group)
-        # 2. respond
-        res = self._respond_group_members(owner=owner, group=group, members=members)
-        return [] if res is None else [res]
+        if session.identifier is None:
+            self.error(msg='session not login, drop report command: %s => %s' % (sender, content))
+            return []
+        assert sender == session.identifier, 'report sender error: %s not %s' % (sender, session.identifier)
+        # check report title
+        title = content.title
+        if title == ReportCommand.ONLINE:
+            # online
+            session.set_active(active=True, when=content.time)
+            return self._respond_receipt(text='Online received.', msg=msg, extra={
+                'template': 'Online command received: ${ID}.',
+                'replacements': {
+                    'ID': str(sender),
+                }
+            })
+        elif title == ReportCommand.OFFLINE:
+            # offline
+            session.set_active(active=False, when=content.time)
+            # respond nothing when user offline
+            return []
+        else:
+            return self._respond_receipt(text='Command not support.', msg=msg, extra={
+                'template': 'Report command (title: ${title}) not support yet!',
+                'replacements': {
+                    'title': title,
+                }
+            })
```

### Comparing `dimples-0.2.1/dimples/client/cpu/grp_quit.py` & `dimples-0.2.2/dimples/client/cpu/grp_quit.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,51 +35,62 @@
     1. quit the group
     2. owner and assistant cannot quit
     3. assistant can be hired/fired by owner
 """
 
 from typing import List
 
+from dimp import ID
 from dimp import ReliableMessage
 from dimp import Content
 from dimp import QuitCommand
 
 from .history import GroupCommandProcessor
 
 
 class QuitCommandProcessor(GroupCommandProcessor):
 
-    STR_OWNER_CANNOT_QUIT = 'Sorry, owner cannot quit.'
-    STR_ASSISTANT_CANNOT_QUIT = 'Sorry, assistant cannot quit.'
-
     # noinspection PyUnusedLocal
-    def _remove_assistant(self, content: QuitCommand, msg: ReliableMessage) -> List[Content]:
+    def _remove_assistant(self, content: QuitCommand, sender: ID, msg: ReliableMessage) -> List[Content]:
         # NOTICE: group assistant should be retired by the owner
-        text = self.STR_ASSISTANT_CANNOT_QUIT
-        return self._respond_text(text=text, group=content.group)
+        group = content.group
+        return self._respond_receipt(text='Permission denied.', msg=msg, group=group, extra={
+            'template': 'Assistant cannot quit from group: ${ID}',
+            'replacements': {
+                'ID': str(group),
+            }
+        })
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, QuitCommand), 'quit command error: %s' % content
         facebook = self.facebook
         group = content.group
         owner = facebook.owner(identifier=group)
         members = facebook.members(identifier=group)
         # 0. check group
         if owner is None or members is None or len(members) == 0:
-            text = self.STR_GROUP_EMPTY
-            return self._respond_text(text=text, group=group)
+            return self._respond_receipt(text='Group empty.', msg=msg, group=group, extra={
+                'template': 'Group empty: ${ID}',
+                'replacements': {
+                    'ID': str(group),
+                }
+            })
         # 1. check permission
         sender = msg.sender
         if sender == owner:
-            text = self.STR_OWNER_CANNOT_QUIT
-            return self._respond_text(text=text, group=group)
+            return self._respond_receipt(text='Permission denied.', msg=msg, group=group, extra={
+                'template': 'Owner cannot quit from group: ${ID}',
+                'replacements': {
+                    'ID': str(group),
+                }
+            })
         assistants = facebook.assistants(identifier=group)
         if assistants is not None and sender in assistants:
-            return self._remove_assistant(content=content, msg=msg)
+            return self._remove_assistant(content=content, sender=sender, msg=msg)
         # 2. remove sender from group members
         if sender in members:
             members.remove(sender)
             man = group_manager()
             man.save_members(members=members, group=group)
         # 3. response (no need to response this group command)
         return []
```

### Comparing `dimples-0.2.1/dimples/client/cpu/grp_reset.py` & `dimples-0.2.2/dimples/client/cpu/grp_reset.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,31 +51,32 @@
 from ...common import CommonMessenger
 
 from .history import GroupCommandProcessor
 
 
 class ResetCommandProcessor(GroupCommandProcessor):
 
-    STR_RESET_CMD_ERROR = 'Reset command error.'
-    STR_RESET_NOT_ALLOWED = 'Sorry, you are not allowed to reset this group.'
-
     def _query_owner(self, owner: ID, group: ID):
         command = GroupCommand.query(group=group)
         messenger = self.messenger
         assert isinstance(messenger, CommonMessenger), 'messenger error: %s' % messenger
         messenger.send_content(sender=None, receiver=owner, content=command, priority=1)
 
-    def _temporary_save(self, content: GroupCommand, sender: ID) -> List[Content]:
+    def _temporary_save(self, content: GroupCommand, sender: ID, msg: ReliableMessage) -> List[Content]:
         facebook = self.facebook
         group = content.group
         # check whether the owner contained in the new members
         new_members = self.members(content=content)
         if new_members is None or len(new_members) == 0:
-            text = self.STR_RESET_CMD_ERROR
-            return self._respond_text(text=text, group=group)
+            return self._respond_receipt(text='Command error.', msg=msg, group=group, extra={
+                'template': 'New member list is empty: ${ID}',
+                'replacements': {
+                    'ID': str(group),
+                }
+            })
         man = group_manager()
         for item in new_members:
             if facebook.meta(identifier=item) is None:
                 # TODO: waiting for member's meta?
                 continue
             elif not man.is_owner(member=item, group=group):
                 # not owner, skip it
@@ -102,32 +103,44 @@
         group = content.group
         owner = facebook.owner(identifier=group)
         members = facebook.members(identifier=group)
         # 0. check group
         if owner is None or members is None or len(members) == 0:
             # FIXME: group profile lost?
             # FIXME: how to avoid strangers impersonating group members?
-            return self._temporary_save(content=content, sender=msg.sender)
+            return self._temporary_save(content=content, sender=msg.sender, msg=msg)
         # 1. check permission
         sender = msg.sender
         if sender != owner:
             # not the owner? check assistants
             assistants = facebook.assistants(identifier=group)
             if assistants is None or sender not in assistants:
-                text = self.STR_RESET_NOT_ALLOWED
-                return self._respond_text(text=text, group=group)
+                return self._respond_receipt(text='Permission denied.', msg=msg, group=group, extra={
+                    'template': 'Not allowed to reset members of group: ${ID}',
+                    'replacements': {
+                        'ID': str(group),
+                    }
+                })
         # 2. resetting members
         new_members = self.members(content=content)
         if new_members is None or len(new_members) == 0:
-            text = self.STR_RESET_CMD_ERROR
-            return self._respond_text(text=text, group=group)
+            return self._respond_receipt(text='Command error.', msg=msg, group=group, extra={
+                'template': 'New member list is empty: ${ID}',
+                'replacements': {
+                    'ID': str(group),
+                }
+            })
         # 2.1. check owner
         if owner not in new_members:
-            text = self.STR_RESET_CMD_ERROR
-            return self._respond_text(text=text, group=group)
+            return self._respond_receipt(text='Permission denied.', msg=msg, group=group, extra={
+                'template': 'Owner not in the new member list of group: ${ID}',
+                'replacements': {
+                    'ID': str(group),
+                }
+            })
         # 2.2. build expelled-list
         remove_list = []
         for item in members:
             if item not in new_members:
                 # removing member found
                 remove_list.append(item)
         # 2.3. build invited-list
```

### Comparing `dimples-0.2.1/dimples/client/cpu/handshake.py` & `dimples-0.2.2/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/cpu/history.py` & `dimples-0.2.2/dimples/client/cpu/history.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,28 +41,27 @@
 from dimp import Command, GroupCommand
 
 from dimsdk.cpu import BaseCommandProcessor
 
 
 class HistoryCommandProcessor(BaseCommandProcessor):
 
-    FMT_HIS_CMD_NOT_SUPPORT = 'History command (name: %s) not support yet!'
-
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, Command), 'history command error: %s' % content
-        text = self.FMT_HIS_CMD_NOT_SUPPORT % content.cmd
-        return self._respond_text(text=text, group=content.group)
+        return self._respond_receipt(text='Command not support.', msg=msg, group=content.group, extra={
+            'template': 'History command (name: ${command}) not support yet!',
+            'replacements': {
+                'command': content.cmd,
+            }
+        })
 
 
 class GroupCommandProcessor(HistoryCommandProcessor):
 
-    FMT_GRP_CMD_NOT_SUPPORT = 'Group command (name: %s) not support yet!'
-    STR_GROUP_EMPTY = 'Group empty.'
-
     @staticmethod
     def members(content: GroupCommand) -> List[ID]:
         # get from 'members'
         array = content.members
         if array is None:
             # get from 'member
             item = content.member
@@ -71,9 +70,13 @@
             else:
                 array = [item]
         return array
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, GroupCommand), 'group command error: %s' % content
-        text = self.FMT_GRP_CMD_NOT_SUPPORT % content.cmd
-        return self._respond_text(text=text, group=content.group)
+        return self._respond_receipt(text='Command not support.', msg=msg, group=content.group, extra={
+            'template': 'Group command (name: ${command}) not support yet!',
+            'replacements': {
+                'command': content.cmd,
+            }
+        })
```

### Comparing `dimples-0.2.1/dimples/client/cpu/login.py` & `dimples-0.2.2/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/cpu/text.py` & `dimples-0.2.2/dimples/client/cpu/text.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/group.py` & `dimples-0.2.2/dimples/client/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/messenger.py` & `dimples-0.2.2/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/network/__init__.py` & `dimples-0.2.2/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/network/session.py` & `dimples-0.2.2/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/network/state.py` & `dimples-0.2.2/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/network/transition.py` & `dimples-0.2.2/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/packer.py` & `dimples-0.2.2/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/processor.py` & `dimples-0.2.2/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/client/terminal.py` & `dimples-0.2.2/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/__init__.py` & `dimples-0.2.2/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/ans.py` & `dimples-0.2.2/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/dbi/__init__.py` & `dimples-0.2.2/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/dbi/account.py` & `dimples-0.2.2/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/dbi/message.py` & `dimples-0.2.2/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/dbi/session.py` & `dimples-0.2.2/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/facebook.py` & `dimples-0.2.2/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/messenger.py` & `dimples-0.2.2/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/packer.py` & `dimples-0.2.2/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/protocol/__init__.py` & `dimples-0.2.2/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/protocol/ans.py` & `dimples-0.2.2/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/protocol/handshake.py` & `dimples-0.2.2/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/protocol/login.py` & `dimples-0.2.2/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/protocol/report.py` & `dimples-0.2.2/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/common/session.py` & `dimples-0.2.2/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/config.py` & `dimples-0.2.2/dimples/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/__init__.py` & `dimples-0.2.2/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/gate.py` & `dimples-0.2.2/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/gatekeeper.py` & `dimples-0.2.2/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/mars.py` & `dimples-0.2.2/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/mtp.py` & `dimples-0.2.2/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/protocol/__init__.py` & `dimples-0.2.2/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/protocol/mars.py` & `dimples-0.2.2/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/protocol/ws.py` & `dimples-0.2.2/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/queue.py` & `dimples-0.2.2/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/seeker.py` & `dimples-0.2.2/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/session.py` & `dimples-0.2.2/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/conn/ws.py` & `dimples-0.2.2/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/__init__.py` & `dimples-0.2.2/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/account.py` & `dimples-0.2.2/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/__init__.py` & `dimples-0.2.2/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/base.py` & `dimples-0.2.2/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/document.py` & `dimples-0.2.2/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/group.py` & `dimples-0.2.2/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/login.py` & `dimples-0.2.2/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/meta.py` & `dimples-0.2.2/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/private.py` & `dimples-0.2.2/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/station.py` & `dimples-0.2.2/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/dos/user.py` & `dimples-0.2.2/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/message.py` & `dimples-0.2.2/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/session.py` & `dimples-0.2.2/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_cipherkey.py` & `dimples-0.2.2/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_document.py` & `dimples-0.2.2/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_group.py` & `dimples-0.2.2/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_login.py` & `dimples-0.2.2/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_message.py` & `dimples-0.2.2/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_meta.py` & `dimples-0.2.2/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_private.py` & `dimples-0.2.2/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_station.py` & `dimples-0.2.2/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/database/t_user.py` & `dimples-0.2.2/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/edge/__init__.py` & `dimples-0.2.2/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/edge/octopus.py` & `dimples-0.2.2/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/edge/shared.py` & `dimples-0.2.2/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/edge/start.py` & `dimples-0.2.2/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/register/__init__.py` & `dimples-0.2.2/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/register/generate.py` & `dimples-0.2.2/dimples/register/generate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/register/modify.py` & `dimples-0.2.2/dimples/register/modify.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/register/run.py` & `dimples-0.2.2/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/register/shared.py` & `dimples-0.2.2/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/__init__.py` & `dimples-0.2.2/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/broadcast.py` & `dimples-0.2.2/dimples/server/broadcast.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/cpu/__init__.py` & `dimples-0.2.2/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/cpu/ans.py` & `dimples-0.2.2/dimples/server/cpu/ans.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 class AnsCommandProcessor(BaseCommandProcessor):
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, AnsCommand), 'report command error: %s' % content
         names = content.names
         if len(names) == 0:
-            text = 'ANS command error.'
-            return self._respond_text(text=text)
+            return self._respond_receipt(text='ANS command error.', msg=msg)
         records = {}
         missed = []
         for item in names:
             # get record from ANS factory
             identifier = self.ans_id(name=item)
             if identifier is None:
                 missed.append(item)
```

### Comparing `dimples-0.2.1/dimples/server/cpu/document.py` & `dimples-0.2.2/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/cpu/handshake.py` & `dimples-0.2.2/dimples/server/cpu/handshake.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, HandshakeCommand), 'handshake command error: %s' % content
         title = content.title
         if title in ['DIM?', 'DIM!']:
             # S -> C
-            return self._respond_text(text='Command not support.', extra={
+            return self._respond_receipt(text='Command not support.', msg=msg, extra={
                 'template': 'Handshake command error: title="${title}".',
                 'replacements': {
                     'title': title,
                 }
             })
         # C -> S: Hello world!
         assert 'Hello world!' == title, 'Handshake command error: %s' % content
```

### Comparing `dimples-0.2.1/dimples/server/cpu/login.py` & `dimples-0.2.2/dimples/server/cpu/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             # forwarded login command
             self.info(msg='user login: %s -> %s, forwarded by %s' % (sender, roaming, session.identifier))
             return []
         # 3. update session flag
         session.set_active(active=True)
         # only respond the user login to this station
         self.info(msg='user login: %s -> %s' % (sender, roaming))
-        return self._respond_text(text='Login received.', extra={
+        return self._respond_receipt(text='Login received.', msg=msg, extra={
             'template': 'Login command received: ${ID}.',
             'replacements': {
                 'ID': str(sender),
             }
         })
```

### Comparing `dimples-0.2.1/dimples/server/dispatcher.py` & `dimples-0.2.2/dimples/server/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/messenger.py` & `dimples-0.2.2/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/packer.py` & `dimples-0.2.2/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/processor.py` & `dimples-0.2.2/dimples/server/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         # 0. process first
         responses = super().process_content(content=content, r_msg=r_msg)
         messenger = self.messenger
         sender = r_msg.sender
         # 1. check login
         session = messenger.session
-        if session.identifier is None or not session.active:
+        if session.identifier is None:  # or not session.active:
             # not login yet, force to handshake again
             if not isinstance(content, HandshakeCommand):
                 handshake = HandshakeCommand.ask(session=session.key)
                 responses.insert(0, handshake)
         # 2. check response
         contents = []
         for res in responses:
```

### Comparing `dimples-0.2.1/dimples/server/push.py` & `dimples-0.2.2/dimples/server/push.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/session.py` & `dimples-0.2.2/dimples/server/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
             load_cached_messages(session=self)
             return True
 
     # Override
     def set_active(self, active: bool, when: float = None):
         if super().set_active(active=active, when=when):
             session_change_active(session=self, active=active)
-            load_cached_messages(session=self)
+            if active:
+                load_cached_messages(session=self)
             return True
 
     @property  # Override
     def running(self) -> bool:
         if super().running:
             gate = self.gate
             conn = gate.get_channel(remote=self.remote_address, local=None)
```

### Comparing `dimples-0.2.1/dimples/server/session_center.py` & `dimples-0.2.2/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/server/trace.py` & `dimples-0.2.2/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/station/__init__.py` & `dimples-0.2.2/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/station/handler.py` & `dimples-0.2.2/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/station/shared.py` & `dimples-0.2.2/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/station/start.py` & `dimples-0.2.2/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/utils/__init__.py` & `dimples-0.2.2/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/utils/cache.py` & `dimples-0.2.2/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/utils/checker.py` & `dimples-0.2.2/dimples/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/utils/dos.py` & `dimples-0.2.2/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/utils/log.py` & `dimples-0.2.2/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples/utils/singleton.py` & `dimples-0.2.2/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/dimples.egg-info/PKG-INFO` & `dimples-0.2.2/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.2.1
+Version: 0.2.2
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.2.1/dimples.egg-info/SOURCES.txt` & `dimples-0.2.2/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimples-0.2.1/setup.py` & `dimples-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -49,15 +49,15 @@
     },
     install_requires=[
         # 'pycryptodome',  # 3.14.1
         # 'base58',  # 1.0.3
         # 'ecdsa',   # 0.16.1
         'dimplugins>=0.1.4',
 
-        'dimsdk>=0.8.6',
+        'dimsdk>=0.8.7',
         'dimp>=0.12.9',
         'dkd>=0.12.7',
         'mkm>=0.12.7',
 
         'startrek>=0.4.1',
         'tcp>=0.4.1',
         'udp>=0.5.10',
```

