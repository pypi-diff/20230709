# Comparing `tmp/pyghelpers-1.0.43.tar.gz` & `tmp/pyghelpers-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghelpers-1.0.43.tar", last modified: Sun Jul  9 18:07:34 2023, max compression
+gzip compressed data, was "pyghelpers-1.1.tar", last modified: Sun Jul  9 18:14:45 2023, max compression
```

## Comparing `pyghelpers-1.0.43.tar` & `pyghelpers-1.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.215996 pyghelpers-1.0.43/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pyghelpers-1.0.43/LICENSE
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      160 2018-12-25 05:37:38.000000 pyghelpers-1.0.43/MANIFEST.in
--rw-r--r--   0 irvkalb    (501) staff       (20)      519 2023-07-09 18:07:34.215596 pyghelpers-1.0.43/PKG-INFO
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1920 2023-07-09 18:02:30.000000 pyghelpers-1.0.43/README
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.131037 pyghelpers-1.0.43/pyghelpers/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-13 19:35:54.000000 pyghelpers-1.0.43/pyghelpers/__init__.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     5192 2023-07-09 17:57:13.000000 pyghelpers-1.0.43/pyghelpers/conf.py
--rw-r--r--   0 irvkalb    (501) staff       (20)    51271 2023-07-09 18:03:17.000000 pyghelpers-1.0.43/pyghelpers/pyghelpers.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.132817 pyghelpers-1.0.43/pyghelpers.egg-info/
--rw-r--r--   0 irvkalb    (501) staff       (20)      519 2023-07-09 18:07:34.000000 pyghelpers-1.0.43/pyghelpers.egg-info/PKG-INFO
--rw-r--r--   0 irvkalb    (501) staff       (20)     4767 2023-07-09 18:07:34.000000 pyghelpers-1.0.43/pyghelpers.egg-info/SOURCES.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-09 18:07:34.000000 pyghelpers-1.0.43/pyghelpers.egg-info/dependency_links.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       31 2023-07-09 18:07:34.000000 pyghelpers-1.0.43/pyghelpers.egg-info/requires.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-09 18:07:34.000000 pyghelpers-1.0.43/pyghelpers.egg-info/top_level.txt
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.133469 pyghelpers-1.0.43/pyghelpers_test/
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.134772 pyghelpers-1.0.43/pyghelpers_test/DialogTester/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     7714 2023-07-05 17:35:47.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/Main_DialogTester.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/__init__.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.151863 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    21412 2018-06-19 19:45:14.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    22141 2018-06-19 19:43:10.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    22283 2018-06-19 19:38:50.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    22264 2018-06-19 19:46:32.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19027 2018-06-19 19:58:28.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18893 2018-06-19 19:59:34.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18985 2018-06-19 20:00:54.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18986 2018-06-19 20:02:18.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/controlsBackground.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     3645 2018-05-15 17:35:14.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/dialog.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    26577 2018-05-15 23:37:20.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/highScoresBackground.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1497 2018-06-16 21:51:20.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1695 2018-06-16 21:51:52.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1606 2018-06-16 21:48:48.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1621 2018-06-16 21:53:06.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19119 2018-06-19 20:15:20.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19825 2018-06-19 20:16:32.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19916 2018-06-19 20:17:42.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    19936 2018-06-19 20:18:50.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17066 2018-06-19 20:12:52.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17631 2018-06-19 20:11:38.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17722 2018-06-19 20:09:16.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    17663 2018-06-19 20:06:54.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1797 2018-06-16 21:50:56.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1959 2018-06-16 21:52:16.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1834 2018-06-16 21:48:36.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesNormal.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1896 2018-06-16 21:52:48.000000 pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesOver.png
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.162290 pyghelpers-1.0.43/pyghelpers_test/Dodger/
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2812 2021-09-06 20:00:39.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/Baddies.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)      445 2021-08-09 04:29:01.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/Constants.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     3599 2021-07-29 04:18:53.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/Goodies.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2468 2021-09-05 19:48:00.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/HighScoresData.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     1169 2023-07-05 17:21:38.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/Main_Dodger.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)      847 2021-11-23 19:31:34.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/Player.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-06-24 22:19:51.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/SceneExample.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     8159 2021-09-05 19:39:41.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/SceneHighScores.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     9837 2021-09-05 19:14:11.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/ScenePlay.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-07-28 03:38:15.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/SceneSplash.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/__init__.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.210572 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    24713 2021-09-05 17:52:14.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    23298 2021-09-05 17:46:48.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    26868 2021-09-05 17:44:38.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    22706 2021-09-05 17:49:02.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     4571 2021-08-03 16:14:09.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3796 2021-08-03 16:06:41.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6270 2021-08-03 15:50:18.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     2696 2021-08-03 16:01:52.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     2416 2018-12-19 17:45:20.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/baddie.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13447 2018-12-16 06:45:56.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13214 2018-12-16 06:46:48.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    14317 2018-12-16 06:45:42.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    12926 2018-12-16 06:46:24.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/controlsBackground.jpg
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6005 2018-09-03 02:09:30.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/dialog.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3602 2018-12-19 18:59:42.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/dodger.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     1199 2017-01-11 03:50:38.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gameOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     3078 2018-12-19 17:45:42.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/goodie.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    17632 2018-12-19 00:36:16.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    16540 2018-12-19 00:36:58.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    18691 2018-12-19 00:35:54.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    15948 2018-12-19 00:36:36.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    65967 2018-09-02 05:38:44.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresBackground.jpg
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     9456 2018-12-16 05:42:22.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8681 2018-12-16 05:44:14.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    10087 2018-12-16 05:41:04.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8375 2018-12-16 05:42:46.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13980 2018-12-16 06:31:54.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13080 2018-12-16 06:32:42.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    15081 2018-12-16 06:31:38.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    12490 2018-12-16 06:32:20.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13388 2018-12-16 06:49:26.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    13000 2018-12-16 06:50:12.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    14237 2018-12-16 06:48:44.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)    12689 2018-12-16 06:49:42.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)      913 2011-03-26 00:48:20.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/player.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5853 2018-12-16 03:12:28.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5770 2018-12-16 03:13:36.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6225 2018-12-16 03:12:08.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5671 2018-12-16 03:12:46.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7511 2018-12-16 05:02:42.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7054 2018-12-16 05:04:16.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7909 2018-12-16 05:02:06.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6675 2018-12-16 05:03:16.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)   133232 2018-09-02 05:47:28.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/splashBackground.jpg
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6102 2018-12-16 03:05:44.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     5847 2018-12-16 03:06:54.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8004 2018-12-16 05:20:00.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewDisabled.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7937 2018-12-16 05:19:16.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewDown.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     9086 2018-12-16 05:20:16.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     8495 2018-12-16 05:19:32.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewOver.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7214 2018-12-16 03:05:00.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNormal.png
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     6517 2018-12-16 03:06:38.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startOver.png
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:07:34.213281 pyghelpers-1.0.43/pyghelpers_test/Dodger/sounds/
--rwxrwxr-x   0 irvkalb    (501) staff       (20)     7162 2011-03-26 00:48:20.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/sounds/background.mid
--rwxrwxr-x   0 irvkalb    (501) staff       (20)   123716 2017-01-06 04:16:32.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/sounds/ding.wav
--rwxrwxr-x   0 irvkalb    (501) staff       (20)   258876 2011-03-26 00:48:20.000000 pyghelpers-1.0.43/pyghelpers_test/Dodger/sounds/gameover.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.0.43/pyghelpers_test/__init__.py
--rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-09 18:07:34.216128 pyghelpers-1.0.43/setup.cfg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      782 2023-07-09 17:57:31.000000 pyghelpers-1.0.43/setup.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.901800 pyghelpers-1.1/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pyghelpers-1.1/LICENSE
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      160 2018-12-25 05:37:38.000000 pyghelpers-1.1/MANIFEST.in
+-rw-r--r--   0 irvkalb    (501) staff       (20)      516 2023-07-09 18:14:45.901519 pyghelpers-1.1/PKG-INFO
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1920 2023-07-09 18:02:30.000000 pyghelpers-1.1/README
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.855508 pyghelpers-1.1/pyghelpers/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-13 19:35:54.000000 pyghelpers-1.1/pyghelpers/__init__.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     5189 2023-07-09 18:13:20.000000 pyghelpers-1.1/pyghelpers/conf.py
+-rw-r--r--   0 irvkalb    (501) staff       (20)    51271 2023-07-09 18:13:34.000000 pyghelpers-1.1/pyghelpers/pyghelpers.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.857407 pyghelpers-1.1/pyghelpers.egg-info/
+-rw-r--r--   0 irvkalb    (501) staff       (20)      516 2023-07-09 18:14:45.000000 pyghelpers-1.1/pyghelpers.egg-info/PKG-INFO
+-rw-r--r--   0 irvkalb    (501) staff       (20)     4767 2023-07-09 18:14:45.000000 pyghelpers-1.1/pyghelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-09 18:14:45.000000 pyghelpers-1.1/pyghelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       31 2023-07-09 18:14:45.000000 pyghelpers-1.1/pyghelpers.egg-info/requires.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-09 18:14:45.000000 pyghelpers-1.1/pyghelpers.egg-info/top_level.txt
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.857902 pyghelpers-1.1/pyghelpers_test/
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.858435 pyghelpers-1.1/pyghelpers_test/DialogTester/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     7714 2023-07-05 17:35:47.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/Main_DialogTester.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/__init__.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.870337 pyghelpers-1.1/pyghelpers_test/DialogTester/images/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    21412 2018-06-19 19:45:14.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/addDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    22141 2018-06-19 19:43:10.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/addDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    22283 2018-06-19 19:38:50.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/addNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    22264 2018-06-19 19:46:32.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/addOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19027 2018-06-19 19:58:28.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18893 2018-06-19 19:59:34.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18985 2018-06-19 20:00:54.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18986 2018-06-19 20:02:18.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/controlsBackground.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     3645 2018-05-15 17:35:14.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/dialog.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    26577 2018-05-15 23:37:20.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/highScoresBackground.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1497 2018-06-16 21:51:20.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1695 2018-06-16 21:51:52.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1606 2018-06-16 21:48:48.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1621 2018-06-16 21:53:06.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19119 2018-06-19 20:15:20.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19825 2018-06-19 20:16:32.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19916 2018-06-19 20:17:42.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    19936 2018-06-19 20:18:50.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17066 2018-06-19 20:12:52.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/okDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17631 2018-06-19 20:11:38.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/okDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17722 2018-06-19 20:09:16.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/okNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    17663 2018-06-19 20:06:54.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/okOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1797 2018-06-16 21:50:56.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1959 2018-06-16 21:52:16.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1834 2018-06-16 21:48:36.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesNormal.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1896 2018-06-16 21:52:48.000000 pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesOver.png
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.875212 pyghelpers-1.1/pyghelpers_test/Dodger/
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2812 2021-09-06 20:00:39.000000 pyghelpers-1.1/pyghelpers_test/Dodger/Baddies.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)      445 2021-08-09 04:29:01.000000 pyghelpers-1.1/pyghelpers_test/Dodger/Constants.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     3599 2021-07-29 04:18:53.000000 pyghelpers-1.1/pyghelpers_test/Dodger/Goodies.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2468 2021-09-05 19:48:00.000000 pyghelpers-1.1/pyghelpers_test/Dodger/HighScoresData.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     1169 2023-07-05 17:21:38.000000 pyghelpers-1.1/pyghelpers_test/Dodger/Main_Dodger.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)      847 2021-11-23 19:31:34.000000 pyghelpers-1.1/pyghelpers_test/Dodger/Player.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-06-24 22:19:51.000000 pyghelpers-1.1/pyghelpers_test/Dodger/SceneExample.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     8159 2021-09-05 19:39:41.000000 pyghelpers-1.1/pyghelpers_test/Dodger/SceneHighScores.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     9837 2021-09-05 19:14:11.000000 pyghelpers-1.1/pyghelpers_test/Dodger/ScenePlay.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)     2443 2021-07-28 03:38:15.000000 pyghelpers-1.1/pyghelpers_test/Dodger/SceneSplash.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.1/pyghelpers_test/Dodger/__init__.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.899742 pyghelpers-1.1/pyghelpers_test/Dodger/images/
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    24713 2021-09-05 17:52:14.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/addDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    23298 2021-09-05 17:46:48.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/addDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    26868 2021-09-05 17:44:38.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/addNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    22706 2021-09-05 17:49:02.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/addOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     4571 2021-08-03 16:14:09.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/backDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3796 2021-08-03 16:06:41.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/backDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6270 2021-08-03 15:50:18.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/backNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     2696 2021-08-03 16:01:52.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/backOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     2416 2018-12-19 17:45:20.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/baddie.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13447 2018-12-16 06:45:56.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13214 2018-12-16 06:46:48.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    14317 2018-12-16 06:45:42.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    12926 2018-12-16 06:46:24.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3727 2018-06-10 00:54:52.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/controlsBackground.jpg
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6005 2018-09-03 02:09:30.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/dialog.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3602 2018-12-19 18:59:42.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/dodger.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     1199 2017-01-11 03:50:38.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/gameOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     3078 2018-12-19 17:45:42.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/goodie.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    17632 2018-12-19 00:36:16.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    16540 2018-12-19 00:36:58.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    18691 2018-12-19 00:35:54.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    15948 2018-12-19 00:36:36.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    65967 2018-09-02 05:38:44.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresBackground.jpg
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     9456 2018-12-16 05:42:22.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8681 2018-12-16 05:44:14.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    10087 2018-12-16 05:41:04.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8375 2018-12-16 05:42:46.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13980 2018-12-16 06:31:54.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13080 2018-12-16 06:32:42.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    15081 2018-12-16 06:31:38.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    12490 2018-12-16 06:32:20.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13388 2018-12-16 06:49:26.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/okDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    13000 2018-12-16 06:50:12.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/okDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    14237 2018-12-16 06:48:44.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/okNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)    12689 2018-12-16 06:49:42.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/okOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)      913 2011-03-26 00:48:20.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/player.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5853 2018-12-16 03:12:28.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/quitDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5770 2018-12-16 03:13:36.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/quitDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6225 2018-12-16 03:12:08.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/quitNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5671 2018-12-16 03:12:46.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/quitOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7511 2018-12-16 05:02:42.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/resetDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7054 2018-12-16 05:04:16.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/resetDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7909 2018-12-16 05:02:06.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/resetNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6675 2018-12-16 05:03:16.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/resetOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)   133232 2018-09-02 05:47:28.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/splashBackground.jpg
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6102 2018-12-16 03:05:44.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     5847 2018-12-16 03:06:54.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8004 2018-12-16 05:20:00.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewDisabled.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7937 2018-12-16 05:19:16.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewDown.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     9086 2018-12-16 05:20:16.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     8495 2018-12-16 05:19:32.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewOver.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7214 2018-12-16 03:05:00.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startNormal.png
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     6517 2018-12-16 03:06:38.000000 pyghelpers-1.1/pyghelpers_test/Dodger/images/startOver.png
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-09 18:14:45.900813 pyghelpers-1.1/pyghelpers_test/Dodger/sounds/
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)     7162 2011-03-26 00:48:20.000000 pyghelpers-1.1/pyghelpers_test/Dodger/sounds/background.mid
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)   123716 2017-01-06 04:16:32.000000 pyghelpers-1.1/pyghelpers_test/Dodger/sounds/ding.wav
+-rwxrwxr-x   0 irvkalb    (501) staff       (20)   258876 2011-03-26 00:48:20.000000 pyghelpers-1.1/pyghelpers_test/Dodger/sounds/gameover.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pyghelpers-1.1/pyghelpers_test/__init__.py
+-rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-09 18:14:45.901884 pyghelpers-1.1/setup.cfg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      779 2023-07-09 18:13:13.000000 pyghelpers-1.1/setup.py
```

### Comparing `pyghelpers-1.0.43/LICENSE` & `pyghelpers-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/README` & `pyghelpers-1.1/README`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers/conf.py` & `pyghelpers-1.1/pyghelpers/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 # -- Project information -----------------------------------------------------
 
 project = 'pyghelpers'
 copyright = '2019, Irv Kalb'
 author = 'Irv Kalb'
 
 # The short X.Y version
-version = '1.0'
+version = '1.1'
 # The full version, including alpha/beta/rc tags
-release = '1.0.43'
+release = '1.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 needs_sphinx = '7.0.1'
```

### Comparing `pyghelpers-1.0.43/pyghelpers/pyghelpers.py` & `pyghelpers-1.1/pyghelpers/pyghelpers.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers.egg-info/SOURCES.txt` & `pyghelpers-1.1/pyghelpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/Main_DialogTester.py` & `pyghelpers-1.1/pyghelpers_test/DialogTester/Main_DialogTester.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addDisabled.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/addDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addDown.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/addDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addNormal.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/addNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/addOver.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/addOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelDisabled.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelDown.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelNormal.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/cancelOver.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/cancelOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/controlsBackground.jpg` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/controlsBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/dialog.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/dialog.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/highScoresBackground.jpg` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/highScoresBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noDisabled.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noDown.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noNormal.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noOver.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksDisabled.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksDown.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksNormal.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/noThanksOver.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/noThanksOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okDisabled.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/okDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okDown.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/okDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okNormal.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/okNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/okOver.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/okOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesDisabled.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesDown.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesNormal.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/DialogTester/images/yesOver.png` & `pyghelpers-1.1/pyghelpers_test/DialogTester/images/yesOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/Baddies.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/Baddies.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/Goodies.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/Goodies.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/HighScoresData.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/HighScoresData.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/Main_Dodger.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/Main_Dodger.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/Player.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/Player.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/SceneExample.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/SceneExample.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/SceneHighScores.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/SceneHighScores.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/ScenePlay.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/ScenePlay.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/SceneSplash.py` & `pyghelpers-1.1/pyghelpers_test/Dodger/SceneSplash.py`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/addDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/addDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/addNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/addOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/addOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/backDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/backDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/backNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/backOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/backOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/baddie.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/baddie.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/cancelOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/cancelOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/controlsBackground.jpg` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/controlsBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/dialog.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/dialog.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/dodger.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/dodger.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gameOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/gameOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/goodie.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/goodie.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/gotoHighScoresOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/gotoHighScoresOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresBackground.jpg` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/highScoresOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/highScoresOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/noThanksOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/noThanksOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/okDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/okDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/okNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/okOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/okOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/player.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/player.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/quitDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/quitDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/quitNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/quitOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/quitOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/resetDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/resetDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/resetNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/resetOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/resetOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/splashBackground.jpg` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/splashBackground.jpg`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewDisabled.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewDisabled.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewDown.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewDown.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNewOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startNewOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startNormal.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startNormal.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/images/startOver.png` & `pyghelpers-1.1/pyghelpers_test/Dodger/images/startOver.png`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/sounds/background.mid` & `pyghelpers-1.1/pyghelpers_test/Dodger/sounds/background.mid`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/sounds/ding.wav` & `pyghelpers-1.1/pyghelpers_test/Dodger/sounds/ding.wav`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/pyghelpers_test/Dodger/sounds/gameover.wav` & `pyghelpers-1.1/pyghelpers_test/Dodger/sounds/gameover.wav`

 * *Files identical despite different names*

### Comparing `pyghelpers-1.0.43/setup.py` & `pyghelpers-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pyghelpers',
-    version='1.0.43',
+    version='1.1',
     author='Irv Kalb',
     author_email='Irv@furrypants.com',
     description='Classes and functions for use with Pygame',
     long_description='A collection of classes and functions for building programs using Pygame',
     packages=find_packages(),
     include_package_data=True,
     license="BSD",
```

